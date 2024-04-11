# Comparing `tmp/olive_ai-0.5.1-py3-none-any.whl.zip` & `tmp/olive_ai-0.5.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,242 +1,246 @@
-Zip file size: 503221 bytes, number of entries: 240
--rw-rw-r--  2.0 unx      608 b- defN 24-Apr-07 07:47 olive/__init__.py
--rw-rw-r--  2.0 unx     9998 b- defN 24-Apr-07 07:47 olive/cache.py
--rw-rw-r--  2.0 unx     1113 b- defN 24-Apr-07 07:47 olive/constants.py
--rw-rw-r--  2.0 unx     2626 b- defN 24-Apr-07 07:47 olive/logging.py
--rw-rw-r--  2.0 unx     7817 b- defN 24-Apr-07 07:47 olive/olive_config.json
--rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-07 07:47 olive/package_config.py
--rw-rw-r--  2.0 unx    22999 b- defN 24-Apr-07 07:47 olive/resource_path.py
--rw-rw-r--  2.0 unx     5181 b- defN 24-Apr-07 07:47 olive/auto_optimizer/__init__.py
--rw-rw-r--  2.0 unx     5871 b- defN 24-Apr-07 07:47 olive/auto_optimizer/regulate_mixins.py
--rw-rw-r--  2.0 unx     3615 b- defN 24-Apr-07 07:47 olive/auto_optimizer/template_mapping.py
--rw-rw-r--  2.0 unx     1171 b- defN 24-Apr-07 07:47 olive/auto_optimizer/config_template/opt_level_passes.yaml
--rw-rw-r--  2.0 unx     2062 b- defN 24-Apr-07 07:47 olive/auto_optimizer/config_template/pass_capability.yaml
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/azureml/__init__.py
--rw-rw-r--  2.0 unx     6412 b- defN 24-Apr-07 07:47 olive/azureml/azureml_client.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/common/__init__.py
--rw-rw-r--  2.0 unx     3430 b- defN 24-Apr-07 07:47 olive/common/auto_config.py
--rw-rw-r--  2.0 unx    10881 b- defN 24-Apr-07 07:47 olive/common/config_utils.py
--rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-07 07:47 olive/common/import_lib.py
--rw-rw-r--  2.0 unx    16029 b- defN 24-Apr-07 07:47 olive/common/ort_inference.py
--rw-rw-r--  2.0 unx      765 b- defN 24-Apr-07 07:47 olive/common/pydantic_v1.py
--rw-rw-r--  2.0 unx     1809 b- defN 24-Apr-07 07:47 olive/common/user_module_loader.py
--rw-rw-r--  2.0 unx    11627 b- defN 24-Apr-07 07:47 olive/common/utils.py
--rw-rw-r--  2.0 unx      345 b- defN 24-Apr-07 07:47 olive/data/__init__.py
--rw-rw-r--  2.0 unx    10680 b- defN 24-Apr-07 07:47 olive/data/config.py
--rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-07 07:47 olive/data/constants.py
--rw-rw-r--  2.0 unx     8119 b- defN 24-Apr-07 07:47 olive/data/registry.py
--rw-rw-r--  2.0 unx     3573 b- defN 24-Apr-07 07:47 olive/data/template.py
--rw-rw-r--  2.0 unx      444 b- defN 24-Apr-07 07:47 olive/data/component/__init__.py
--rw-rw-r--  2.0 unx     1955 b- defN 24-Apr-07 07:47 olive/data/component/dataloader.py
--rw-rw-r--  2.0 unx    10679 b- defN 24-Apr-07 07:47 olive/data/component/dataset.py
--rw-rw-r--  2.0 unx     1928 b- defN 24-Apr-07 07:47 olive/data/component/load_dataset.py
--rw-rw-r--  2.0 unx     2256 b- defN 24-Apr-07 07:47 olive/data/component/post_process_data.py
--rw-rw-r--  2.0 unx    11446 b- defN 24-Apr-07 07:47 olive/data/component/pre_process_data.py
--rw-rw-r--  2.0 unx    29278 b- defN 24-Apr-07 07:47 olive/data/component/text_generation.py
--rw-rw-r--  2.0 unx      480 b- defN 24-Apr-07 07:47 olive/data/container/__init__.py
--rw-rw-r--  2.0 unx     3385 b- defN 24-Apr-07 07:47 olive/data/container/data_container.py
--rw-rw-r--  2.0 unx     1159 b- defN 24-Apr-07 07:47 olive/data/container/dummy_data_container.py
--rw-rw-r--  2.0 unx     1690 b- defN 24-Apr-07 07:47 olive/data/container/huggingface_container.py
--rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-07 07:47 olive/data/container/raw_data_container.py
--rw-rw-r--  2.0 unx      411 b- defN 24-Apr-07 07:47 olive/engine/__init__.py
--rw-rw-r--  2.0 unx     1447 b- defN 24-Apr-07 07:47 olive/engine/config.py
--rw-rw-r--  2.0 unx    46635 b- defN 24-Apr-07 07:47 olive/engine/engine.py
--rw-rw-r--  2.0 unx    17410 b- defN 24-Apr-07 07:47 olive/engine/footprint.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/engine/packaging/__init__.py
--rw-rw-r--  2.0 unx     1642 b- defN 24-Apr-07 07:47 olive/engine/packaging/packaging_config.py
--rw-rw-r--  2.0 unx    19748 b- defN 24-Apr-07 07:47 olive/engine/packaging/packaging_generator.py
--rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
--rw-rw-r--  2.0 unx     4990 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
--rw-rw-r--  2.0 unx     1590 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/cs/README.md
--rw-rw-r--  2.0 unx     4991 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
--rw-rw-r--  2.0 unx     2296 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/python/README.md
--rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-07 07:47 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/evaluator/__init__.py
--rw-rw-r--  2.0 unx     6473 b- defN 24-Apr-07 07:47 olive/evaluator/accuracy.py
--rw-rw-r--  2.0 unx     8723 b- defN 24-Apr-07 07:47 olive/evaluator/metric.py
--rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-07 07:47 olive/evaluator/metric_backend.py
--rw-rw-r--  2.0 unx     4395 b- defN 24-Apr-07 07:47 olive/evaluator/metric_config.py
--rw-rw-r--  2.0 unx    47429 b- defN 24-Apr-07 07:47 olive/evaluator/olive_evaluator.py
--rw-rw-r--  2.0 unx      592 b- defN 24-Apr-07 07:47 olive/exception/__init__.py
--rw-rw-r--  2.0 unx      621 b- defN 24-Apr-07 07:47 olive/hardware/__init__.py
--rw-rw-r--  2.0 unx    15059 b- defN 24-Apr-07 07:47 olive/hardware/accelerator.py
--rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-07 07:47 olive/hardware/constants.py
--rw-rw-r--  2.0 unx      451 b- defN 24-Apr-07 07:47 olive/model/__init__.py
--rw-rw-r--  2.0 unx      482 b- defN 24-Apr-07 07:47 olive/model/config/__init__.py
--rw-rw-r--  2.0 unx    10950 b- defN 24-Apr-07 07:47 olive/model/config/hf_config.py
--rw-rw-r--  2.0 unx     4843 b- defN 24-Apr-07 07:47 olive/model/config/io_config.py
--rw-rw-r--  2.0 unx     3943 b- defN 24-Apr-07 07:47 olive/model/config/model_config.py
--rw-rw-r--  2.0 unx     1045 b- defN 24-Apr-07 07:47 olive/model/config/registry.py
--rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-07 07:47 olive/model/handler/__init__.py
--rw-rw-r--  2.0 unx     3190 b- defN 24-Apr-07 07:47 olive/model/handler/base.py
--rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-07 07:47 olive/model/handler/composite.py
--rw-rw-r--  2.0 unx     8706 b- defN 24-Apr-07 07:47 olive/model/handler/onnx.py
--rw-rw-r--  2.0 unx     3556 b- defN 24-Apr-07 07:47 olive/model/handler/openvino.py
--rw-rw-r--  2.0 unx    16490 b- defN 24-Apr-07 07:47 olive/model/handler/pytorch.py
--rw-rw-r--  2.0 unx     4704 b- defN 24-Apr-07 07:47 olive/model/handler/qnn.py
--rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-07 07:47 olive/model/handler/snpe.py
--rw-rw-r--  2.0 unx     1474 b- defN 24-Apr-07 07:47 olive/model/handler/tensorflow.py
--rw-rw-r--  2.0 unx      936 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/__init__.py
--rw-rw-r--  2.0 unx      418 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/composite.py
--rw-rw-r--  2.0 unx     3021 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/dummy_inputs.py
--rw-rw-r--  2.0 unx     3967 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/hf_config.py
--rw-rw-r--  2.0 unx      613 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/io_config.py
--rw-rw-r--  2.0 unx     1472 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/json.py
--rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/onnx_ep.py
--rw-rw-r--  2.0 unx     3946 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/onnx_graph.py
--rw-rw-r--  2.0 unx     2998 b- defN 24-Apr-07 07:47 olive/model/handler/mixin/resource.py
--rw-rw-r--  2.0 unx      609 b- defN 24-Apr-07 07:47 olive/model/utils/__init__.py
--rw-rw-r--  2.0 unx     3091 b- defN 24-Apr-07 07:47 olive/model/utils/hf_mappings.py
--rw-rw-r--  2.0 unx     4517 b- defN 24-Apr-07 07:47 olive/model/utils/hf_onnx_config.py
--rw-rw-r--  2.0 unx     8183 b- defN 24-Apr-07 07:47 olive/model/utils/hf_utils.py
--rw-rw-r--  2.0 unx     2893 b- defN 24-Apr-07 07:47 olive/model/utils/onnx_utils.py
--rw-rw-r--  2.0 unx     1510 b- defN 24-Apr-07 07:47 olive/model/utils/path_utils.py
--rw-rw-r--  2.0 unx      499 b- defN 24-Apr-07 07:47 olive/passes/__init__.py
--rw-rw-r--  2.0 unx    19895 b- defN 24-Apr-07 07:47 olive/passes/olive_pass.py
--rw-rw-r--  2.0 unx     6139 b- defN 24-Apr-07 07:47 olive/passes/pass_config.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/onnx/__init__.py
--rw-rw-r--  2.0 unx     8408 b- defN 24-Apr-07 07:47 olive/passes/onnx/append_pre_post_processing_ops.py
--rw-rw-r--  2.0 unx     5524 b- defN 24-Apr-07 07:47 olive/passes/onnx/bnb_quantization.py
--rw-rw-r--  2.0 unx     7485 b- defN 24-Apr-07 07:47 olive/passes/onnx/common.py
--rw-rw-r--  2.0 unx    27072 b- defN 24-Apr-07 07:47 olive/passes/onnx/conversion.py
--rw-rw-r--  2.0 unx     4862 b- defN 24-Apr-07 07:47 olive/passes/onnx/dynamic_to_fixed_shape.py
--rw-rw-r--  2.0 unx     3090 b- defN 24-Apr-07 07:47 olive/passes/onnx/float16_conversion.py
--rw-rw-r--  2.0 unx     3491 b- defN 24-Apr-07 07:47 olive/passes/onnx/genai_model_exporter.py
--rw-rw-r--  2.0 unx    27095 b- defN 24-Apr-07 07:47 olive/passes/onnx/inc_quantization.py
--rw-rw-r--  2.0 unx    15972 b- defN 24-Apr-07 07:47 olive/passes/onnx/insert_beam_search.py
--rw-rw-r--  2.0 unx    18495 b- defN 24-Apr-07 07:47 olive/passes/onnx/merge_decoders.py
--rw-rw-r--  2.0 unx     9054 b- defN 24-Apr-07 07:47 olive/passes/onnx/mixed_precision.py
--rw-rw-r--  2.0 unx    10011 b- defN 24-Apr-07 07:47 olive/passes/onnx/model_optimizer.py
--rw-rw-r--  2.0 unx    15752 b- defN 24-Apr-07 07:47 olive/passes/onnx/moe_experts_distributor.py
--rw-rw-r--  2.0 unx     6162 b- defN 24-Apr-07 07:47 olive/passes/onnx/optimum_conversion.py
--rw-rw-r--  2.0 unx     3709 b- defN 24-Apr-07 07:47 olive/passes/onnx/optimum_merging.py
--rw-rw-r--  2.0 unx    29003 b- defN 24-Apr-07 07:47 olive/passes/onnx/perf_tuning.py
--rw-rw-r--  2.0 unx     5375 b- defN 24-Apr-07 07:47 olive/passes/onnx/qnn_preprocess.py
--rw-rw-r--  2.0 unx    37646 b- defN 24-Apr-07 07:47 olive/passes/onnx/quantization.py
--rw-rw-r--  2.0 unx    19253 b- defN 24-Apr-07 07:47 olive/passes/onnx/transformer_optimization.py
--rw-rw-r--  2.0 unx    15134 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai_quantization.py
--rw-rw-r--  2.0 unx     3239 b- defN 24-Apr-07 07:47 olive/passes/onnx/pipeline/__init__.py
--rw-rw-r--  2.0 unx     8457 b- defN 24-Apr-07 07:47 olive/passes/onnx/pipeline/step_utils.py
--rw-rw-r--  2.0 unx      508 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/__init__.py
--rw-rw-r--  2.0 unx     7762 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/calibrate.py
--rw-rw-r--  2.0 unx    15332 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/quant_utils.py
--rw-rw-r--  2.0 unx    13580 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/quantize.py
--rw-rw-r--  2.0 unx    36359 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/quantizer.py
--rw-rw-r--  2.0 unx    18700 b- defN 24-Apr-07 07:47 olive/passes/onnx/vitis_ai/refine.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/openvino/__init__.py
--rw-rw-r--  2.0 unx     4555 b- defN 24-Apr-07 07:47 olive/passes/openvino/conversion.py
--rw-rw-r--  2.0 unx    12610 b- defN 24-Apr-07 07:47 olive/passes/openvino/quantization.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/pytorch/__init__.py
--rw-rw-r--  2.0 unx     7058 b- defN 24-Apr-07 07:47 olive/passes/pytorch/cluster.py
--rw-rw-r--  2.0 unx     9842 b- defN 24-Apr-07 07:47 olive/passes/pytorch/gptq.py
--rw-rw-r--  2.0 unx    11528 b- defN 24-Apr-07 07:47 olive/passes/pytorch/gptq_utils.py
--rw-rw-r--  2.0 unx    48812 b- defN 24-Apr-07 07:47 olive/passes/pytorch/lora.py
--rw-rw-r--  2.0 unx     1021 b- defN 24-Apr-07 07:47 olive/passes/pytorch/pytorch_lightning_utils.py
--rw-rw-r--  2.0 unx     8038 b- defN 24-Apr-07 07:47 olive/passes/pytorch/qat_utils.py
--rw-rw-r--  2.0 unx     6444 b- defN 24-Apr-07 07:47 olive/passes/pytorch/quantization_aware_training.py
--rw-rw-r--  2.0 unx     9021 b- defN 24-Apr-07 07:47 olive/passes/pytorch/sparsegpt.py
--rw-rw-r--  2.0 unx    10774 b- defN 24-Apr-07 07:47 olive/passes/pytorch/sparsegpt_utils.py
--rw-rw-r--  2.0 unx     7032 b- defN 24-Apr-07 07:47 olive/passes/pytorch/tensor_parallel.py
--rw-rw-r--  2.0 unx     5372 b- defN 24-Apr-07 07:47 olive/passes/pytorch/tensor_parallel_layers.py
--rw-rw-r--  2.0 unx    17239 b- defN 24-Apr-07 07:47 olive/passes/pytorch/tensor_parallel_llama2.py
--rw-rw-r--  2.0 unx     8053 b- defN 24-Apr-07 07:47 olive/passes/pytorch/torch_trt_conversion.py
--rw-rw-r--  2.0 unx     3185 b- defN 24-Apr-07 07:47 olive/passes/pytorch/trt_utils.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/qnn/__init__.py
--rw-rw-r--  2.0 unx     3192 b- defN 24-Apr-07 07:47 olive/passes/qnn/context_binary_generator.py
--rw-rw-r--  2.0 unx     5268 b- defN 24-Apr-07 07:47 olive/passes/qnn/conversion.py
--rw-rw-r--  2.0 unx     3298 b- defN 24-Apr-07 07:47 olive/passes/qnn/model_lib_generator.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/snpe/__init__.py
--rw-rw-r--  2.0 unx     4802 b- defN 24-Apr-07 07:47 olive/passes/snpe/conversion.py
--rw-rw-r--  2.0 unx     5254 b- defN 24-Apr-07 07:47 olive/passes/snpe/quantization.py
--rw-rw-r--  2.0 unx     2637 b- defN 24-Apr-07 07:47 olive/passes/snpe/snpe_to_onnx.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/passes/utils/__init__.py
--rw-rw-r--  2.0 unx     1619 b- defN 24-Apr-07 07:47 olive/passes/utils/whisper_prepost.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/platform_sdk/__init__.py
--rw-rw-r--  2.0 unx      341 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/__init__.py
--rw-rw-r--  2.0 unx     3740 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/configure.py
--rw-rw-r--  2.0 unx     1348 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/constants.py
--rw-rw-r--  2.0 unx     1046 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1
--rw-rw-r--  2.0 unx     2387 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/create_python_env.ps1
--rw-rw-r--  2.0 unx     2431 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/create_python_env.sh
--rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/env.py
--rw-rw-r--  2.0 unx     3652 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/runner.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/qnn/__init__.py
--rw-rw-r--  2.0 unx     2034 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/qnn/env.py
--rw-rw-r--  2.0 unx     7269 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/qnn/qnn.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/qnn/utils/__init__.py
--rw-rw-r--  2.0 unx      396 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/__init__.py
--rw-rw-r--  2.0 unx     2117 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/env.py
--rw-rw-r--  2.0 unx     3969 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/snpe.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/tools/__init__.py
--rw-rw-r--  2.0 unx    10951 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/tools/dev.py
--rw-rw-r--  2.0 unx    19039 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/tools/inference.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/utils/__init__.py
--rw-rw-r--  2.0 unx     6978 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/snpe/utils/adb.py
--rw-rw-r--  2.0 unx      374 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/utils/__init__.py
--rw-rw-r--  2.0 unx    14746 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/utils/data_loader.py
--rw-rw-r--  2.0 unx     8878 b- defN 24-Apr-07 07:47 olive/platform_sdk/qualcomm/utils/input_list.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/scripts/__init__.py
--rw-rw-r--  2.0 unx     6435 b- defN 24-Apr-07 07:47 olive/scripts/manage_compute_instance.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/strategy/__init__.py
--rw-rw-r--  2.0 unx    11837 b- defN 24-Apr-07 07:47 olive/strategy/search_parameter.py
--rw-rw-r--  2.0 unx     5631 b- defN 24-Apr-07 07:47 olive/strategy/search_results.py
--rw-rw-r--  2.0 unx     4702 b- defN 24-Apr-07 07:47 olive/strategy/search_space.py
--rw-rw-r--  2.0 unx    12873 b- defN 24-Apr-07 07:47 olive/strategy/search_strategy.py
--rw-rw-r--  2.0 unx     2817 b- defN 24-Apr-07 07:47 olive/strategy/utils.py
--rw-rw-r--  2.0 unx      705 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/__init__.py
--rw-rw-r--  2.0 unx     1091 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/exhaustive.py
--rw-rw-r--  2.0 unx     4334 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/optuna_sampler.py
--rw-rw-r--  2.0 unx     2421 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/random_sampler.py
--rw-rw-r--  2.0 unx     2306 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/search_algorithm.py
--rw-rw-r--  2.0 unx     1841 b- defN 24-Apr-07 07:47 olive/strategy/search_algorithm/tpe_sampler.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/systems/__init__.py
--rw-rw-r--  2.0 unx     2227 b- defN 24-Apr-07 07:47 olive/systems/common.py
--rw-rw-r--  2.0 unx     2300 b- defN 24-Apr-07 07:47 olive/systems/local.py
--rw-rw-r--  2.0 unx     2158 b- defN 24-Apr-07 07:47 olive/systems/olive_system.py
--rw-rw-r--  2.0 unx     3140 b- defN 24-Apr-07 07:47 olive/systems/system_alias.py
--rw-rw-r--  2.0 unx     7048 b- defN 24-Apr-07 07:47 olive/systems/system_config.py
--rw-rw-r--  2.0 unx      411 b- defN 24-Apr-07 07:47 olive/systems/azureml/__init__.py
--rw-rw-r--  2.0 unx     2883 b- defN 24-Apr-07 07:47 olive/systems/azureml/aml_evaluation_runner.py
--rw-rw-r--  2.0 unx     8763 b- defN 24-Apr-07 07:47 olive/systems/azureml/aml_pass_runner.py
--rw-rw-r--  2.0 unx    31831 b- defN 24-Apr-07 07:47 olive/systems/azureml/aml_system.py
--rw-rw-r--  2.0 unx      717 b- defN 24-Apr-07 07:47 olive/systems/docker/Dockerfile
--rw-rw-r--  2.0 unx      464 b- defN 24-Apr-07 07:47 olive/systems/docker/Dockerfile.cpu
--rw-rw-r--  2.0 unx     1006 b- defN 24-Apr-07 07:47 olive/systems/docker/Dockerfile.gpu
--rw-rw-r--  2.0 unx     2531 b- defN 24-Apr-07 07:47 olive/systems/docker/Dockerfile.openvino
--rw-rw-r--  2.0 unx      407 b- defN 24-Apr-07 07:47 olive/systems/docker/__init__.py
--rw-rw-r--  2.0 unx    18244 b- defN 24-Apr-07 07:47 olive/systems/docker/docker_system.py
--rw-rw-r--  2.0 unx     2187 b- defN 24-Apr-07 07:47 olive/systems/docker/eval.py
--rw-rw-r--  2.0 unx     1956 b- defN 24-Apr-07 07:47 olive/systems/docker/runner.py
--rw-rw-r--  2.0 unx     6200 b- defN 24-Apr-07 07:47 olive/systems/docker/utils.py
--rw-rw-r--  2.0 unx      357 b- defN 24-Apr-07 07:47 olive/systems/isolated_ort/__init__.py
--rw-rw-r--  2.0 unx     3077 b- defN 24-Apr-07 07:47 olive/systems/isolated_ort/inference_runner.py
--rw-rw-r--  2.0 unx    10877 b- defN 24-Apr-07 07:47 olive/systems/isolated_ort/isolated_ort_system.py
--rw-rw-r--  2.0 unx      381 b- defN 24-Apr-07 07:47 olive/systems/python_environment/__init__.py
--rw-rw-r--  2.0 unx       37 b- defN 24-Apr-07 07:47 olive/systems/python_environment/common_requirements.txt
--rw-rw-r--  2.0 unx     2279 b- defN 24-Apr-07 07:47 olive/systems/python_environment/evaluation_runner.py
--rw-rw-r--  2.0 unx     2037 b- defN 24-Apr-07 07:47 olive/systems/python_environment/pass_runner.py
--rw-rw-r--  2.0 unx     7892 b- defN 24-Apr-07 07:47 olive/systems/python_environment/python_environment_system.py
--rw-rw-r--  2.0 unx      705 b- defN 24-Apr-07 07:47 olive/systems/utils/__init__.py
--rw-rw-r--  2.0 unx     2082 b- defN 24-Apr-07 07:47 olive/systems/utils/arg_parser.py
--rw-rw-r--  2.0 unx      913 b- defN 24-Apr-07 07:47 olive/systems/utils/available_providers_runner.py
--rw-rw-r--  2.0 unx     7419 b- defN 24-Apr-07 07:47 olive/systems/utils/misc.py
--rw-rw-r--  2.0 unx      306 b- defN 24-Apr-07 07:47 olive/workflows/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/workflows/run/__init__.py
--rw-rw-r--  2.0 unx     1418 b- defN 24-Apr-07 07:47 olive/workflows/run/__main__.py
--rw-rw-r--  2.0 unx    13710 b- defN 24-Apr-07 07:47 olive/workflows/run/config.py
--rw-rw-r--  2.0 unx    13451 b- defN 24-Apr-07 07:47 olive/workflows/run/run.py
--rw-rw-r--  2.0 unx      431 b- defN 24-Apr-07 07:47 olive/workflows/snpe/__init__.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/workflows/snpe/convertquantize/__init__.py
--rw-rw-r--  2.0 unx     1339 b- defN 24-Apr-07 07:47 olive/workflows/snpe/convertquantize/__main__.py
--rw-rw-r--  2.0 unx     4445 b- defN 24-Apr-07 07:47 olive/workflows/snpe/convertquantize/convertquantize.py
--rw-rw-r--  2.0 unx      247 b- defN 24-Apr-07 07:47 olive/workflows/snpe/evaluate/__init__.py
--rw-rw-r--  2.0 unx      955 b- defN 24-Apr-07 07:47 olive/workflows/snpe/evaluate/__main__.py
--rw-rw-r--  2.0 unx     2974 b- defN 24-Apr-07 07:47 olive/workflows/snpe/evaluate/evaluate.py
--rw-rw-r--  2.0 unx     1141 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/LICENSE
--rw-rw-r--  2.0 unx     3438 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/METADATA
--rw-rw-r--  2.0 unx   764423 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/NOTICE.txt
--rw-rw-r--  2.0 unx       92 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/WHEEL
--rw-rw-r--  2.0 unx      101 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/entry_points.txt
--rw-rw-r--  2.0 unx        6 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    22214 b- defN 24-Apr-07 07:47 olive_ai-0.5.1.dist-info/RECORD
-240 files, 2230015 bytes uncompressed, 467757 bytes compressed:  79.0%
+Zip file size: 517025 bytes, number of entries: 244
+-rw-rw-r--  2.0 unx      608 b- defN 24-Apr-11 05:46 olive/__init__.py
+-rw-rw-r--  2.0 unx     9998 b- defN 24-Apr-11 05:46 olive/cache.py
+-rw-rw-r--  2.0 unx     1162 b- defN 24-Apr-11 05:46 olive/constants.py
+-rw-rw-r--  2.0 unx     2626 b- defN 24-Apr-11 05:46 olive/logging.py
+-rw-rw-r--  2.0 unx     8038 b- defN 24-Apr-11 05:46 olive/olive_config.json
+-rw-rw-r--  2.0 unx     1406 b- defN 24-Apr-11 05:46 olive/package_config.py
+-rw-rw-r--  2.0 unx    22999 b- defN 24-Apr-11 05:46 olive/resource_path.py
+-rw-rw-r--  2.0 unx     5181 b- defN 24-Apr-11 05:46 olive/auto_optimizer/__init__.py
+-rw-rw-r--  2.0 unx     5871 b- defN 24-Apr-11 05:46 olive/auto_optimizer/regulate_mixins.py
+-rw-rw-r--  2.0 unx     3615 b- defN 24-Apr-11 05:46 olive/auto_optimizer/template_mapping.py
+-rw-rw-r--  2.0 unx     1171 b- defN 24-Apr-11 05:46 olive/auto_optimizer/config_template/opt_level_passes.yaml
+-rw-rw-r--  2.0 unx     2062 b- defN 24-Apr-11 05:46 olive/auto_optimizer/config_template/pass_capability.yaml
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/azureml/__init__.py
+-rw-rw-r--  2.0 unx     6699 b- defN 24-Apr-11 05:46 olive/azureml/azureml_client.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/common/__init__.py
+-rw-rw-r--  2.0 unx     3430 b- defN 24-Apr-11 05:46 olive/common/auto_config.py
+-rw-rw-r--  2.0 unx    10881 b- defN 24-Apr-11 05:46 olive/common/config_utils.py
+-rw-rw-r--  2.0 unx     1488 b- defN 24-Apr-11 05:46 olive/common/import_lib.py
+-rw-rw-r--  2.0 unx    18360 b- defN 24-Apr-11 05:46 olive/common/ort_inference.py
+-rw-rw-r--  2.0 unx      765 b- defN 24-Apr-11 05:46 olive/common/pydantic_v1.py
+-rw-rw-r--  2.0 unx     1809 b- defN 24-Apr-11 05:46 olive/common/user_module_loader.py
+-rw-rw-r--  2.0 unx    11789 b- defN 24-Apr-11 05:46 olive/common/utils.py
+-rw-rw-r--  2.0 unx      345 b- defN 24-Apr-11 05:46 olive/data/__init__.py
+-rw-rw-r--  2.0 unx    10680 b- defN 24-Apr-11 05:46 olive/data/config.py
+-rw-rw-r--  2.0 unx     1443 b- defN 24-Apr-11 05:46 olive/data/constants.py
+-rw-rw-r--  2.0 unx     8119 b- defN 24-Apr-11 05:46 olive/data/registry.py
+-rw-rw-r--  2.0 unx     3573 b- defN 24-Apr-11 05:46 olive/data/template.py
+-rw-rw-r--  2.0 unx      444 b- defN 24-Apr-11 05:46 olive/data/component/__init__.py
+-rw-rw-r--  2.0 unx     1955 b- defN 24-Apr-11 05:46 olive/data/component/dataloader.py
+-rw-rw-r--  2.0 unx    10679 b- defN 24-Apr-11 05:46 olive/data/component/dataset.py
+-rw-rw-r--  2.0 unx     1928 b- defN 24-Apr-11 05:46 olive/data/component/load_dataset.py
+-rw-rw-r--  2.0 unx     2256 b- defN 24-Apr-11 05:46 olive/data/component/post_process_data.py
+-rw-rw-r--  2.0 unx    11446 b- defN 24-Apr-11 05:46 olive/data/component/pre_process_data.py
+-rw-rw-r--  2.0 unx    29278 b- defN 24-Apr-11 05:46 olive/data/component/text_generation.py
+-rw-rw-r--  2.0 unx      480 b- defN 24-Apr-11 05:46 olive/data/container/__init__.py
+-rw-rw-r--  2.0 unx     3385 b- defN 24-Apr-11 05:46 olive/data/container/data_container.py
+-rw-rw-r--  2.0 unx     1159 b- defN 24-Apr-11 05:46 olive/data/container/dummy_data_container.py
+-rw-rw-r--  2.0 unx     1690 b- defN 24-Apr-11 05:46 olive/data/container/huggingface_container.py
+-rw-rw-r--  2.0 unx     1721 b- defN 24-Apr-11 05:46 olive/data/container/raw_data_container.py
+-rw-rw-r--  2.0 unx      442 b- defN 24-Apr-11 05:46 olive/engine/__init__.py
+-rw-rw-r--  2.0 unx     1199 b- defN 24-Apr-11 05:46 olive/engine/config.py
+-rw-rw-r--  2.0 unx    45969 b- defN 24-Apr-11 05:46 olive/engine/engine.py
+-rw-rw-r--  2.0 unx    17410 b- defN 24-Apr-11 05:46 olive/engine/footprint.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/engine/packaging/__init__.py
+-rw-rw-r--  2.0 unx     1642 b- defN 24-Apr-11 05:46 olive/engine/packaging/packaging_config.py
+-rw-rw-r--  2.0 unx    19748 b- defN 24-Apr-11 05:46 olive/engine/packaging/packaging_generator.py
+-rw-rw-r--  2.0 unx     1588 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md
+-rw-rw-r--  2.0 unx     4990 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp
+-rw-rw-r--  2.0 unx     1590 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cs/README.md
+-rw-rw-r--  2.0 unx     4991 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/cs/code_sample.cs
+-rw-rw-r--  2.0 unx     2296 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/python/README.md
+-rw-rw-r--  2.0 unx     2545 b- defN 24-Apr-11 05:46 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/evaluator/__init__.py
+-rw-rw-r--  2.0 unx     6473 b- defN 24-Apr-11 05:46 olive/evaluator/accuracy.py
+-rw-rw-r--  2.0 unx     8723 b- defN 24-Apr-11 05:46 olive/evaluator/metric.py
+-rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-11 05:46 olive/evaluator/metric_backend.py
+-rw-rw-r--  2.0 unx     4395 b- defN 24-Apr-11 05:46 olive/evaluator/metric_config.py
+-rw-rw-r--  2.0 unx    47694 b- defN 24-Apr-11 05:46 olive/evaluator/olive_evaluator.py
+-rw-rw-r--  2.0 unx      592 b- defN 24-Apr-11 05:46 olive/exception/__init__.py
+-rw-rw-r--  2.0 unx      621 b- defN 24-Apr-11 05:46 olive/hardware/__init__.py
+-rw-rw-r--  2.0 unx    15059 b- defN 24-Apr-11 05:46 olive/hardware/accelerator.py
+-rw-rw-r--  2.0 unx     1273 b- defN 24-Apr-11 05:46 olive/hardware/constants.py
+-rw-rw-r--  2.0 unx      451 b- defN 24-Apr-11 05:46 olive/model/__init__.py
+-rw-rw-r--  2.0 unx      482 b- defN 24-Apr-11 05:46 olive/model/config/__init__.py
+-rw-rw-r--  2.0 unx    10950 b- defN 24-Apr-11 05:46 olive/model/config/hf_config.py
+-rw-rw-r--  2.0 unx     4843 b- defN 24-Apr-11 05:46 olive/model/config/io_config.py
+-rw-rw-r--  2.0 unx     3943 b- defN 24-Apr-11 05:46 olive/model/config/model_config.py
+-rw-rw-r--  2.0 unx     1045 b- defN 24-Apr-11 05:46 olive/model/config/registry.py
+-rw-rw-r--  2.0 unx     1139 b- defN 24-Apr-11 05:46 olive/model/handler/__init__.py
+-rw-rw-r--  2.0 unx     3190 b- defN 24-Apr-11 05:46 olive/model/handler/base.py
+-rw-rw-r--  2.0 unx     4461 b- defN 24-Apr-11 05:46 olive/model/handler/composite.py
+-rw-rw-r--  2.0 unx    10069 b- defN 24-Apr-11 05:46 olive/model/handler/onnx.py
+-rw-rw-r--  2.0 unx     3556 b- defN 24-Apr-11 05:46 olive/model/handler/openvino.py
+-rw-rw-r--  2.0 unx    16898 b- defN 24-Apr-11 05:46 olive/model/handler/pytorch.py
+-rw-rw-r--  2.0 unx     4704 b- defN 24-Apr-11 05:46 olive/model/handler/qnn.py
+-rw-rw-r--  2.0 unx     2597 b- defN 24-Apr-11 05:46 olive/model/handler/snpe.py
+-rw-rw-r--  2.0 unx     1474 b- defN 24-Apr-11 05:46 olive/model/handler/tensorflow.py
+-rw-rw-r--  2.0 unx      936 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/__init__.py
+-rw-rw-r--  2.0 unx      418 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/composite.py
+-rw-rw-r--  2.0 unx     3021 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/dummy_inputs.py
+-rw-rw-r--  2.0 unx     3967 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/hf_config.py
+-rw-rw-r--  2.0 unx      613 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/io_config.py
+-rw-rw-r--  2.0 unx     1472 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/json.py
+-rw-rw-r--  2.0 unx     1402 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/onnx_ep.py
+-rw-rw-r--  2.0 unx     3946 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/onnx_graph.py
+-rw-rw-r--  2.0 unx     2998 b- defN 24-Apr-11 05:46 olive/model/handler/mixin/resource.py
+-rw-rw-r--  2.0 unx      609 b- defN 24-Apr-11 05:46 olive/model/utils/__init__.py
+-rw-rw-r--  2.0 unx     3091 b- defN 24-Apr-11 05:46 olive/model/utils/hf_mappings.py
+-rw-rw-r--  2.0 unx     4517 b- defN 24-Apr-11 05:46 olive/model/utils/hf_onnx_config.py
+-rw-rw-r--  2.0 unx     8183 b- defN 24-Apr-11 05:46 olive/model/utils/hf_utils.py
+-rw-rw-r--  2.0 unx     3467 b- defN 24-Apr-11 05:46 olive/model/utils/onnx_utils.py
+-rw-rw-r--  2.0 unx     1510 b- defN 24-Apr-11 05:46 olive/model/utils/path_utils.py
+-rw-rw-r--  2.0 unx      499 b- defN 24-Apr-11 05:46 olive/passes/__init__.py
+-rw-rw-r--  2.0 unx    19895 b- defN 24-Apr-11 05:46 olive/passes/olive_pass.py
+-rw-rw-r--  2.0 unx     6139 b- defN 24-Apr-11 05:46 olive/passes/pass_config.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/onnx/__init__.py
+-rw-rw-r--  2.0 unx     8408 b- defN 24-Apr-11 05:46 olive/passes/onnx/append_pre_post_processing_ops.py
+-rw-rw-r--  2.0 unx     5524 b- defN 24-Apr-11 05:46 olive/passes/onnx/bnb_quantization.py
+-rw-rw-r--  2.0 unx     7639 b- defN 24-Apr-11 05:46 olive/passes/onnx/common.py
+-rw-rw-r--  2.0 unx    27526 b- defN 24-Apr-11 05:46 olive/passes/onnx/conversion.py
+-rw-rw-r--  2.0 unx     4862 b- defN 24-Apr-11 05:46 olive/passes/onnx/dynamic_to_fixed_shape.py
+-rw-rw-r--  2.0 unx    14055 b- defN 24-Apr-11 05:46 olive/passes/onnx/extract_adapters.py
+-rw-rw-r--  2.0 unx     3090 b- defN 24-Apr-11 05:46 olive/passes/onnx/float16_conversion.py
+-rw-rw-r--  2.0 unx     4556 b- defN 24-Apr-11 05:46 olive/passes/onnx/genai_model_exporter.py
+-rw-rw-r--  2.0 unx    27096 b- defN 24-Apr-11 05:46 olive/passes/onnx/inc_quantization.py
+-rw-rw-r--  2.0 unx    15972 b- defN 24-Apr-11 05:46 olive/passes/onnx/insert_beam_search.py
+-rw-rw-r--  2.0 unx    18495 b- defN 24-Apr-11 05:46 olive/passes/onnx/merge_decoders.py
+-rw-rw-r--  2.0 unx     9054 b- defN 24-Apr-11 05:46 olive/passes/onnx/mixed_precision.py
+-rw-rw-r--  2.0 unx    10011 b- defN 24-Apr-11 05:46 olive/passes/onnx/model_optimizer.py
+-rw-rw-r--  2.0 unx    15752 b- defN 24-Apr-11 05:46 olive/passes/onnx/moe_experts_distributor.py
+-rw-rw-r--  2.0 unx    18666 b- defN 24-Apr-11 05:46 olive/passes/onnx/onnx_dag.py
+-rw-rw-r--  2.0 unx     6162 b- defN 24-Apr-11 05:46 olive/passes/onnx/optimum_conversion.py
+-rw-rw-r--  2.0 unx     3709 b- defN 24-Apr-11 05:46 olive/passes/onnx/optimum_merging.py
+-rw-rw-r--  2.0 unx    29003 b- defN 24-Apr-11 05:46 olive/passes/onnx/perf_tuning.py
+-rw-rw-r--  2.0 unx     5375 b- defN 24-Apr-11 05:46 olive/passes/onnx/qnn_preprocess.py
+-rw-rw-r--  2.0 unx    37566 b- defN 24-Apr-11 05:46 olive/passes/onnx/quantization.py
+-rw-rw-r--  2.0 unx    19292 b- defN 24-Apr-11 05:46 olive/passes/onnx/transformer_optimization.py
+-rw-rw-r--  2.0 unx    15105 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai_quantization.py
+-rw-rw-r--  2.0 unx     3239 b- defN 24-Apr-11 05:46 olive/passes/onnx/pipeline/__init__.py
+-rw-rw-r--  2.0 unx     8457 b- defN 24-Apr-11 05:46 olive/passes/onnx/pipeline/step_utils.py
+-rw-rw-r--  2.0 unx      508 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/__init__.py
+-rw-rw-r--  2.0 unx     7762 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/calibrate.py
+-rw-rw-r--  2.0 unx    15332 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quant_utils.py
+-rw-rw-r--  2.0 unx    13580 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quantize.py
+-rw-rw-r--  2.0 unx    36359 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/quantizer.py
+-rw-rw-r--  2.0 unx    18700 b- defN 24-Apr-11 05:46 olive/passes/onnx/vitis_ai/refine.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/openvino/__init__.py
+-rw-rw-r--  2.0 unx     4555 b- defN 24-Apr-11 05:46 olive/passes/openvino/conversion.py
+-rw-rw-r--  2.0 unx    12610 b- defN 24-Apr-11 05:46 olive/passes/openvino/quantization.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/pytorch/__init__.py
+-rw-rw-r--  2.0 unx     7058 b- defN 24-Apr-11 05:46 olive/passes/pytorch/cluster.py
+-rw-rw-r--  2.0 unx     9842 b- defN 24-Apr-11 05:46 olive/passes/pytorch/gptq.py
+-rw-rw-r--  2.0 unx    11528 b- defN 24-Apr-11 05:46 olive/passes/pytorch/gptq_utils.py
+-rw-rw-r--  2.0 unx    48812 b- defN 24-Apr-11 05:46 olive/passes/pytorch/lora.py
+-rw-rw-r--  2.0 unx     1021 b- defN 24-Apr-11 05:46 olive/passes/pytorch/pytorch_lightning_utils.py
+-rw-rw-r--  2.0 unx     8038 b- defN 24-Apr-11 05:46 olive/passes/pytorch/qat_utils.py
+-rw-rw-r--  2.0 unx     6444 b- defN 24-Apr-11 05:46 olive/passes/pytorch/quantization_aware_training.py
+-rw-rw-r--  2.0 unx     7085 b- defN 24-Apr-11 05:46 olive/passes/pytorch/slicegpt.py
+-rw-rw-r--  2.0 unx     9021 b- defN 24-Apr-11 05:46 olive/passes/pytorch/sparsegpt.py
+-rw-rw-r--  2.0 unx    10774 b- defN 24-Apr-11 05:46 olive/passes/pytorch/sparsegpt_utils.py
+-rw-rw-r--  2.0 unx     7032 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel.py
+-rw-rw-r--  2.0 unx     5372 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel_layers.py
+-rw-rw-r--  2.0 unx    17239 b- defN 24-Apr-11 05:46 olive/passes/pytorch/tensor_parallel_llama2.py
+-rw-rw-r--  2.0 unx     8172 b- defN 24-Apr-11 05:46 olive/passes/pytorch/torch_trt_conversion.py
+-rw-rw-r--  2.0 unx     3185 b- defN 24-Apr-11 05:46 olive/passes/pytorch/trt_utils.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/qnn/__init__.py
+-rw-rw-r--  2.0 unx     3192 b- defN 24-Apr-11 05:46 olive/passes/qnn/context_binary_generator.py
+-rw-rw-r--  2.0 unx     5268 b- defN 24-Apr-11 05:46 olive/passes/qnn/conversion.py
+-rw-rw-r--  2.0 unx     3298 b- defN 24-Apr-11 05:46 olive/passes/qnn/model_lib_generator.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/snpe/__init__.py
+-rw-rw-r--  2.0 unx     4802 b- defN 24-Apr-11 05:46 olive/passes/snpe/conversion.py
+-rw-rw-r--  2.0 unx     5254 b- defN 24-Apr-11 05:46 olive/passes/snpe/quantization.py
+-rw-rw-r--  2.0 unx     2637 b- defN 24-Apr-11 05:46 olive/passes/snpe/snpe_to_onnx.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/passes/utils/__init__.py
+-rw-rw-r--  2.0 unx     1619 b- defN 24-Apr-11 05:46 olive/passes/utils/whisper_prepost.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/__init__.py
+-rw-rw-r--  2.0 unx      341 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/__init__.py
+-rw-rw-r--  2.0 unx     3740 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/configure.py
+-rw-rw-r--  2.0 unx     1348 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/constants.py
+-rw-rw-r--  2.0 unx     1046 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/copy_libcdsprpc.ps1
+-rw-rw-r--  2.0 unx     2387 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/create_python_env.ps1
+-rw-rw-r--  2.0 unx     2431 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/create_python_env.sh
+-rw-rw-r--  2.0 unx     4034 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/env.py
+-rw-rw-r--  2.0 unx     3652 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/runner.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/__init__.py
+-rw-rw-r--  2.0 unx     2034 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/env.py
+-rw-rw-r--  2.0 unx     7269 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/qnn.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/qnn/utils/__init__.py
+-rw-rw-r--  2.0 unx      396 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/__init__.py
+-rw-rw-r--  2.0 unx     2117 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/env.py
+-rw-rw-r--  2.0 unx     3969 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/snpe.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/__init__.py
+-rw-rw-r--  2.0 unx    10951 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/dev.py
+-rw-rw-r--  2.0 unx    19039 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/tools/inference.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/utils/__init__.py
+-rw-rw-r--  2.0 unx     6978 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/snpe/utils/adb.py
+-rw-rw-r--  2.0 unx      374 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/__init__.py
+-rw-rw-r--  2.0 unx    14746 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/data_loader.py
+-rw-rw-r--  2.0 unx     8878 b- defN 24-Apr-11 05:46 olive/platform_sdk/qualcomm/utils/input_list.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/scripts/__init__.py
+-rw-rw-r--  2.0 unx     3130 b- defN 24-Apr-11 05:46 olive/scripts/export_adapters.py
+-rw-rw-r--  2.0 unx     6435 b- defN 24-Apr-11 05:46 olive/scripts/manage_compute_instance.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/strategy/__init__.py
+-rw-rw-r--  2.0 unx    11837 b- defN 24-Apr-11 05:46 olive/strategy/search_parameter.py
+-rw-rw-r--  2.0 unx     5631 b- defN 24-Apr-11 05:46 olive/strategy/search_results.py
+-rw-rw-r--  2.0 unx     4702 b- defN 24-Apr-11 05:46 olive/strategy/search_space.py
+-rw-rw-r--  2.0 unx    12873 b- defN 24-Apr-11 05:46 olive/strategy/search_strategy.py
+-rw-rw-r--  2.0 unx     2817 b- defN 24-Apr-11 05:46 olive/strategy/utils.py
+-rw-rw-r--  2.0 unx      705 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/__init__.py
+-rw-rw-r--  2.0 unx     1091 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/exhaustive.py
+-rw-rw-r--  2.0 unx     4334 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/optuna_sampler.py
+-rw-rw-r--  2.0 unx     2421 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/random_sampler.py
+-rw-rw-r--  2.0 unx     2306 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/search_algorithm.py
+-rw-rw-r--  2.0 unx     1841 b- defN 24-Apr-11 05:46 olive/strategy/search_algorithm/tpe_sampler.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/systems/__init__.py
+-rw-rw-r--  2.0 unx     2227 b- defN 24-Apr-11 05:46 olive/systems/common.py
+-rw-rw-r--  2.0 unx     2300 b- defN 24-Apr-11 05:46 olive/systems/local.py
+-rw-rw-r--  2.0 unx     2158 b- defN 24-Apr-11 05:46 olive/systems/olive_system.py
+-rw-rw-r--  2.0 unx     3140 b- defN 24-Apr-11 05:46 olive/systems/system_alias.py
+-rw-rw-r--  2.0 unx     7048 b- defN 24-Apr-11 05:46 olive/systems/system_config.py
+-rw-rw-r--  2.0 unx      411 b- defN 24-Apr-11 05:46 olive/systems/azureml/__init__.py
+-rw-rw-r--  2.0 unx     2883 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_evaluation_runner.py
+-rw-rw-r--  2.0 unx     8763 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_pass_runner.py
+-rw-rw-r--  2.0 unx    32108 b- defN 24-Apr-11 05:46 olive/systems/azureml/aml_system.py
+-rw-rw-r--  2.0 unx      717 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile
+-rw-rw-r--  2.0 unx      464 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.cpu
+-rw-rw-r--  2.0 unx     1006 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.gpu
+-rw-rw-r--  2.0 unx     2531 b- defN 24-Apr-11 05:46 olive/systems/docker/Dockerfile.openvino
+-rw-rw-r--  2.0 unx      407 b- defN 24-Apr-11 05:46 olive/systems/docker/__init__.py
+-rw-rw-r--  2.0 unx    18244 b- defN 24-Apr-11 05:46 olive/systems/docker/docker_system.py
+-rw-rw-r--  2.0 unx     2187 b- defN 24-Apr-11 05:46 olive/systems/docker/eval.py
+-rw-rw-r--  2.0 unx     1956 b- defN 24-Apr-11 05:46 olive/systems/docker/runner.py
+-rw-rw-r--  2.0 unx     6200 b- defN 24-Apr-11 05:46 olive/systems/docker/utils.py
+-rw-rw-r--  2.0 unx      357 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/__init__.py
+-rw-rw-r--  2.0 unx     3600 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/inference_runner.py
+-rw-rw-r--  2.0 unx    11269 b- defN 24-Apr-11 05:46 olive/systems/isolated_ort/isolated_ort_system.py
+-rw-rw-r--  2.0 unx      381 b- defN 24-Apr-11 05:46 olive/systems/python_environment/__init__.py
+-rw-rw-r--  2.0 unx       37 b- defN 24-Apr-11 05:46 olive/systems/python_environment/common_requirements.txt
+-rw-rw-r--  2.0 unx     2279 b- defN 24-Apr-11 05:46 olive/systems/python_environment/evaluation_runner.py
+-rw-rw-r--  2.0 unx     2037 b- defN 24-Apr-11 05:46 olive/systems/python_environment/pass_runner.py
+-rw-rw-r--  2.0 unx     7892 b- defN 24-Apr-11 05:46 olive/systems/python_environment/python_environment_system.py
+-rw-rw-r--  2.0 unx      705 b- defN 24-Apr-11 05:46 olive/systems/utils/__init__.py
+-rw-rw-r--  2.0 unx     2082 b- defN 24-Apr-11 05:46 olive/systems/utils/arg_parser.py
+-rw-rw-r--  2.0 unx      913 b- defN 24-Apr-11 05:46 olive/systems/utils/available_providers_runner.py
+-rw-rw-r--  2.0 unx     7419 b- defN 24-Apr-11 05:46 olive/systems/utils/misc.py
+-rw-rw-r--  2.0 unx      306 b- defN 24-Apr-11 05:46 olive/workflows/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/run/__init__.py
+-rw-rw-r--  2.0 unx     1418 b- defN 24-Apr-11 05:46 olive/workflows/run/__main__.py
+-rw-rw-r--  2.0 unx    13473 b- defN 24-Apr-11 05:46 olive/workflows/run/config.py
+-rw-rw-r--  2.0 unx    13365 b- defN 24-Apr-11 05:46 olive/workflows/run/run.py
+-rw-rw-r--  2.0 unx      431 b- defN 24-Apr-11 05:46 olive/workflows/snpe/__init__.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/__init__.py
+-rw-rw-r--  2.0 unx     1339 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/__main__.py
+-rw-rw-r--  2.0 unx     4445 b- defN 24-Apr-11 05:46 olive/workflows/snpe/convertquantize/convertquantize.py
+-rw-rw-r--  2.0 unx      247 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/__init__.py
+-rw-rw-r--  2.0 unx      955 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/__main__.py
+-rw-rw-r--  2.0 unx     2974 b- defN 24-Apr-11 05:46 olive/workflows/snpe/evaluate/evaluate.py
+-rw-rw-r--  2.0 unx     1141 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     3438 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/METADATA
+-rw-rw-r--  2.0 unx   764423 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/NOTICE.txt
+-rw-rw-r--  2.0 unx       92 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/WHEEL
+-rw-rw-r--  2.0 unx      101 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/entry_points.txt
+-rw-rw-r--  2.0 unx        6 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    22575 b- defN 24-Apr-11 05:46 olive_ai-0.5.2.dist-info/RECORD
+244 files, 2280681 bytes uncompressed, 480997 bytes compressed:  78.9%
```

## zipnote {}

```diff
@@ -297,14 +297,17 @@
 
 Filename: olive/passes/onnx/conversion.py
 Comment: 
 
 Filename: olive/passes/onnx/dynamic_to_fixed_shape.py
 Comment: 
 
+Filename: olive/passes/onnx/extract_adapters.py
+Comment: 
+
 Filename: olive/passes/onnx/float16_conversion.py
 Comment: 
 
 Filename: olive/passes/onnx/genai_model_exporter.py
 Comment: 
 
 Filename: olive/passes/onnx/inc_quantization.py
@@ -321,14 +324,17 @@
 
 Filename: olive/passes/onnx/model_optimizer.py
 Comment: 
 
 Filename: olive/passes/onnx/moe_experts_distributor.py
 Comment: 
 
+Filename: olive/passes/onnx/onnx_dag.py
+Comment: 
+
 Filename: olive/passes/onnx/optimum_conversion.py
 Comment: 
 
 Filename: olive/passes/onnx/optimum_merging.py
 Comment: 
 
 Filename: olive/passes/onnx/perf_tuning.py
@@ -399,14 +405,17 @@
 
 Filename: olive/passes/pytorch/qat_utils.py
 Comment: 
 
 Filename: olive/passes/pytorch/quantization_aware_training.py
 Comment: 
 
+Filename: olive/passes/pytorch/slicegpt.py
+Comment: 
+
 Filename: olive/passes/pytorch/sparsegpt.py
 Comment: 
 
 Filename: olive/passes/pytorch/sparsegpt_utils.py
 Comment: 
 
 Filename: olive/passes/pytorch/tensor_parallel.py
@@ -525,14 +534,17 @@
 
 Filename: olive/platform_sdk/qualcomm/utils/input_list.py
 Comment: 
 
 Filename: olive/scripts/__init__.py
 Comment: 
 
+Filename: olive/scripts/export_adapters.py
+Comment: 
+
 Filename: olive/scripts/manage_compute_instance.py
 Comment: 
 
 Filename: olive/strategy/__init__.py
 Comment: 
 
 Filename: olive/strategy/search_parameter.py
@@ -693,29 +705,29 @@
 
 Filename: olive/workflows/snpe/evaluate/__main__.py
 Comment: 
 
 Filename: olive/workflows/snpe/evaluate/evaluate.py
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/LICENSE
+Filename: olive_ai-0.5.2.dist-info/LICENSE
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/METADATA
+Filename: olive_ai-0.5.2.dist-info/METADATA
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/NOTICE.txt
+Filename: olive_ai-0.5.2.dist-info/NOTICE.txt
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/WHEEL
+Filename: olive_ai-0.5.2.dist-info/WHEEL
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/entry_points.txt
+Filename: olive_ai-0.5.2.dist-info/entry_points.txt
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/top_level.txt
+Filename: olive_ai-0.5.2.dist-info/top_level.txt
 Comment: 
 
-Filename: olive_ai-0.5.1.dist-info/RECORD
+Filename: olive_ai-0.5.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## olive/__init__.py

```diff
@@ -10,8 +10,8 @@
 
 _sc = logging.StreamHandler(stream=sys.stdout)
 _formatter = logging.Formatter("[%(asctime)s] [%(levelname)s] [%(filename)s:%(lineno)d:%(funcName)s] %(message)s")
 _sc.setFormatter(_formatter)
 _logger.addHandler(_sc)
 _logger.propagate = False
 
-__version__ = "0.5.1"
+__version__ = "0.5.2"
```

## olive/constants.py

```diff
@@ -20,14 +20,15 @@
     """Given a framework, there might be 1 or more on-disk model file format(s), model save/Load logic may differ."""
 
     ONNX = "ONNX"
     PYTORCH_ENTIRE_MODEL = "PyTorch.EntireModel"
     PYTORCH_STATE_DICT = "PyTorch.StateDict"
     PYTORCH_TORCH_SCRIPT = "PyTorch.TorchScript"
     PYTORCH_MLFLOW_MODEL = "PyTorch.MLflow"
+    PYTORCH_SLICE_GPT_MODEL = "PyTorch.SliceGPT"
     TENSORFLOW_PROTOBUF = "TensorFlow.Protobuf"
     TENSORFLOW_SAVED_MODEL = "TensorFlow.SavedModel"
     SNPE_DLC = "SNPE.DLC"
     QNN_CPP = "QNN.CPP"
     QNN_LIB = "QNN.LIB"
     QNN_SERIALIZED_BIN = "QNN.SERIALIZED.BIN"
     OPENVINO_IR = "OpenVINO.IR"
```

## olive/olive_config.json

### Pretty-printed

 * *Similarity: 0.9891304347826086%*

 * *Differences: {"'passes'": "{'ExtractAdapters': OrderedDict([('module_path', "*

 * *             "'olive.passes.onnx.extract_adapters.ExtractAdapters')]), 'SliceGPT': "*

 * *             "OrderedDict([('module_path', 'olive.passes.pytorch.slicegpt.SliceGPT')])}"}*

```diff
@@ -56,14 +56,17 @@
     "passes": {
         "AppendPrePostProcessingOps": {
             "module_path": "olive.passes.onnx.append_pre_post_processing_ops.AppendPrePostProcessingOps"
         },
         "DynamicToFixedShape": {
             "module_path": "olive.passes.onnx.dynamic_to_fixed_shape.DynamicToFixedShape"
         },
+        "ExtractAdapters": {
+            "module_path": "olive.passes.onnx.extract_adapters.ExtractAdapters"
+        },
         "GenAIModelExporter": {
             "module_path": "olive.passes.onnx.genai_model_exporter.GenAIModelExporter"
         },
         "GptqQuantizer": {
             "module_dependencies": [
                 "auto-gptq",
                 "optimum"
@@ -205,14 +208,17 @@
         },
         "SNPEQuantization": {
             "module_path": "olive.passes.snpe.quantization.SNPEQuantization"
         },
         "SNPEtoONNXConversion": {
             "module_path": "olive.passes.snpe.snpe_to_onnx.SNPEtoONNXConversion"
         },
+        "SliceGPT": {
+            "module_path": "olive.passes.pytorch.slicegpt.SliceGPT"
+        },
         "SparseGPT": {
             "module_path": "olive.passes.pytorch.sparsegpt.SparseGPT"
         },
         "TorchTRTConversion": {
             "extra_dependencies": [
                 "torch-tensorrt"
             ],
```

## olive/azureml/azureml_client.py

```diff
@@ -76,17 +76,15 @@
                 "workspace_name": self.workspace_name,
             }
 
     def create_client(self):
         """Create an MLClient instance."""
         from azure.ai.ml import MLClient
 
-        # set logger level to error to avoid too many logs from azure sdk
-        logging.getLogger("azure.ai.ml").setLevel(logging.ERROR)
-        logging.getLogger("azure.identity").setLevel(logging.ERROR)
+        set_azure_logging_if_noset()
 
         if self.aml_config_path is None:
             if self.subscription_id is None:
                 raise ValueError("subscription_id must be provided if aml_config_path is not provided")
             if self.resource_group is None:
                 raise ValueError("resource_group must be provided if aml_config_path is not provided")
             if self.workspace_name is None:
@@ -105,17 +103,15 @@
                 read_timeout=self.read_timeout,
             )
 
     def create_registry_client(self, registry_name: str):
         """Create an MLClient instance."""
         from azure.ai.ml import MLClient
 
-        # set logger level to error to avoid too many logs from azure sdk
-        logging.getLogger("azure.ai.ml").setLevel(logging.ERROR)
-        logging.getLogger("azure.identity").setLevel(logging.ERROR)
+        set_azure_logging_if_noset()
 
         return MLClient(credential=self._get_credentials(), registry_name=registry_name)
 
     def _get_credentials(self):
         """Get credentials for MLClient.
 
         Order of credential providers:
@@ -129,12 +125,24 @@
         try:
             default_auth_params = self.default_auth_params or {}
             credential = DefaultAzureCredential(**default_auth_params)
             # Check if given credential can get token successfully.
             credential.get_token("https://management.azure.com/.default")
             logger.debug("Using DefaultAzureCredential")
         except Exception:
+            logger.warning("Using InteractiveBrowserCredential since of default credential errors", exc_info=True)
             # Fall back to InteractiveBrowserCredential in case DefaultAzureCredential not work
             credential = InteractiveBrowserCredential()
-            logger.debug("Using InteractiveBrowserCredential")
 
         return credential
+
+
+def set_azure_logging_if_noset():
+    # set logger level to error to avoid too many logs from azure sdk
+    azure_ml_logger = logging.getLogger("azure.ai.ml")
+    # only set the level if it is not set, to avoid changing the level set by the user
+    if not azure_ml_logger.level:
+        azure_ml_logger.setLevel(logging.ERROR)
+    azure_identity_logger = logging.getLogger("azure.identity")
+    # only set the level if it is not set, to avoid changing the level set by the user
+    if not azure_identity_logger.level:
+        azure_identity_logger.setLevel(logging.ERROR)
```

## olive/common/ort_inference.py

```diff
@@ -10,14 +10,15 @@
 import time
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, Optional, Sequence, Tuple, Union
 
 import numpy as np
 
 if TYPE_CHECKING:
+    from numpy.typing import NDArray
     from onnxruntime import InferenceSession, IOBinding
 
 
 logger = logging.getLogger(__name__)
 
 
 class OrtSessionFallbackError(Exception):
@@ -28,34 +29,49 @@
 # For regular ONNX models, the recommended way to specify the device is to set the environment variable
 # `CUDA_VISIBLE_DEVICES` before runnning a workflow.
 def get_ort_inference_session(
     model_path: Union[Path, str],
     inference_settings: Dict[str, Any],
     use_ort_extensions: bool = False,
     device_id: Optional[int] = None,
+    external_initializers: Optional[Dict[str, "NDArray"]] = None,
 ):
     """Get an ONNXRuntime inference session.
 
     :param model_path: Path to the ONNX model file.
     :param inference_settings: Inference settings for the session.
         session_options: dict, optional. Session options for the session.
         execution_provider: list. List of execution providers to use. Can be a list of provider names or a list of
             (provider name, provider options) tuples.
         provider_options: list, optional. List of provider options for the execution providers.
     :param use_ort_extensions: Whether to use onnxruntime-extensions. Default is False.
     :param device_id: Optional device id to use for CUDA or DML execution providers.
+    :param external_initializers: Optional external initializers for the session. A dictionary of external initializer
+        names and numpy arrays.
     """
     import onnxruntime as ort
 
     sess_options = ort.SessionOptions()
     if use_ort_extensions:
         # register custom ops for onnxruntime-extensions
         from onnxruntime_extensions import get_library_path
 
         sess_options.register_custom_ops_library(get_library_path())
+    if external_initializers:
+        from onnxruntime import OrtValue
+
+        # convert external initializers to OrtValue
+        initializer_names = []
+        initializer_values = []
+        for name, value in external_initializers.items():
+            initializer_names.append(name)
+            initializer_values.append(OrtValue.ortvalue_from_numpy(value))
+
+        # add external initializers to the session
+        sess_options.add_external_initializers(initializer_names, initializer_values)
 
     logger.debug("inference_settings: %s", inference_settings)
 
     # session options
     session_options = inference_settings.get("session_options", {})
     inter_op_num_threads = session_options.get("inter_op_num_threads")
     intra_op_num_threads = session_options.get("intra_op_num_threads")
@@ -212,47 +228,70 @@
     def __init__(
         self,
         session: "InferenceSession",
         io_bind: bool = False,
         device: str = "cpu",
         shared_kv_buffer: bool = False,
         use_fp16: bool = False,
-        input_feed: Optional[Dict[str, np.ndarray]] = None,
+        input_feed: Optional[Dict[str, "NDArray"]] = None,
+        constant_inputs: Optional[Dict[str, "NDArray"]] = None,
     ):
+        """Initialize self.
+
+        :param session: ONNXRuntime InferenceSession
+        :param io_bind: Whether to use IO binding. Default is False.
+        :param device: Device to run inference on. Default is "cpu".
+        :param shared_kv_buffer: Whether to share the key/value buffer across multiple runs.
+            Default is False. Only valid if io_bind is True.
+        :param use_fp16: Whether to use fp16. Default is False. Both shared_kv_buffer and use_fp16 must be True
+            at the same time to use shared key/value buffer.
+        :param input_feed: Optional input feed for the session. Required when shared_kv_buffer and use_fp16 are True.
+        :param constant_inputs: Optional constant inputs for the session. These will be passed to the session every
+            inference run.
+        """
+        # TODO(anyone): use_fp16 is redundant with shared_kv_buffer. Remove it.
         self.session = session
         self.io_bind = io_bind
         self.device = device
         self.shared_kv_buffer = shared_kv_buffer
         self.use_fp16 = use_fp16
         self.kv_cache_ortvalues = {} if (self.shared_kv_buffer and self.use_fp16) else None
+        # TODO(jambayk): investigate if io binding can be run without having to bind constant
+        # inputs every time.
+        self.constant_inputs = constant_inputs or {}
 
         self.io_binding = None
         if self.io_bind:
             self.io_binding = self.session.io_binding()
             if self.shared_kv_buffer and self.use_fp16:
                 assert input_feed is not None, "input_feed is required when shared_kv_buffer and use_fp16 are True"
                 bind_input_data(
                     self.io_binding,
-                    input_feed,
+                    {**input_feed, **self.constant_inputs},
                     self.use_fp16,
                     self.device,
                     shared_kv_buffer=self.shared_kv_buffer,
                     kv_cache_ortvalues=self.kv_cache_ortvalues,
                 )
             bind_output_data(
                 self.io_binding,
                 self.session.get_outputs(),
                 self.use_fp16,
                 self.device,
                 shared_kv_buffer=self.shared_kv_buffer,
                 kv_cache_ortvalues=self.kv_cache_ortvalues,
             )
 
-    def run(self, input_feed: Dict[str, np.ndarray]) -> Sequence[np.ndarray]:
+    def get_full_input_feed(self, input_feed: Dict[str, "NDArray"]) -> Dict[str, "NDArray"]:
+        """Get the full input feed including constant inputs."""
+        return {**input_feed, **self.constant_inputs}
+
+    def run(self, input_feed: Dict[str, "NDArray"]) -> Sequence["NDArray"]:
         """Run inference with the given input data."""
+        input_feed = self.get_full_input_feed(input_feed)
         if self.io_bind and self.device == "gpu":
             bind_input_data(
                 self.io_binding,
                 input_feed,
                 self.use_fp16,
                 self.device,
                 shared_kv_buffer=self.shared_kv_buffer,
@@ -264,17 +303,18 @@
             res = [i.numpy() for i in self.io_binding.get_outputs()]
             self.io_binding.clear_binding_inputs()
         else:
             res = self.session.run(input_feed=input_feed, output_names=None)
         return res
 
     def time_run(
-        self, input_feed: Dict[str, np.ndarray], num_runs: int, num_warmup: int = 0, sleep_time: int = 0
+        self, input_feed: Dict[str, "NDArray"], num_runs: int, num_warmup: int = 0, sleep_time: int = 0
     ) -> Sequence[float]:
         """Time inference runs with the given input data."""
+        input_feed = self.get_full_input_feed(input_feed)
         latencies = []
         if self.io_bind:
             bind_input_data(
                 self.io_binding,
                 input_feed,
                 self.use_fp16,
                 self.device,
@@ -298,15 +338,15 @@
         if self.io_bind:
             self.io_binding.clear_binding_inputs()
         return latencies[num_warmup:]
 
 
 def bind_input_data(
     io_bind_op: "IOBinding",
-    input_data: Dict[str, np.ndarray],
+    input_data: Dict[str, "NDArray"],
     use_fp16: bool,
     device: str,
     device_id: int = 0,
     shared_kv_buffer: bool = False,
     kv_cache_ortvalues: dict = None,
 ):
     from onnxruntime import OrtValue
@@ -347,29 +387,30 @@
             io_bind_op.bind_ortvalue_output(name, kv_cache_ortvalues[output_name])
         else:
             io_bind_op.bind_output(name, io_bind_device)
 
 
 def prepare_io_bindings(
     session: "InferenceSession",
-    input_data: Dict[str, np.ndarray],
+    input_data: Dict[str, "NDArray"],
     device: str,
     device_id: int = 0,
     shared_kv_buffer: bool = False,
     kv_cache_ortvalues: dict = None,
 ) -> "IOBinding":
     """Convert input from numpy array to OrtValue.
 
     session: ONNXRuntime session
     input_data: dict of input data, value is numpy array
     device: olive device
     device_id: 0 by default. TODO(trajep): support user to specified device id
     shared_kv_buffer: whether to share the key/value buffer across multiple runs, it is False by default,
         and only used when we observe kv cache and fp16 is used.
         TODO(trajep): how shared_kv_buffer works with generation task
+    kv_cache_ortvalues: dict of OrtValue for shared kv cache, it is None by default.
     """
     use_fp16 = any(v.dtype == np.float16 for v in input_data.values())
     io_bind_op = session.io_binding()
 
     if shared_kv_buffer:
         kv_cache_ortvalues = kv_cache_ortvalues or {}
```

## olive/common/utils.py

```diff
@@ -11,14 +11,15 @@
 import platform
 import shlex
 import shutil
 import subprocess
 import tempfile
 import time
 from pathlib import Path
+from typing import Dict
 
 logger = logging.getLogger(__name__)
 
 
 def run_subprocess(cmd, env=None, cwd=None, check=False):
     logger.debug("Running command: %s", cmd)
 
@@ -337,7 +338,11 @@
         return
 
     tempdir = Path(tempdir).resolve()
     tempdir.mkdir(parents=True, exist_ok=True)
     # setting as string to be safe
     logger.debug("Setting tempdir to %s from %s", tempdir, tempfile.tempdir)
     tempfile.tempdir = str(tempdir)
+
+
+def exclude_keys(original_dict: Dict, keys_to_exclude):
+    return {k: v for k, v in original_dict.items() if k not in keys_to_exclude}
```

## olive/engine/__init__.py

```diff
@@ -1,12 +1,13 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
-from olive.engine.engine import Engine, EngineConfig
+from olive.engine.config import EngineConfig
+from olive.engine.engine import Engine
 from olive.engine.footprint import Footprint
 
 __all__ = [
     "Engine",
     "EngineConfig",
     "Footprint",
 ]
```

## olive/engine/config.py

```diff
@@ -1,18 +1,16 @@
 # -------------------------------------------------------------------------
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 from pathlib import Path
-from typing import Optional, Union
+from typing import Union
 
-from olive.azureml.azureml_client import AzureMLClientConfig
 from olive.common.config_utils import ConfigBase
 from olive.common.pydantic_v1 import Extra
-from olive.engine.packaging.packaging_config import PackagingConfig
 from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
 from olive.strategy.search_strategy import SearchStrategyConfig
 from olive.systems.system_config import SystemConfig
 
 # pass search-point was pruned due to failed run
 FAILED_CONFIG = "failed-config"
 # pass search-point was pruned due to invalid config
@@ -22,13 +20,11 @@
 
 
 class EngineConfig(ConfigBase, extra=Extra.forbid):
     search_strategy: Union[SearchStrategyConfig, bool] = None
     host: SystemConfig = None
     target: SystemConfig = None
     evaluator: OliveEvaluatorConfig = None
-    azureml_client_config: Optional[AzureMLClientConfig] = None
-    packaging_config: PackagingConfig = None
     cache_dir: Union[Path, str] = ".olive-cache"
     clean_cache: bool = False
     clean_evaluation_cache: bool = False
     plot_pareto_frontier: bool = False
```

## olive/engine/engine.py

```diff
@@ -8,119 +8,110 @@
 from collections import OrderedDict, defaultdict
 from contextlib import contextmanager
 from datetime import datetime
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Optional, Tuple, Type, Union
 
 import olive.cache as cache_utils
-from olive.common.config_utils import ConfigBase, validate_config
+from olive.common.config_utils import validate_config
 from olive.common.utils import hash_dict
-from olive.engine.config import FAILED_CONFIG, INVALID_CONFIG, PRUNED_CONFIGS, EngineConfig
+from olive.engine.config import FAILED_CONFIG, INVALID_CONFIG, PRUNED_CONFIGS
 from olive.engine.footprint import Footprint, FootprintNodeMetric
 from olive.engine.packaging.packaging_generator import generate_output_artifacts
 from olive.evaluator.metric import Metric, MetricResult, joint_metric_key
+from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
 from olive.exception import EXCEPTIONS_TO_RAISE, OlivePassError
 from olive.hardware import AcceleratorSpec
 from olive.model import ModelConfig
-from olive.strategy.search_strategy import SearchStrategy
+from olive.strategy.search_strategy import SearchStrategy, SearchStrategyConfig
 from olive.systems.common import SystemType
-from olive.systems.olive_system import OliveSystem
-from olive.systems.system_config import LocalTargetUserConfig, SystemConfig
+from olive.systems.system_config import SystemConfig
 from olive.systems.utils import create_managed_system_with_cache
 
 if TYPE_CHECKING:
     from olive.engine.packaging.packaging_config import PackagingConfig
-    from olive.evaluator.olive_evaluator import OliveEvaluatorConfig
     from olive.passes.olive_pass import Pass
+    from olive.systems.olive_system import OliveSystem
 
 logger = logging.getLogger(__name__)
 
 
 class Engine:
     """The engine executes the registered Olive Steps.
 
     It facilitate evaluation of the output models using provided evaluation criteria and produces output model(s).
     """
 
     def __init__(
         self,
-        config: Union[Dict[str, Any], EngineConfig] = None,
-        search_strategy: Optional[SearchStrategy] = None,
-        host_config: Optional[SystemConfig] = None,
-        target_config: Optional[SystemConfig] = None,
-        evaluator_config: Optional["OliveEvaluatorConfig"] = None,
+        search_strategy: Optional[Union[Dict[str, Any], SearchStrategyConfig]] = None,
+        host: Optional[Union[Dict[str, Any], "SystemConfig"]] = None,
+        target: Optional[Union[Dict[str, Any], "SystemConfig"]] = None,
+        evaluator: Optional[Union[Dict[str, Any], "OliveEvaluatorConfig"]] = None,
+        cache_dir=".olive-cache",
+        clean_cache=False,
+        clean_evaluation_cache=False,
+        plot_pareto_frontier=False,
+        *,
+        azureml_client_config=None,
     ):
-        self._config = validate_config(config, EngineConfig)
-
         self.no_search = False
-        # default search strategy
-        self.search_strategy = SearchStrategy({"execution_order": "joint", "search_algorithm": "exhaustive"})
-        if search_strategy is not None:
-            # if search strategy is provided, use it. It takes precedence
-            self.search_strategy = search_strategy
-        elif isinstance(self._config.search_strategy, (ConfigBase, dict)):
-            # if search strategy is provided in config, use it
-            self.search_strategy = SearchStrategy(self._config.search_strategy)
-        elif not self._config.search_strategy:
+        if not search_strategy:
             # if search strategy is None or False, disable search
             self.no_search = True
+            self.search_strategy = None
+        else:
+            # if search strategy is provided in config, use it
+            self.search_strategy = SearchStrategy(search_strategy)
 
         # default host
-        if host_config is not None:
-            self.host_config = host_config
-        elif self._config.host is not None:
-            self.host_config = self._config.host
-        else:
-            # host accelerator is not used, so no need to specify it
-            self.host_config = SystemConfig(type=SystemType.Local, config=LocalTargetUserConfig())
+        host = host or {"type": SystemType.Local}
+        self.host_config = validate_config(host, SystemConfig)
         self.host = None
 
         # engine target
-        if target_config is not None:
-            self.target_config = target_config
-        elif self._config.target is not None:
-            self.target_config = self._config.target
-        else:
-            self.target_config = SystemConfig(type=SystemType.Local, config=LocalTargetUserConfig())
+        target = target or {"type": SystemType.Local}
+        self.target_config = validate_config(target, SystemConfig)
         self.target = None
 
         # default evaluator
-        self.evaluator_config = None
-        if evaluator_config is not None:
-            self.evaluator_config = evaluator_config
-        elif self._config.evaluator is not None:
-            self.evaluator_config = self._config.evaluator
+        self.evaluator_config = validate_config(evaluator, OliveEvaluatorConfig) if evaluator else None
+
+        self.cache_dir = cache_dir
+        self.clean_cache = clean_cache
+        self.clean_evaluation_cache = clean_evaluation_cache
+        self.plot_pareto_frontier = plot_pareto_frontier
+        self.azureml_client_config = azureml_client_config
 
         # dictionary of passes
         self.pass_config = OrderedDict()
 
         # {"pass_name": {"pass": pass, "host": host, "evaluator": evaluator, "clean_run_cache": clean_run_cache}}
         self.passes = OrderedDict()
         self.pass_flows = None
         self.pass_flows_search_spaces = None
 
         self.footprints = defaultdict(Footprint)
-        self.azureml_client_config = self._config.azureml_client_config
+
         self._initialized = False
 
     def initialize(self):
         """Initialize engine state. This should be done before running the registered passes."""
         # pylint: disable=attribute-defined-outside-init
 
-        cache_dir = self._config.cache_dir
-        if self._config.clean_cache:
-            cache_utils.clean_cache(cache_dir)
-        if self._config.clean_evaluation_cache:
-            cache_utils.clean_evaluation_cache(cache_dir)
+        if self.clean_cache:
+            cache_utils.clean_cache(self.cache_dir)
+        if self.clean_evaluation_cache:
+            cache_utils.clean_evaluation_cache(self.cache_dir)
 
-        logger.info("Using cache directory: %s", cache_dir)
+        logger.info("Using cache directory: %s", self.cache_dir)
         self._model_cache_path, self._run_cache_path, self._evaluation_cache_path, _ = cache_utils.get_cache_sub_dirs(
-            cache_dir
+            self.cache_dir
         )
-        cache_utils.create_cache(cache_dir)
+        cache_utils.create_cache(self.cache_dir)
 
         # initialize counters
         # we do this before cleaning pass run caches to ensure we don't reuse model numbers even if the model was
         # deleted from the cache
         self._new_model_number = 0
         # model jsons have the format <model_number>_<pass_type>-<source_model>-<pass_config_hash>.json
         # model contents are stored in <model_number>_<pass_type>-<source_model>-<pass_config_hash> folder
@@ -131,26 +122,26 @@
             self._new_model_number = max(int(model_file.stem.split("_")[0]) for model_file in model_files) + 1
 
         # clean pass run cache if requested
         # removes all run cache for pass type and all children elements
         for pass_config in self.pass_config.values():
             clean_run_cache = pass_config["clean_run_cache"]
             if clean_run_cache:
-                cache_utils.clean_pass_run_cache(pass_config["type"].__name__, cache_dir)
+                cache_utils.clean_pass_run_cache(pass_config["type"].__name__, self.cache_dir)
 
         self.set_pass_flows(self.pass_flows)
         self._initialized = True
 
     def register(
         self,
         pass_type: Type["Pass"],
         config: Dict[str, Any] = None,
         disable_search=False,
         name: str = None,
-        host: OliveSystem = None,
+        host: "OliveSystem" = None,
         evaluator_config: "OliveEvaluatorConfig" = None,
         clean_run_cache: bool = False,
         output_name: str = None,
     ):
         """Register a pass configuration so that it could be instantiated and executed later."""
         if name is not None:
             assert name not in self.passes, f"Pass with name {name} already registered"
@@ -174,15 +165,15 @@
             "output_name": output_name,
         }
 
     def register_pass(
         self,
         p: "Pass",
         name: str = None,
-        host: OliveSystem = None,
+        host: "OliveSystem" = None,
         evaluator_config: "OliveEvaluatorConfig" = None,
         output_name: str = None,
     ):
         """Register a pass instance."""
         if name is not None:
             assert name not in self.passes, f"Pass with name {name} already registered"
         else:
@@ -462,15 +453,15 @@
                 if not pass_output_name:
                     continue
                 output_model_json = cache_utils.save_model(
                     model_number=pass_output_model_id,
                     output_dir=output_dir_with_pf,
                     output_name=f"{pass_output_name}_model",
                     overwrite=True,
-                    cache_dir=self._config.cache_dir,
+                    cache_dir=self.cache_dir,
                 )
                 # it is not supported to save compositepytorchmodel/compositemodel again
                 # so the output_model_json could be None
                 output_models[pass_output_model_id] = output_model_json
 
             # save the evaluation results to output_dir
             if signal is not None:
@@ -553,15 +544,15 @@
 
     def create_pareto_frontier_footprints(self, accelerator_spec, output_model_num, output_dir, prefix_output_name):
         pf_footprints = self.footprints[accelerator_spec].create_pareto_frontier(output_model_num)
         if not pf_footprints:
             return None
         pf_footprints.to_file(output_dir / f"{prefix_output_name}_pareto_frontier_footprints.json")
 
-        if self._config.plot_pareto_frontier:
+        if self.plot_pareto_frontier:
             pf_footprints.plot_pareto_frontier_to_html(
                 save_path=output_dir / f"{prefix_output_name}_pareto_frontier_footprints_chart.html"
             )
 
         return pf_footprints
 
     def dump_run_history(self, run_history, output_path: str = None):
@@ -736,15 +727,15 @@
     def _prepare_non_local_model(self, model_config: ModelConfig) -> ModelConfig:
         """Prepare models with non-local model path for local run by downloading the model resources to cache."""
         # TODO(myguo): maybe we can move this method into OliveSystem?
         resource_paths = model_config.get_resource_paths()
         for resource_name, resource_path in resource_paths.items():
             if not resource_path or resource_path.is_local_resource_or_string_name():
                 continue
-            downloaded_resource_path = cache_utils.download_resource(resource_path, self._config.cache_dir)
+            downloaded_resource_path = cache_utils.download_resource(resource_path, self.cache_dir)
             if downloaded_resource_path:
                 # set local resource path
                 model_config.config[resource_name] = downloaded_resource_path
 
         return model_config
 
     def _init_input_model(self, input_model_config: ModelConfig):
```

## olive/evaluator/olive_evaluator.py

```diff
@@ -443,22 +443,28 @@
         io_bind = OnnxEvaluator.io_bind_enabled(metric, model.inference_settings)
         shared_kv_buffer = metric.user_config.shared_kv_buffer
         use_fp16 = any(v == "float16" for v in io_config["input_types"])
         input_feed = None
         if io_bind and shared_kv_buffer and use_fp16:
             input_feed = OnnxEvaluator.format_input(next(iter(dataloader))[0], io_config)
 
+        # load constant inputs if any
+        constant_inputs = None
+        if model.constant_inputs_path:
+            constant_inputs = OnnxEvaluator.format_input(dict(np.load(model.constant_inputs_path)), io_config)
+
         # create session wrapper
         session_wrapper = OrtInferenceSession(
             session,
             io_bind=io_bind,
             device=device,
             shared_kv_buffer=shared_kv_buffer,
             use_fp16=use_fp16,
             input_feed=input_feed,
+            constant_inputs=constant_inputs,
         )
 
         return session_wrapper, inference_settings
 
     def _inference(
         self,
         model: ONNXModelHandler,
```

## olive/model/handler/onnx.py

```diff
@@ -2,25 +2,26 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 import logging
 from pathlib import Path
 from typing import Any, ClassVar, Dict, List, Optional, Tuple, Union
 
+import numpy as np
 import onnx
 from onnx import GraphProto, ModelProto
 
 from olive.common.ort_inference import OrtSessionFallbackError, get_ort_inference_session
 from olive.constants import Framework, ModelFileFormat
 from olive.exception import OliveEvaluationError
 from olive.hardware.accelerator import AcceleratorLookup, Device
 from olive.model.config.registry import model_handler_registry
 from olive.model.handler.base import OliveModelHandler
 from olive.model.handler.mixin import OnnxEpValidateMixin, OnnxGraphMixin
-from olive.model.utils.onnx_utils import get_onnx_file_path
+from olive.model.utils.onnx_utils import get_additional_file_path, get_onnx_file_path
 from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS
 
 logger = logging.getLogger(__name__)
 
 
 @model_handler_registry("ONNXModel")
 class ONNXModelHandler(OliveModelHandler, OnnxEpValidateMixin, OnnxGraphMixin):  # pylint: disable=too-many-ancestors
@@ -28,46 +29,70 @@
 
     Besides the model loading functionalities, the model handler also provider the onnx graph functionality by mixin
 
     the mixin class OnnxEpValidateMixin is used to validate the execution providers.
     the mixin class OnnxGraphMixin is used to support onnx graph operations.
     """
 
-    json_config_keys: Tuple[str, ...] = ("onnx_file_name", "inference_settings", "use_ort_extensions")
+    json_config_keys: Tuple[str, ...] = (
+        "onnx_file_name",
+        "inference_settings",
+        "use_ort_extensions",
+        "external_initializers_file_name",
+        "constant_inputs_file_name",
+    )
 
     def __init__(
         self,
         model_path: OLIVE_RESOURCE_ANNOTATIONS = None,
         onnx_file_name: Optional[str] = None,
         inference_settings: Optional[dict] = None,
         use_ort_extensions: bool = False,
         model_attributes: Optional[Dict[str, Any]] = None,
+        external_initializers_file_name: Optional[str] = None,
+        constant_inputs_file_name: Optional[str] = None,
     ):
         super().__init__(
             framework=Framework.ONNX,
             model_file_format=ModelFileFormat.ONNX,
             model_path=model_path,
             model_attributes=model_attributes,
         )
         self.inference_settings = inference_settings
         self.use_ort_extensions = use_ort_extensions
         self.onnx_file_name = onnx_file_name
+        self.external_initializers_file_name = external_initializers_file_name
+        self.constant_inputs_file_name = constant_inputs_file_name
 
         self.io_config = None
         self.graph = None
         self.all_graphs: Optional[List[GraphProto]] = None
 
-        # check for onnx file name since it will do validation
-        _ = self.model_path
+        # check for file names since it will automatically validate the paths
+        # these call the property methods which in turn validate the paths using get_onnx_file_path
+        # and get_additional_file_path
+        to_check = ["model_path", "external_initializers_path", "constant_inputs_path"]
+        for attr in to_check:
+            getattr(self, attr)
 
     @property
     def model_path(self) -> str:
         model_path = super().model_path
         return get_onnx_file_path(model_path, self.onnx_file_name) if model_path else None
 
+    @property
+    def external_initializers_path(self) -> Optional[str]:
+        model_path = super().model_path
+        return get_additional_file_path(model_path, self.external_initializers_file_name) if model_path else None
+
+    @property
+    def constant_inputs_path(self) -> Optional[str]:
+        model_path = super().model_path
+        return get_additional_file_path(model_path, self.constant_inputs_file_name) if model_path else None
+
     def load_model(self, rank: int = None) -> ModelProto:
         return onnx.load(self.model_path)
 
     def prepare_session(
         self,
         inference_settings: Optional[Dict[str, Any]] = None,
         device: Device = Device.CPU,
@@ -78,17 +103,21 @@
         inference_settings = self.merge_inference_settings(inference_settings, execution_providers)
         if not inference_settings["execution_provider"]:
             # if no execution_providers are provided, use the default ones
             inference_settings["execution_provider"] = self._get_default_execution_providers(device)
             inference_settings["provider_options"] = None
         # device id for ranked model
         device_id = rank if device == Device.GPU else None
+        # load external initializers if available
+        external_initializers = np.load(self.external_initializers_path) if self.external_initializers_path else None
 
         try:
-            return get_ort_inference_session(self.model_path, inference_settings, self.use_ort_extensions, device_id)
+            return get_ort_inference_session(
+                self.model_path, inference_settings, self.use_ort_extensions, device_id, external_initializers
+            )
         except OrtSessionFallbackError as e:
             raise OliveEvaluationError(e) from e
 
     def merge_inference_settings(
         self, inference_settings: Optional[Dict[str, Any]] = None, execution_providers: List[str] = None
     ):
         """Merge user provided inference settings with model's inference settings.
```

## olive/model/handler/pytorch.py

```diff
@@ -136,14 +136,16 @@
             model = torch.jit.load(self.model_path)
         elif self.model_file_format == ModelFileFormat.PYTORCH_MLFLOW_MODEL:
             model = self._load_mlflow_model()
         elif self.hf_config and (self.hf_config.model_class or self.hf_config.task):
             model = self.load_hf_model(self.model_path)
         elif self.model_file_format == ModelFileFormat.PYTORCH_ENTIRE_MODEL:
             model = torch.load(self.model_path)
+        elif self.model_file_format == ModelFileFormat.PYTORCH_SLICE_GPT_MODEL:
+            model = self._load_slicegpt_model()
         elif self.model_file_format == ModelFileFormat.PYTORCH_STATE_DICT:
             raise ValueError("Please use customized model loader to load state dict of model.")
         else:
             raise ValueError(f"Unsupported model file format: {self.model_file_format}")
 
         # we only have peft adapters for now
         if self.adapter_path:
@@ -220,14 +222,21 @@
                         "Unsupported MLFlow model flavor. Currently only support hftransformersv2/hftransformers."
                     )
             loading_args = self.hf_config.get_loading_args_from_pretrained() if self.hf_config else {}
             loaded_model = load_hf_model_from_model_class(hf_pretrained_class, tmp_dir, **loading_args)
             loaded_model.eval()
             return loaded_model
 
+    def _load_slicegpt_model(self):
+        logger.info("Loading SliceGPT model from %s", self.model_path)
+        from slicgpt.hf_utils import load_sliced_model
+
+        loaded_model, _ = load_sliced_model(self.hf_config.model_name, self.model_path)
+        return loaded_model
+
     def to_json(self, check_object: bool = False):
         config = super().to_json(check_object)
         # only keep model_attributes that are not in hf_config
         if self.model_attributes and self.hf_config:
             model_attributes = {}
             hf_config_dict = self.get_hf_model_config().to_dict()
             for key, value in self.model_attributes.items():
```

## olive/model/utils/onnx_utils.py

```diff
@@ -59,12 +59,27 @@
             f"Multiple .onnx model files found in the model folder {model_path}. Please specify one using the"
             " onnx_file_name argument."
         )
     else:
         raise ValueError(f"No .onnx file found in the model folder {model_path}.")
 
 
+def get_additional_file_path(model_dir: str, file_name: str) -> Optional[str]:
+    """Get the full path to the additional file.
+
+    If file_name is specified, it is assumed to be a file in the model_dir and the full path
+    is returned.
+    """
+    if file_name:
+        model_dir = Path(model_dir)
+        assert model_dir.is_dir(), f"Model path {model_dir} is not a directory."
+        file_path = model_dir / file_name
+        assert file_path.exists(), f"{file_name} does not exist in model path directory {model_dir}."
+        return str(file_path)
+    return None
+
+
 def dump_tuning_result(session, tuning_result_path):
     assert tuning_result_path.endswith(".json")
     tuning_result = session.get_tuning_results()
     with Path(tuning_result_path).open("w") as f:
         json.dump(tuning_result, f, indent=2)
```

## olive/passes/onnx/common.py

```diff
@@ -89,33 +89,28 @@
         logger.info("Deleting existing onnx file: %s", output_path)
         output_path.unlink()
 
     # parent directory of .onnx file
     output_dir = output_path.parent
     output_dir.mkdir(parents=True, exist_ok=True)
 
+    model_size = model.ByteSize()
+    # model size for large models might be negative (overflow?) on Windows
+    # see https://github.com/onnx/onnx/issues/5861
+    if not save_as_external_data and (model_size <= 0 or model_size >= onnx.checker.MAXIMUM_PROTOBUF):
+        save_as_external_data = True
+        logger.info(
+            "Model is too large to save as a single file but 'save_as_external_data' is False. Saving tensors as"
+            " external data, regardless."
+        )
+
     if not save_as_external_data:
-        try:
-            # save model
-            onnx.save_model(model, str(output_path))
-            return False
-        except ValueError as e:
-            # there are different types of error message for large model (>2GB) based on onnx version
-            # just try to save as external data
-            # if it fails, raise the original error
-            try:
-                logger.debug("Model save failed with error: %s. Trying to save as external data.", e)
-                model_proto_to_file(model, output_path, True, all_tensors_to_one_file, external_data_name)
-                logger.warning(
-                    "Model is too large to save as a single file but 'save_as_external_data' is False. Saved tensors"
-                    " as external data regardless."
-                )
-                return True
-            except Exception:
-                raise e from None
+        # save model
+        onnx.save_model(model, str(output_path))
+        return False
 
     # location for external data
     external_data_path = output_dir / (external_data_name if external_data_name else f"{output_path.name}.data")
     location = external_data_path.name if all_tensors_to_one_file else None
 
     if all_tensors_to_one_file:
         if external_data_path.exists():
@@ -140,43 +135,51 @@
 
 
 def model_proto_to_olive_model(
     model_proto: onnx.ModelProto,
     output_model_path: Union[str, Path],
     external_data_config: dict,
     check_model: bool = False,
+    external_initializers_file_name: Optional[str] = None,
+    constant_inputs_file_name: Optional[str] = None,
 ) -> ONNXModelHandler:
     """Save the ONNX model to the specified path and return the ONNXModelHandler.
 
     :param model_proto: The ONNX model to save.
     :param output_model_path: The path to save the ONNX model to.
     :param external_data_config: The external data configuration. Must be a dictionary with keys
         "save_as_external_data", "all_tensors_to_one_file", and "external_data_name".
-    :param name: The name of the model.
-    :check_model: If True, run onnx.checker.check_model on the model before returning.
+    :param check_model: If True, run onnx.checker.check_model on the model before returning.
+    :param external_initializers_file_name: The name of the external initializers file.
+    :param constant_inputs_file_name: The name of the constant inputs file.
 
     :return: The ONNXModelHandler.
     """
     config_keys = [
         "save_as_external_data",
         "all_tensors_to_one_file",
         "external_data_name",
         "size_threshold",
         "convert_attribute",
     ]
     has_external_data = model_proto_to_file(
         model_proto, output_model_path, **{k: external_data_config[k] for k in config_keys if k in external_data_config}
     )
-    if has_external_data:
+    if has_external_data or external_initializers_file_name or constant_inputs_file_name:
         model_path = LocalFolder({"path": Path(output_model_path).parent})
 
         onnx_file_name = Path(output_model_path).name
     else:
         model_path = LocalFile({"path": output_model_path})
         onnx_file_name = None
 
-    olive_model = ONNXModelHandler(model_path=model_path, onnx_file_name=onnx_file_name)
+    olive_model = ONNXModelHandler(
+        model_path=model_path,
+        onnx_file_name=onnx_file_name,
+        external_initializers_file_name=external_initializers_file_name,
+        constant_inputs_file_name=constant_inputs_file_name,
+    )
 
     if check_model:
         onnx.checker.check_model(olive_model.model_path)
 
     return olive_model
```

## olive/passes/onnx/conversion.py

```diff
@@ -11,15 +11,15 @@
 from typing import Any, Dict, Optional, Tuple, Union
 
 import onnx
 import torch
 from packaging import version
 
 from olive.common.config_utils import validate_config
-from olive.common.utils import find_submodules, resolve_torch_dtype, tensor_data_to_device
+from olive.common.utils import exclude_keys, find_submodules, resolve_torch_dtype, tensor_data_to_device
 from olive.hardware import AcceleratorSpec
 from olive.model import (
     CompositeModelHandler,
     DistributedOnnxModelHandler,
     DistributedPyTorchModelHandler,
     HfFromPretrainedArgs,
     ONNXModelHandler,
@@ -96,18 +96,20 @@
                 type_=bool,
                 default_value=False,
                 description="Whether to merge the converted components.",
             ),
             "merge_adapter_weights": PassConfigParam(
                 type_=bool,
                 default_value=False,
-                description="Whether to merge adapter weights before conversion. "
-                "After merging, the model structure is consistent with base model. "
-                "That is useful if you cannot run conversion for some fine-tuned "
-                "models with adapter weights",
+                description=(
+                    "Whether to merge adapter weights before conversion. "
+                    "After merging, the model structure is consistent with base model. "
+                    "That is useful if you cannot run conversion for some fine-tuned "
+                    "models with adapter weights"
+                ),
             ),
         }
         config.update(get_external_data_config())
         return config
 
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
@@ -250,16 +252,15 @@
                 ).save(tmp_model_path)
                 onnx.checker.check_model(tmp_model_path)
                 onnx.shape_inference.infer_shapes_path(tmp_model_path)
                 onnx_model = onnx.load(tmp_model_path)
         else:
             # Standard ONNX export
             if isinstance(dummy_inputs, dict):
-                for key in unused_keys:
-                    del dummy_inputs[key]
+                dummy_inputs = exclude_keys(dummy_inputs, unused_keys)
 
             output_names = io_config.output_names
             dynamic_axes = io_config.dynamic_axes
 
             # there might be multiple files created during export, so we need to track the dir
             # if there are other processes writing to the same dir, we might end up deleting files created by
             # other processes
@@ -316,81 +317,85 @@
                 conversion on the specified device
             - if quantization_method == "bitsandbytes" and load_in_4bit is True
                 - remove quantization config from the model loading args
                 - find quantized modules and add them to the model attributes
                 - the onnx model must be quantized using OnnxBnb4Quantization pass after conversion
         Model attributes is None if the output model should inherit the model attributes from the input model.
         """
+        pytorch_model = None
+        model_attributes = deepcopy(model.model_attributes or {})
         if not model.is_model_loaded_from_hf_config() or not model.hf_config.from_pretrained_args:
             # if the model is not loaded from hf config, or the model loading args is not specified,
             # we can load the model directly
-            return model.load_model(), None
-
-        from_pretrained_args = model.hf_config.from_pretrained_args
-        model_dtype = from_pretrained_args.get_torch_dtype()
-        new_from_pretrained_args = deepcopy(from_pretrained_args.dict())
-        new_model_attributes = model.model_attributes or {}
-        if torch_dtype and torch_dtype != model_dtype:
-            # if the model loading args specify a different dtype, update the model loading args
-            logger.debug(
-                "Changing torch_dtype in model loading args from %s to %s.",
-                from_pretrained_args.get_torch_dtype(),
-                torch_dtype,
-            )
-            new_from_pretrained_args["torch_dtype"] = torch_dtype
-            new_model_attributes["torch_dtype"] = str(torch_dtype).replace("torch.", "")
-        elif model_dtype == torch.float16 and device == "cpu":
-            logger.warning(
-                "Loading model on CPU, but the model loading args specify dtype float16 which is not supported  for"
-                " conversion on CPU. The dtype is changed to float32. If float16 model is desired, please specify"
-                " device as 'cuda' or use OrtTransformerOptimization/OnnxFloatToFloat16 pass after conversion to"
-                " convert the model to float16."
-            )
-            new_from_pretrained_args["torch_dtype"] = torch.float32
-            new_model_attributes["torch_dtype"] = "float32"
+            pytorch_model = model.load_model()
+        else:
+            from_pretrained_args = model.hf_config.from_pretrained_args
+            model_dtype = from_pretrained_args.get_torch_dtype()
+            new_from_pretrained_args = deepcopy(from_pretrained_args.dict())
+            if torch_dtype and torch_dtype != model_dtype:
+                # if the model loading args specify a different dtype, update the model loading args
+                logger.debug(
+                    "Changing torch_dtype in model loading args from %s to %s.",
+                    from_pretrained_args.get_torch_dtype(),
+                    torch_dtype,
+                )
+                new_from_pretrained_args["torch_dtype"] = torch_dtype
+                model_attributes["torch_dtype"] = str(torch_dtype).replace("torch.", "")
+            elif model_dtype == torch.float16 and device == "cpu":
+                logger.warning(
+                    "Loading model on CPU, but the model loading args specify dtype float16 which is not supported  for"
+                    " conversion on CPU. The dtype is changed to float32. If float16 model is desired, please specify"
+                    " device as 'cuda' or use OrtTransformerOptimization/OnnxFloatToFloat16 pass after conversion to"
+                    " convert the model to float16."
+                )
+                new_from_pretrained_args["torch_dtype"] = torch.float32
+                model_attributes["torch_dtype"] = "float32"
 
-        if (
-            from_pretrained_args.quantization_method == "bitsandbytes"
-            and from_pretrained_args.quantization_config["load_in_4bit"]
-        ):
-            logger.warning(
-                "Bitsandbytes 4bit quantization is not supported for conversion. The quantization config is removed"
-                " from the model loading args. Use OnnxBnb4Quantization pass after conversion to quantize the model."
-            )
-            new_from_pretrained_args["quantization_method"] = None
-            new_from_pretrained_args["quantization_config"] = None
-            new_model_attributes["quantization_config"] = from_pretrained_args.quantization_config
-            if "quantized_modules" not in new_model_attributes:
-                # find and add quantized modules to the model attributes
-                # the QLoRA pass already adds quantized_modules to the model attributes, so this will not be executed
-                # if the model was generated by QLoRA
-                quantized_model = model.load_model()
-
-                # if PeftModel, need to unload adapter before finding quantized modules
-                if is_peft_model(quantized_model):
-                    quantized_model = quantized_model.unload()
-
-                import bitsandbytes as bnb
-
-                new_model_attributes["quantized_modules"] = find_submodules(quantized_model, bnb.nn.Linear4bit)
-
-                # required for peft models since unloading changes the model
-                # for others, do this to free gpu memory as quantized model is always on gpu
-                del quantized_model
-                model.model = None
-
-        # load the model with the updated model loading args
-        new_hf_config = deepcopy(model.hf_config)
-        new_hf_config.from_pretrained_args = HfFromPretrainedArgs(**new_from_pretrained_args)
-        return (
-            PyTorchModelHandler(
+            if (
+                from_pretrained_args.quantization_method == "bitsandbytes"
+                and from_pretrained_args.quantization_config["load_in_4bit"]
+            ):
+                logger.warning(
+                    "Bitsandbytes 4bit quantization is not supported for conversion. The quantization config is removed"
+                    " from the model loading args. Use OnnxBnb4Quantization pass after conversion to quantize the"
+                    " model."
+                )
+                new_from_pretrained_args["quantization_method"] = None
+                new_from_pretrained_args["quantization_config"] = None
+                model_attributes["quantization_config"] = from_pretrained_args.quantization_config
+                if "quantized_modules" not in model_attributes:
+                    # find and add quantized modules to the model attributes
+                    # the QLoRA pass already adds quantized_modules to the model attributes, so this will not be
+                    # executed if the model was generated by QLoRA
+                    quantized_model = model.load_model()
+
+                    # if PeftModel, need to unload adapter before finding quantized modules
+                    if is_peft_model(quantized_model):
+                        quantized_model = quantized_model.unload()
+
+                    import bitsandbytes as bnb
+
+                    model_attributes["quantized_modules"] = find_submodules(quantized_model, bnb.nn.Linear4bit)
+
+                    # required for peft models since unloading changes the model
+                    # for others, do this to free gpu memory as quantized model is always on gpu
+                    del quantized_model
+                    model.model = None
+
+            # load the model with the updated model loading args
+            new_hf_config = deepcopy(model.hf_config)
+            new_hf_config.from_pretrained_args = HfFromPretrainedArgs(**new_from_pretrained_args)
+            pytorch_model = PyTorchModelHandler(
                 model_path=model.model_path, adapter_path=model.adapter_path, hf_config=new_hf_config
-            ).load_model(),
-            new_model_attributes,
-        )
+            ).load_model()
+
+        if is_peft_model(pytorch_model):
+            model_attributes["lora_modules"] = list(pytorch_model.peft_config["default"].target_modules)
+
+        return pytorch_model, model_attributes
 
     def _convert_model_on_device(
         self,
         model: PyTorchModelHandler,
         data_root: str,
         config: Dict[str, Any],
         output_model_path: str,
```

## olive/passes/onnx/genai_model_exporter.py

```diff
@@ -2,14 +2,15 @@
 # Copyright (c) Microsoft Corporation. All rights reserved.
 # Licensed under the MIT License.
 # --------------------------------------------------------------------------
 # Export a PyTorch model using the onnxruntime-genai package.
 # --------------------------------------------------------------------------
 import logging
 import os
+import tempfile
 from enum import Enum
 from pathlib import Path
 from typing import Any, Dict
 
 from olive.hardware.accelerator import AcceleratorLookup, AcceleratorSpec, Device
 from olive.model import ONNXModelHandler, PyTorchModelHandler
 from olive.model.utils import resolve_onnx_path
@@ -26,63 +27,87 @@
     """
 
     class Precision(str, Enum):
         FP32 = "fp32"
         FP16 = "fp16"
         INT4 = "int4"
 
+        def __str__(self) -> str:
+            return self.value
+
     @classmethod
     def _default_config(cls, accelerator_spec: AcceleratorSpec) -> Dict[str, PassConfigParam]:
         return {
             "precision": PassConfigParam(
                 type_=GenAIModelExporter.Precision,
                 required=True,
                 description="Precision of model.",
             )
         }
 
+    def validate_search_point(
+        self, search_point: Dict[str, Any], accelerator_spec: AcceleratorSpec, with_fixed_value: bool = False
+    ) -> bool:
+        if with_fixed_value:
+            search_point = self.config_at_search_point(search_point or {})
+        precision = search_point.get("precision")
+        device = (
+            Device.CPU
+            if self.accelerator_spec.execution_provider
+            in AcceleratorLookup.get_execution_providers_for_device(Device.CPU)
+            else Device.GPU
+        )
+        if precision == GenAIModelExporter.Precision.FP16 and device == Device.CPU:
+            logger.info(
+                "FP16 is not supported on CPU. Valid precision + execution"
+                "provider combinations are: FP32 CPU, FP32 CUDA, FP16 CUDA, INT4 CPU, INT4 CUDA"
+            )
+            return False
+        return True
+
+    @staticmethod
+    def is_accelerator_agnostic(accelerator_spec: AcceleratorSpec) -> bool:
+        return False
+
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
     ) -> ONNXModelHandler:
         from onnxruntime_genai.models.builder import create_model
 
         if not model.hf_config:
             raise ValueError(
                 "GenAIModelExporter pass only supports exporting HF models i.e. PyTorchModelHandler with hf_config."
             )
 
         Path(output_model_path).mkdir(parents=True, exist_ok=True)
         output_model_filepath = Path(resolve_onnx_path(output_model_path))
 
         precision = config["precision"]
-        device = (
-            Device.CPU
+        target_execution_provider = (
+            "cpu"
             if self.accelerator_spec.execution_provider
             in AcceleratorLookup.get_execution_providers_for_device(Device.CPU)
-            else Device.GPU
-        )
-
-        logger.info(
-            "Valid precision + execution provider combinations are: FP32 CPU, FP32 CUDA, FP16 CUDA, INT4 CPU, INT4 CUDA"
+            else "cuda"
         )
-
         # Select cache location based on priority
         # HF_CACHE (HF >= v5) -> TRANSFORMERS_CACHE (HF < v5) -> local dir
         cache_dir = os.environ.get("HF_HOME", None)
         if not cache_dir:
             cache_dir = os.environ.get("TRANSFORMERS_CACHE", None)
         if not cache_dir:
-            cache_dir = output_model_filepath.parent / "genai_cache_dir"
+            # please do not clean up the cache dir as it contains huggingface model
+            # snapshots that can be reused for future runs
+            cache_dir = str(Path(tempfile.gettempdir()) / "hf_cache")
 
         # currently we only support regular hf models so we can pass the name_or_path directly to model_name
         # could also check if it is a locally saved model and pass the path to input_path but it is not necessary
         create_model(
             model_name=str(model.model_path or model.hf_config.model_name),
             input_path="",  # empty string for now
             output_dir=str(output_model_filepath.parent),
-            precision=str(precision),
-            execution_provider=str(device),
-            cache_dir=str(cache_dir),
+            precision=precision,
+            execution_provider=target_execution_provider,
+            cache_dir=cache_dir,
             filename=str(output_model_filepath.name),
         )
 
         return ONNXModelHandler(output_model_filepath.parent, onnx_file_name=output_model_filepath.name)
```

## olive/passes/onnx/inc_quantization.py

```diff
@@ -9,14 +9,15 @@
 from pathlib import Path
 from typing import Any, Callable, Dict, Optional, Union
 
 from packaging import version
 
 from olive.cache import get_local_path_from_root
 from olive.common.config_utils import validate_config
+from olive.common.utils import exclude_keys
 from olive.data.config import DataConfig
 from olive.evaluator.metric import Metric, joint_metric_key
 from olive.evaluator.olive_evaluator import OliveEvaluatorFactory
 from olive.exception import OlivePassError
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
@@ -530,17 +531,15 @@
             "dataloader_func_kwargs",
             "tuning_criterion",
             "data_config",
             "metric",
             "weight_only_config",
         ]
         to_delete += list(get_external_data_config().keys())
-        for key in to_delete:
-            if key in run_config:
-                del run_config[key]
+        run_config = exclude_keys(run_config, to_delete)
 
         run_config["op_type_dict"] = (
             run_config["op_type_dict"] or {".*": {"weight": weight_only_config}}
             if run_config["approach"] == "weight_only"
             else None
         )
```

## olive/passes/onnx/quantization.py

```diff
@@ -11,15 +11,15 @@
 
 import onnx
 from packaging import version
 
 from olive.cache import get_local_path_from_root
 from olive.common.config_utils import validate_config
 from olive.common.pydantic_v1 import validator
-from olive.common.utils import hash_string
+from olive.common.utils import exclude_keys, hash_string
 from olive.data.config import DataConfig
 from olive.exception import OlivePassError
 from olive.hardware.accelerator import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_file, model_proto_to_olive_model
@@ -419,17 +419,15 @@
                 {
                     "weight_type": QuantType[run_config["weight_type"]],
                     "extra_options": extra_options,
                 }
             )
 
         # remove keys not needed for quantization
-        for key in to_delete:
-            if key in run_config:
-                del run_config[key]
+        run_config = exclude_keys(run_config, to_delete)
 
         # for ORT version < 1.16.0, set optimize_model to False
         # always set it to False since it is not recommended and is removed in ORT 1.16.0
         # user needs to call pre-process to optimize the model, we already have pre-process option
         if version.parse(OrtVersion) < version.parse("1.16.0"):
             run_config["optimize_model"] = False
 
@@ -459,17 +457,15 @@
                 )
                 # override the run_config with qnn_config
                 # get all attributes of qnn_config
                 run_config = {k: v for k, v in inspect.getmembers(qnn_config) if not k.startswith("_")}
                 # remove the calibration_data_reader from run_config
                 run_config.pop("calibration_data_reader", None)
 
-            for key in ("calibration_data_reader", "use_external_data_format"):
-                if key in run_config:
-                    del run_config[key]
+            run_config = exclude_keys(run_config, ("calibration_data_reader", "use_external_data_format"))
             try:
                 quantize_static(
                     model_input=model.model_path,
                     model_output=tmp_model_path,
                     calibration_data_reader=dataloader,
                     use_external_data_format=True,
                     **run_config,
```

## olive/passes/onnx/transformer_optimization.py

```diff
@@ -5,14 +5,15 @@
 import logging
 from copy import deepcopy
 from pathlib import Path
 from typing import TYPE_CHECKING, Any, Dict, List, Union
 
 import onnx
 
+from olive.common.utils import exclude_keys
 from olive.hardware.accelerator import AcceleratorSpec, Device
 from olive.model import ONNXModelHandler
 from olive.model.utils import HIDDEN_SIZE_NAMES, MODEL_TYPE_MAPPING, NUM_HEADS_NAMES, resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_olive_model
 from olive.passes.pass_config import PassConfigParam
 from olive.strategy.search_parameter import Boolean, Categorical, Conditional
@@ -216,16 +217,15 @@
             "force_fp32_ops",
             "force_fp32_nodes",
             "force_fp16_inputs",
             "use_gqa",
             "input_int32",
         ]
         keys_to_remove += get_external_data_config()
-        for key in keys_to_remove:
-            del run_config[key]
+        run_config = exclude_keys(run_config, keys_to_remove)
 
         if model.model_attributes:
             model_attributes = model.model_attributes
             input_model_type = model_attributes.get("model_type")
             if input_model_type:
                 model_type = MODEL_TYPE_MAPPING.get(input_model_type, input_model_type)
             else:
```

## olive/passes/onnx/vitis_ai_quantization.py

```diff
@@ -7,15 +7,15 @@
 from copy import deepcopy
 from pathlib import Path
 from typing import Any, Callable, Dict, Union
 
 import onnx
 
 from olive.cache import get_local_path_from_root
-from olive.common.utils import hash_string
+from olive.common.utils import exclude_keys, hash_string
 from olive.hardware import AcceleratorSpec
 from olive.model import ONNXModelHandler
 from olive.model.utils import resolve_onnx_path
 from olive.passes import Pass
 from olive.passes.onnx.common import get_external_data_config, model_proto_to_file, model_proto_to_olive_model
 from olive.passes.pass_config import ParamCategory, PassConfigParam
 from olive.resource_path import OLIVE_RESOURCE_ANNOTATIONS, LocalFile
@@ -322,17 +322,15 @@
                 "activation_type": QuantType[run_config["activation_type"]],
                 "weight_type": QuantType[run_config["weight_type"]],
                 "extra_options": extra_options,
             }
         )
 
         # remove keys not needed for quantization
-        for key in to_delete:
-            if key in run_config:
-                del run_config[key]
+        run_config = exclude_keys(run_config, to_delete)
 
         # to be safe, run the quantizer with use_external_data_format set to `True` and
         # `model_output` to a temporary directory
         # reload the model and save to output_model_path using the external data config
         # TODO(XiaoSheng): don't default to use_external_data_format=True if the loading and saving model makes
         # the pass inefficient
         tmp_dir = tempfile.TemporaryDirectory(prefix="olive_vaiq_tmp")
```

## olive/passes/pytorch/torch_trt_conversion.py

```diff
@@ -65,15 +65,17 @@
                 ),
             ),
         }
 
     def validate_search_point(
         self, search_point: Dict[str, Any], accelerator_spec: AcceleratorSpec, with_fixed_value: bool = False
     ) -> bool:
-        if accelerator_spec.accelerator_type != Device.GPU:
+        # since the run will leverage the host device to move the model to device,
+        # we need to check if the host device is GPU
+        if self.host_device != Device.GPU:
             logger.info("TorchTRTConversion only supports GPU.")
             return False
         return True
 
     @torch.no_grad()
     def _run_for_config(
         self, model: PyTorchModelHandler, data_root: str, config: Dict[str, Any], output_model_path: str
```

## olive/systems/azureml/aml_system.py

```diff
@@ -345,16 +345,18 @@
         outputs = outputs or {}
         parameters.extend([f"--{param} ${{{{outputs.{param}}}}}" for param in outputs])
 
         cmd_line = f"python {script_name} {' '.join(parameters)}"
         env_vars = copy.deepcopy(self.env_vars) if self.env_vars else {}
         env_vars["OLIVE_LOG_LEVEL"] = logging.getLevelName(logger.getEffectiveLevel())
 
+        # the name need to be lowercase
+        # https://github.com/Azure/azure-sdk-for-python/blob/8b5217499caedba762b47fa6a118e51209f6f604/sdk/ml/azure-ai-ml/azure/ai/ml/entities/_builders/base_node.py#L217
         return command(
-            name=name,
+            name=name.lower(),  # convert to lowercase to avoid AzureML name restrictions
             display_name=display_name,
             description=description,
             command=cmd_line,
             resources=resources,
             environment=aml_environment,
             environment_variables=env_vars,
             code=str(code),
```

## olive/systems/isolated_ort/inference_runner.py

```diff
@@ -24,14 +24,16 @@
 def get_args(raw_args):
     parser = argparse.ArgumentParser(description="Onnx model inference")
 
     parser.add_argument(
         "--config_path", type=Path, required=True, help="Path to configuration for the inference to be run"
     )
     parser.add_argument("--model_path", type=Path, required=True, help="Path to onnx model")
+    parser.add_argument("--external_initializers_path", type=Path, help="Path to external initializers")
+    parser.add_argument("--constant_inputs_path", type=Path, help="Path to constant inputs")
     parser.add_argument("--input_dir", type=Path, required=True, help="Path to input directory")
     parser.add_argument("--output_dir", type=Path, required=True, help="Path to output directory")
 
     return parser.parse_args(raw_args)
 
 
 def load_batch(input_dir: Path, batch_file: str) -> Dict:
@@ -43,26 +45,35 @@
 
     # load inference setting
     with args.config_path.open() as f:
         config = json.load(f)
 
     # create session
     session = get_ort_inference_session(
-        args.model_path, config["inference_settings"], config.get("use_ort_extensions", False)
+        args.model_path,
+        config["inference_settings"],
+        config.get("use_ort_extensions", False),
+        external_initializers=np.load(args.external_initializers_path) if args.external_initializers_path else None,
     )
 
+    # load constant inputs
+    constant_inputs = None
+    if args.constant_inputs_path:
+        constant_inputs = np.load(args.constant_inputs_path)
+
     # get first batch
     input_feed = load_batch(args.input_dir, "input_0.npz" if config["mode"] == "inference" else "input.npz")
     session_wrapper = OrtInferenceSession(
         session,
         io_bind=config.get("io_bind", False),
         device=config.get("device", "cpu"),
         shared_kv_buffer=config.get("shared_kv_buffer", False),
         use_fp16=config.get("use_fp16", False),
         input_feed=input_feed,
+        constant_inputs=constant_inputs,
     )
 
     # run inference
     if config["mode"] == "inference":
         for i in range(config["num_batches"]):
             input_feed = load_batch(args.input_dir, f"input_{i}.npz")
             result = session_wrapper.run(input_feed)
```

## olive/systems/isolated_ort/isolated_ort_system.py

```diff
@@ -117,33 +117,24 @@
             "use_ort_extensions": model.use_ort_extensions,
             "io_bind": cls.io_bind_enabled(metric, model.inference_settings),
             "device": str(device),
             "share_kv_buffer": metric.user_config.shared_kv_buffer,
             "use_fp16": any(v == "float16" for v in model.get_io_config()["input_types"]),
         }
 
-    def _run_inference(
-        self,
-        config_path: Union[str, Path],
-        model_path: Union[str, Path],
-        input_dir: Union[str, Path],
-        output_dir: Union[str, Path],
-    ):
-        command = [
-            self.executable,
-            str(self.inference_runner_path),
-            "--config_path",
-            str(config_path),
-            "--model_path",
-            str(model_path),
-            "--input_dir",
-            str(input_dir),
-            "--output_dir",
-            str(output_dir),
-        ]
+    def _run_inference(self, **kwargs):
+        """Run inference using the inference runner.
+
+        :param kwargs: arguments to be passed to the inference runner
+        """
+        command = [self.executable, str(self.inference_runner_path)]
+        for key, value in kwargs.items():
+            if not value:
+                continue
+            command.extend([f"--{key}", str(value)])
         run_subprocess(command, self.environ, check=True)
 
     def _inference(
         self,
         model: "ONNXModelHandler",
         metric: "Metric",
         dataloader: Dataset,
@@ -182,15 +173,22 @@
             # save inference config
             config_path = temp_dir_path / "config.json"
             with config_path.open("w") as f:
                 json.dump(inference_config, f)
             logger.debug("Inference config: %s", inference_config)
 
             # run inference
-            self._run_inference(config_path, model.model_path, input_dir, output_dir)
+            self._run_inference(
+                config_path=config_path,
+                model_path=model.model_path,
+                input_dir=input_dir,
+                output_dir=output_dir,
+                external_initializers_path=model.external_initializers_path,
+                constant_inputs_path=model.constant_inputs_path,
+            )
 
             # load and process output
             for idx in range(num_batches):
                 result = np.load(output_dir / f"output_{idx}.npy")
                 if is_single_tensor_output:
                     result = torch.Tensor(result[0])
                 else:
@@ -263,11 +261,18 @@
 
             # save inference config
             config_path = temp_dir_path / "config.json"
             with config_path.open("w") as f:
                 json.dump(inference_config, f)
 
             # run inference
-            self._run_inference(config_path, model.model_path, input_dir, output_dir)
+            self._run_inference(
+                config_path=config_path,
+                model_path=model.model_path,
+                input_dir=input_dir,
+                output_dir=output_dir,
+                external_initializers_path=model.external_initializers_path,
+                constant_inputs_path=model.constant_inputs_path,
+            )
 
             # load output
             return np.load(output_dir / "output.npy").tolist()
```

## olive/workflows/run/config.py

```diff
@@ -37,29 +37,17 @@
     output_name: str = None
     packaging_config: Union[PackagingConfig, List[PackagingConfig]] = None
     log_severity_level: int = 1
     ort_log_severity_level: int = 3
     ort_py_log_severity_level: int = 3
     log_to_file: bool = False
 
-    def create_engine(self):
-        config = self.dict()
-        to_del = [
-            "evaluate_input_model",
-            "output_dir",
-            "output_name",
-            "packaging_config",
-            "log_severity_level",
-            "ort_log_severity_level",
-            "ort_py_log_severity_level",
-            "log_to_file",
-        ]
-        for key in to_del:
-            del config[key]
-        return Engine(config)
+    def create_engine(self, azureml_client_config):
+        config = self.dict(include=EngineConfig.__fields__.keys())
+        return Engine(**config, azureml_client_config=azureml_client_config)
 
 
 INPUT_MODEL_DATA_CONFIG = "__input_model_data_config__"
 
 
 class RunConfig(ConfigBase):
     azureml_client: AzureMLClientConfig = None
```

## olive/workflows/run/run.py

```diff
@@ -131,18 +131,15 @@
     # ort_log_severity_level: C++ logging levels
     ort.set_default_logger_severity(run_config.engine.ort_log_severity_level)
 
     # input model
     input_model = run_config.input_model
 
     # Azure ML Client
-    if run_config.azureml_client:
-        run_config.engine.azureml_client_config = run_config.azureml_client
-
-    engine = run_config.engine.create_engine()
+    engine = run_config.engine.create_engine(run_config.azureml_client)
 
     # run_config file will be uploaded to AML job
     is_azureml_system = (run_config.engine.host is not None and run_config.engine.host.type == SystemType.AzureML) or (
         run_config.engine.target is not None and run_config.engine.target.type == SystemType.AzureML
     )
 
     if is_azureml_system:
```

## Comparing `olive_ai-0.5.1.dist-info/LICENSE` & `olive_ai-0.5.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `olive_ai-0.5.1.dist-info/METADATA` & `olive_ai-0.5.2.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olive-ai
-Version: 0.5.1
+Version: 0.5.2
 Summary: Olive is an easy-to-use hardware-aware model optimization tool that composes industry-leading techniques across model compression, optimization, and compilation.
 Home-page: https://microsoft.github.io/Olive/
 Download-URL: https://github.com/microsoft/Olive/tags
 Author: Microsoft Corporation
 Author-email: olivedevteam@microsoft.com
 License: MIT License
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `olive_ai-0.5.1.dist-info/NOTICE.txt` & `olive_ai-0.5.2.dist-info/NOTICE.txt`

 * *Files identical despite different names*

## Comparing `olive_ai-0.5.1.dist-info/RECORD` & `olive_ai-0.5.2.dist-info/RECORD`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,29 @@
-olive/__init__.py,sha256=srNwPJte4clvSqTC73GA3slcx1kTDs6NxNW6LNhuqHk,608
+olive/__init__.py,sha256=rMh3IndQNs7Kpguw0x6VP4CDSLbFKe3MEmhVwBAJ9po,608
 olive/cache.py,sha256=8fTz93_iPpzM6UGr0y04fhVw-Xpip4dBLxVKxHM_2kQ,9998
-olive/constants.py,sha256=20IZURQJHfX4spfzUjcLZ-HsFqgdM2-JrwcJ8QnFKJo,1113
+olive/constants.py,sha256=vHZgfVTreESqTShRFI9dmx9IfdLlfHL3fegwmYQzNE0,1162
 olive/logging.py,sha256=VcJnHwDqDsWuw46HqgMOCfCgCNi2axFQYaxVFhrd8lI,2626
-olive/olive_config.json,sha256=aRrvxMiUiz2-tt6h54nZrLSI8s30rK5XlWew2TTa5SY,7817
+olive/olive_config.json,sha256=cZQv-qU4CA2A36QHHxqKpN-pXGUKKJdFMMHjuvlJ_Dw,8038
 olive/package_config.py,sha256=ZsgHwNHGwjh0zIzlZn7qBmLiz8yB9nXXfA6azwh_S28,1406
 olive/resource_path.py,sha256=dPBcwg9KqYib7N75O8-ZT-_MxlXqGdHC2kiY2oDzLiU,22999
 olive/auto_optimizer/__init__.py,sha256=DC-U5sReV5weVF-A6Rn2-OA9BGxeBpYpg1VBpNrygCw,5181
 olive/auto_optimizer/regulate_mixins.py,sha256=X7G3UOOSH7Z9ZhD3QfCVpfIMtWksP_84UlK6ijItjJQ,5871
 olive/auto_optimizer/template_mapping.py,sha256=6wgYD_X61GilGYRVCEvkwcYXSuhEWokgsdBKNxujaiQ,3615
 olive/auto_optimizer/config_template/opt_level_passes.yaml,sha256=A2ZE_u8mrWQ1I30tcHuft7FdY70eWFxuD6r_VMEgn90,1171
 olive/auto_optimizer/config_template/pass_capability.yaml,sha256=FfmafalzQSkImDnqCnJvZCgqXaDdZlMh9J2VIClWhOo,2062
 olive/azureml/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
-olive/azureml/azureml_client.py,sha256=Fccb0afmMc2PKXi1bH-8V9Nj4Z_mMBtfyRrC5LZnuPY,6412
+olive/azureml/azureml_client.py,sha256=8IpXgGImz9WLNHTyjHbnK4DjXR_vkDXLVfFtaWNwbrw,6699
 olive/common/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/common/auto_config.py,sha256=yNfcSrh1z_gQLSsiYFn63k5x-qT33t-S1y97J42uvnA,3430
 olive/common/config_utils.py,sha256=57gPIim-aDFScw3AamYnRZccXz8sc4KC_uOAUfvTObQ,10881
 olive/common/import_lib.py,sha256=KrWnGR2Pe1RWfOqe3DL96Aq0O8zXzYHxJc0d2zgMdlU,1488
-olive/common/ort_inference.py,sha256=hVS2ep47Nx3d8WNhnT6BhsA3VGcU13iSPgFNEDl2LTk,16029
+olive/common/ort_inference.py,sha256=oI1swvgxWi4BR_ENKiOnn030GFcCTge7MIto414mZN4,18360
 olive/common/pydantic_v1.py,sha256=vNddf08_5YT58wfDL3A38TaniE6xku-CMa7rIdesOZ8,765
 olive/common/user_module_loader.py,sha256=FfRLFiEvGw2yT9EKULc4eIr4a0CP_lGms2SkXNg0xa0,1809
-olive/common/utils.py,sha256=GttHdpJPy2PxcA330lIqzs8oVRuyzXsCj0AJPr00pdE,11627
+olive/common/utils.py,sha256=tG0WIdwp0Y0FUkHwQlfKIduP5YdOHp76mDYEmd2XS_Y,11789
 olive/data/__init__.py,sha256=e6E8AVlCoJ-LNfbshkiyOVopkfgUmg6dRo9LH51Mafw,345
 olive/data/config.py,sha256=Ro9bPuIHe6V1mhm9DcdHggq2gdu1_2bbAJ8krwewOIc,10680
 olive/data/constants.py,sha256=v4_EcRT473PBqIJDJW54HiMWP_OboMKILUd7cf4MwR4,1443
 olive/data/registry.py,sha256=hZi_GKCKWu9SbxpMiJ9OR7q-yNKIunpTUzdXY9cPipI,8119
 olive/data/template.py,sha256=wJQGctfoMiJGIf5gB1Kp2kbJlofYujSg9vl3KGO-47E,3573
 olive/data/component/__init__.py,sha256=fo0PIFNXx16c4CMOTlxaIj8UlZvApJ3-Pca18AK3qQY,444
 olive/data/component/dataloader.py,sha256=beCT0mojWX09OGPyL2cR2pUSXMRv_kHohHDv4tJwj1s,1955
@@ -33,17 +33,17 @@
 olive/data/component/pre_process_data.py,sha256=nrzmMxKHlRu8V3C4E88sqyVrtCe3_99R_Q-vFv8aXss,11446
 olive/data/component/text_generation.py,sha256=gxaKqJAoUpR84WVJUUuBFsSkXRV6MBgIX9pAkV03Vck,29278
 olive/data/container/__init__.py,sha256=LDGROQwmhlEeOzEtSRG0UWushVKko-gu_EvHw0g6XJg,480
 olive/data/container/data_container.py,sha256=CJ8HBjcoDPAOX-zVUaOtS7wJGSnrkvNK5-QkSjSho1E,3385
 olive/data/container/dummy_data_container.py,sha256=4C_mhjK1qUKaytBrCzHR3TUfYYvQxDtgOXP2iRMhPwk,1159
 olive/data/container/huggingface_container.py,sha256=C1nMtdmVkDDviL-jyY5_lK9aN2dzRMcAKASoQ9Iysjk,1690
 olive/data/container/raw_data_container.py,sha256=YqjbFWH6KI51_TEI_YFBjjDMFKwKMx2M7SN8jbbBZYI,1721
-olive/engine/__init__.py,sha256=QSFcQLIESkRdgcFPbgVNHRg3iVSHmlRQWZtpdS_74K4,411
-olive/engine/config.py,sha256=1kz_aLyD0c7jHQZjgY4Nsk9SJdpSDx4zP7xXJWKa2As,1447
-olive/engine/engine.py,sha256=MSv7V_kuOMwT1nShj54RqE0n39w1JGhl2xdodr8CZkU,46635
+olive/engine/__init__.py,sha256=sK_oyURVPbwXYIzb3PcUG3Lh0dUZJ-Ot7SWL9laJojk,442
+olive/engine/config.py,sha256=LBDTo3OtIu__EMl3xKys0C-FRO1QKX92rf0Q7Ognyew,1199
+olive/engine/engine.py,sha256=LQvsYIqYhEQzE5CNQ-kw39KQ5_e8vOeJqy8ozedwths,45969
 olive/engine/footprint.py,sha256=C_s1OyI9yt8pal76WQ13WbHfu-B1oD0oKb3pvjzdvJI,17410
 olive/engine/packaging/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/engine/packaging/packaging_config.py,sha256=LImhOApwoSPlKNV7dbVC1BenR2I_-M9H6td5T4TZAzo,1642
 olive/engine/packaging/packaging_generator.py,sha256=y9we8MVWV5H3V6uIZ0NR5f63Am27YFVmt_ZbUx5r3DA,19748
 olive/engine/packaging/sample_code/ONNXModel/cpp/README.md,sha256=JnLAiNYgEZCvsP0rwG5rTOwn_px6XeLFjrchXUDWO4s,1588
 olive/engine/packaging/sample_code/ONNXModel/cpp/code_sample.cpp,sha256=4FejpIKRXN9-9LuWvkoFGMCgnuhRZxFA6m_9E6yrNQs,4990
 olive/engine/packaging/sample_code/ONNXModel/cs/README.md,sha256=V7tDnmXiisTAbiCec7Us-pUvI3XuJEc6EE1cO2WXt0A,1590
@@ -51,31 +51,31 @@
 olive/engine/packaging/sample_code/ONNXModel/python/README.md,sha256=z2awTxd97vnQwNuQ08WOid4MiuGQghTJ3EI4Fo5Zb38,2296
 olive/engine/packaging/sample_code/ONNXModel/python/code_sample.py,sha256=HYIiEfvQObTDI6Bh3DP3fSbwvEp9PQ7YcdX8YGTGzw8,2545
 olive/evaluator/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/evaluator/accuracy.py,sha256=HV17zTBx2U-H9BkM9cF7EbLWkOUyzHkySWX77mb9DaU,6473
 olive/evaluator/metric.py,sha256=yE3_zK_JanrxKM5LBhPb1zNJwgIt1sofW-4BxhjT6n0,8723
 olive/evaluator/metric_backend.py,sha256=2Trmgtcet7bmJTCKb3jDYzNYdLBwtY4xqnpDGG-O6po,4461
 olive/evaluator/metric_config.py,sha256=HDA9Ek4PgtY3QQj5tMGVHjqu-2d64cUEIOscTLqQkoI,4395
-olive/evaluator/olive_evaluator.py,sha256=ndyiABMBa875RecgQ90zrPR3e-5FaezkAx4BX09ZVNc,47429
+olive/evaluator/olive_evaluator.py,sha256=QRrora4pTGWP62H020g2dm4c40T6GwdzbNnbWoqmfKg,47694
 olive/exception/__init__.py,sha256=ycjIjR_iwg4ZcCuRtbHZpEbIw-4RzlurOa6o5tz8NA0,592
 olive/hardware/__init__.py,sha256=89KKeZDoW0jvqeOOrgaLoGFKZxVhh2jFLbAioi0hEi0,621
 olive/hardware/accelerator.py,sha256=2i_qGlWhxCsVVmRTnclDr7X_4jkgGDnjRQLFSBQuk6g,15059
 olive/hardware/constants.py,sha256=ZzHG-NRYy6L_XM-CSKSxv7pxcGLyXrKzLapqtafKmV0,1273
 olive/model/__init__.py,sha256=ogykDHRcG2bcvxHJMYLzJb30SbpNmtDpzbIBfboVVV4,451
 olive/model/config/__init__.py,sha256=HqUlWk6oUdFksNgoz9z77mgE8r8Xlb2DkZl2iub40yw,482
 olive/model/config/hf_config.py,sha256=ZGMo6BnTMs7M4WfqcDmqTO-Wbuj-NgG8S6IKcvBZuPw,10950
 olive/model/config/io_config.py,sha256=NF3LMWwwaNkSnT7iShk04aISRVJ3T4g_5odt-t8l08A,4843
 olive/model/config/model_config.py,sha256=X-kPWyMmHjB3WI6KUV7fgze2o3sS93SpiMsVpyqCbJk,3943
 olive/model/config/registry.py,sha256=PFa1p9xVBRHduXDa8UyzjXH8M6YSJ91nSyXa5e7Z8aE,1045
 olive/model/handler/__init__.py,sha256=dAx_DTEF4JOGePcPECDBqFWnkh1lHxAU7pYBrsxa9Ko,1139
 olive/model/handler/base.py,sha256=lPZOI9fAkCXpXZp4Yzi8xIhAtqDbR-Izccq5UYqtNiQ,3190
 olive/model/handler/composite.py,sha256=HaKW30CPj6G_nqFbWDQoo-DEHnBBSk1e4vS550Adc68,4461
-olive/model/handler/onnx.py,sha256=EuqtSqiFWg64xeSKROPXIcEpKpFsFxuedH_jw3bwIhg,8706
+olive/model/handler/onnx.py,sha256=NOl-g6T2lIuInehFFdO88b8__TzzkCCkzcylyOqvd7c,10069
 olive/model/handler/openvino.py,sha256=JIcZsjZ1wrsUgHVE4sYb8mwXnoS2zN2wGV4OZdE7Ajw,3556
-olive/model/handler/pytorch.py,sha256=WAMqQltXVH48zw6B3oCLWGa5Nvqg9P7GJ8yDhXCterY,16490
+olive/model/handler/pytorch.py,sha256=6WunjjQElAa1iW_sOeIpbv0mUtWrgXhqinHjePBJOCo,16898
 olive/model/handler/qnn.py,sha256=77nhGBAa1KL5mxGWOOmNJcV7vkCqsLoina_5YWrq23M,4704
 olive/model/handler/snpe.py,sha256=QRxfGSQ6FrPCZGtQXjfRKhHHMvvFbuGq_j1Y_AL-IVE,2597
 olive/model/handler/tensorflow.py,sha256=dLLkfXrpuxG0ab93p7k1c3M0c_Kjjub78Rde__lox2o,1474
 olive/model/handler/mixin/__init__.py,sha256=HnupHTH3k-xB5XlpRjx8uuRQdKTiRX1tFu_vhb-xN4w,936
 olive/model/handler/mixin/composite.py,sha256=qpQ41-7XsIz2l5X8ab2-gt6OZJDPZUInacW-1H9HopQ,418
 olive/model/handler/mixin/dummy_inputs.py,sha256=U-e257lcwqEkLgNTMPO5VczLU92Le7w-CXdBvZh5DDw,3021
 olive/model/handler/mixin/hf_config.py,sha256=hiffIeyfFDJ1klhOwJ8dgRgq6-5ivOMtB2Lio1PLNXc,3967
@@ -84,40 +84,42 @@
 olive/model/handler/mixin/onnx_ep.py,sha256=bZ4xKLSDpdR-AZaB2w_785IRU_qStLqs-G9eTPNQeJA,1402
 olive/model/handler/mixin/onnx_graph.py,sha256=PwVntvtKZuxFTPjssee_Hbc-xUrLTUBkbsDEtozuyHA,3946
 olive/model/handler/mixin/resource.py,sha256=VvVsto2k1AfNSzH7zxdgpYvt6gDiTcWlFsaPelA3M_M,2998
 olive/model/utils/__init__.py,sha256=OViqJhejw6VYFg7BO_zhp2WeCJzr9YPjUXumynwhARs,609
 olive/model/utils/hf_mappings.py,sha256=HJLxWMhTXSCmYW9NnCsn4Wr9PmGO39i2H9xEdrZ4L4U,3091
 olive/model/utils/hf_onnx_config.py,sha256=5njt4Ko5NCL_3Ipy0wdUwvjmaxLmwdACT5iuNWXnw9g,4517
 olive/model/utils/hf_utils.py,sha256=8LPvDe50b_Eaf6qdmawaGdLOVFwE7eKvmtTXlVUsBo0,8183
-olive/model/utils/onnx_utils.py,sha256=dMC2_m7rvLx9NTt8KxUCucrC70wFkSF48hNv6IlBrN4,2893
+olive/model/utils/onnx_utils.py,sha256=zo0CtDRWOyStOKMHJZdL7Ad5ocMgN9vuui2CFtY-dM0,3467
 olive/model/utils/path_utils.py,sha256=lu4r8V_PjCyFrlzxfAUZrRKAa3VhV67o9_4noYE1V2g,1510
 olive/passes/__init__.py,sha256=kzwYdsbpTo9ipqKgoTRf1hV-Jr2OnJlqdg_3-3iiECM,499
 olive/passes/olive_pass.py,sha256=GjmwtSVu8ZXuJxmyESxczmvs6ALpR58lm6qadIj-7QI,19895
 olive/passes/pass_config.py,sha256=Ijdjp_1NAtMkhrM7jE-024aTdJF98CQsRTtb0xHp8hw,6139
 olive/passes/onnx/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/onnx/append_pre_post_processing_ops.py,sha256=pYwd1LeAFym37hLknAIi90UqLTeCCzLRuzhbJVfUifQ,8408
 olive/passes/onnx/bnb_quantization.py,sha256=s9SfMEHXizkwP85VBpmPYxPiqTnCgyMA-7Sj0FqzXmI,5524
-olive/passes/onnx/common.py,sha256=Y53MVrBhIKDQLCnvOlsRkxa_A6p9I2djDXVDMTbYnNw,7485
-olive/passes/onnx/conversion.py,sha256=TkyQrRrO1Tcc6DOi3U8C3PScmHLHte1g1rOqTtJsKi0,27072
+olive/passes/onnx/common.py,sha256=lmPktG3KFd9b_akPtnvUXgkEr7lKtlANkv4zHMxXmXE,7639
+olive/passes/onnx/conversion.py,sha256=v2lDq-_T3P7R0_mxSDsOJieMtPd6ZAUjGMIr65i7hn8,27526
 olive/passes/onnx/dynamic_to_fixed_shape.py,sha256=Qf9WEa088IZgFddNX-aFANEy_2N6aWaHXg9-Bwo5Qqc,4862
+olive/passes/onnx/extract_adapters.py,sha256=cG4nuifwAXOSSDu6EC2GxcPksbRcYytjzsoQ6dMRXx4,14055
 olive/passes/onnx/float16_conversion.py,sha256=zzBB4q8I_MXExjwVJTFD_W4KGMtAJRxowwU5sEqKrRY,3090
-olive/passes/onnx/genai_model_exporter.py,sha256=cQ3HLl93BdvqBr7xZ8aNHnHNUvuG4J8qJDHfBoYYCl4,3491
-olive/passes/onnx/inc_quantization.py,sha256=owgy3tnFxDO57RIzV2xGPDEfe1OFRMH9xXnLK4xYFjg,27095
+olive/passes/onnx/genai_model_exporter.py,sha256=IMhlvLHuOB_LLiLHrp2aKgFWCpK1eoqMoOtNIY8bl4k,4556
+olive/passes/onnx/inc_quantization.py,sha256=hHKslRJsbxCemHQDtAqIKfldVRl4E25sOaglbEcCIzE,27096
 olive/passes/onnx/insert_beam_search.py,sha256=6hEavIrzEK8VoSzhrFp05hprSCKzNn6UFdjyHg_bkJU,15972
 olive/passes/onnx/merge_decoders.py,sha256=NNKKa0-FVa1vog_g-4LPSf916Zk3aFVA1wEVUhnj6tw,18495
 olive/passes/onnx/mixed_precision.py,sha256=RS7Rmaoknc76_0qdMw_tEnIdJxvlAIku7LHunjjj4oU,9054
 olive/passes/onnx/model_optimizer.py,sha256=0l2BmghwWBCK-08F90TO7VY1swU6_AY3-LqVXyQCH-Q,10011
 olive/passes/onnx/moe_experts_distributor.py,sha256=GBdDgDpiTjWCVwHFnwmubZGxNJP8smz6KCqzTraJHiw,15752
+olive/passes/onnx/onnx_dag.py,sha256=P6_tPFH6zFxx2xxkjJYQK0uFDG6Q0EHMDBeny9enUrA,18666
 olive/passes/onnx/optimum_conversion.py,sha256=HDcMkyrfeIFSvuQbD33YGzqS7A2JDn_B1zKJGUbDedk,6162
 olive/passes/onnx/optimum_merging.py,sha256=OSh2gSAOjXj_BIFX_NfRMWWlDPTHlKWmEjYIcAXhSps,3709
 olive/passes/onnx/perf_tuning.py,sha256=HaEHnIkQK5nVJe2dVwfhAvLi0jRE0LtQaznDj9tKKRc,29003
 olive/passes/onnx/qnn_preprocess.py,sha256=C3KsKo7DpJP-L030LvVnoCzW1ax4CDefn03yRiCy8BM,5375
-olive/passes/onnx/quantization.py,sha256=suwQHlhS5emvQ5Ru8TBJ_HPWCarM8bSqVp2fcWN0gHg,37646
-olive/passes/onnx/transformer_optimization.py,sha256=HYxWW5kBQ0zVCn4nLsQvCbeE41cuNHJcC6kRO9eVCtQ,19253
-olive/passes/onnx/vitis_ai_quantization.py,sha256=F0jveoEo8Qb1Jbg4EZwadhQv26PpWD6naq-BC4glvks,15134
+olive/passes/onnx/quantization.py,sha256=JL971yrSgwuiTMPwgwQNPfuWb7F6TJrYTWzjZu-ZYcA,37566
+olive/passes/onnx/transformer_optimization.py,sha256=t-4W-l1NNENerO33IVFimZWaOnMkaYnabSZpiYnwTME,19292
+olive/passes/onnx/vitis_ai_quantization.py,sha256=Y6cZexKW6cLAaJ3Ii1L9cXdNwN0zeMIdsXiRFCJys8c,15105
 olive/passes/onnx/pipeline/__init__.py,sha256=hy6ZqdDw4q53FSvRAM5nh7dCOGt1ESZagOqThowBZAI,3239
 olive/passes/onnx/pipeline/step_utils.py,sha256=YxajZp5gVU0UVpHrbonNJwZL8CHiNI5TVpye0WGpIVw,8457
 olive/passes/onnx/vitis_ai/__init__.py,sha256=WcngHdIXOp4kglwsc_G4qqBKU-wsyNk94ibGQkSv-eU,508
 olive/passes/onnx/vitis_ai/calibrate.py,sha256=IXLi6rSAwJ4fX-POa9dwHSlwPYSKsXN62g7tdUat5CY,7762
 olive/passes/onnx/vitis_ai/quant_utils.py,sha256=5YrlKa3QLpCd8rgZ1uSnRFApXlH9tQ68J4RPASX73U0,15332
 olive/passes/onnx/vitis_ai/quantize.py,sha256=2p6fpiJ8WGxeMhH9h1rWo83ocfc9lHtp2fcrCnf3A2w,13580
 olive/passes/onnx/vitis_ai/quantizer.py,sha256=n8IK8jb3b7PIFDmBK1WCxzsq3LvWxCUUgoxgg2td4LI,36359
@@ -129,20 +131,21 @@
 olive/passes/pytorch/cluster.py,sha256=wPZilm6bpu8_KvhVYUdy4fM9b1US3bE-3IWPqDqi9gs,7058
 olive/passes/pytorch/gptq.py,sha256=Ytq51gMdHVfOVJR0SCFlGnBMhvuH35CtIBNF9twgFJQ,9842
 olive/passes/pytorch/gptq_utils.py,sha256=oCTV62B4jmffUDVQm2ceBN4iY91cAhSntLn8EKF6jEM,11528
 olive/passes/pytorch/lora.py,sha256=ljq2FmlNvjL1asoZZtXhn-oWpfNEJFUTkgbHb5ZsHYI,48812
 olive/passes/pytorch/pytorch_lightning_utils.py,sha256=JyHsdwapI9Z1d7b95MMCEGqpT3FvwzPMT8iOO84CsZU,1021
 olive/passes/pytorch/qat_utils.py,sha256=f08zUGQTvEMsSTDKmIl1Aa2VkRjAW4_sFxhrGZOMp_o,8038
 olive/passes/pytorch/quantization_aware_training.py,sha256=dl2YSOJoXuTWG8vQM_uQqvnrqBu86IGXEQrH9J4UPU4,6444
+olive/passes/pytorch/slicegpt.py,sha256=CP0HlDxEvMWcoUUIDg2DsnsTdLiPqROX_C229nVfcHk,7085
 olive/passes/pytorch/sparsegpt.py,sha256=96vnAWMe4KMcG4-LcdNlxluyUBuO9fIpH2mjx4s5JPE,9021
 olive/passes/pytorch/sparsegpt_utils.py,sha256=PgqZh_HYV9DTzURT0T269r984KxDNhKZQ10sfDDEjpc,10774
 olive/passes/pytorch/tensor_parallel.py,sha256=Ft798VoHjXKLlDItvwydPnvF9ak2FKyOYbVPg7rWkiU,7032
 olive/passes/pytorch/tensor_parallel_layers.py,sha256=91Cc4y_xfP_TNBg83izDXxD7Ot8g4zWkc-ajMc-8AmM,5372
 olive/passes/pytorch/tensor_parallel_llama2.py,sha256=X3lbqPif5VoVia03lma5AuLYrx8SCp5NGXKXh6DS7Zw,17239
-olive/passes/pytorch/torch_trt_conversion.py,sha256=QhZUtkmPCCMeAilZrobpW95hwYz_yQ4j6gQH_C2tpCw,8053
+olive/passes/pytorch/torch_trt_conversion.py,sha256=lEJcNC-gXR_xXBps7R-HBAu3qlqMdSkWONe9Gb63v4s,8172
 olive/passes/pytorch/trt_utils.py,sha256=yXqmVoRruHl8raI3ySj8GItaPEbRstqbZo7G-HLZiBI,3185
 olive/passes/qnn/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/qnn/context_binary_generator.py,sha256=2EEBfThotk2288WXsU-eTjZWq410sv8bMfdqG_ICBx0,3192
 olive/passes/qnn/conversion.py,sha256=atW7a7OsXL3YvxeeOr7q1X0hx5QnSkN5RwMCs4QGRys,5268
 olive/passes/qnn/model_lib_generator.py,sha256=aDjHkUZ4To8JEu-9wo7RHbF2j278dCPwhSSiGnrG0RQ,3298
 olive/passes/snpe/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/passes/snpe/conversion.py,sha256=0zUfbIP_3NKgyDxK5bKrm4AA5lSbJAF0yVXO-R8n7S8,4802
@@ -171,14 +174,15 @@
 olive/platform_sdk/qualcomm/snpe/tools/inference.py,sha256=W0Om9Z203cISj38813WuVXuP8Wif0DWOYwtcTEJZ_qg,19039
 olive/platform_sdk/qualcomm/snpe/utils/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/platform_sdk/qualcomm/snpe/utils/adb.py,sha256=fW9nG-7YARNAglJIRry4t-9UwcycbFhSYWoByNHKxhE,6978
 olive/platform_sdk/qualcomm/utils/__init__.py,sha256=nU7Vcr7_IqPRj7pYSd2ApPT_KRQxpQUapEQAlVR3yG8,374
 olive/platform_sdk/qualcomm/utils/data_loader.py,sha256=BAWOMxoDKKZESo0Owlegae3gtBl8WWnDvGgDSSt1YSs,14746
 olive/platform_sdk/qualcomm/utils/input_list.py,sha256=mvQQlu154du1f4iawpw-FwxPWEHMfSXR-2EPxDtlUCs,8878
 olive/scripts/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
+olive/scripts/export_adapters.py,sha256=tJuteakhOnkQjjLL71vmqoQFjwN-uQAycCElAOLR-Ac,3130
 olive/scripts/manage_compute_instance.py,sha256=9yRsfSbIQDMrlI90wUMk1SWr8-yFnxRm9vLwKg8710I,6435
 olive/strategy/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/strategy/search_parameter.py,sha256=FmKvyblJHZbS1gAh1S7589WE6yL2MbIKL38-io_yDyQ,11837
 olive/strategy/search_results.py,sha256=fD0uXHefoLDWdRzM5I36yGyM8OBLHrY9NFqGqBiTTs0,5631
 olive/strategy/search_space.py,sha256=jYGOECHWZkkVahQVTUbPe09cXoiSIxcr4iZBCoWbOFs,4702
 olive/strategy/search_strategy.py,sha256=nO9T1dy06O4-yZ0FX_9c-j8eRgr3syREF1R5GmpDg8c,12873
 olive/strategy/utils.py,sha256=5_JB0POwrCN30LFehSafjzeK6I5AJUT0Qfm0xznjZV0,2817
@@ -193,48 +197,48 @@
 olive/systems/local.py,sha256=kWfHWzfPLxybq35FqchqJ7v2PuKIpPzG23qekTH8mUU,2300
 olive/systems/olive_system.py,sha256=guo9D784bL9k9Va9tWOfmtHDDhytrEe0A8Hplnoruvs,2158
 olive/systems/system_alias.py,sha256=rqDxUPiJZNFArMX_mg5No3W7MWOlyppiyG0pk1SmITE,3140
 olive/systems/system_config.py,sha256=M6axCyIKodee8bBYvBJHEaIQRXO4AW9fIZ2aAbJQq0o,7048
 olive/systems/azureml/__init__.py,sha256=XMk00ngVPkLq8SAjhtDDXDUC6FDin5K_s_eu1FGi3qA,411
 olive/systems/azureml/aml_evaluation_runner.py,sha256=nI6kKyA9xsV7oJO5jd_B9h2zZ_5Ez0lknwGyXiZQrZQ,2883
 olive/systems/azureml/aml_pass_runner.py,sha256=rb4KVQS_23l-ogpiV-0TjuOnlRyUI1jJSW8eIXzxEC4,8763
-olive/systems/azureml/aml_system.py,sha256=KP3E2wXj6bu8sz4CqhiPye4Xs3e3mdmFCxowqRFt58w,31831
+olive/systems/azureml/aml_system.py,sha256=Nt89vRaJjjHJe7acyDKb05fMa-7LDaaVciaUFm-GCXU,32108
 olive/systems/docker/Dockerfile,sha256=XAQOT_ruAGlgmeoXG2E7n6clsjMEV03BSwyVps5njpo,717
 olive/systems/docker/Dockerfile.cpu,sha256=o5F5Pc2J_FhtZZT2YrXnLDb1vwhx0OYlTQ_m6LqV7VQ,464
 olive/systems/docker/Dockerfile.gpu,sha256=GdrY3B1IZVB-PADSXF2cEwJWwXjxomJP-qG29a1G45w,1006
 olive/systems/docker/Dockerfile.openvino,sha256=kFtqfQys13L0hx66YxuCMY9XXx-i0D0jtgSL5bASOng,2531
 olive/systems/docker/__init__.py,sha256=nrCMDPi17qCk3iGuH-Hbpq9JIOYkR8nOdvWsfXy9uqM,407
 olive/systems/docker/docker_system.py,sha256=eHFtKIIp8GhtLoCRe4QOKGgUkOzFH4TEA3DYhv-KDzM,18244
 olive/systems/docker/eval.py,sha256=bfeDsxCb6H3P8EqtQGzlzHWpE10D_gUyoZzAZlo4sds,2187
 olive/systems/docker/runner.py,sha256=E9bahyiRo56ZfADz9iiF1FbDDlHwpk1QlEdlRu1IxkQ,1956
 olive/systems/docker/utils.py,sha256=eU0Khr8nvn_BO9j3z6Kp3JRPZpSXVxRSs9qu2Om3XvY,6200
 olive/systems/isolated_ort/__init__.py,sha256=vITx_9_O5lJ6lVD-Eh8f0mbLB5d5sYHX__HgjpAYOLg,357
-olive/systems/isolated_ort/inference_runner.py,sha256=4zxrduxioctdc-80iVjqeqUkKUlegiSBuBE_BrtUqJE,3077
-olive/systems/isolated_ort/isolated_ort_system.py,sha256=CuZf_qhnIXE7RDkdGm4r3ME6N0dtA21Owlr6jgXaTSk,10877
+olive/systems/isolated_ort/inference_runner.py,sha256=Ob69cZe_nFbM0SKj0CaUBVuLhftprHZyQ_yr8RMdDvw,3600
+olive/systems/isolated_ort/isolated_ort_system.py,sha256=GPD97K3VXhZXgbA8BrSUJ9Ao_iDbZ4QAZYYlg7A_dqs,11269
 olive/systems/python_environment/__init__.py,sha256=cu6jFeXKLees7MkoNddzPVre_eE-FwXwA3pihv4yWi4,381
 olive/systems/python_environment/common_requirements.txt,sha256=chggo_d82Zdffa3G3ZKCCpI27wcCn2f17Cziy-x4f0Q,37
 olive/systems/python_environment/evaluation_runner.py,sha256=isVzvA2aHVuCK-qfIyAqjnS03c7vzIXmYIhFjGtiCME,2279
 olive/systems/python_environment/pass_runner.py,sha256=IdvBa0Nd3D8WspdWj8ops3OVJl8b6SDnFYfVVtAlbSM,2037
 olive/systems/python_environment/python_environment_system.py,sha256=PTNWHKu8CJ8KqnUHxpqYLhjVwi-xktz4m5aCGTBLAkY,7892
 olive/systems/utils/__init__.py,sha256=VCiDPtACqpIXj-k-8rpHv2xsW4JYiRVfylM5qkF36RY,705
 olive/systems/utils/arg_parser.py,sha256=ZyFvQ9o6i7SqrNffnmuYvn_jjnGlWcRNSkGkZk9HZhE,2082
 olive/systems/utils/available_providers_runner.py,sha256=0A2C61-D5r9ke5ya2hOBEp1RP_6jgeG67cJC4NlqTH8,913
 olive/systems/utils/misc.py,sha256=YFgTeaBiKXx3ibnDMpORj3U4-dwsqqQ4mkEtJ-sKx-A,7419
 olive/workflows/__init__.py,sha256=2mLegObegOEd5p6MDGX_4-Eto2XvWBFPyr3HIrz4D0g,306
 olive/workflows/run/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/workflows/run/__main__.py,sha256=6awG6OZneIa769QDU6X86X5BxSzBtFByd0K5YQ671RY,1418
-olive/workflows/run/config.py,sha256=PRPdFfa_86Kel4ilOdVAxEy7RQX-Y9VbFsP-po6edjc,13710
-olive/workflows/run/run.py,sha256=_LyCQGMTcz21iP7GrydJgqr-xtXQsTinN9RU3ZSvXQw,13451
+olive/workflows/run/config.py,sha256=t2c2vMli_hVcBpjikrGAll1ddAnE8fPlULALg8Ox2EU,13473
+olive/workflows/run/run.py,sha256=5N4_KMuALfyvPz3PcVelDBGvFTZNgfktab2smuiMg4w,13365
 olive/workflows/snpe/__init__.py,sha256=wqFn-4s3Sxzuy0Oa2euleTB7qUO-4g63bV2h7TW5XGU,431
 olive/workflows/snpe/convertquantize/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/workflows/snpe/convertquantize/__main__.py,sha256=re1UWNmJI_E9ubcrAEs4JeP_A4C3LBQMnVofw9TvI40,1339
 olive/workflows/snpe/convertquantize/convertquantize.py,sha256=GaM0LpjcZVgi89vh8r0losJDltNC6sKZtRB1rUVxXbU,4445
 olive/workflows/snpe/evaluate/__init__.py,sha256=WSNxt3l4lkWA_0vhw1ED4I7KOO0mnAuHwSgFYqbq0Lg,247
 olive/workflows/snpe/evaluate/__main__.py,sha256=UAmzVqOnC90Ns3l8oBhHPheyEC2kncFgC-Gl7qXAoEQ,955
 olive/workflows/snpe/evaluate/evaluate.py,sha256=NGRS_9whYc4wvSola46jLiQduSb4mVr1AKlpCr-bmB0,2974
-olive_ai-0.5.1.dist-info/LICENSE,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
-olive_ai-0.5.1.dist-info/METADATA,sha256=pyYmSPw0apWCIMgkJJuoqnX4OJb1iJNCEALraV0Js2E,3438
-olive_ai-0.5.1.dist-info/NOTICE.txt,sha256=h7RtTa8A8uYhoKJ-nO_kScaD8qHLYj0en8UYEqpy5_E,764423
-olive_ai-0.5.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-olive_ai-0.5.1.dist-info/entry_points.txt,sha256=XVTpnzIsU7uElE03r2zsuqXrvUKWbMw-ndKgwSBYAoM,101
-olive_ai-0.5.1.dist-info/top_level.txt,sha256=V9j-sv9fsgSHbZLD-a-cxoocQvfzNaWA8w_3snFQbhQ,6
-olive_ai-0.5.1.dist-info/RECORD,,
+olive_ai-0.5.2.dist-info/LICENSE,sha256=ws_MuBL-SCEBqPBFl9_FqZkaaydIJmxHrJG2parhU4M,1141
+olive_ai-0.5.2.dist-info/METADATA,sha256=8RMPQHAhHYlX5c6ggbq1era2aQ5BVuVv3z63AcC5lWA,3438
+olive_ai-0.5.2.dist-info/NOTICE.txt,sha256=h7RtTa8A8uYhoKJ-nO_kScaD8qHLYj0en8UYEqpy5_E,764423
+olive_ai-0.5.2.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+olive_ai-0.5.2.dist-info/entry_points.txt,sha256=XVTpnzIsU7uElE03r2zsuqXrvUKWbMw-ndKgwSBYAoM,101
+olive_ai-0.5.2.dist-info/top_level.txt,sha256=V9j-sv9fsgSHbZLD-a-cxoocQvfzNaWA8w_3snFQbhQ,6
+olive_ai-0.5.2.dist-info/RECORD,,
```

