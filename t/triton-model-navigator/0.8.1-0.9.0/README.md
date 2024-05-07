# Comparing `tmp/triton_model_navigator-0.8.1-py3-none-any.whl.zip` & `tmp/triton_model_navigator-0.9.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,172 +1,174 @@
-Zip file size: 317922 bytes, number of entries: 170
--rw-r--r--  2.0 unx      869 b- defN 24-Apr-04 10:34 model_navigator/__init__.py
--rw-r--r--  2.0 unx      637 b- defN 24-Apr-04 10:34 model_navigator/__version__.py
--rw-r--r--  2.0 unx     4077 b- defN 24-Apr-04 10:34 model_navigator/exceptions.py
--rw-r--r--  2.0 unx     1880 b- defN 24-Apr-04 10:34 model_navigator/api/__init__.py
--rw-r--r--  2.0 unx    30122 b- defN 24-Apr-04 10:34 model_navigator/api/config.py
--rw-r--r--  2.0 unx      991 b- defN 24-Apr-04 10:34 model_navigator/api/inplace.py
--rw-r--r--  2.0 unx     6252 b- defN 24-Apr-04 10:34 model_navigator/api/jax.py
--rw-r--r--  2.0 unx     5233 b- defN 24-Apr-04 10:34 model_navigator/api/onnx.py
--rw-r--r--  2.0 unx    17313 b- defN 24-Apr-04 10:34 model_navigator/api/package.py
--rw-r--r--  2.0 unx     4622 b- defN 24-Apr-04 10:34 model_navigator/api/python.py
--rw-r--r--  2.0 unx     8379 b- defN 24-Apr-04 10:34 model_navigator/api/pytriton.py
--rw-r--r--  2.0 unx     6312 b- defN 24-Apr-04 10:34 model_navigator/api/tensorflow.py
--rw-r--r--  2.0 unx     4461 b- defN 24-Apr-04 10:34 model_navigator/api/tensorrt.py
--rw-r--r--  2.0 unx     6096 b- defN 24-Apr-04 10:34 model_navigator/api/torch.py
--rw-r--r--  2.0 unx     1655 b- defN 24-Apr-04 10:34 model_navigator/api/triton.py
--rw-r--r--  2.0 unx     5807 b- defN 24-Apr-04 10:34 model_navigator/api/utilities.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/__init__.py
--rw-r--r--  2.0 unx     5992 b- defN 24-Apr-04 10:34 model_navigator/commands/base.py
--rw-r--r--  2.0 unx     1837 b- defN 24-Apr-04 10:34 model_navigator/commands/delete_model.py
--rw-r--r--  2.0 unx     9564 b- defN 24-Apr-04 10:34 model_navigator/commands/execution_context.py
--rw-r--r--  2.0 unx    13934 b- defN 24-Apr-04 10:34 model_navigator/commands/infer_metadata.py
--rw-r--r--  2.0 unx     3324 b- defN 24-Apr-04 10:34 model_navigator/commands/load.py
--rw-r--r--  2.0 unx     9086 b- defN 24-Apr-04 10:34 model_navigator/commands/tensorrt_profile_builder.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/__init__.py
--rw-r--r--  2.0 unx     9691 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/base.py
--rw-r--r--  2.0 unx     8428 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/tf.py
--rw-r--r--  2.0 unx    10636 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/torch.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/converters/__init__.py
--rw-r--r--  2.0 unx     6142 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/converters/onnx2trt.py
--rw-r--r--  2.0 unx     3750 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/converters/sm2tftrt.py
--rw-r--r--  2.0 unx     3642 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/converters/ts2onnx.py
--rw-r--r--  2.0 unx     5272 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/converters/ts2torchtrt.py
--rw-r--r--  2.0 unx      668 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/onnx/__init__.py
--rw-r--r--  2.0 unx     1728 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
--rw-r--r--  2.0 unx     8679 b- defN 24-Apr-04 10:34 model_navigator/commands/convert/onnx/onnx2trt.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/copy/__init__.py
--rw-r--r--  2.0 unx     1780 b- defN 24-Apr-04 10:34 model_navigator/commands/copy/copy_model.py
--rw-r--r--  2.0 unx      666 b- defN 24-Apr-04 10:34 model_navigator/commands/correctness/__init__.py
--rw-r--r--  2.0 unx     5814 b- defN 24-Apr-04 10:34 model_navigator/commands/correctness/correctness.py
--rw-r--r--  2.0 unx     4878 b- defN 24-Apr-04 10:34 model_navigator/commands/correctness/correctness_script.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/data_dump/__init__.py
--rw-r--r--  2.0 unx     8903 b- defN 24-Apr-04 10:34 model_navigator/commands/data_dump/samples.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/export/__init__.py
--rw-r--r--  2.0 unx     3806 b- defN 24-Apr-04 10:34 model_navigator/commands/export/jax.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-04 10:34 model_navigator/commands/export/tf.py
--rw-r--r--  2.0 unx    16150 b- defN 24-Apr-04 10:34 model_navigator/commands/export/torch.py
--rw-r--r--  2.0 unx     1222 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/__init__.py
--rw-r--r--  2.0 unx     4293 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/jax2savedmodel.py
--rw-r--r--  2.0 unx     2801 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/keras2savedmodel.py
--rw-r--r--  2.0 unx     3147 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
--rw-r--r--  2.0 unx     2918 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/torch2dynamo_onnx.py
--rw-r--r--  2.0 unx     2919 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/torch2exportedprogram.py
--rw-r--r--  2.0 unx     4542 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/torch2onnx.py
--rw-r--r--  2.0 unx     5020 b- defN 24-Apr-04 10:34 model_navigator/commands/export/exporters/torch2torchscript.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-04 10:34 model_navigator/commands/find_max_batch_size/__init__.py
--rw-r--r--  2.0 unx     7645 b- defN 24-Apr-04 10:34 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-04 10:34 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
--rw-r--r--  2.0 unx      609 b- defN 24-Apr-04 10:34 model_navigator/commands/optimize/__init__.py
--rw-r--r--  2.0 unx     2426 b- defN 24-Apr-04 10:34 model_navigator/commands/optimize/graph_surgeon.py
--rw-r--r--  2.0 unx     3543 b- defN 24-Apr-04 10:34 model_navigator/commands/optimize/graph_surgeon_script.py
--rw-r--r--  2.0 unx      772 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/__init__.py
--rw-r--r--  2.0 unx     3067 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/nvml_handler.py
--rw-r--r--  2.0 unx     5584 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/performance.py
--rw-r--r--  2.0 unx     7412 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/profile.py
--rw-r--r--  2.0 unx     3355 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/profile_script.py
--rw-r--r--  2.0 unx     8428 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/profiler.py
--rw-r--r--  2.0 unx    10305 b- defN 24-Apr-04 10:34 model_navigator/commands/performance/results.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/commands/verification/__init__.py
--rw-r--r--  2.0 unx     5022 b- defN 24-Apr-04 10:34 model_navigator/commands/verification/verify.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/configuration/__init__.py
--rw-r--r--  2.0 unx     1927 b- defN 24-Apr-04 10:34 model_navigator/configuration/common_config.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/configuration/model/__init__.py
--rw-r--r--  2.0 unx    21816 b- defN 24-Apr-04 10:34 model_navigator/configuration/model/model_config.py
--rw-r--r--  2.0 unx    20211 b- defN 24-Apr-04 10:34 model_navigator/configuration/model/model_config_builder.py
--rw-r--r--  2.0 unx      609 b- defN 24-Apr-04 10:34 model_navigator/configuration/runner/__init__.py
--rw-r--r--  2.0 unx     3822 b- defN 24-Apr-04 10:34 model_navigator/configuration/runner/runner_config.py
--rw-r--r--  2.0 unx      609 b- defN 24-Apr-04 10:34 model_navigator/configuration/validation/__init__.py
--rw-r--r--  2.0 unx     1835 b- defN 24-Apr-04 10:34 model_navigator/configuration/validation/device.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/core/__init__.py
--rw-r--r--  2.0 unx     1494 b- defN 24-Apr-04 10:34 model_navigator/core/constants.py
--rw-r--r--  2.0 unx    13018 b- defN 24-Apr-04 10:34 model_navigator/core/dataloader.py
--rw-r--r--  2.0 unx     5300 b- defN 24-Apr-04 10:34 model_navigator/core/logger.py
--rw-r--r--  2.0 unx    23119 b- defN 24-Apr-04 10:34 model_navigator/core/tensor.py
--rw-r--r--  2.0 unx     2214 b- defN 24-Apr-04 10:34 model_navigator/core/workspace.py
--rw-r--r--  2.0 unx     2844 b- defN 24-Apr-04 10:34 model_navigator/frameworks/__init__.py
--rw-r--r--  2.0 unx      657 b- defN 24-Apr-04 10:34 model_navigator/frameworks/jax/__init__.py
--rw-r--r--  2.0 unx     1558 b- defN 24-Apr-04 10:34 model_navigator/frameworks/jax/model.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/frameworks/onnx/__init__.py
--rw-r--r--  2.0 unx     1493 b- defN 24-Apr-04 10:34 model_navigator/frameworks/onnx/utils.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/frameworks/tensorrt/__init__.py
--rw-r--r--  2.0 unx    31492 b- defN 24-Apr-04 10:34 model_navigator/frameworks/tensorrt/cuda.py
--rw-r--r--  2.0 unx     2062 b- defN 24-Apr-04 10:34 model_navigator/frameworks/tensorrt/type_mapping.py
--rw-r--r--  2.0 unx    15989 b- defN 24-Apr-04 10:34 model_navigator/frameworks/tensorrt/utils.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/frameworks/torch/__init__.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Apr-04 10:34 model_navigator/frameworks/torch/utils.py
--rw-r--r--  2.0 unx    11870 b- defN 24-Apr-04 10:34 model_navigator/inplace/__init__.py
--rw-r--r--  2.0 unx     4791 b- defN 24-Apr-04 10:34 model_navigator/inplace/config.py
--rw-r--r--  2.0 unx    12666 b- defN 24-Apr-04 10:34 model_navigator/inplace/model.py
--rw-r--r--  2.0 unx    10024 b- defN 24-Apr-04 10:34 model_navigator/inplace/profiling.py
--rw-r--r--  2.0 unx     2392 b- defN 24-Apr-04 10:34 model_navigator/inplace/registry.py
--rw-r--r--  2.0 unx    14679 b- defN 24-Apr-04 10:34 model_navigator/inplace/timer.py
--rw-r--r--  2.0 unx     3069 b- defN 24-Apr-04 10:34 model_navigator/inplace/utils.py
--rw-r--r--  2.0 unx     7982 b- defN 24-Apr-04 10:34 model_navigator/inplace/wrapper.py
--rw-r--r--  2.0 unx      609 b- defN 24-Apr-04 10:34 model_navigator/package/__init__.py
--rw-r--r--  2.0 unx    12399 b- defN 24-Apr-04 10:34 model_navigator/package/builder.py
--rw-r--r--  2.0 unx     5523 b- defN 24-Apr-04 10:34 model_navigator/package/loader.py
--rw-r--r--  2.0 unx    12052 b- defN 24-Apr-04 10:34 model_navigator/package/package.py
--rw-r--r--  2.0 unx     2885 b- defN 24-Apr-04 10:34 model_navigator/package/profiling_results.py
--rw-r--r--  2.0 unx    23564 b- defN 24-Apr-04 10:34 model_navigator/package/status.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/pipelines/__init__.py
--rw-r--r--  2.0 unx     5380 b- defN 24-Apr-04 10:34 model_navigator/pipelines/pipeline.py
--rw-r--r--  2.0 unx    15240 b- defN 24-Apr-04 10:34 model_navigator/pipelines/pipeline_context.py
--rw-r--r--  2.0 unx     3805 b- defN 24-Apr-04 10:34 model_navigator/pipelines/pipeline_manager.py
--rw-r--r--  2.0 unx     8963 b- defN 24-Apr-04 10:34 model_navigator/pipelines/validation.py
--rw-r--r--  2.0 unx     2028 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/__init__.py
--rw-r--r--  2.0 unx     2105 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/correctness.py
--rw-r--r--  2.0 unx     4616 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/find_device_max_batch_size.py
--rw-r--r--  2.0 unx     1660 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/jax.py
--rw-r--r--  2.0 unx     2515 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/performance.py
--rw-r--r--  2.0 unx     2624 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/preprocessing.py
--rw-r--r--  2.0 unx     2503 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/profiling.py
--rw-r--r--  2.0 unx     2732 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/tensorflow.py
--rw-r--r--  2.0 unx     3674 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/tensorflow_tensorrt.py
--rw-r--r--  2.0 unx     3564 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/tensorrt.py
--rw-r--r--  2.0 unx     3797 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/torch.py
--rw-r--r--  2.0 unx     3638 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/torch_tensorrt.py
--rw-r--r--  2.0 unx     2111 b- defN 24-Apr-04 10:34 model_navigator/pipelines/builders/verify.py
--rw-r--r--  2.0 unx      609 b- defN 24-Apr-04 10:34 model_navigator/pipelines/wrappers/__init__.py
--rw-r--r--  2.0 unx     2795 b- defN 24-Apr-04 10:34 model_navigator/pipelines/wrappers/optimize.py
--rw-r--r--  2.0 unx     4911 b- defN 24-Apr-04 10:34 model_navigator/pipelines/wrappers/profile.py
--rw-r--r--  2.0 unx     1572 b- defN 24-Apr-04 10:34 model_navigator/runners/__init__.py
--rw-r--r--  2.0 unx    16141 b- defN 24-Apr-04 10:34 model_navigator/runners/base.py
--rw-r--r--  2.0 unx     2065 b- defN 24-Apr-04 10:34 model_navigator/runners/jax.py
--rw-r--r--  2.0 unx    13466 b- defN 24-Apr-04 10:34 model_navigator/runners/onnx.py
--rw-r--r--  2.0 unx     2004 b- defN 24-Apr-04 10:34 model_navigator/runners/python.py
--rw-r--r--  2.0 unx     2291 b- defN 24-Apr-04 10:34 model_navigator/runners/registry.py
--rw-r--r--  2.0 unx     7524 b- defN 24-Apr-04 10:34 model_navigator/runners/tensorflow.py
--rw-r--r--  2.0 unx    31280 b- defN 24-Apr-04 10:34 model_navigator/runners/tensorrt.py
--rw-r--r--  2.0 unx    15362 b- defN 24-Apr-04 10:34 model_navigator/runners/torch.py
--rw-r--r--  2.0 unx     3582 b- defN 24-Apr-04 10:34 model_navigator/runners/utils.py
--rw-r--r--  2.0 unx      937 b- defN 24-Apr-04 10:34 model_navigator/runtime_analyzer/__init__.py
--rw-r--r--  2.0 unx    11715 b- defN 24-Apr-04 10:34 model_navigator/runtime_analyzer/analyzer.py
--rw-r--r--  2.0 unx     2304 b- defN 24-Apr-04 10:34 model_navigator/runtime_analyzer/strategy.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/triton/__init__.py
--rw-r--r--  2.0 unx     4384 b- defN 24-Apr-04 10:34 model_navigator/triton/model_config.py
--rw-r--r--  2.0 unx     5219 b- defN 24-Apr-04 10:34 model_navigator/triton/model_config_builder.py
--rw-r--r--  2.0 unx    25428 b- defN 24-Apr-04 10:34 model_navigator/triton/model_config_generator.py
--rw-r--r--  2.0 unx    25200 b- defN 24-Apr-04 10:34 model_navigator/triton/model_repository.py
--rw-r--r--  2.0 unx      985 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/__init__.py
--rw-r--r--  2.0 unx     3404 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/base_model_config.py
--rw-r--r--  2.0 unx    25405 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/common.py
--rw-r--r--  2.0 unx     2230 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/internal.py
--rw-r--r--  2.0 unx     2685 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/onnx_model_config.py
--rw-r--r--  2.0 unx     1786 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/python_model_config.py
--rw-r--r--  2.0 unx     2021 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/pytorch_model_config.py
--rw-r--r--  2.0 unx     3162 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/tensorflow_model_config.py
--rw-r--r--  2.0 unx     3041 b- defN 24-Apr-04 10:34 model_navigator/triton/specialized_configs/tensorrt_model_config.py
--rw-r--r--  2.0 unx      614 b- defN 24-Apr-04 10:34 model_navigator/utils/__init__.py
--rw-r--r--  2.0 unx    14607 b- defN 24-Apr-04 10:34 model_navigator/utils/common.py
--rw-r--r--  2.0 unx     2495 b- defN 24-Apr-04 10:34 model_navigator/utils/config_helpers.py
--rw-r--r--  2.0 unx     3912 b- defN 24-Apr-04 10:34 model_navigator/utils/devices.py
--rw-r--r--  2.0 unx     1309 b- defN 24-Apr-04 10:34 model_navigator/utils/enums.py
--rw-r--r--  2.0 unx     6175 b- defN 24-Apr-04 10:34 model_navigator/utils/environment.py
--rw-r--r--  2.0 unx     5338 b- defN 24-Apr-04 10:34 model_navigator/utils/format_helpers.py
--rw-r--r--  2.0 unx     2331 b- defN 24-Apr-04 10:34 model_navigator/utils/module.py
--rw-r--r--  2.0 unx    10140 b- defN 24-Apr-04 10:41 triton_model_navigator-0.8.1.dist-info/LICENSE
--rw-r--r--  2.0 unx    13486 b- defN 24-Apr-04 10:41 triton_model_navigator-0.8.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-04 10:41 triton_model_navigator-0.8.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       16 b- defN 24-Apr-04 10:41 triton_model_navigator-0.8.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    17054 b- defN 24-Apr-04 10:41 triton_model_navigator-0.8.1.dist-info/RECORD
-170 files, 1002649 bytes uncompressed, 290136 bytes compressed:  71.1%
+Zip file size: 323685 bytes, number of entries: 172
+-rw-r--r--  2.0 unx      869 b- defN 24-May-07 14:49 model_navigator/__init__.py
+-rw-r--r--  2.0 unx      637 b- defN 24-May-07 14:49 model_navigator/__version__.py
+-rw-r--r--  2.0 unx     4077 b- defN 24-May-07 14:49 model_navigator/exceptions.py
+-rw-r--r--  2.0 unx     1880 b- defN 24-May-07 14:49 model_navigator/api/__init__.py
+-rw-r--r--  2.0 unx    30304 b- defN 24-May-07 14:49 model_navigator/api/config.py
+-rw-r--r--  2.0 unx      991 b- defN 24-May-07 14:49 model_navigator/api/inplace.py
+-rw-r--r--  2.0 unx     6252 b- defN 24-May-07 14:49 model_navigator/api/jax.py
+-rw-r--r--  2.0 unx     5233 b- defN 24-May-07 14:49 model_navigator/api/onnx.py
+-rw-r--r--  2.0 unx    17313 b- defN 24-May-07 14:49 model_navigator/api/package.py
+-rw-r--r--  2.0 unx     4622 b- defN 24-May-07 14:49 model_navigator/api/python.py
+-rw-r--r--  2.0 unx     8379 b- defN 24-May-07 14:49 model_navigator/api/pytriton.py
+-rw-r--r--  2.0 unx     6312 b- defN 24-May-07 14:49 model_navigator/api/tensorflow.py
+-rw-r--r--  2.0 unx     4461 b- defN 24-May-07 14:49 model_navigator/api/tensorrt.py
+-rw-r--r--  2.0 unx     6096 b- defN 24-May-07 14:49 model_navigator/api/torch.py
+-rw-r--r--  2.0 unx     1655 b- defN 24-May-07 14:49 model_navigator/api/triton.py
+-rw-r--r--  2.0 unx     5809 b- defN 24-May-07 14:49 model_navigator/api/utilities.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/__init__.py
+-rw-r--r--  2.0 unx     5992 b- defN 24-May-07 14:49 model_navigator/commands/base.py
+-rw-r--r--  2.0 unx     1837 b- defN 24-May-07 14:49 model_navigator/commands/delete_model.py
+-rw-r--r--  2.0 unx     9564 b- defN 24-May-07 14:49 model_navigator/commands/execution_context.py
+-rw-r--r--  2.0 unx    14044 b- defN 24-May-07 14:49 model_navigator/commands/infer_metadata.py
+-rw-r--r--  2.0 unx     3324 b- defN 24-May-07 14:49 model_navigator/commands/load.py
+-rw-r--r--  2.0 unx     9086 b- defN 24-May-07 14:49 model_navigator/commands/tensorrt_profile_builder.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/convert/__init__.py
+-rw-r--r--  2.0 unx     9691 b- defN 24-May-07 14:49 model_navigator/commands/convert/base.py
+-rw-r--r--  2.0 unx     8368 b- defN 24-May-07 14:49 model_navigator/commands/convert/tf.py
+-rw-r--r--  2.0 unx    10566 b- defN 24-May-07 14:49 model_navigator/commands/convert/torch.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/convert/converters/__init__.py
+-rw-r--r--  2.0 unx     7279 b- defN 24-May-07 14:49 model_navigator/commands/convert/converters/onnx2trt.py
+-rw-r--r--  2.0 unx     3750 b- defN 24-May-07 14:49 model_navigator/commands/convert/converters/sm2tftrt.py
+-rw-r--r--  2.0 unx     3642 b- defN 24-May-07 14:49 model_navigator/commands/convert/converters/ts2onnx.py
+-rw-r--r--  2.0 unx     5272 b- defN 24-May-07 14:49 model_navigator/commands/convert/converters/ts2torchtrt.py
+-rw-r--r--  2.0 unx      668 b- defN 24-May-07 14:49 model_navigator/commands/convert/onnx/__init__.py
+-rw-r--r--  2.0 unx     1728 b- defN 24-May-07 14:49 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py
+-rw-r--r--  2.0 unx     8924 b- defN 24-May-07 14:49 model_navigator/commands/convert/onnx/onnx2trt.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/copy/__init__.py
+-rw-r--r--  2.0 unx     1780 b- defN 24-May-07 14:49 model_navigator/commands/copy/copy_model.py
+-rw-r--r--  2.0 unx      666 b- defN 24-May-07 14:49 model_navigator/commands/correctness/__init__.py
+-rw-r--r--  2.0 unx     5814 b- defN 24-May-07 14:49 model_navigator/commands/correctness/correctness.py
+-rw-r--r--  2.0 unx     4878 b- defN 24-May-07 14:49 model_navigator/commands/correctness/correctness_script.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/data_dump/__init__.py
+-rw-r--r--  2.0 unx     8903 b- defN 24-May-07 14:49 model_navigator/commands/data_dump/samples.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/export/__init__.py
+-rw-r--r--  2.0 unx     3806 b- defN 24-May-07 14:49 model_navigator/commands/export/jax.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-May-07 14:49 model_navigator/commands/export/tf.py
+-rw-r--r--  2.0 unx    16150 b- defN 24-May-07 14:49 model_navigator/commands/export/torch.py
+-rw-r--r--  2.0 unx     1222 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/__init__.py
+-rw-r--r--  2.0 unx     4293 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/jax2savedmodel.py
+-rw-r--r--  2.0 unx     2801 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/keras2savedmodel.py
+-rw-r--r--  2.0 unx     3147 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/savedmodel2savedmodel.py
+-rw-r--r--  2.0 unx     3130 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/torch2dynamo_onnx.py
+-rw-r--r--  2.0 unx     3148 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/torch2exportedprogram.py
+-rw-r--r--  2.0 unx     4542 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/torch2onnx.py
+-rw-r--r--  2.0 unx     5020 b- defN 24-May-07 14:49 model_navigator/commands/export/exporters/torch2torchscript.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-07 14:49 model_navigator/commands/find_max_batch_size/__init__.py
+-rw-r--r--  2.0 unx     7647 b- defN 24-May-07 14:49 model_navigator/commands/find_max_batch_size/find_max_batch_size.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-07 14:49 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py
+-rw-r--r--  2.0 unx      609 b- defN 24-May-07 14:49 model_navigator/commands/optimize/__init__.py
+-rw-r--r--  2.0 unx     2426 b- defN 24-May-07 14:49 model_navigator/commands/optimize/graph_surgeon.py
+-rw-r--r--  2.0 unx     3543 b- defN 24-May-07 14:49 model_navigator/commands/optimize/graph_surgeon_script.py
+-rw-r--r--  2.0 unx      772 b- defN 24-May-07 14:49 model_navigator/commands/performance/__init__.py
+-rw-r--r--  2.0 unx     3067 b- defN 24-May-07 14:49 model_navigator/commands/performance/nvml_handler.py
+-rw-r--r--  2.0 unx     5584 b- defN 24-May-07 14:49 model_navigator/commands/performance/performance.py
+-rw-r--r--  2.0 unx     7412 b- defN 24-May-07 14:49 model_navigator/commands/performance/profile.py
+-rw-r--r--  2.0 unx     3355 b- defN 24-May-07 14:49 model_navigator/commands/performance/profile_script.py
+-rw-r--r--  2.0 unx     7850 b- defN 24-May-07 14:49 model_navigator/commands/performance/profiler.py
+-rw-r--r--  2.0 unx    10305 b- defN 24-May-07 14:49 model_navigator/commands/performance/results.py
+-rw-r--r--  2.0 unx     2275 b- defN 24-May-07 14:49 model_navigator/commands/performance/utils.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/commands/verification/__init__.py
+-rw-r--r--  2.0 unx     5022 b- defN 24-May-07 14:49 model_navigator/commands/verification/verify.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/configuration/__init__.py
+-rw-r--r--  2.0 unx     1927 b- defN 24-May-07 14:49 model_navigator/configuration/common_config.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/configuration/model/__init__.py
+-rw-r--r--  2.0 unx    22039 b- defN 24-May-07 14:49 model_navigator/configuration/model/model_config.py
+-rw-r--r--  2.0 unx    20347 b- defN 24-May-07 14:49 model_navigator/configuration/model/model_config_builder.py
+-rw-r--r--  2.0 unx      609 b- defN 24-May-07 14:49 model_navigator/configuration/runner/__init__.py
+-rw-r--r--  2.0 unx     3822 b- defN 24-May-07 14:49 model_navigator/configuration/runner/runner_config.py
+-rw-r--r--  2.0 unx      609 b- defN 24-May-07 14:49 model_navigator/configuration/validation/__init__.py
+-rw-r--r--  2.0 unx     1835 b- defN 24-May-07 14:49 model_navigator/configuration/validation/device.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/core/__init__.py
+-rw-r--r--  2.0 unx     1494 b- defN 24-May-07 14:49 model_navigator/core/constants.py
+-rw-r--r--  2.0 unx    13018 b- defN 24-May-07 14:49 model_navigator/core/dataloader.py
+-rw-r--r--  2.0 unx     5300 b- defN 24-May-07 14:49 model_navigator/core/logger.py
+-rw-r--r--  2.0 unx    23119 b- defN 24-May-07 14:49 model_navigator/core/tensor.py
+-rw-r--r--  2.0 unx     2214 b- defN 24-May-07 14:49 model_navigator/core/workspace.py
+-rw-r--r--  2.0 unx     2844 b- defN 24-May-07 14:49 model_navigator/frameworks/__init__.py
+-rw-r--r--  2.0 unx      657 b- defN 24-May-07 14:49 model_navigator/frameworks/jax/__init__.py
+-rw-r--r--  2.0 unx     1558 b- defN 24-May-07 14:49 model_navigator/frameworks/jax/model.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/frameworks/onnx/__init__.py
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-07 14:49 model_navigator/frameworks/onnx/utils.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/frameworks/tensorrt/__init__.py
+-rw-r--r--  2.0 unx    31492 b- defN 24-May-07 14:49 model_navigator/frameworks/tensorrt/cuda.py
+-rw-r--r--  2.0 unx     9970 b- defN 24-May-07 14:49 model_navigator/frameworks/tensorrt/timing_tactics.py
+-rw-r--r--  2.0 unx     2062 b- defN 24-May-07 14:49 model_navigator/frameworks/tensorrt/type_mapping.py
+-rw-r--r--  2.0 unx    15764 b- defN 24-May-07 14:49 model_navigator/frameworks/tensorrt/utils.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/frameworks/torch/__init__.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-07 14:49 model_navigator/frameworks/torch/utils.py
+-rw-r--r--  2.0 unx    12709 b- defN 24-May-07 14:49 model_navigator/inplace/__init__.py
+-rw-r--r--  2.0 unx     5281 b- defN 24-May-07 14:49 model_navigator/inplace/config.py
+-rw-r--r--  2.0 unx    13036 b- defN 24-May-07 14:49 model_navigator/inplace/model.py
+-rw-r--r--  2.0 unx    10031 b- defN 24-May-07 14:49 model_navigator/inplace/profiling.py
+-rw-r--r--  2.0 unx     2392 b- defN 24-May-07 14:49 model_navigator/inplace/registry.py
+-rw-r--r--  2.0 unx    14679 b- defN 24-May-07 14:49 model_navigator/inplace/timer.py
+-rw-r--r--  2.0 unx     3069 b- defN 24-May-07 14:49 model_navigator/inplace/utils.py
+-rw-r--r--  2.0 unx     8805 b- defN 24-May-07 14:49 model_navigator/inplace/wrapper.py
+-rw-r--r--  2.0 unx      609 b- defN 24-May-07 14:49 model_navigator/package/__init__.py
+-rw-r--r--  2.0 unx    12399 b- defN 24-May-07 14:49 model_navigator/package/builder.py
+-rw-r--r--  2.0 unx     5523 b- defN 24-May-07 14:49 model_navigator/package/loader.py
+-rw-r--r--  2.0 unx    12052 b- defN 24-May-07 14:49 model_navigator/package/package.py
+-rw-r--r--  2.0 unx     2885 b- defN 24-May-07 14:49 model_navigator/package/profiling_results.py
+-rw-r--r--  2.0 unx    23564 b- defN 24-May-07 14:49 model_navigator/package/status.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/pipelines/__init__.py
+-rw-r--r--  2.0 unx     5380 b- defN 24-May-07 14:49 model_navigator/pipelines/pipeline.py
+-rw-r--r--  2.0 unx    15240 b- defN 24-May-07 14:49 model_navigator/pipelines/pipeline_context.py
+-rw-r--r--  2.0 unx     3805 b- defN 24-May-07 14:49 model_navigator/pipelines/pipeline_manager.py
+-rw-r--r--  2.0 unx     8963 b- defN 24-May-07 14:49 model_navigator/pipelines/validation.py
+-rw-r--r--  2.0 unx     2028 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/__init__.py
+-rw-r--r--  2.0 unx     2105 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/correctness.py
+-rw-r--r--  2.0 unx     4616 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/find_device_max_batch_size.py
+-rw-r--r--  2.0 unx     1660 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/jax.py
+-rw-r--r--  2.0 unx     2515 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/performance.py
+-rw-r--r--  2.0 unx     2624 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/preprocessing.py
+-rw-r--r--  2.0 unx     2503 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/profiling.py
+-rw-r--r--  2.0 unx     2732 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/tensorflow.py
+-rw-r--r--  2.0 unx     3441 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/tensorflow_tensorrt.py
+-rw-r--r--  2.0 unx     3320 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/tensorrt.py
+-rw-r--r--  2.0 unx     3797 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/torch.py
+-rw-r--r--  2.0 unx     3394 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/torch_tensorrt.py
+-rw-r--r--  2.0 unx     2111 b- defN 24-May-07 14:49 model_navigator/pipelines/builders/verify.py
+-rw-r--r--  2.0 unx      609 b- defN 24-May-07 14:49 model_navigator/pipelines/wrappers/__init__.py
+-rw-r--r--  2.0 unx     2795 b- defN 24-May-07 14:49 model_navigator/pipelines/wrappers/optimize.py
+-rw-r--r--  2.0 unx     4911 b- defN 24-May-07 14:49 model_navigator/pipelines/wrappers/profile.py
+-rw-r--r--  2.0 unx     1572 b- defN 24-May-07 14:49 model_navigator/runners/__init__.py
+-rw-r--r--  2.0 unx    16141 b- defN 24-May-07 14:49 model_navigator/runners/base.py
+-rw-r--r--  2.0 unx     2065 b- defN 24-May-07 14:49 model_navigator/runners/jax.py
+-rw-r--r--  2.0 unx    14203 b- defN 24-May-07 14:49 model_navigator/runners/onnx.py
+-rw-r--r--  2.0 unx     2004 b- defN 24-May-07 14:49 model_navigator/runners/python.py
+-rw-r--r--  2.0 unx     2291 b- defN 24-May-07 14:49 model_navigator/runners/registry.py
+-rw-r--r--  2.0 unx     7524 b- defN 24-May-07 14:49 model_navigator/runners/tensorflow.py
+-rw-r--r--  2.0 unx    31280 b- defN 24-May-07 14:49 model_navigator/runners/tensorrt.py
+-rw-r--r--  2.0 unx    15973 b- defN 24-May-07 14:49 model_navigator/runners/torch.py
+-rw-r--r--  2.0 unx     3582 b- defN 24-May-07 14:49 model_navigator/runners/utils.py
+-rw-r--r--  2.0 unx      937 b- defN 24-May-07 14:49 model_navigator/runtime_analyzer/__init__.py
+-rw-r--r--  2.0 unx    11715 b- defN 24-May-07 14:49 model_navigator/runtime_analyzer/analyzer.py
+-rw-r--r--  2.0 unx     2304 b- defN 24-May-07 14:49 model_navigator/runtime_analyzer/strategy.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/triton/__init__.py
+-rw-r--r--  2.0 unx     4384 b- defN 24-May-07 14:49 model_navigator/triton/model_config.py
+-rw-r--r--  2.0 unx     5219 b- defN 24-May-07 14:49 model_navigator/triton/model_config_builder.py
+-rw-r--r--  2.0 unx    25428 b- defN 24-May-07 14:49 model_navigator/triton/model_config_generator.py
+-rw-r--r--  2.0 unx    25200 b- defN 24-May-07 14:49 model_navigator/triton/model_repository.py
+-rw-r--r--  2.0 unx      985 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/__init__.py
+-rw-r--r--  2.0 unx     3404 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/base_model_config.py
+-rw-r--r--  2.0 unx    25405 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/common.py
+-rw-r--r--  2.0 unx     2230 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/internal.py
+-rw-r--r--  2.0 unx     2685 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/onnx_model_config.py
+-rw-r--r--  2.0 unx     1786 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/python_model_config.py
+-rw-r--r--  2.0 unx     2021 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/pytorch_model_config.py
+-rw-r--r--  2.0 unx     3162 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/tensorflow_model_config.py
+-rw-r--r--  2.0 unx     3041 b- defN 24-May-07 14:49 model_navigator/triton/specialized_configs/tensorrt_model_config.py
+-rw-r--r--  2.0 unx      614 b- defN 24-May-07 14:49 model_navigator/utils/__init__.py
+-rw-r--r--  2.0 unx    15089 b- defN 24-May-07 14:49 model_navigator/utils/common.py
+-rw-r--r--  2.0 unx     2495 b- defN 24-May-07 14:49 model_navigator/utils/config_helpers.py
+-rw-r--r--  2.0 unx     3912 b- defN 24-May-07 14:49 model_navigator/utils/devices.py
+-rw-r--r--  2.0 unx     1309 b- defN 24-May-07 14:49 model_navigator/utils/enums.py
+-rw-r--r--  2.0 unx     6175 b- defN 24-May-07 14:49 model_navigator/utils/environment.py
+-rw-r--r--  2.0 unx     5338 b- defN 24-May-07 14:49 model_navigator/utils/format_helpers.py
+-rw-r--r--  2.0 unx     2331 b- defN 24-May-07 14:49 model_navigator/utils/module.py
+-rw-r--r--  2.0 unx    10140 b- defN 24-May-07 14:54 triton_model_navigator-0.9.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    13486 b- defN 24-May-07 14:54 triton_model_navigator-0.9.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 14:54 triton_model_navigator-0.9.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       16 b- defN 24-May-07 14:54 triton_model_navigator-0.9.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    17266 b- defN 24-May-07 14:54 triton_model_navigator-0.9.0.dist-info/RECORD
+172 files, 1020289 bytes uncompressed, 295551 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -195,14 +195,17 @@
 
 Filename: model_navigator/commands/performance/profiler.py
 Comment: 
 
 Filename: model_navigator/commands/performance/results.py
 Comment: 
 
+Filename: model_navigator/commands/performance/utils.py
+Comment: 
+
 Filename: model_navigator/commands/verification/__init__.py
 Comment: 
 
 Filename: model_navigator/commands/verification/verify.py
 Comment: 
 
 Filename: model_navigator/configuration/__init__.py
@@ -267,14 +270,17 @@
 
 Filename: model_navigator/frameworks/tensorrt/__init__.py
 Comment: 
 
 Filename: model_navigator/frameworks/tensorrt/cuda.py
 Comment: 
 
+Filename: model_navigator/frameworks/tensorrt/timing_tactics.py
+Comment: 
+
 Filename: model_navigator/frameworks/tensorrt/type_mapping.py
 Comment: 
 
 Filename: model_navigator/frameworks/tensorrt/utils.py
 Comment: 
 
 Filename: model_navigator/frameworks/torch/__init__.py
@@ -489,23 +495,23 @@
 
 Filename: model_navigator/utils/format_helpers.py
 Comment: 
 
 Filename: model_navigator/utils/module.py
 Comment: 
 
-Filename: triton_model_navigator-0.8.1.dist-info/LICENSE
+Filename: triton_model_navigator-0.9.0.dist-info/LICENSE
 Comment: 
 
-Filename: triton_model_navigator-0.8.1.dist-info/METADATA
+Filename: triton_model_navigator-0.9.0.dist-info/METADATA
 Comment: 
 
-Filename: triton_model_navigator-0.8.1.dist-info/WHEEL
+Filename: triton_model_navigator-0.9.0.dist-info/WHEEL
 Comment: 
 
-Filename: triton_model_navigator-0.8.1.dist-info/top_level.txt
+Filename: triton_model_navigator-0.9.0.dist-info/top_level.txt
 Comment: 
 
-Filename: triton_model_navigator-0.8.1.dist-info/RECORD
+Filename: triton_model_navigator-0.9.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## model_navigator/__version__.py

```diff
@@ -8,8 +8,8 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "0.8.1"
+__version__ = "0.9.0"
```

## model_navigator/api/config.py

```diff
@@ -13,14 +13,15 @@
 # limitations under the License.
 """Definition of enums and classes representing configuration for Model Navigator."""
 
 import abc
 import dataclasses
 import inspect
 import itertools
+import pathlib
 import warnings
 from enum import Enum
 from typing import (
     Any,
     Callable,
     Dict,
     Iterable,
@@ -241,15 +242,15 @@
     max_batch_size: Optional[int] = None
     batch_sizes: Optional[List[Union[int, None]]] = None
     window_size: int = 50
     stability_percentage: float = 10.0
     stabilization_windows: int = 3
     min_trials: int = 3
     max_trials: int = 10
-    throughput_cutoff_threshold: float = DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD
+    throughput_cutoff_threshold: Optional[float] = DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD
     dataloader: Optional[SizedDataLoader] = None
 
     def __post_init__(self):
         """Validate OptimizationProfile definition to avoid unsupported configurations."""
         if self.stability_percentage <= 0:
             raise ModelNavigatorConfigurationError("`stability_percentage` must be greater than 0.0.")
 
@@ -430,20 +431,18 @@
 
 DEFAULT_NONE_FRAMEWORK_TARGET_FORMATS = (Format.PYTHON,)
 
 DEFAULT_JAX_TARGET_FORMATS = (
     Format.TF_SAVEDMODEL,
     Format.ONNX,
     Format.TENSORRT,
-    Format.TF_TRT,
 )
 
 DEFAULT_TENSORFLOW_TARGET_FORMATS = (
     Format.TF_SAVEDMODEL,
-    Format.TF_TRT,
     Format.ONNX,
     Format.TENSORRT,
 )
 
 DEFAULT_TORCH_TARGET_FORMATS = (
     Format.TORCHSCRIPT,
     Format.TORCH_EXPORTEDPROGRAM,
@@ -848,19 +847,21 @@
     """TensorRT custom config used for TensorRT conversion.
 
     Args:
         optimization_level: Optimization level for TensorRT conversion. Allowed values are fom 0 to 5. Where default is
                             3 based on TensorRT API documentation.
         compatibility_level: Compatibility level for TensorRT conversion.
         onnx_parser_flags: List of TensorRT OnnxParserFlags used for conversion.
+        timing_cache_dir: Storage directory for TRT tactic timing info collected from builder
     """
 
     optimization_level: Optional[int] = None
     compatibility_level: Optional[TensorRTCompatibilityLevel] = None
     onnx_parser_flags: Optional[List[int]] = None
+    timing_cache_dir: Optional[Union[str, pathlib.Path]] = None
 
     def __post_init__(self) -> None:
         """Parse dataclass enums."""
         super().__post_init__()
         if self.optimization_level is not None and (self.optimization_level < 0 or self.optimization_level > 5):
             raise ModelNavigatorConfigurationError(
                 f"TensorRT `optimization_level` must be between 0 and 5. Provided value: {self.optimization_level}."
@@ -882,14 +883,15 @@
 
     def defaults(self) -> None:
         """Update parameters to defaults."""
         super().defaults()
         self.optimization_level = None
         self.compatibility_level = None
         self.onnx_parser_flags = None
+        self.timing_cache_dir = None
 
     @classmethod
     def from_dict(cls, config_dict: Dict[str, Any]) -> "TensorRTConfig":
         """Instantiate TensorRTConfig from a dictionary."""
         if config_dict.get("trt_profiles") is not None:
             parsed_trt_profiles = []
             for trt_profile in config_dict.get("trt_profiles"):
```

## model_navigator/api/utilities.py

```diff
@@ -114,15 +114,15 @@
 
     optimization_profile = OptimizationProfile(
         max_batch_size=max_batch_size_search_limit,
         window_size=1,
         stabilization_windows=1,
         min_trials=1,
         max_trials=1,
-        throughput_cutoff_threshold=-2,
+        throughput_cutoff_threshold=None,
     )
 
     with tempfile.NamedTemporaryFile() as temp_file:
         results_path = pathlib.Path(temp_file.name)
 
         runner = get_runner(runner_name)(
             model=model,
```

## model_navigator/commands/infer_metadata.py

```diff
@@ -27,14 +27,15 @@
 from model_navigator.core.workspace import Workspace
 from model_navigator.exceptions import ModelNavigatorUserInputError
 from model_navigator.frameworks import Framework, is_torch_available
 from model_navigator.frameworks.onnx.utils import get_onnx_io_names
 from model_navigator.frameworks.tensorrt.utils import get_tensorrt_io_names
 from model_navigator.runners.utils import get_format_default_runners
 from model_navigator.utils import module
+from model_navigator.utils.common import optimal_batch_size
 from model_navigator.utils.format_helpers import FRAMEWORK2BASE_FORMAT
 
 torch = module.lazy_import("torch")
 
 
 def _extract_axes_shapes(
     dataloader: Union[SizedDataLoader, Iterator],
@@ -93,15 +94,16 @@
             if ax == batch_dim:  # min bs = 1
                 if config_max_batch_size and (config_max_batch_size < max(shapes)):
                     raise ModelNavigatorUserInputError(
                         f"Given configuration maximum batch size ({config_max_batch_size}) "
                         f"is smaller than the encountered batch size ({max(shapes)})."
                     )
                 max_batch_size = config_max_batch_size or max(shapes)
-                min_opt_max.append((1, int(np.median(shapes)), max_batch_size))
+                opt_shape = optimal_batch_size(max_batch_size)
+                min_opt_max.append((1, opt_shape, max_batch_size))
             else:
                 min_opt_max.append((min(shapes), int(np.median(shapes)), max(shapes)))
         if min_opt_max:
             trt_profile.add(name, *list(zip(*min_opt_max)))
     return trt_profile
```

## model_navigator/commands/convert/tf.py

```diff
@@ -104,15 +104,15 @@
         precision: TensorRTPrecision,
         verbose: bool,
         dataloader_trt_profile: TensorRTProfile,
         custom_args: Dict[str, Any],
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
-        optimized_trt_profiles: Optional[List[TensorRTProfile]] = None,
+        trt_profiles: Optional[List[TensorRTProfile]] = None,
     ) -> CommandOutput:
         """Run conversion from SavedModel to Tensorflow-TensorRT.
 
         Args:
             max_workspace_size (int): TRT max workspace size in bytes.
             minimum_segment_size (int): TRT minium segment size.
             workspace (Path): navigator workspace.
@@ -122,15 +122,15 @@
             verbose (bool): If True verbose logging.
             dataloader_trt_profile (TensorRTProfile): Dataloader TensorRT profile.
             batch_dim (Optional[int], optional): Batching axis.. Defaults to None.
             dataloader_max_batch_size (Optional[int], optional): Maximum batch size from the dataloader.
                 Defaults to None.
             device_max_batch_size (Optional[int], optional): Maximum batch size that fits on the device.
                 Defaults to None.
-            optimized_trt_profiles: List of TensorRT profiles that will be used by Model Navigator for conversion, user provided or optimized by TensorRTProfileBuilder command.
+            trt_profiles: List of TensorRT profiles that will be used by Model Navigator for conversion, user provided or optimized by TensorRTProfileBuilder command.
             custom_args (Optional[Dict[str, Any]], optional): Passthrough parameters for TrtGraphConverterV2
         Raises:
             RuntimeError: When no GPUs are available.
 
         Returns:
             CommandOutput: Conversion output.
         """
@@ -144,20 +144,20 @@
 
         if not exported_model_path.exists():
             LOGGER.warning(f"Exported SavedModel model not found at {exported_model_path}. Skipping conversion")
             return CommandOutput(status=CommandStatus.SKIPPED)
 
         if batch_dim is not None:
             # NOTE: TenserFlow-TensorRT does not support custom profiles. Use first profile to get max batch size.
-            profile = optimized_trt_profiles[0] if optimized_trt_profiles else dataloader_trt_profile
+            profile = trt_profiles[0] if trt_profiles else dataloader_trt_profile
             max_batch_size = list(profile.values())[0].max[batch_dim]
         else:
             max_batch_size = None
 
-        if optimized_trt_profiles is not None:
+        if trt_profiles is not None:
             LOGGER.info("TensorFlow-TensorRT conversion currently does not support custom profiles.")
 
         def get_args(max_batch_size: int = max_batch_size):
             kwargs = {
                 "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "max_workspace_size": max_workspace_size,
@@ -180,12 +180,12 @@
         ) as context:
             conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_external_runtime_script(sm2tftrt.__file__, args),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
-                custom_trt_profile_available=bool(optimized_trt_profiles),
+                custom_trt_profile_available=bool(trt_profiles),
             )
 
         LOGGER.info("Converted SavedModel to Tensorflow-TensorRT.")
         return CommandOutput(status=CommandStatus.OK, output={"conversion_max_batch_size": conversion_max_batch_size})
```

## model_navigator/commands/convert/torch.py

```diff
@@ -110,15 +110,15 @@
         verbose: bool,
         debug: bool,
         dataloader_trt_profile: TensorRTProfile,
         custom_args: Dict[str, Any],
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
-        optimized_trt_profiles: Optional[List[TensorRTProfile]] = None,
+        trt_profiles: Optional[List[TensorRTProfile]] = None,
     ) -> CommandOutput:
         """Run Torchscript ot Torch-TensorRT conversion.
 
         For detailed explanation of TensorRT parameters please refer to [documentation]
         [documentation]: https://pytorch.org/TensorRT/
 
         Args:
@@ -135,15 +135,15 @@
             dataloader_trt_profile (TensorRTProfile): Dataloader TensorRT profile.
             custom_args (Dict[str, Any]): Custom arguments for conversion.
             batch_dim (Optional[int], optional): Batch dimension. Defaults to None.
             dataloader_max_batch_size (Optional[int], optional): Maximum batch size form the dataloader.
                 Defaults to None.
             device_max_batch_size (Optional[int], optional): Device maximum batch size.
                 Defaults to None.
-            optimized_trt_profiles (Optional[TensorRTProfile], optional): User specified TensorRT profile. Defaults to None.
+            trt_profiles (Optional[TensorRTProfile], optional): User specified TensorRT profile. Defaults to None.
 
         Raises:
             RuntimeError: When no GPU is available.
 
         Returns:
             CommandOutput: Status OK.
         """
@@ -161,15 +161,15 @@
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         input_dtypes_str = [tensorrt_utils.cast_type(input_spec.dtype).name for input_spec in input_metadata.values()]
 
         def get_args(max_batch_size=None):
             # NOTE: Torch-TensorRT does not support multiple profiles. Use first profile.
             # TODO: Add support for multiple profiles when Torch-TensorRT supports it.
-            profile = optimized_trt_profiles[0] if optimized_trt_profiles else dataloader_trt_profile
+            profile = trt_profiles[0] if trt_profiles else dataloader_trt_profile
             shapes = self._get_shape_args(trt_profile=profile, batch_dim=batch_dim, max_batch_size=max_batch_size)
 
             kwargs = {
                 "exported_model_path": exported_model_path.relative_to(workspace.path).as_posix(),
                 "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "shapes": shapes,
                 "input_dtypes": input_dtypes_str,
@@ -192,19 +192,19 @@
         ) as context:
             conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_external_runtime_script(ts2torchtrt.__file__, args),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
-                custom_trt_profile_available=bool(optimized_trt_profiles),
+                custom_trt_profile_available=bool(trt_profiles),
             )
 
         conversion_profiles = self._get_shape_args(
-            trt_profile=optimized_trt_profiles[0] if optimized_trt_profiles else dataloader_trt_profile,
+            trt_profile=trt_profiles[0] if trt_profiles else dataloader_trt_profile,
             batch_dim=batch_dim,
             max_batch_size=conversion_max_batch_size,
         )
         LOGGER.info("Converted TorchScript to Torch-TensorRT.")
         return CommandOutput(
             status=CommandStatus.OK,
             output={"conversion_max_batch_size": conversion_max_batch_size, "conversion_profiles": conversion_profiles},
```

## model_navigator/commands/convert/converters/onnx2trt.py

```diff
@@ -17,14 +17,16 @@
 from typing import Any, Dict, List, Optional, Tuple
 
 import fire
 from polygraphy import mod
 from polygraphy.backend.trt import CreateConfig, Profile, engine_from_network, network_from_onnx_path, save_engine
 
 from model_navigator.api.config import TensorRTPrecision, TensorRTPrecisionMode
+from model_navigator.frameworks.tensorrt.timing_tactics import TimingCacheManager
+from model_navigator.inplace.config import DEFAULT_CACHE_DIR
 
 trt = mod.lazy_import("tensorrt")
 
 
 def _get_precisions(precision, precision_mode):
     precision = TensorRTPrecision(precision)
     precision_mode = TensorRTPrecisionMode(precision_mode)
@@ -63,14 +65,16 @@
     max_workspace_size: int,
     precision: str,
     precision_mode: str,
     optimization_level: Optional[int] = None,
     compatibility_level: Optional[str] = None,
     navigator_workspace: Optional[str] = None,
     onnx_parser_flags: Optional[List[int]] = None,
+    timing_cache_dir: Optional[str] = None,
+    model_name: Optional[str] = None,
     custom_args: Optional[Dict[str, Any]] = None,
 ) -> None:
     """Run conversion from TorchScript to Torch-TensorRT.
 
     Args:
         exported_model_path (str): TorchScript model path.
         converted_model_path (str): Output Torch-TensorRT model path.
@@ -81,25 +85,30 @@
         precision (str): TensorRT precision. Could be "fp16" or "fp32".
         precision_mode (str): TensorRT precision mode.
         navigator_workspace (Optional[str], optional): Model Navigator workspace path.
             When None use current workdir. Defaults to None.
         optimization_level: Optimization level for TensorRT engine
         compatibility_level: Hardware compatibility level for generated engine
         onnx_parser_flags (Optional[List[trt.OnnxParserFlag]], optional): List of flags to set ONNX parser behavior.
+        timing_cache_dir: (Optional[str]): Directory to save timing cache. Defaults to None which means it will be saved in workspace root.
+        model_name: (Optional[str]): Model name for the timing cache. Defaults to None which means it will be named after the model file.
         custom_args (Optional[Dict[str, str]], optional): Dictionary with passthrough parameters.
             For available arguments check PyTorch documentation: https://pytorch.org/TensorRT/py_api/torch_tensorrt.html
     """
     if not navigator_workspace:
         navigator_workspace = pathlib.Path.cwd()
     navigator_workspace = pathlib.Path(navigator_workspace)
 
     exported_model_path = pathlib.Path(exported_model_path)
     if not exported_model_path.is_absolute():
         exported_model_path = navigator_workspace / exported_model_path
 
+    if model_name is None:
+        model_name = exported_model_path.stem
+
     converted_model_path = pathlib.Path(converted_model_path)
     if not converted_model_path.is_absolute():
         converted_model_path = navigator_workspace / converted_model_path
 
     custom_args = custom_args or {}
 
     trt_profiles = []
@@ -121,25 +130,36 @@
         config_kwargs["hardware_compatibility_level"] = compatibility_level
 
     if max_workspace_size:
         config_kwargs["memory_pool_limits"] = {
             trt.MemoryPoolType.WORKSPACE: max_workspace_size,
         }
 
-    engine = engine_from_network(
-        network,
-        config=CreateConfig(
-            tf32=tf32,
-            fp16=fp16,
-            bf16=bf16,
-            fp8=fp8,
-            int8=int8,
-            profiles=trt_profiles,
-            **config_kwargs,
-            **custom_args,
-        ),
-    )
-    save_engine(engine, path=converted_model_path.as_posix())
+    # saving timing cache in model_navigator workspace root
+    timing_cache = DEFAULT_CACHE_DIR / "timing_cache"
+
+    # .. or in user provided directory
+    if timing_cache_dir is not None:
+        timing_cache = pathlib.Path(timing_cache_dir)
+
+    with TimingCacheManager(model_name=model_name, cache_path=timing_cache) as timing_cache:
+        timing_cache = timing_cache.as_posix() if timing_cache else None
+        engine = engine_from_network(
+            network,
+            config=CreateConfig(
+                tf32=tf32,
+                fp16=fp16,
+                bf16=bf16,
+                fp8=fp8,
+                int8=int8,
+                profiles=trt_profiles,
+                load_timing_cache=timing_cache,
+                **config_kwargs,
+                **custom_args,
+            ),
+            save_timing_cache=timing_cache,
+        )
+        save_engine(engine, path=converted_model_path.as_posix())
 
 
 if __name__ == "__main__":
     fire.Fire(convert)
```

## model_navigator/commands/convert/onnx/onnx2trt.py

```diff
@@ -47,16 +47,17 @@
         custom_args: Dict[str, Any],
         max_workspace_size: Optional[int] = None,
         batch_dim: Optional[int] = None,
         dataloader_max_batch_size: Optional[int] = None,
         device_max_batch_size: Optional[int] = None,
         optimization_level: Optional[int] = None,
         compatibility_level: Optional[TensorRTCompatibilityLevel] = None,
-        optimized_trt_profiles: Optional[List[TensorRTProfile]] = None,
+        trt_profiles: Optional[List[TensorRTProfile]] = None,
         onnx_parser_flags: Optional[List[int]] = None,
+        timing_cache_dir: Optional[str] = None,
         verbose: bool = False,
     ) -> CommandOutput:
         """Run the ConvertONNX2TRT Command.
 
         Used for initial conversion (with max batch size search) of ONNX model to TensorRT plan and for optimized conversion with generated TensortRT profiles.
         TensorRT profiles are generated by TensorRTProfileBuilder command and saved in status.yaml file.
 
@@ -73,16 +74,17 @@
             batch_dim: Dimension of the batching, None if model does not support batching.
                 Defaults to None.
             dataloader_max_batch_size (Optional[int], optional): Maximum batch size in the dataloader. Defaults to None.
             device_max_batch_size: Maximum batch size that fits on the device.
                 Defaults to None.
             optimization_level: Optimization level for TensorRT engine
             compatibility_level: Hardware compatibility level for generated engine
-            optimized_trt_profiles: List of TensorRT profiles that will be used by Model Navigator for conversion, user provided or optimized by TensorRTProfileBuilder command.
+            trt_profiles: List of TensorRT profiles that will be used by Model Navigator for conversion, user provided.
             onnx_parser_flags (Optional[List[trt.OnnxParserFlag]], optional): List of flags to set ONNX parser behavior.
+            timing_cache_dir: (Optional[str]): Directory to save timing cache. Defaults to None which means it will be saved in workspace root.
             verbose: enable verbose logging for command
             custom_args (Optional[Dict[str, Any]], optional): Passthrough parameters for Polygraphy convert command
                 For available arguments check Polygraphy documentation: https://docs.nvidia.com/deeplearning/tensorrt/developer-guide/index.html#polygraphy
                 or Polygraphy repository: https://github.com/NVIDIA/TensorRT/tree/main/tools/Polygraphy
 
         Returns:
             CommandOutput: Status and results of the command.
@@ -99,16 +101,16 @@
             LOGGER.warning(f"Exported ONNX model not found at {input_model_path}. Skipping conversion.")
             return CommandOutput(status=CommandStatus.SKIPPED)
         converted_model_path.parent.mkdir(parents=True, exist_ok=True)
 
         onnx_input_names, _ = get_onnx_io_names(onnx_path=input_model_path)
 
         def get_args(max_batch_size=None):
-            if optimized_trt_profiles:
-                profiles = optimized_trt_profiles
+            if trt_profiles:
+                profiles = trt_profiles
             else:
                 profiles = [
                     self._get_conversion_profiles(
                         trt_profile=dataloader_trt_profile,
                         batch_dim=batch_dim,
                         max_batch_size=max_batch_size,
                     )
@@ -123,22 +125,25 @@
                 "exported_model_path": input_model_path.relative_to(workspace.path).as_posix(),
                 "converted_model_path": converted_model_path.relative_to(workspace.path).as_posix(),
                 "profiles": profiles_dicts,
                 "max_workspace_size": max_workspace_size,
                 "precision": precision.value,
                 "precision_mode": precision_mode.value,
                 "navigator_workspace": workspace.path.as_posix(),
+                "model_name": workspace.path.parent.name,
                 "custom_args": custom_args,
             }
             if optimization_level is not None:
                 kwargs["optimization_level"] = optimization_level
             if compatibility_level is not None:
                 kwargs["compatibility_level"] = compatibility_level.value
             if onnx_parser_flags:
                 kwargs["onnx_parser_flags"] = onnx_parser_flags
+            if timing_cache_dir is not None:
+                kwargs["timing_cache_dir"] = str(timing_cache_dir)
             args = parse_kwargs_to_cmd(kwargs)
             return args
 
         with ExecutionContext(
             workspace=workspace,
             script_path=converted_model_path.parent / "reproduce_conversion.py",
             cmd_path=converted_model_path.parent / "reproduce_conversion.sh",
@@ -148,19 +153,19 @@
 
             conversion_max_batch_size = self._execute_conversion(
                 convert_func=lambda args: context.execute_external_runtime_script(onnx2trt.__file__, args),
                 get_args=get_args,
                 batch_dim=batch_dim,
                 device_max_batch_size=device_max_batch_size,
                 dataloader_max_batch_size=dataloader_max_batch_size,
-                custom_trt_profile_available=bool(optimized_trt_profiles),
+                custom_trt_profile_available=bool(trt_profiles),
             )
 
         conversion_profiles = self._get_conversion_profiles(
-            trt_profile=optimized_trt_profiles[0] if optimized_trt_profiles else dataloader_trt_profile,
+            trt_profile=trt_profiles[0] if trt_profiles else dataloader_trt_profile,
             batch_dim=batch_dim,
             max_batch_size=conversion_max_batch_size,
         )
 
         LOGGER.info("Converted ONNX to TensorRT.")
         return CommandOutput(
             status=CommandStatus.OK,
```

## model_navigator/commands/export/exporters/torch2dynamo_onnx.py

```diff
@@ -60,17 +60,24 @@
 
     profiling_sample = load_samples("profiling_sample", navigator_workspace, batch_dim)[0]
     input_metadata = TensorMetadata.from_json(input_metadata)
 
     dummy_input = {n: torch.from_numpy(val).to(target_device) for n, val in profiling_sample.items()}
     dummy_input = input_metadata.unflatten_sample(dummy_input, wrap_input=False)
 
+    if not isinstance(dummy_input, tuple):
+        dummy_input = (dummy_input,)
+    if not isinstance(dummy_input[-1], dict):
+        dummy_input = (*dummy_input, {})
+    *args, kwargs = dummy_input
+
     exported_model = torch.onnx.dynamo_export(
         model,
-        dummy_input,
+        *args,
         **custom_args,
+        **kwargs,
     )
 
     exported_model_path = pathlib.Path(exported_model_path)
     if not exported_model_path.is_absolute():
         exported_model_path = navigator_workspace / exported_model_path
     exported_model.save(exported_model_path.as_posix())
```

## model_navigator/commands/export/exporters/torch2exportedprogram.py

```diff
@@ -58,19 +58,26 @@
         navigator_workspace = pathlib.Path.cwd()
     navigator_workspace = pathlib.Path(navigator_workspace)
 
     profiling_sample = load_samples("profiling_sample", navigator_workspace, batch_dim)[0]
     input_metadata = TensorMetadata.from_json(input_metadata)
 
     dummy_input = {n: torch.from_numpy(val).to(target_device) for n, val in profiling_sample.items()}
-    dummy_input = input_metadata.unflatten_sample(dummy_input, wrap_input=True)
+    dummy_input = input_metadata.unflatten_sample(dummy_input, wrap_input=False)
+
+    if not isinstance(dummy_input, tuple):
+        dummy_input = (dummy_input,)
+    if not isinstance(dummy_input[-1], dict):
+        dummy_input = (*dummy_input, {})
+    *args, kwargs = dummy_input
 
     exported_model = torch.export.export(
         model,
-        dummy_input,
+        args=tuple(args),
+        kwargs=kwargs,
         **custom_args,
     )
 
     exported_model_path = pathlib.Path(exported_model_path)
     if not exported_model_path.is_absolute():
         exported_model_path = navigator_workspace / exported_model_path
     torch.save(exported_model, exported_model_path.as_posix())
```

## model_navigator/commands/find_max_batch_size/find_max_batch_size.py

```diff
@@ -138,15 +138,15 @@
             return device_max_batch_size
 
         optimization_profile = OptimizationProfile(
             min_trials=1,
             max_trials=1,
             window_size=1,
             stabilization_windows=1,
-            throughput_cutoff_threshold=-2,
+            throughput_cutoff_threshold=None,
         )
 
         with ExecutionContext(
             workspace=workspace,
             script_path=reproduce_script_dir / f"reproduce_max_batch_size-{runner_cls.slug()}.py",
             cmd_path=reproduce_script_dir / f"reproduce_max_batch_size-{runner_cls.slug()}.sh",
             verbose=verbose,
```

## model_navigator/commands/performance/profiler.py

```diff
@@ -20,14 +20,15 @@
 
 import numpy as np
 from jsonlines import jsonlines
 
 from model_navigator.api.config import OptimizationProfile, Sample
 from model_navigator.commands.performance.nvml_handler import NvmlHandler
 from model_navigator.commands.performance.results import ProfilingResults
+from model_navigator.commands.performance.utils import is_measurement_stable, is_throughput_saturated
 from model_navigator.core.dataloader import expand_sample
 from model_navigator.core.logger import LOGGER
 from model_navigator.exceptions import ModelNavigatorError
 from model_navigator.runners.base import InferenceStep, NavigatorRunner, NavigatorStabilizedRunner
 
 
 class Profiler:
@@ -117,17 +118,15 @@
                 steps_coverage = total_steps_latency / total_latency
                 LOGGER.log(self._profiling_results_logging_level, f"Inference steps coverage: {steps_coverage:.3f}")
 
                 with jsonlines.open(self._results_path.as_posix(), "a") as f:
                     f.write(profiling_result.to_dict(parse=True))
 
                 results.append(profiling_result)
-                if prev_result is not None and profiling_result.throughput < prev_result.throughput * (
-                    1 + self._profile.throughput_cutoff_threshold
-                ):
+                if is_throughput_saturated(profiling_result, prev_result, self._profile.throughput_cutoff_threshold):
                     break
                 prev_result = profiling_result
 
         return results
 
     @property
     def _profiling_results_logging_level(self):
@@ -146,33 +145,22 @@
         for _ in range(self._profile.window_size):
             runner.infer(sample)
             gpu_clocks.append(nvml_handler.gpu_clock)
             measurements.append(runner.last_inference_time())
 
         return ProfilingResults.from_measurements(measurements, gpu_clocks, batch_size, sample_id)
 
-    def _is_measurement_stable(self, profiling_results: List[ProfilingResults], count: int = 3) -> bool:
-        if len(profiling_results) < count:
-            return False
+    def _measurements_result(self, profiling_results: List[ProfilingResults], last_n: int = 3) -> ProfilingResults:
+        if len(profiling_results) < last_n:
+            raise ModelNavigatorError(
+                f"Measurements results requires at least {last_n} consecutive stable measurements."
+            )
 
-        profiling_results = profiling_results[-count:]
-        avg_latencies = [result.avg_latency for result in profiling_results]
-        avg_latency = np.mean(avg_latencies)
-        deviation_perc = np.abs((avg_latencies - avg_latency) / avg_latency * 100)
-
-        return np.all(deviation_perc < self._profile.stability_percentage)
-
-    def _measurements_result(self, profiling_results: List[ProfilingResults], count: int = 3) -> ProfilingResults:
-        if len(profiling_results) < count:
-            raise ModelNavigatorError("Measurements results requires at least 3 consecutive stable measurements.")
-
-        profiling_results = profiling_results[-count:]
-        profiling_result = ProfilingResults.from_profiling_results(profiling_results)
-
-        return profiling_result
+        profiling_results = profiling_results[-last_n:]
+        return ProfilingResults.from_profiling_results(profiling_results)
 
     def _run_measurement(
         self,
         runner: NavigatorRunner,
         nvml_handler: NvmlHandler,
         sample: Sample,
         batch_size: Optional[int],
@@ -189,19 +177,16 @@
             for idx in range(self._profile.max_trials):
                 measurement_id = idx + 1
                 profiling_result = self._run_window_measurement(runner, nvml_handler, sample, batch_size, sample_id)
                 profiling_results.append(profiling_result)
                 LOGGER.debug(
                     f"Measurement [{measurement_id}]: {profiling_result.throughput} infer/sec, {profiling_result.avg_latency} ms"
                 )
-                is_stable = self._is_measurement_stable(
-                    profiling_results, count=min(self._profile.stabilization_windows, self._profile.max_trials)
-                )
+                last_n = min(self._profile.stabilization_windows, self._profile.max_trials)
+                is_stable = is_measurement_stable(profiling_results, last_n, self._profile.stability_percentage)
                 if measurement_id >= self._profile.min_trials and is_stable:
-                    return self._measurements_result(
-                        profiling_results, count=min(self._profile.stabilization_windows, self._profile.max_trials)
-                    )
+                    return self._measurements_result(profiling_results, last_n)
 
         raise RuntimeError(
             "Unable to get stable performance results. Consider increasing "
             "measurement_interval | measurement_request_count | stability_percentage | max_trials in OptimizationProfile."
         )
```

## model_navigator/configuration/model/model_config.py

```diff
@@ -450,39 +450,42 @@
         compatibility_level: Optional[TensorRTCompatibilityLevel],
         precision: Optional[TensorRTPrecision] = None,
         trt_profiles: Optional[List[TensorRTProfile]] = None,
         parent: Optional[ModelConfig] = None,
         onnx_parser_flags: Optional[List[int]] = None,
         custom_args: Optional[Dict[str, Any]] = None,
         device: Optional[str] = None,
+        timing_cache_dir: Optional[str] = None,
     ) -> None:
         """Initializes TensorRT (plan) model configuration class.
 
         Args:
             parent: Parent model configuration/
             precision_mode: Mode how the precision flags are combined
             max_workspace_size: The maximum GPU memory the model can use temporarily during execution
             optimization_level: Level of TensorRT engine optimization
             precision: TensorRT model precision
             trt_profiles: TensorRT profiles
             compatibility_level: Hardware compatibility level
             onnx_parser_flags: ONNX parser flags
             custom_args: Custom arguments passed to TensorRT conversion
             device: runtime device e.g. "cuda:0"
+            timing_cache_dir: Directory to store timing cache
         """
         super().__init__(parent=parent)
         self.precision = precision
         self.precision_mode = precision_mode
         self.max_workspace_size = max_workspace_size
         self.trt_profiles = trt_profiles
         self.optimization_level = optimization_level
         self.compatibility_level = compatibility_level
         self.onnx_parser_flags = onnx_parser_flags
         self.custom_args = custom_args
         self.runner_config = DeviceRunnerConfig(device=device)
+        self.timing_cache_dir = timing_cache_dir
 
     def _get_path_params_as_array_of_strings(self) -> List[str]:
         return [self.precision.value] if self.precision else []
 
     @classmethod
     def _from_dict(cls, data_dict: Dict):
         trt_profiles = data_dict.get("trt_profiles")
@@ -495,14 +498,15 @@
             precision=cls._parse_string(TensorRTPrecision, data_dict.get("precision")),
             precision_mode=cls._parse_string(TensorRTPrecisionMode, data_dict.get("precision_mode")),
             max_workspace_size=cls._parse_string(int, data_dict.get("max_workspace_size")),
             trt_profiles=trt_profiles,
             optimization_level=cls._parse_string(int, data_dict.get("optimization_level")),
             compatibility_level=cls._parse_string(TensorRTCompatibilityLevel, data_dict.get("compatibility_level")),
             onnx_parser_flags=onnx_parser_flags,
+            timing_cache_dir=data_dict.get("timing_cache_dir"),
         )
 
 
 class TensorFlowTensorRTConfig(_SerializedModelConfig, format=Format.TF_TRT):
     """TensorFlow TensorRT model configuration class."""
 
     def __init__(
```

## model_navigator/configuration/model/model_config_builder.py

```diff
@@ -433,14 +433,15 @@
                     max_workspace_size=trt_config.max_workspace_size,
                     trt_profiles=trt_config.trt_profiles,
                     optimization_level=trt_config.optimization_level,
                     compatibility_level=trt_config.compatibility_level,
                     onnx_parser_flags=trt_config.onnx_parser_flags,
                     custom_args=trt_config.custom_args,
                     device=trt_config.device,
+                    timing_cache_dir=trt_config.timing_cache_dir,
                 )
             )
         else:
             for model_configuration, precision in product(model_configs[Format.ONNX], trt_config.precision):
                 model_configs[Format.TENSORRT].append(
                     model_config.TensorRTConfig(
                         parent=model_configuration,
@@ -449,9 +450,10 @@
                         max_workspace_size=trt_config.max_workspace_size,
                         trt_profiles=trt_config.trt_profiles,
                         optimization_level=trt_config.optimization_level,
                         compatibility_level=trt_config.compatibility_level,
                         onnx_parser_flags=trt_config.onnx_parser_flags,
                         custom_args=trt_config.custom_args,
                         device=trt_config.device,
+                        timing_cache_dir=trt_config.timing_cache_dir,
                     )
                 )
```

## model_navigator/frameworks/tensorrt/utils.py

```diff
@@ -11,30 +11,33 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """TensorRT utils."""
 
 import contextlib
 import logging
-import math
 import os
 import pathlib
 import signal
 from distutils.version import LooseVersion
 from typing import Callable, List, Optional, Tuple, TypeVar, Union
 
 import numpy as np
 
 from model_navigator.api.config import ShapeTuple, TensorRTProfile, TensorType
-from model_navigator.core.constants import OPT_MAX_SHAPE_RATIO
 from model_navigator.core.tensor import TensorMetadata, get_tensor_type
 from model_navigator.exceptions import ModelNavigatorNotFoundError
 from model_navigator.utils import common as utils
 from model_navigator.utils import module
-from model_navigator.utils.common import invoke_if_callable, numpy_to_torch_dtype, torch_to_numpy_dtype
+from model_navigator.utils.common import (
+    invoke_if_callable,
+    numpy_to_torch_dtype,
+    optimal_batch_size,
+    torch_to_numpy_dtype,
+)
 
 trt = module.lazy_import("tensorrt")
 torch = module.lazy_import("torch")
 
 T = TypeVar("T")
 
 LOGGER = logging.getLogger(__name__)
@@ -167,27 +170,20 @@
     """
     new_profile = TensorRTProfile()
     for input_name in trt_profile:
         max_shapes = list(trt_profile[input_name].max)
         opt_shapes = list(trt_profile[input_name].opt)
 
         max_shapes[batch_dim] = max_batch_size
-        opt_shapes[batch_dim] = _opt_batch_size(max_batch_size)
+        opt_shapes[batch_dim] = optimal_batch_size(max_batch_size)
 
         new_profile[input_name] = ShapeTuple(trt_profile[input_name].min, tuple(opt_shapes), tuple(max_shapes))
     return new_profile
 
 
-def _opt_batch_size(max_batch_size):
-    magnitude = math.floor(math.log2(max_batch_size))
-    opt_batch_size = 2 ** int(math.ceil(magnitude * OPT_MAX_SHAPE_RATIO))
-
-    return opt_batch_size
-
-
 def _should_use_v3_api():
     return LooseVersion(trt.__version__) > LooseVersion("8.5.0.9")
 
 
 def get_bindings_per_profile(engine):
     """Return bindings per profile."""
     if _should_use_v3_api():
```

## model_navigator/inplace/__init__.py

```diff
@@ -20,14 +20,16 @@
 
 import yaml
 
 from model_navigator.api.config import DEFAULT_TORCH_TARGET_FORMATS_FOR_PROFILING, Format
 from model_navigator.commands.correctness.correctness import Correctness
 from model_navigator.commands.performance.nvml_handler import NvmlHandler
 from model_navigator.commands.performance.performance import Performance
+from model_navigator.commands.performance.utils import is_throughput_saturated
+from model_navigator.core.constants import DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD
 from model_navigator.core.logger import LOGGER, pad_string
 from model_navigator.exceptions import ModelNavigatorModuleNotOptimizedError
 from model_navigator.package.status import CommandStatus
 from model_navigator.runners.base import NavigatorRunner
 from model_navigator.runners.registry import runner_registry
 from model_navigator.runtime_analyzer.strategy import SelectedRuntimeStrategy
 from model_navigator.utils.common import DataObject
@@ -59,15 +61,17 @@
         config: Optimize config.
         status_path: Path to store the optimization status.
     """
     if config is None:
         config = OptimizeConfig()
 
     for module in module_registry.values():
-        module.optimize_config = config
+        # set main config if user did not provide one for a module
+        if module.optimize_config is None:
+            module.optimize_config = config
         module.load_recorded()
 
     for input_ in dataloader:
         _, sample = input_  # unpack batch_size and sample
         if not isinstance(sample, tuple):
             sample = (sample,)
         if not isinstance(sample[-1], dict):
@@ -89,14 +93,15 @@
     runners: Optional[Tuple[Union[str, Type[NavigatorRunner]], ...]] = None,
     status_path: Optional[Union[pathlib.Path, str]] = None,
     min_trials: int = 3,
     max_trials: int = 10,
     stabilization_windows: int = 3,
     window_size: int = 50,
     stability_percentage: float = 10.0,
+    throughput_cutoff_threshold: Optional[float] = DEFAULT_PROFILING_THROUGHPUT_CUTOFF_THRESHOLD,
     verbose: bool = False,
 ) -> None:
     """Profile `func` and all registered modules.
 
     Args:
         func: Function to profile.
         dataloader: List of tuples with batch size and input.
@@ -104,14 +109,16 @@
         runners: Use only runners provided as parameter
         status_path: Path to store the profiling results.
         min_trials: Minimum number of trials.
         max_trials: Maximum number of trials.
         stabilization_windows: Number of stabilization windows.
         window_size: Number of inference queries performed in measurement window
         stability_percentage: Allowed percentage of variation from the mean in three consecutive windows.
+        throughput_cutoff_threshold: Minimum throughput increase to continue profiling. If None is provided,
+                                     profiling run through whole dataloader
         verbose: Provide verbose logging
     """
     if target_formats is None:
         target_formats = DEFAULT_TORCH_TARGET_FORMATS_FOR_PROFILING
     if runners is None:
         runners = list(runner_registry.values())
 
@@ -124,31 +131,38 @@
     profiling_results = ProfilingResults()
     for model_key, runner_name in modelkeys_runners:
         LOGGER.info(pad_string(f"Profiling of {model_key} and {runner_name}"))
 
         _load_modules(model_key, runner_name, verbose=verbose)
         runner_profiling_results = RunnerProfilingResults()
         try:
+            prev_result = None
             for sample_id, input_ in enumerate(dataloader):
                 with NvmlHandler() as nvml_handler:
                     profiling_result = run_measurement(
                         func=func,
                         sample=input_,
                         nvml_handler=nvml_handler,
                         min_trials=min_trials,
                         max_trials=max_trials,
                         stabilization_windows=stabilization_windows,
                         window_size=window_size,
                         stability_percentage=stability_percentage,
                     )
+
                     LOGGER.info(
                         f"Performance profiling result for {runner_name} "
                         f"and sample id: {sample_id}:\n{profiling_result}"
                     )
                     runner_profiling_results.detailed[sample_id] = profiling_result
+
+                    if is_throughput_saturated(profiling_result, prev_result, throughput_cutoff_threshold):
+                        break
+                    prev_result = profiling_result
+
             runner_profiling_results.status = CommandStatus.OK
         except Exception as e:
             LOGGER.error(f"Profiling failed for model_key {model_key} and runner {runner_name}.")
             LOGGER.error(str(e))
             if verbose:
                 LOGGER.error(f"Traceback: {traceback.format_exc()}")
 
@@ -282,8 +296,10 @@
                         runner_status.status.get(Correctness.__name__)
                         == runner_status.status.get(Performance.__name__)
                         == CommandStatus.OK
                         and modelkey in modelkeys
                         and runner_name in runners
                     ):
                         modelkeys_runners.add((modelkey, runner_name))
+
+    modelkeys_runners = sorted(modelkeys_runners)
     return modelkeys_runners
```

## model_navigator/inplace/config.py

```diff
@@ -9,37 +9,49 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Inplace Optimize configuration."""
 
+import copy
 import dataclasses
+import os
 import pathlib
 from typing import Any, Dict, Optional, Sequence, Tuple, Type, Union
 
 from model_navigator.api.config import CustomConfig, DeviceKind, Format, OptimizationProfile, VerifyFunction
 from model_navigator.core.constants import DEFAULT_SAMPLE_COUNT
 from model_navigator.runners.base import NavigatorRunner
-from model_navigator.runtime_analyzer.strategy import MinLatencyStrategy, RuntimeSearchStrategy
+from model_navigator.runtime_analyzer.strategy import MaxThroughputStrategy, RuntimeSearchStrategy
 
 DEFAULT_CACHE_DIR = pathlib.Path.home() / ".cache" / "model_navigator"
 DEFAULT_MIN_NUM_SAMPLES = 100
 DEFAULT_MAX_NUM_SAMPLES_STORED = 1
 
 
+def inplace_cache_dir() -> pathlib.Path:
+    """Configure cache dir location based on environment variable.
+
+    Returns:
+        Cache dir from environment variable or DEFAULT_CACHE_DIR.
+    """
+    cache_dir = os.environ.get("MODEL_NAVIGATOR_DEFAULT_CACHE_DIR", DEFAULT_CACHE_DIR)
+    return pathlib.Path(cache_dir)
+
+
 class InplaceConfig:
     """Inplace Optimize configuration."""
 
     def __init__(self) -> None:
         """Initialize InplaceConfig."""
-        self._cache_dir: pathlib.Path = DEFAULT_CACHE_DIR
+        self._cache_dir: pathlib.Path = inplace_cache_dir()
         self._min_num_samples: int = DEFAULT_MIN_NUM_SAMPLES
         self._max_num_samples_stored: int = DEFAULT_MAX_NUM_SAMPLES_STORED
-        self.strategy: RuntimeSearchStrategy = MinLatencyStrategy()
+        self.strategy: RuntimeSearchStrategy = MaxThroughputStrategy()
 
     @property
     def min_num_samples(self) -> int:
         """Get the minimum number of samples to collect before optimizing."""
         return self._min_num_samples
 
     @min_num_samples.setter
@@ -108,9 +120,13 @@
         """Convert OptimizeConfig to dictionary."""
         config_dict = {}
         for field in dataclasses.fields(self):
             value = getattr(self, field.name)
             config_dict[field.name] = value
         return config_dict
 
+    def clone(self) -> "OptimizeConfig":
+        """Clone the current OptimizeConfig using deepcopy."""
+        return copy.deepcopy(self)
+
 
 inplace_config = InplaceConfig()
```

## model_navigator/inplace/model.py

```diff
@@ -12,15 +12,14 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Inplace models."""
 
 import abc
 import collections
 import copy
-import dataclasses
 import inspect
 import pathlib
 import tempfile
 from typing import Any, Callable, List, Optional
 
 from model_navigator.api.config import Framework, OnnxConfig, TensorRTConfig, TensorType, TorchTensorRTConfig
 from model_navigator.api.package import load_from_workspace
@@ -45,33 +44,36 @@
     def __init__(
         self,
         module,
         name: str,
         input_mapping: Callable,
         output_mapping: Callable,
         optimize_config: Optional[OptimizeConfig] = None,
+        forward: Optional[Callable] = None,
     ) -> None:
         """Initialize BaseModule.
 
         Args:
             module: module to be optimized.
             name: name of the module.
             input_mapping: function mapping module input to runner input.
             output_mapping: function mapping runner output to module output.
             optimize_config: configuration for module optimization.
+            forward: method to replace navigator default __call__
         """
         self._module = module
         self._name = name
         self._signature = self._get_signature()
         self._input_mapping = input_mapping
         self._output_mapping = output_mapping
         if optimize_config:
             self._optimize_config = self._update_optimize_config(optimize_config)
         else:
             self._optimize_config = optimize_config
+        self._forward_call = forward or self._module
 
     @property
     def name(self) -> str:
         """Module name."""
         return self._name
 
     @abc.abstractclassmethod
@@ -80,15 +82,15 @@
         pass
 
     @property
     def _workspace(self):
         return pathlib.Path(inplace_config.cache_dir) / f"{self._name}"
 
     def _update_optimize_config(self, optimize_config: OptimizeConfig) -> OptimizeConfig:
-        config = dataclasses.replace(optimize_config)
+        config = optimize_config.clone()
         if config.workspace is None:
             config.workspace = self._workspace
             LOGGER.info(f"Setting workspace to {config.workspace}")
 
         return config
 
     def _get_signature(self) -> List[str]:
@@ -132,26 +134,29 @@
 
         shapes = {n: to_numpy(t, Framework.TORCH).shape for n, t in pytree_metadata.flatten_sample(sample).items()}
         self._samples_shapes[pytree_metadata].append(shapes)
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Record a sample and run the module."""
         self.record_sample(*args, **kwargs)
-        output = self._module(*args, **kwargs)
+        output = self._forward_call(*args, **kwargs)
         return output
 
     def optimize(self):
         """Optimize the module using the recorded samples."""
         from model_navigator.api.torch import optimize
 
         batch_dim = 0 if self._optimize_config.batching else None
+        max_batch_size = None
         if self._optimize_config.optimization_profile is not None:
-            max_batch_size = self._optimize_config.optimization_profile.max_batch_size
-        else:
-            max_batch_size = None
+            if self._optimize_config.optimization_profile.max_batch_size:
+                max_batch_size = self._optimize_config.optimization_profile.max_batch_size
+            elif self._optimize_config.optimization_profile.batch_sizes:
+                max_batch_size = max(self._optimize_config.optimization_profile.batch_sizes)
+
         config_dict = {k: v for k, v in self._optimize_config.to_dict().items() if k != "workspace"}
 
         for i, pytree_metadata in enumerate(self._samples):
             config_dict["workspace"] = self._optimize_config.workspace / str(i)
             samples = self._samples[pytree_metadata]
             samples_shapes = self._samples_shapes[pytree_metadata]
             dynamic_axes = get_dynamic_axes_from_shapes(samples_shapes, pytree_metadata, batch_dim)
@@ -318,8 +323,8 @@
 
 
 class PassthroughModule(BaseModule):
     """Module that passes through the original module."""
 
     def __call__(self, *args: Any, **kwargs: Any) -> Any:
         """Pass through the original module."""
-        return self._module(*args, **kwargs)
+        return self._forward_call(*args, **kwargs)
```

## model_navigator/inplace/profiling.py

```diff
@@ -20,15 +20,17 @@
 from typing import Any, Callable, Dict, List, Optional, Union
 
 import numpy as np
 import yaml
 
 from model_navigator.commands.base import CommandStatus
 from model_navigator.commands.performance.nvml_handler import NvmlHandler
+from model_navigator.commands.performance.utils import is_measurement_stable
 from model_navigator.core.logger import LOGGER
+from model_navigator.exceptions import ModelNavigatorError
 from model_navigator.utils.common import dataclass2dict
 
 
 @dataclasses.dataclass
 class ProfilingResult:
     """Profiling results."""
 
@@ -196,25 +198,14 @@
         """
         path = pathlib.Path(path)
         data = self.to_dict()
         with path.open("w") as f:
             yaml.safe_dump(data, f, sort_keys=False)
 
 
-def _is_measurement_stable(profiling_results: List[ProfilingResult], count: int, stability_percentage: float) -> bool:
-    if len(profiling_results) < count:
-        return False
-    profiling_results = profiling_results[-count:]
-    avg_latencies = [result.avg_latency for result in profiling_results]
-    avg_latency = np.mean(avg_latencies)
-    deviation_perc = np.abs((avg_latencies - avg_latency) / avg_latency * 100)
-
-    return np.all(deviation_perc < stability_percentage)
-
-
 def _run_window_measurement(
     func: Callable,
     sample: Any,
     batch_size: int,
     nvml_handler: NvmlHandler,
     window_size: int,
 ) -> ProfilingResult:
@@ -232,14 +223,22 @@
         end = time.monotonic()
         gpu_clocks.append(nvml_handler.gpu_clock)
         measurements.append((end - start) * 1000.0)  # ms
 
     return ProfilingResult.from_measurements(measurements=measurements, batch_size=batch_size, gpu_clocks=gpu_clocks)
 
 
+def _measurements_result(profiling_results: List[ProfilingResult], last_n: int = 3) -> ProfilingResult:
+    if len(profiling_results) < last_n:
+        raise ModelNavigatorError(f"Measurements results requires at least {last_n} consecutive stable measurements.")
+
+    profiling_results = profiling_results[-last_n:]
+    return ProfilingResult.from_profiling_results(profiling_results)
+
+
 def run_measurement(
     func: Callable,
     sample: Any,
     nvml_handler: NvmlHandler,
     min_trials: int,
     max_trials: int,
     stabilization_windows: int,
@@ -265,18 +264,20 @@
     batch_size = sample[0]
     sample = sample[1:]
     for idx in range(max_trials):
         measurement_id = idx + 1
         profiling_result = _run_window_measurement(
             func=func, sample=sample, batch_size=batch_size, window_size=window_size, nvml_handler=nvml_handler
         )
+
         profiling_results.append(profiling_result)
         LOGGER.debug(f"Measurement [{measurement_id}], avg_latency: {profiling_result.avg_latency} ms")
-        is_stable = _is_measurement_stable(profiling_results, count=3, stability_percentage=stability_percentage)
+
+        last_n = min(stabilization_windows, max_trials)
+        is_stable = is_measurement_stable(profiling_results, last_n=last_n, stability_percentage=stability_percentage)
         if measurement_id >= min_trials and is_stable:
-            count_from_idx = min(stabilization_windows, max_trials)
-            return ProfilingResult.from_profiling_results(profiling_results[-count_from_idx:])
+            return _measurements_result(profiling_results, last_n)
 
     raise RuntimeError(
         "Unable to get stable performance results. Consider increasing "
         "window_size | stability_percentage | max_trials"
     )
```

## model_navigator/inplace/wrapper.py

```diff
@@ -14,14 +14,15 @@
 """Inplace Optimize model wrapper."""
 
 import functools
 from typing import Any, Callable, Optional
 
 import wrapt
 
+from model_navigator.exceptions import ModelNavigatorUserInputError
 from model_navigator.inplace.timer import Timer
 from model_navigator.runtime_analyzer.strategy import RuntimeSearchStrategy
 from model_navigator.utils.module import lazy_import
 
 from .config import OptimizeConfig
 from .model import BaseModule, OptimizedModule, PassthroughModule, RecordAndOptimizeModule, RecordModule
 from .registry import module_registry
@@ -42,62 +43,73 @@
 
     Args:
         module: torch module to wrap.
         name: module name.
         input_mapping: function to map module inputs to the expected input.
         output_mapping: function to map module outputs to the expected output.
         offload_parameters_to_cpu: offload parameters to cpu.
+        forward_func: forwarding function name used by the module, if None, the module __call__ is used.
 
     Example:
         >>> import torch
         >>> import model_navigator as nav
         >>> model = torch.nn.Linear(10, 10)
         >>> model = nav.Module(model)
     """
 
     def __init__(
         self,
-        module: torch.nn.Module,
+        module: "torch.nn.Module",
         name: Optional[str] = None,
         input_mapping: Optional[Callable] = None,
         output_mapping: Optional[Callable] = None,
         timer: Optional[Timer] = None,
         offload_parameters_to_cpu: bool = False,
+        forward_func: Optional[str] = None,
     ) -> None:
         """Initialize Module."""
         super().__init__(module)
         self._name = name or get_object_name(module)
         self._input_mapping = input_mapping or (lambda x: x)
         self._output_mapping = output_mapping or (lambda x: x)
-        self._optimize_config = OptimizeConfig()
+        self._optimize_config = None
         if timer:
             self.add_timer(timer=timer)
         else:
             self._module_timer = None
 
+        current_forward = None
+        if forward_func:
+            try:
+                current_forward = getattr(module, forward_func)
+            except AttributeError as e:
+                raise ModelNavigatorUserInputError(f"Forward method must exist, got {forward_func}.") from e
+            setattr(module, forward_func, self.__call__)
+
         self._wrapper = RecordAndOptimizeModule(
             module,
             # OptimizeConfig(),
             self._name,
             self._input_mapping,
             self._output_mapping,
+            forward=current_forward,
         )
         module_registry.register(self._name, self)
 
     def add_timer(self, timer: Timer) -> None:
         """Add timer to module."""
         self._module_timer = timer.register_module(self._name)
 
     @property
     def name(self) -> str:
         """Module name."""
         return self._name
 
     @property
-    def optimize_config(self) -> OptimizeConfig:
+    def optimize_config(self) -> Optional[OptimizeConfig]:
         """Module optimize config."""
         return self._optimize_config
 
     @optimize_config.setter
     def optimize_config(self, value: OptimizeConfig) -> None:
         """Module optimize config."""
         self._optimize_config = value
@@ -174,18 +186,19 @@
             input_mapping=self._input_mapping,
             output_mapping=self._output_mapping,
             optimize_config=self._optimize_config,
         )
 
 
 def module(
-    module_callable: Optional[Callable[[Any], torch.nn.Module]] = None,
+    module_callable: Optional[Callable[[Any], "torch.nn.Module"]] = None,
     name: Optional[str] = None,
     input_mapping: Optional[Callable] = None,
     output_mapping: Optional[Callable] = None,
+    forward_func: Optional[str] = None,
 ):
     """Inplace Optimize module wrapper decorator.
 
     This decorator wraps a torch module and provides inplace optimization functionality.
     Depending on the configuration set in config, the module will be
     optimized, recorded, or passed through.
 
@@ -193,14 +206,15 @@
     identically to the original module.
 
     Args:
         module_callable: decorated callable.
         name: module name.
         input_mapping: function to map module inputs to the expected input.
         output_mapping: function to map module outputs to the expected output.
+        forward_func: forwarding function name used by the module, if None, the module __call__ is used.
 
     Example:
         >>> import torch
         >>> import model_navigator as nav
         >>> @nav.module
         ... def my_model():
         ...     return torch.nn.Linear(10, 10)
@@ -208,19 +222,21 @@
     """
     if module_callable is None:
         return functools.partial(
             module,
             name=name,
             input_mapping=input_mapping,
             output_mapping=output_mapping,
+            forward_func=forward_func,
         )
 
     @wrapt.decorator
     def wrap_module(wrapped, instance, args, kwargs):
         return Module(
             wrapped(*args, **kwargs),
             name=name,
             input_mapping=input_mapping,
             output_mapping=output_mapping,
+            forward_func=forward_func,
         )
 
     return wrap_module(module_callable)
```

## model_navigator/pipelines/builders/tensorflow_tensorrt.py

```diff
@@ -14,20 +14,16 @@
 """Pipeline builders for TensorFlow TensorRT models."""
 
 from typing import Dict, List
 
 from model_navigator.api.config import DeviceKind, Format
 from model_navigator.commands.base import ExecutionUnit
 from model_navigator.commands.convert.tf import ConvertSavedModel2TFTRT
-from model_navigator.commands.delete_model import DeleteModel
-from model_navigator.commands.performance.performance import Performance
-from model_navigator.commands.tensorrt_profile_builder import TensorRTProfileBuilder
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
-from model_navigator.frameworks.tensorrt.utils import search_for_optimized_profiles
 from model_navigator.pipelines.pipeline import Pipeline
 from model_navigator.runners.registry import get_runner
 from model_navigator.runners.tensorflow import TensorFlowTensorRTRunner
 
 
 def tensorflow_tensorrt_conversion_builder(
     config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]
@@ -41,42 +37,42 @@
     Returns:
         Pipeline with steps for conversion
     """
     if config.target_device != DeviceKind.CUDA:
         return Pipeline(name="TensorFlow-TensorRT Conversion", execution_units=[])
 
     tensorflow_trt_models_config = models_config.get(Format.TF_TRT, [])
-    run_profiles_search = search_for_optimized_profiles(config, tensorflow_trt_models_config)
+    # run_profiles_search = search_for_optimized_profiles(config, tensorflow_trt_models_config)
 
     execution_units: List[ExecutionUnit] = []
     for model_cfg in tensorflow_trt_models_config:
-        if run_profiles_search:
-            # Run initial conversion to TensorFlow TensorRT
-            execution_units.append(ExecutionUnit(command=ConvertSavedModel2TFTRT, model_config=model_cfg))
-
-            # Generate preliminary profiling results
-            execution_units.append(
-                ExecutionUnit(
-                    command=Performance,
-                    model_config=model_cfg,
-                    runner_cls=get_runner(TensorFlowTensorRTRunner),
-                )
-            )
-
-            # Delete temporary TensorFlow TensorRT models
-            execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
-
-        # Generate TensorRT profiles or use user provided ones
-        execution_units.append(
-            ExecutionUnit(
-                command=TensorRTProfileBuilder,
-                model_config=model_cfg,
-                results_lookup_runner_cls=get_runner(TensorFlowTensorRTRunner),
-            )
-        )
+        # if run_profiles_search:
+        #     # Run initial conversion to TensorFlow TensorRT
+        #     execution_units.append(ExecutionUnit(command=ConvertSavedModel2TFTRT, model_config=model_cfg))
+        #
+        #     # Generate preliminary profiling results
+        #     execution_units.append(
+        #         ExecutionUnit(
+        #             command=Performance,
+        #             model_config=model_cfg,
+        #             runner_cls=get_runner(TensorFlowTensorRTRunner),
+        #         )
+        #     )
+        #
+        #     # Delete temporary TensorFlow TensorRT models
+        #     execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
+        #
+        # # Generate TensorRT profiles or use user provided ones
+        # execution_units.append(
+        #     ExecutionUnit(
+        #         command=TensorRTProfileBuilder,
+        #         model_config=model_cfg,
+        #         results_lookup_runner_cls=get_runner(TensorFlowTensorRTRunner),
+        #     )
+        # )
 
         # Convert to TensorFlow TensorRT again, this time with optimized profiles
         execution_units.append(
             ExecutionUnit(
                 command=ConvertSavedModel2TFTRT,
                 model_config=model_cfg,
                 results_lookup_runner_cls=get_runner(TensorFlowTensorRTRunner),
```

## model_navigator/pipelines/builders/tensorrt.py

```diff
@@ -13,21 +13,17 @@
 # limitations under the License.
 """Pipeline builders for TensorRT models."""
 
 from typing import Dict, List
 
 from model_navigator.api.config import DeviceKind, Format
 from model_navigator.commands.base import ExecutionUnit
-from model_navigator.commands.delete_model import DeleteModel
-from model_navigator.commands.performance.performance import Performance
-from model_navigator.commands.tensorrt_profile_builder import TensorRTProfileBuilder
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
 from model_navigator.frameworks import is_trt_available
-from model_navigator.frameworks.tensorrt.utils import search_for_optimized_profiles
 from model_navigator.pipelines.pipeline import Pipeline
 from model_navigator.runners.registry import get_runner
 from model_navigator.runners.tensorrt import TensorRTRunner
 
 
 def tensorrt_conversion_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Prepare conversion steps for pipeline.
@@ -39,44 +35,44 @@
     Returns:
         Pipeline with steps for conversion
     """
     if not is_trt_available() or config.target_device != DeviceKind.CUDA:
         return Pipeline(name="TensorRT Conversion", execution_units=[])
 
     trt_models_config = models_config.get(Format.TENSORRT, [])
-    run_profiles_search = search_for_optimized_profiles(config, trt_models_config)
+    # run_profiles_search = search_for_optimized_profiles(config, trt_models_config)
 
     from model_navigator.commands.convert.onnx.onnx2trt import ConvertONNX2TRT
 
     execution_units: List[ExecutionUnit] = []
     for model_cfg in trt_models_config:
-        if run_profiles_search:
-            # Run initial conversion to TensorRT
-            execution_units.append(ExecutionUnit(command=ConvertONNX2TRT, model_config=model_cfg))
-
-            # Generate preliminary profiling results
-            execution_units.append(
-                ExecutionUnit(
-                    command=Performance,
-                    model_config=model_cfg,
-                    runner_cls=get_runner(TensorRTRunner),
-                )
-            )
-
-            # Delete temporary TensorRT models
-            execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
+        # if run_profiles_search:
+        #     # Run initial conversion to TensorRT
+        #     execution_units.append(ExecutionUnit(command=ConvertONNX2TRT, model_config=model_cfg))
+        #
+        #     # Generate preliminary profiling results
+        #     execution_units.append(
+        #         ExecutionUnit(
+        #             command=Performance,
+        #             model_config=model_cfg,
+        #             runner_cls=get_runner(TensorRTRunner),
+        #         )
+        #     )
+        #
+        #     # Delete temporary TensorRT models
+        #     execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
 
         # Generate TensorRT profiles or use user provided ones
-        execution_units.append(
-            ExecutionUnit(
-                command=TensorRTProfileBuilder,
-                model_config=model_cfg,
-                results_lookup_runner_cls=get_runner(TensorRTRunner),
-            )
-        )
+        # execution_units.append(
+        #     ExecutionUnit(
+        #         command=TensorRTProfileBuilder,
+        #         model_config=model_cfg,
+        #         results_lookup_runner_cls=get_runner(TensorRTRunner),
+        #     )
+        # )
 
         # Convert ONNX to TensorRT again, this time with optimized profiles
         execution_units.append(
             ExecutionUnit(
                 command=ConvertONNX2TRT, model_config=model_cfg, results_lookup_runner_cls=get_runner(TensorRTRunner)
             )
         )
```

## model_navigator/pipelines/builders/torch_tensorrt.py

```diff
@@ -14,20 +14,16 @@
 """Pipeline builders for Torch TensorRT models."""
 
 from typing import Dict, List
 
 from model_navigator.api.config import DeviceKind, Format
 from model_navigator.commands.base import ExecutionUnit
 from model_navigator.commands.convert.torch import ConvertTorchScript2TorchTensorRT
-from model_navigator.commands.delete_model import DeleteModel
-from model_navigator.commands.performance.performance import Performance
-from model_navigator.commands.tensorrt_profile_builder import TensorRTProfileBuilder
 from model_navigator.configuration.common_config import CommonConfig
 from model_navigator.configuration.model.model_config import ModelConfig
-from model_navigator.frameworks.tensorrt.utils import search_for_optimized_profiles
 from model_navigator.pipelines.pipeline import Pipeline
 from model_navigator.runners.registry import get_runner
 from model_navigator.runners.torch import TorchTensorRTRunner
 
 
 def torch_tensorrt_conversion_builder(config: CommonConfig, models_config: Dict[Format, List[ModelConfig]]) -> Pipeline:
     """Prepare conversion steps for pipeline.
@@ -39,42 +35,42 @@
     Returns:
         Pipeline with steps for conversion
     """
     if config.target_device != DeviceKind.CUDA:
         return Pipeline(name="Torch-TensorRT Conversion", execution_units=[])
 
     torch_trt_models_config = models_config.get(Format.TORCH_TRT, [])
-    run_profiles_search = search_for_optimized_profiles(config, torch_trt_models_config)
+    # run_profiles_search = search_for_optimized_profiles(config, torch_trt_models_config)
 
     execution_units: List[ExecutionUnit] = []
     for model_cfg in torch_trt_models_config:
-        if run_profiles_search:
-            # Run initial conversion to Torch TensorRT
-            execution_units.append(ExecutionUnit(command=ConvertTorchScript2TorchTensorRT, model_config=model_cfg))
-
-            # Generate preliminary profiling results
-            execution_units.append(
-                ExecutionUnit(
-                    command=Performance,
-                    model_config=model_cfg,
-                    runner_cls=get_runner(TorchTensorRTRunner),
-                )
-            )
-
-            # Delete temporary Torch TensorRT models
-            execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
+        # if run_profiles_search:
+        #     # Run initial conversion to Torch TensorRT
+        #     execution_units.append(ExecutionUnit(command=ConvertTorchScript2TorchTensorRT, model_config=model_cfg))
+        #
+        #     # Generate preliminary profiling results
+        #     execution_units.append(
+        #         ExecutionUnit(
+        #             command=Performance,
+        #             model_config=model_cfg,
+        #             runner_cls=get_runner(TorchTensorRTRunner),
+        #         )
+        #     )
+        #
+        #     # Delete temporary Torch TensorRT models
+        #     execution_units.append(ExecutionUnit(command=DeleteModel, model_config=model_cfg))
 
         # Generate TensorRT profiles or use user provided ones
-        execution_units.append(
-            ExecutionUnit(
-                command=TensorRTProfileBuilder,
-                model_config=model_cfg,
-                results_lookup_runner_cls=get_runner(TorchTensorRTRunner),
-            )
-        )
+        # execution_units.append(
+        #     ExecutionUnit(
+        #         command=TensorRTProfileBuilder,
+        #         model_config=model_cfg,
+        #         results_lookup_runner_cls=get_runner(TorchTensorRTRunner),
+        #     )
+        # )
 
         # Convert TorchScript to Torch TensorRT again, this time with optimized profiles
         execution_units.append(
             ExecutionUnit(
                 command=ConvertTorchScript2TorchTensorRT,
                 model_config=model_cfg,
                 results_lookup_runner_cls=get_runner(TorchTensorRTRunner),
```

## model_navigator/runners/onnx.py

```diff
@@ -140,14 +140,23 @@
         input_metadata = TensorMetadata()
         for node in self.sess.get_inputs():
             dtype = ONNX_RT_TYPE_TO_NP[node.type] if node.type in ONNX_RT_TYPE_TO_NP else None
             shape = tuple(dim if isinstance(dim, int) else -1 for dim in node.shape)
             input_metadata.add(node.name, shape, dtype)
         return input_metadata
 
+    def get_onnx_output_metadata(self):
+        assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
+        output_metadata = TensorMetadata()
+        for node in self.sess.get_outputs():
+            dtype = ONNX_RT_TYPE_TO_NP[node.type] if node.type in ONNX_RT_TYPE_TO_NP else None
+            shape = tuple(dim if isinstance(dim, int) else -1 for dim in node.shape)
+            output_metadata.add(node.name, shape, dtype)
+        return output_metadata
+
     def check_input_metadata(self):
         assert self.input_metadata is not None, "Set `input_metadata`."
         onnx_input_metadata = self.get_onnx_input_metadata()
         for name in self.input_metadata:
             assert self.input_metadata[name].dtype == onnx_input_metadata[name].dtype
             assert self.input_metadata[name].shape == onnx_input_metadata[name].shape
 
@@ -244,15 +253,15 @@
 
     def infer_impl(self, feed_dict, *args, **kwargs):
         """Run inference."""
         assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
 
         with self._inference_step_timer.measure_step(InferenceStep.PREPROCESSING):
             input_metadata = self.get_onnx_input_metadata()
-            feed_dict = {name: tensor for name, tensor in feed_dict.items() if name in input_metadata}
+            feed_dict = dict(zip(input_metadata.keys(), feed_dict.values()))
 
         inputs, tensor_types = self._prepare_inputs(feed_dict)
 
         with self._inference_step_timer.measure_step(InferenceStep.COMPUTE):
             io_binding = self._get_io_bindings(inputs, tensor_types)
             self.sess.run_with_iobinding(io_binding)
             io_binding.synchronize_outputs()
@@ -262,20 +271,21 @@
         ):
             out_dict = {}
             for node, out in zip(self.sess.get_outputs(), io_binding.get_outputs()):
                 device_view = DeviceView(out.data_ptr(), out.shape(), ONNX_RT_TYPE_TO_NP[out.data_type()])
                 out_dict[node.name] = (
                     device_view.torch() if self.return_type == TensorType.TORCH else device_view.numpy()
                 )
-
         if self.output_metadata is None:
             return out_dict
 
         with self._inference_step_timer.measure_step(InferenceStep.POSTPROCESSING):
-            out_dict = {k: v for k, v in out_dict.items() if k in self.output_metadata}
+            sess_output_metadata = self.get_onnx_output_metadata()
+            out_dict = {k: v for k, v in out_dict.items() if k in sess_output_metadata}
+            out_dict = dict(zip(self.output_metadata.keys(), out_dict.values()))
 
         return out_dict
 
     def _prepare_inputs(self, feed_dict):
         with self._inference_step_timer.measure_step(InferenceStep.PREPROCESSING):
             inputs = {}
             tensor_types = {}
@@ -295,31 +305,34 @@
                     inputs[name] = tensor.to(self._torch.device(DeviceKind.CUDA.value, self.device_id))
 
         return inputs, tensor_types
 
     def _get_io_bindings(self, inputs, tensor_types):
         assert self.is_active and hasattr(self, "sess"), "Runner must be activated."
 
+        input_names = self.get_onnx_input_metadata().keys()
+
         io_binding = self.sess.io_binding()
-        for name, tensor in inputs.items():
+        for name, tensor in zip(input_names, inputs.values()):
             if tensor_types[name] == TensorType.TORCH:
                 io_binding.bind_input(
                     name,
                     DeviceKind.CUDA.value,
                     0,
                     utils.torch_to_numpy_dtype(tensor.dtype),
                     tensor.shape,
                     tensor.data_ptr(),
                 )
             else:
                 assert tensor_types[name] == TensorType.NUMPY
                 io_binding.bind_cpu_input(name, tensor)
         io_binding.synchronize_inputs()
 
-        for name in self.output_metadata:
+        output_names = self.get_onnx_output_metadata().keys()
+        for name in output_names:
             io_binding.bind_output(name, DeviceKind.CUDA.value, self.device_id)
 
         return io_binding
 
 
 class OnnxrtTensorRTRunner(OnnxrtCUDARunner):
     """ONNX runner for TensorRT runtime provider."""
```

## model_navigator/runners/torch.py

```diff
@@ -99,15 +99,16 @@
         with self._inference_step_timer.measure_step(InferenceStep.D2H_MEMCPY):
             out_dict = self._prepare_outputs(out_dict)
 
         return out_dict
 
     def inplace_infer(self, *args, **kwargs):
         """Inplace inference handler implementation."""
-        return self._loaded_model(*args, **kwargs)
+        args, kwargs = self._prepare_inplace_inputs(*args, **kwargs)
+        return self._inplace_infer(*args, **kwargs)
 
     def get_available_input_types(self) -> List[TensorType]:
         return [TensorType.NUMPY, TensorType.TORCH]
 
     def get_available_return_types_impl(self) -> List[TensorType]:
         return [TensorType.NUMPY, TensorType.TORCH]
 
@@ -141,14 +142,32 @@
     def _inplace_infer_v1(self, *args, **kwargs):
         with torch.no_grad():
             with torch.autocast(device_type=self.device, enabled=self._autocast):
                 outputs = self._loaded_model(*args, **kwargs)
 
         return outputs
 
+    def _prepare_inplace_inputs(self, *args, **kwargs):
+        """Prepare inputs for inplace inference."""
+        device_args = []
+        device_kwargs = {}
+        for value in args:
+            if isinstance(value, torch.Tensor):
+                value = value.to(self.device)
+
+            device_args.append(value)
+
+        for key, value in kwargs.items():
+            if isinstance(value, torch.Tensor):
+                value = value.to(self.device)
+
+            device_kwargs[key] = value
+
+        return device_args, device_kwargs
+
     def _prepare_inputs(self, feed_dict):
         """Prepare inputs for inference."""
         with self._inference_step_timer.measure_step(InferenceStep.PREPROCESSING):
             inputs = {}
             for input_name, spec in self.input_metadata.items():
                 value = feed_dict[input_name]
                 if spec.dtype != torch.bfloat16:
```

## model_navigator/utils/common.py

```diff
@@ -11,22 +11,24 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 """Common utils."""
 
 import dataclasses
 import glob
+import math
 import os
 import pathlib
 from enum import Enum
 from typing import Any, Dict, Iterable, List, Mapping, Optional, Sequence, Tuple, Type, TypeVar, Union
 
 import numpy
 from polygraphy.backend.trt.profile import Profile, ShapeTuple
 
+from model_navigator.core.constants import OPT_MAX_SHAPE_RATIO
 from model_navigator.core.logger import LOGGER
 from model_navigator.utils import module
 
 torch = module.lazy_import("torch")
 
 T = TypeVar("T")
 
@@ -493,7 +495,22 @@
         The paths found, or an empty list if it could not be found.
     """
     for dir_name in dirs:
         paths = glob.glob(os.path.join(dir_name, name_glob))
         if paths:
             return paths
     return []
+
+
+def optimal_batch_size(max_batch_size: int) -> int:
+    """Estimate the optimal shape based on batch size.
+
+    Args:
+        max_batch_size: The maximum batch size used during optimization.
+
+    Returns:
+        The optimal batch size.
+    """
+    magnitude = math.floor(math.log2(max_batch_size))
+    opt_batch_size = int(2 ** int(math.ceil(magnitude * OPT_MAX_SHAPE_RATIO)))
+
+    return opt_batch_size
```

## Comparing `triton_model_navigator-0.8.1.dist-info/LICENSE` & `triton_model_navigator-0.9.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `triton_model_navigator-0.8.1.dist-info/METADATA` & `triton_model_navigator-0.9.0.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: triton-model-navigator
-Version: 0.8.1
+Version: 0.9.0
 Summary: Triton Model Navigator: An inference toolkit for optimizing and deploying machine learning models and pipelines on the Triton Inference Server and PyTriton.
 License: Apache 2.0
 Project-URL: Documentation, https://triton-inference-server.github.io/model_navigator
 Project-URL: Source, https://github.com/triton-inference-server/model_navigator
 Project-URL: Tracker, https://github.com/triton-inference-server/model_navigator/issues
 Keywords: triton,inference,server,pytriton,inference,optimization,service,nvidia,tensorrt,onnx,tensorflow,pytorch,jax
 Classifier: Development Status :: 3 - Alpha
```

## Comparing `triton_model_navigator-0.8.1.dist-info/RECORD` & `triton_model_navigator-0.9.0.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,42 @@
 model_navigator/__init__.py,sha256=h_4eYBSNcRI-kfNnFYCJ-E1pBZqha17CQrcfZR0PIGQ,869
-model_navigator/__version__.py,sha256=lT2Nn16rqhoibeILAlD44W0V8Urq20LTxRzrKEjsDtg,637
+model_navigator/__version__.py,sha256=PofdYe19C9tXe6H1JTN2lCCXY_dgj5mgfxbGua7qeoM,637
 model_navigator/exceptions.py,sha256=imPeV8tMQfVKJJrqbxv8VNQHehF_puyjTZe0Y1Y-Gac,4077
 model_navigator/api/__init__.py,sha256=zMWRy719Y6T63LVEH54NX2mcgr0x32zvmboMdJR1cuI,1880
-model_navigator/api/config.py,sha256=Br_j9I4gG1fBCfk2TAlo3hKZpHtwnUzlO1pg_cy1uu0,30122
+model_navigator/api/config.py,sha256=ekKy-WbeFNrjPqUoiQHN5qDWZEivNbRg6wEdOlDvvrA,30304
 model_navigator/api/inplace.py,sha256=8I2ZkC2ol_XGJQmvjd9U2A4nVfGCt61M8EC1CNzpwj8,991
 model_navigator/api/jax.py,sha256=jW3ytmjCBO9w_8QuqwX5CBYEr-lWDE6Lbqird9iUzFA,6252
 model_navigator/api/onnx.py,sha256=NJQS2JsUTtTuzk668OVOeC7eHzjb_BYgXNt1HTaS5mE,5233
 model_navigator/api/package.py,sha256=ZIv2zZvaevJnaUC54wCtY-mzfcuwB8QSWt79FCPYdxA,17313
 model_navigator/api/python.py,sha256=NsuaezVQW0Wsa2iuJofTRvyMLACOaOyK2vWLkjtZhgc,4622
 model_navigator/api/pytriton.py,sha256=pX-ZtIk_WlpaljNL4pzuqItXJj4JUjwQxUqg6xrZZKY,8379
 model_navigator/api/tensorflow.py,sha256=HZe1pB0PEcIOfDL8oVFwodzWbCEHYTXMntO3jrZZyDY,6312
 model_navigator/api/tensorrt.py,sha256=byM1IqW6y-Y5TmlXuPOy-wSEqooxwnBtgbUqoeS_XC4,4461
 model_navigator/api/torch.py,sha256=jYybbzuEqyzJyM8ah_Dsicm7SkadN-Q6vlN01gK2Jr0,6096
 model_navigator/api/triton.py,sha256=r106-JcjphIfp1XHW5P-MKoKrn_dKyR5FIRzNNLC0dU,1655
-model_navigator/api/utilities.py,sha256=AbwSZwVxAHyiuo5MfBoOys-GOpLXOM5mPncIGrHZLvA,5807
+model_navigator/api/utilities.py,sha256=6CKQCtQ6nGp-R4jsfkJSvLz2uTM-0gtulCXeRfz6ObM,5809
 model_navigator/commands/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/commands/base.py,sha256=TD2iRytvTD7yh-VE3ENnPc-AN-hbjboonYi14q45tNw,5992
 model_navigator/commands/delete_model.py,sha256=eVW6OX_uYPkBXmhDWrRPHMHgwVP9R5YY1j-DFM2Jmis,1837
 model_navigator/commands/execution_context.py,sha256=nYfDzA62G4SInf570r6PyTfFjGhDyckrJTId0mxnM4E,9564
-model_navigator/commands/infer_metadata.py,sha256=g2Ig52RQkiddPD70B9cANmEpBMx7WY_NGT5c8omasL4,13934
+model_navigator/commands/infer_metadata.py,sha256=A-sv_EdW_55mT9fExfKitxmXm9wK_MmsZSwzOGzjZco,14044
 model_navigator/commands/load.py,sha256=GkrYiB1AbXFMWrNXLqw8wugHRspEY6LBn2qYdBfGiWA,3324
 model_navigator/commands/tensorrt_profile_builder.py,sha256=ldZ6noAfTm8TASNhMuSqD8KKbmqYKisz8TAetKZpmjE,9086
 model_navigator/commands/convert/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/commands/convert/base.py,sha256=NAI3k29GsANlAHcdOs2YZD2kh3uSm1K8Nod9aTcD9Js,9691
-model_navigator/commands/convert/tf.py,sha256=m4inKTP0xCcBbZW1M1-Br17DzYoTF3UHz1uq135Z-aw,8428
-model_navigator/commands/convert/torch.py,sha256=Fn2d6IO82Qcbzeuvmgg0UctiS-SMgYTxlnozkBFWcWk,10636
+model_navigator/commands/convert/tf.py,sha256=gw_7jkUS0I5qcdgdLKHbcGKxm6k3ZOpG94SYreGdP48,8368
+model_navigator/commands/convert/torch.py,sha256=3TdOFW0lJlVPe4UR1EWwXHHjddK3m8V9IffHi92fpP8,10566
 model_navigator/commands/convert/converters/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
-model_navigator/commands/convert/converters/onnx2trt.py,sha256=A9kvL68sJjXme5wcQooTpAujGjy9f288y3rkFr44wFA,6142
+model_navigator/commands/convert/converters/onnx2trt.py,sha256=b_aRoYhh4QGODxvFo9FQj-FcMsIymxCoHn4Qh0mpeiE,7279
 model_navigator/commands/convert/converters/sm2tftrt.py,sha256=f1O_N1ImvS4T4nABhfA-9NSkiyb2Zp_TrtIHS6QroEw,3750
 model_navigator/commands/convert/converters/ts2onnx.py,sha256=u-0ZhyzfVhwozsYXY-Jk2tAwjYmTP60p3jPTRRL8DIw,3642
 model_navigator/commands/convert/converters/ts2torchtrt.py,sha256=N0B7KkBW6OBP7mfiQHRIJQaWUb2HORmmE8uKKqW5pcI,5272
 model_navigator/commands/convert/onnx/__init__.py,sha256=UyVgzmxdd4mJGhvLBbbUymxl7c6by-A_lCh2rNNwRGk,668
 model_navigator/commands/convert/onnx/collect_onnx_input_metadata.py,sha256=x6zZ8V7C_cJl-6_weF6paaapUNidpIZxGb0AVL70lTM,1728
-model_navigator/commands/convert/onnx/onnx2trt.py,sha256=hhSVIPzwwHgJLDYBBP97mUj_uU__FyUjsO8WTNng6Fk,8679
+model_navigator/commands/convert/onnx/onnx2trt.py,sha256=TkA-dFTGJWyFYuNRnPKvQcRUohSbfaAVm0iXl_FjQ9g,8924
 model_navigator/commands/copy/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/commands/copy/copy_model.py,sha256=MqGT6UObESLhJ_YDo3_xZncr12r5b9qEmYtAzlSHSk4,1780
 model_navigator/commands/correctness/__init__.py,sha256=Vvwx07mqHeUfpg05oQLrljG2kleVqawgHeHm5EsFuu4,666
 model_navigator/commands/correctness/correctness.py,sha256=WmobZ0NRxiEyAGpBLSdAPiAHWIhJzY5eG-R7Hd9I33s,5814
 model_navigator/commands/correctness/correctness_script.py,sha256=sGAbOrDlYdp4tkbY8dbEOHMKZlBP73C6MgTh0PnMYo4,4878
 model_navigator/commands/data_dump/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/commands/data_dump/samples.py,sha256=saaLzqtrOltKaKoEerSq98ow-RuB9dZVxgWlvGYheSc,8903
@@ -44,38 +44,39 @@
 model_navigator/commands/export/jax.py,sha256=jnePY5tzSC9UxGN1rte-tt4S8SOQGTiov1ddd3zWw_k,3806
 model_navigator/commands/export/tf.py,sha256=6lqr8lzKBl1-8Tz4bFFfX8pu1QVxcTSE4Dn2mjIKk1s,5317
 model_navigator/commands/export/torch.py,sha256=nLgFWAZzxeCQy8AiMYnDZnBOkWF6WYCNOMd7oFrtw7U,16150
 model_navigator/commands/export/exporters/__init__.py,sha256=SKn-L_0vpyEc16kZkkwWinObo5KANbfYnDTKt-QhtTQ,1222
 model_navigator/commands/export/exporters/jax2savedmodel.py,sha256=7DEEVwqsPyo-zztgtLon-X-VVuOh0nfnwTgh7pYfFqY,4293
 model_navigator/commands/export/exporters/keras2savedmodel.py,sha256=RnvKHssNhYvW1N49dh0EkJ-4g50dgvvm94M-B3k6Wfg,2801
 model_navigator/commands/export/exporters/savedmodel2savedmodel.py,sha256=_Z9BZPw-DdNKxqOT_fd8y7OGAHs6kbBdHAJigMY0C7M,3147
-model_navigator/commands/export/exporters/torch2dynamo_onnx.py,sha256=1QR3e7ZT846v7nOV0o3HChvt-65G6-mqSgoggKNhkH8,2918
-model_navigator/commands/export/exporters/torch2exportedprogram.py,sha256=SiyJ5byKsjABn0LXcTJ_09fh3EirZx64IhC_gQ4WAhs,2919
+model_navigator/commands/export/exporters/torch2dynamo_onnx.py,sha256=mZS4tEg51uSM7e3O9N1kOqMUPJIjQSTG0VJ4iYrCvNk,3130
+model_navigator/commands/export/exporters/torch2exportedprogram.py,sha256=Mizu2UJ4XvO33cIGMRu_JhwkG8G0gJmcvl4IMgNedgg,3148
 model_navigator/commands/export/exporters/torch2onnx.py,sha256=P3vnY6fQkrEcLwD0Q2BTBitfUROubK8iLJmLv6utNOc,4542
 model_navigator/commands/export/exporters/torch2torchscript.py,sha256=jG3P3Lidxr0T1fzpx2wTnFChdeTQIM5sAsuxW0Ogf7c,5020
 model_navigator/commands/find_max_batch_size/__init__.py,sha256=tmO7NuRs7h-dnKvusXfr4uLxwKiK_BZUfjWnQUeSxMk,703
-model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=Yy6BaEDBS63_XAzCyCR0aT3O4ww9FXBBK7BYYspxzNo,7645
+model_navigator/commands/find_max_batch_size/find_max_batch_size.py,sha256=j_HmZUzz7abFWD6j7QqWKdDRV5wrK_jlhkPvZ7lyOdg,7647
 model_navigator/commands/find_max_batch_size/find_max_batch_size_script.py,sha256=SAgNdaZ2HqUs0UVFJ9sx2qEM-U0QQNeBBDmEuLJvmks,3193
 model_navigator/commands/optimize/__init__.py,sha256=3ZKkeSD7hcp_ZrpcvcgpzJ4FAFX2yEucp3H5s63diOs,609
 model_navigator/commands/optimize/graph_surgeon.py,sha256=hDn9Rqv1UlB6Rd8MR176v7mWkQGeD7Ri3oXvCIPGVVQ,2426
 model_navigator/commands/optimize/graph_surgeon_script.py,sha256=gA5HbkS_XywyVr90vm1pezxrr3ipiX8RGF0gSK42Qd0,3543
 model_navigator/commands/performance/__init__.py,sha256=baSuoKWNQvqeOaCSUgu8RUooz2677PpXZhWmN2ozcbA,772
 model_navigator/commands/performance/nvml_handler.py,sha256=qa9D91_r2EbCiSNfF5s9WRbWXxV0aXBpND6MEz8MGWE,3067
 model_navigator/commands/performance/performance.py,sha256=hKp-iszgAHDHAhKPFhgdIsD5fyk_jA4bkrbJE-TOAog,5584
 model_navigator/commands/performance/profile.py,sha256=0npo_73cPyRwv1IpE9iqpEIm_39qNvGYAnALdvmQQF0,7412
 model_navigator/commands/performance/profile_script.py,sha256=huinmwXkZr3gDlONWzuXBywFZRGpyVBhDcyjusL8KUg,3355
-model_navigator/commands/performance/profiler.py,sha256=KouMu3Ro1ONfU-Ytkllo0-fY7bd9AkQlRtoi6f2PqXo,8428
+model_navigator/commands/performance/profiler.py,sha256=C6zAkOHhwAyz7TeKq0psjFKy4k4iJzDfkxbnrUsFWLo,7850
 model_navigator/commands/performance/results.py,sha256=YpWkdKP0IJ439NO7HI9D_2JN0GIv1m7_2GWSwRyWiWo,10305
+model_navigator/commands/performance/utils.py,sha256=WraHaDULKVxcSzBwHYq_apBjjEOLMnZ3n6hkWxJGa50,2275
 model_navigator/commands/verification/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/commands/verification/verify.py,sha256=VEngOmIbN3AWM7WDQ9wlrU98PehGCx1QLlw8bOWIXnI,5022
 model_navigator/configuration/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/configuration/common_config.py,sha256=iDFDtBcfGgE1Nw-ICvx7KIW_xDKIAhwjWv9bi_u21A4,1927
 model_navigator/configuration/model/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
-model_navigator/configuration/model/model_config.py,sha256=7kCzAx_yaf6JEkfSfA3x-ccOSq-VBg-z_tSD9IvDmxQ,21816
-model_navigator/configuration/model/model_config_builder.py,sha256=mfKU2daLWtdph8yU-5wtqLF89IsOJUvN0Jh3tAmHzrI,20211
+model_navigator/configuration/model/model_config.py,sha256=30Ay3vPkzCrydrmzzo9JSuqpcl60VlJq6viyQRYYq2c,22039
+model_navigator/configuration/model/model_config_builder.py,sha256=S2d5IGhtDfwwkMysivW6TVu5-hLzsKDuzOadAINYDZE,20347
 model_navigator/configuration/runner/__init__.py,sha256=3ZKkeSD7hcp_ZrpcvcgpzJ4FAFX2yEucp3H5s63diOs,609
 model_navigator/configuration/runner/runner_config.py,sha256=FXrzFRLxHe-wiBIpLmG2YavIu2_ZN4j9bqPr4FA47Do,3822
 model_navigator/configuration/validation/__init__.py,sha256=wIf-elUXkGGvPkxpErP9nB6wfaafVl5stxMa643KtfA,609
 model_navigator/configuration/validation/device.py,sha256=gOhpc6ohq4apc2JXJ5zf8emeRCLEIIHbhdZMrDvVXO4,1835
 model_navigator/core/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/core/constants.py,sha256=DNLxWTiHrbVFGC7C85BakIPZ0M9VgB_mpbf0sVn5eEU,1494
 model_navigator/core/dataloader.py,sha256=vC0yPdJlrrvIyGi_bItruAeEOUIeq4_fXyGLl8xobhg,13018
@@ -85,26 +86,27 @@
 model_navigator/frameworks/__init__.py,sha256=EwQ_kg4LMYH3c9xl-WTg8wzjGh8MbdNX9JK7Ersw5-M,2844
 model_navigator/frameworks/jax/__init__.py,sha256=yTNvNVWbYVl5SXRWbHFDvNDdeMWKXNgqKoCGUI1_Y-k,657
 model_navigator/frameworks/jax/model.py,sha256=hXlDlTEQCmwt-abtGKp57IJtUHYMzviovqwHzybIuZo,1558
 model_navigator/frameworks/onnx/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/frameworks/onnx/utils.py,sha256=kBcvEsf3P2ryTX93iDwcgpjz36bU5XB_eGS5ZRk11i8,1493
 model_navigator/frameworks/tensorrt/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/frameworks/tensorrt/cuda.py,sha256=Wf0sgONkzjkpiatA9iLeqUVJauE-Jq2hC2MOCD42e4w,31492
+model_navigator/frameworks/tensorrt/timing_tactics.py,sha256=3lzQAmY0ejwVRYyEKbx4nAm5TfqOe4Ii7IZFYsxISO0,9970
 model_navigator/frameworks/tensorrt/type_mapping.py,sha256=YmpknkiKQR6rm5UyMAJvuopTrZhxC9e1lQyFhWktksw,2062
-model_navigator/frameworks/tensorrt/utils.py,sha256=7pAovAPMAdnHSyO9VhqQoPqBp3dncfBYnWy8mGT9JEg,15989
+model_navigator/frameworks/tensorrt/utils.py,sha256=Iw5JTH7wyjmSYKklHw89OET3q-tPBWra1RyyO5Q_q2w,15764
 model_navigator/frameworks/torch/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/frameworks/torch/utils.py,sha256=iEKYGSpahAdrftKJJZvxiqCEie-HkY2YqAk70Q4FxMQ,1514
-model_navigator/inplace/__init__.py,sha256=GTidU7XOp9mjcgj1b_o_88oAHhefbQDrSvmoK8VymPo,11870
-model_navigator/inplace/config.py,sha256=LSz6xVvovAqtNAE3xzJkNfTwCbNiDjqP1IVhA5sH-es,4791
-model_navigator/inplace/model.py,sha256=BGcUI_fBlQIeS1YlDD-EEezJhw_v3bysjit5A0wHPlA,12666
-model_navigator/inplace/profiling.py,sha256=YhzqsxKNqldLKZzSDkcLbYcvEO_aHlIdbU2pNiYLFg0,10024
+model_navigator/inplace/__init__.py,sha256=AL8S5xdvs1w7vIYSOiJBVKGBCeoGzatB5FkHMAldGYw,12709
+model_navigator/inplace/config.py,sha256=7pJp55vKtBc5Z3tFQXnQIKaC5BsPuC1hsfsomVeYwNs,5281
+model_navigator/inplace/model.py,sha256=rrFB-_sQgYnhQoCLiVHeSoCG6CHV261gvdJ7awca5Is,13036
+model_navigator/inplace/profiling.py,sha256=eGmVmOSw2MXNQVk016jBIIM_YoAHVC2VqV_V8i1yaSw,10031
 model_navigator/inplace/registry.py,sha256=S_NcOQnOUk200CXb034qECduF5BSZ63YjFbwWIfQHLA,2392
 model_navigator/inplace/timer.py,sha256=HpgmqwXw3KaMsOS5Db_cvLY__ytN-vpCeyVT0eDpHRY,14679
 model_navigator/inplace/utils.py,sha256=1fn_7zFc2SF7QiRAFa5f91hc8m4D1ZTswU_aAD6vJcM,3069
-model_navigator/inplace/wrapper.py,sha256=DppbcRYOd5Kiu-ydi28VquPe6kpWwOSkmPTYiIc_5Xw,7982
+model_navigator/inplace/wrapper.py,sha256=317JTbYo6TqiRITjzCZEjG_1GXgVezoYENxsB3I6OQY,8805
 model_navigator/package/__init__.py,sha256=3ZKkeSD7hcp_ZrpcvcgpzJ4FAFX2yEucp3H5s63diOs,609
 model_navigator/package/builder.py,sha256=MGUg_Sa7sQ8TTbrq3gsi3pnmu0TyEyoktHb1FXgUtbA,12399
 model_navigator/package/loader.py,sha256=iCEmtQpyYx_RaXx0gZqRVmrJ9c6H8W9AsRZS5cvimQc,5523
 model_navigator/package/package.py,sha256=v4NRSQi2LC9L5iNBdOim79gVTFUz-ywcO56LmfJBY-w,12052
 model_navigator/package/profiling_results.py,sha256=0ZKd7WSJ7EDJV7fEunV00Tu25OwpiY5T1XQqh9Q7wno,2885
 model_navigator/package/status.py,sha256=AVhrAFgL8iXaYFUbGqxD5zc2yMG7klF4gYSJyNwBTII,23564
 model_navigator/pipelines/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
@@ -116,31 +118,31 @@
 model_navigator/pipelines/builders/correctness.py,sha256=4mD9sripMmFiP_yxrJgfwrLl_I6z84jVHtMS3NY454k,2105
 model_navigator/pipelines/builders/find_device_max_batch_size.py,sha256=3r1lZDfC5My8wmS-RQyY2471QamaVp_ndwmTgBb7Bm0,4616
 model_navigator/pipelines/builders/jax.py,sha256=YA16JCveG3xChhcA4_GX5Rvd42OOdadXeMXbylmmFII,1660
 model_navigator/pipelines/builders/performance.py,sha256=P_2i3INyLsJgEuzr1nOLBznxRGiLUTHwmshsZ3088Vw,2515
 model_navigator/pipelines/builders/preprocessing.py,sha256=in3_RjZ8puqdxso2WRDEx0sSeFXEXkwV7gX4xzamSB8,2624
 model_navigator/pipelines/builders/profiling.py,sha256=vAJX341oPdlTTP1Ga7qCh_pm2UI4hz324TM7YU3ErJE,2503
 model_navigator/pipelines/builders/tensorflow.py,sha256=Zmc6kOZiXBTTjyV_Fu5sYWIdOiTcx9nbfxhuiHWbLrY,2732
-model_navigator/pipelines/builders/tensorflow_tensorrt.py,sha256=lMuws8eSHS6-30b1JuxOXQLq50fvnJ1lw5g7Zv8MGi8,3674
-model_navigator/pipelines/builders/tensorrt.py,sha256=gPko8hAP_goTz6dW5KwambyJivh-kQagYIdYzVozevc,3564
+model_navigator/pipelines/builders/tensorflow_tensorrt.py,sha256=fkiuZM52qlejnAp8k9Clavb06s8MwdrOLu-vq75w3B8,3441
+model_navigator/pipelines/builders/tensorrt.py,sha256=2_sFJ9YJ_TO-nC2H7FAMq-IHPwI15pUOEcBVtscwjZs,3320
 model_navigator/pipelines/builders/torch.py,sha256=h98yqYGrHqVzabRk-W8H49pRV-hgg3JxhKjO3E5-eXY,3797
-model_navigator/pipelines/builders/torch_tensorrt.py,sha256=Bb3HKOMU4oGy5yWLoJWEQrLYDL4OdjJC0PHwtm4M5os,3638
+model_navigator/pipelines/builders/torch_tensorrt.py,sha256=irWCQS-1E4XYZ7m2CXwtioal8hHJI4o4i0K8jFPUXLg,3394
 model_navigator/pipelines/builders/verify.py,sha256=sy8r4VgciT9k7Tb_mIfsB_XjOK3bqKTCr-Qiq8l6Z2w,2111
 model_navigator/pipelines/wrappers/__init__.py,sha256=3ZKkeSD7hcp_ZrpcvcgpzJ4FAFX2yEucp3H5s63diOs,609
 model_navigator/pipelines/wrappers/optimize.py,sha256=CpZ9zAuh2EAnV6o8GtpolpBF4r3ALBDn4CrwH4IB0YA,2795
 model_navigator/pipelines/wrappers/profile.py,sha256=7UQCUwvuSf0ko4EP8GazGTsoy11Eh_VvJ5uwwwjHLMs,4911
 model_navigator/runners/__init__.py,sha256=x3WKEM55a0z7S51SnAD2uGm77HNVt2L_TUgFquTNPwo,1572
 model_navigator/runners/base.py,sha256=Y4k_C-BhX1DPrXglx0xoxhRkVgS7zd5gaFXPEvBVrmI,16141
 model_navigator/runners/jax.py,sha256=RYReIyaLShpwhyK40BZRZdJ4H5fOIIH_hC-JpuL2cF0,2065
-model_navigator/runners/onnx.py,sha256=89k0fPNX49mboymwPchKMox1rAS_xAIcQEUd-Mn-Iw4,13466
+model_navigator/runners/onnx.py,sha256=Y_yvBh2xtj6I9dpOSrncjts9hDVkk67lF5qKXn5t9m0,14203
 model_navigator/runners/python.py,sha256=XKkMGC_vKBOkjyDIddW92ocTJ8DS2ANjSHvHrcQz73A,2004
 model_navigator/runners/registry.py,sha256=O2m5KY8J8pq5gUjGV7v6X0KdzTPjDjYEwscZlu3k7GY,2291
 model_navigator/runners/tensorflow.py,sha256=5fe0r5EMS0-p3oH4DD-JKMw3SUdNhmtwZMPmmmfJj08,7524
 model_navigator/runners/tensorrt.py,sha256=pkbszbsrayXu8f4HcmzOtTyBmSC8iDF1Jj7ckB2SgHM,31280
-model_navigator/runners/torch.py,sha256=PIAqjXtF20GDjs2T3DamaB47RwavOyVkwVWLZGisxU0,15362
+model_navigator/runners/torch.py,sha256=_Nz37EBoO4B9E79gtGYvf2USrB9wO7IR4VEZNp4lk0U,15973
 model_navigator/runners/utils.py,sha256=AVm9cy-cUSHxdLe1wj0QqIWgbf_th89gW129Y7exzmw,3582
 model_navigator/runtime_analyzer/__init__.py,sha256=BrhKs-NzpT0ilLmYe38kUtOS7AJ-KfzyV-Hc7ANJWEE,937
 model_navigator/runtime_analyzer/analyzer.py,sha256=5ZjNEWR6K-Pj4DbQ5vMIZdz1GlGsGQytfxpj6ATdnfk,11715
 model_navigator/runtime_analyzer/strategy.py,sha256=L6dqnf1OS0s5mrBvxTTFgNPghKbuEFC2X_2tMm3_Hs4,2304
 model_navigator/triton/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
 model_navigator/triton/model_config.py,sha256=rlJxcDiXljLgxEWgxexMHLOYD5TxG3Wu13s71XR4DgI,4384
 model_navigator/triton/model_config_builder.py,sha256=dHSzaigeOfQIvH4rxxrmP0QbS2E00nMz_Deb4g2bN8I,5219
@@ -152,19 +154,19 @@
 model_navigator/triton/specialized_configs/internal.py,sha256=nJF2NIHjnRrUFDxbglIZHe_ytP5ZNMxJiRBZY1I-CL8,2230
 model_navigator/triton/specialized_configs/onnx_model_config.py,sha256=3zvQ-z7uz0ACrYHoFcHQRejipa0WovOsBA2-BUzzPmQ,2685
 model_navigator/triton/specialized_configs/python_model_config.py,sha256=TkqzyE0OH59Qk0m6qcZznAHTI-KzZIlRIdNv0_TM3wk,1786
 model_navigator/triton/specialized_configs/pytorch_model_config.py,sha256=yVs8sow5m5_Q64pm7nMgsK5sXAjNnUM96oYumalta-U,2021
 model_navigator/triton/specialized_configs/tensorflow_model_config.py,sha256=_Hzw1mnyu5vS2Yj1ggJJw7n_lZ_6iayzuqExNe7avPk,3162
 model_navigator/triton/specialized_configs/tensorrt_model_config.py,sha256=1BUADorNwcZKr348_QEcrqlg2qr3ytQbUifNt2JQtzA,3041
 model_navigator/utils/__init__.py,sha256=jahgN4-hPiDba3hK8_njbpy4tKX1KOvP08XSFgg-5cQ,614
-model_navigator/utils/common.py,sha256=nC1ZVjG9rjsmNvwFRuMXxrFSMZ8YVoAHMAYVlBVe9wQ,14607
+model_navigator/utils/common.py,sha256=cM7SBa_ebc_myS43IfbtwmviBPIWK208YxNyg2ybzzI,15089
 model_navigator/utils/config_helpers.py,sha256=V4nUkNrLmk-DsWTB8ukRNBksfZOCbWIakqqbZHPwsEQ,2495
 model_navigator/utils/devices.py,sha256=RESvu-eyD4LGwzXF1rCxE-3SMc_Vume0IWROQ8dqR1k,3912
 model_navigator/utils/enums.py,sha256=LyUAwa0x5paYPMbzfuB2-OV-QLZMi_bn5MyefcQ9Z3E,1309
 model_navigator/utils/environment.py,sha256=QhjwdNf5HAjQUB_nGbEASzGi9LrJMEatFjUDZsluffw,6175
 model_navigator/utils/format_helpers.py,sha256=6wpgYJqG4qjFpv-zF-KLDfybdZL16Bj7xNzlEfBBVjw,5338
 model_navigator/utils/module.py,sha256=pll8QcbHLdSZDrwZEnHXOHfn4Bjz4IA4VoiO5_rUNN8,2331
-triton_model_navigator-0.8.1.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
-triton_model_navigator-0.8.1.dist-info/METADATA,sha256=Ciu728koFJQ_H8OD5fH-SEiGbP41yTtYk34x-uf1MHo,13486
-triton_model_navigator-0.8.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-triton_model_navigator-0.8.1.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
-triton_model_navigator-0.8.1.dist-info/RECORD,,
+triton_model_navigator-0.9.0.dist-info/LICENSE,sha256=TNE_ejHpj1HE-5YKEV6amrnEIoTKXVybXMvPMi3kW_0,10140
+triton_model_navigator-0.9.0.dist-info/METADATA,sha256=fv_eaIxO4kWSb1qzhj9OEzRTR1a7-1YO93nMlJTMZxE,13486
+triton_model_navigator-0.9.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+triton_model_navigator-0.9.0.dist-info/top_level.txt,sha256=oWPi6CvN9rCcFJQ2tSee50OsSz3VCwl0gED86pG5glI,16
+triton_model_navigator-0.9.0.dist-info/RECORD,,
```

