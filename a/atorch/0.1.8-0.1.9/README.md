# Comparing `tmp/atorch-0.1.8-py3-none-any.whl.zip` & `tmp/atorch-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,291 +1,297 @@
-Zip file size: 578430 bytes, number of entries: 289
--rw-r--r--  2.0 unx      958 b- defN 24-Jan-18 02:35 atorch/__init__.py
--rw-r--r--  2.0 unx      255 b- defN 23-Dec-20 06:58 atorch/amp/__init__.py
--rw-r--r--  2.0 unx     3412 b- defN 23-Dec-20 06:58 atorch/amp/amp.py
--rw-r--r--  2.0 unx      868 b- defN 23-Dec-20 06:58 atorch/amp/hook.py
--rw-r--r--  2.0 unx    12488 b- defN 23-Dec-20 06:58 atorch/amp/pipe_amp.py
--rw-r--r--  2.0 unx       83 b- defN 24-Jan-17 06:24 atorch/auto/__init__.py
--rw-r--r--  2.0 unx    28847 b- defN 24-Apr-10 08:59 atorch/auto/accelerate.py
--rw-r--r--  2.0 unx     1095 b- defN 24-Jan-17 06:24 atorch/auto/auto_accelerate_context.py
--rw-r--r--  2.0 unx    13550 b- defN 24-Jan-17 06:24 atorch/auto/clip_grad_norm.py
--rw-r--r--  2.0 unx     6456 b- defN 24-Jan-17 06:24 atorch/auto/device_context.py
--rw-r--r--  2.0 unx     2480 b- defN 24-Jan-17 06:24 atorch/auto/engine_client.py
--rw-r--r--  2.0 unx    37647 b- defN 24-Apr-10 08:59 atorch/auto/model_context.py
--rw-r--r--  2.0 unx     4803 b- defN 24-Apr-10 08:59 atorch/auto/strategy.py
--rw-r--r--  2.0 unx      468 b- defN 24-Jan-17 06:24 atorch/auto/task.py
--rw-r--r--  2.0 unx       31 b- defN 24-Jan-17 06:24 atorch/auto/analyser/__init__.py
--rw-r--r--  2.0 unx    12008 b- defN 24-Jan-17 06:24 atorch/auto/analyser/analyser.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/dry_runner/__init__.py
--rw-r--r--  2.0 unx     6435 b- defN 24-Jan-17 06:24 atorch/auto/dry_runner/dry_runner.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/__init__.py
--rw-r--r--  2.0 unx     3241 b- defN 24-Jan-17 06:24 atorch/auto/engine/acceleration_engine.py
--rw-r--r--  2.0 unx      948 b- defN 24-Jan-17 06:24 atorch/auto/engine/analyser_result.py
--rw-r--r--  2.0 unx     3064 b- defN 24-Jan-17 06:24 atorch/auto/engine/client.py
--rw-r--r--  2.0 unx    11304 b- defN 24-Jan-17 06:24 atorch/auto/engine/executor.py
--rw-r--r--  2.0 unx     6810 b- defN 24-Jan-17 06:24 atorch/auto/engine/optimization_method.py
--rw-r--r--  2.0 unx     4587 b- defN 24-Jan-17 06:24 atorch/auto/engine/planner.py
--rw-r--r--  2.0 unx     3035 b- defN 24-Apr-10 08:59 atorch/auto/engine/servicer.py
--rw-r--r--  2.0 unx     6306 b- defN 24-Jan-17 06:24 atorch/auto/engine/strategy.py
--rw-r--r--  2.0 unx     1693 b- defN 24-Jan-17 06:24 atorch/auto/engine/task.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/__init__.py
--rw-r--r--  2.0 unx     5713 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/bayes_opt_sg.py
--rw-r--r--  2.0 unx     2271 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/combination_sg.py
--rw-r--r--  2.0 unx      896 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/sg_algo_lib.py
--rw-r--r--  2.0 unx      886 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/sg_algorithm.py
--rw-r--r--  2.0 unx    14213 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/utils.py
--rw-r--r--  2.0 unx      150 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/acq_optimizers/__init__.py
--rw-r--r--  2.0 unx     5851 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/acq_optimizers/evolution_optimizer.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/acquisitions/__init__.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/acquisitions/acq.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/design_space/__init__.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/design_space/categorical_param.py
--rw-r--r--  2.0 unx     3119 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/design_space/design_space.py
--rw-r--r--  2.0 unx     1063 b- defN 24-Apr-10 08:59 atorch/auto/engine/sg_algo/hebo/design_space/param.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/__init__.py
--rw-r--r--  2.0 unx     2105 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/base_model.py
--rw-r--r--  2.0 unx      666 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/layers.py
--rw-r--r--  2.0 unx      598 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/model_factory.py
--rw-r--r--  2.0 unx      541 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/util.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/gauss_process/__init__.py
--rw-r--r--  2.0 unx     4516 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/gauss_process/gpy_wgp.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/random_forest/__init__.py
--rw-r--r--  2.0 unx     1815 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/models/random_forest/rf.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/optimizers/__init__.py
--rw-r--r--  2.0 unx     1174 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/optimizers/abstract_optimizer.py
--rw-r--r--  2.0 unx     8272 b- defN 24-Apr-10 08:59 atorch/auto/engine/sg_algo/hebo/optimizers/hebo.py
--rw-r--r--  2.0 unx     1608 b- defN 24-Jan-17 06:24 atorch/auto/engine/sg_algo/hebo/optimizers/util.py
--rw-r--r--  2.0 unx       54 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/__init__.py
--rw-r--r--  2.0 unx    16692 b- defN 24-Apr-10 08:59 atorch/auto/opt_lib/amp_optimization.py
--rw-r--r--  2.0 unx    10362 b- defN 24-Apr-12 05:44 atorch/auto/opt_lib/checkpoint_optimization.py
--rw-r--r--  2.0 unx     7195 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/ds_3d_parallel_optimization.py
--rw-r--r--  2.0 unx      356 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/dynamo_backends.py
--rw-r--r--  2.0 unx     2639 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/dynamo_optimization.py
--rw-r--r--  2.0 unx     1856 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/half_optimization.py
--rw-r--r--  2.0 unx    13786 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/mixed_parallel_optimization.py
--rw-r--r--  2.0 unx     7217 b- defN 24-Jan-18 02:35 atorch/auto/opt_lib/module_replace_optimization.py
--rw-r--r--  2.0 unx    10892 b- defN 24-Apr-10 08:59 atorch/auto/opt_lib/optimization.py
--rw-r--r--  2.0 unx     2787 b- defN 24-Jan-18 02:35 atorch/auto/opt_lib/optimization_library.py
--rw-r--r--  2.0 unx     2112 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/parallel_mode_optimization.py
--rw-r--r--  2.0 unx    11721 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/pipeline_parallel_optimization.py
--rw-r--r--  2.0 unx    10728 b- defN 24-Apr-10 08:59 atorch/auto/opt_lib/selective_offloading_checkpoint.py
--rw-r--r--  2.0 unx     7992 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/tensor_parallel_optimization.py
--rw-r--r--  2.0 unx     6182 b- defN 24-Apr-10 08:59 atorch/auto/opt_lib/utils.py
--rw-r--r--  2.0 unx    22731 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/zero_optimization.py
--rw-r--r--  2.0 unx      241 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/__init__.py
--rw-r--r--  2.0 unx     5145 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/base_stage_planner.py
--rw-r--r--  2.0 unx     9408 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/base_tp_planner.py
--rw-r--r--  2.0 unx     8974 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/dim_planner.py
--rw-r--r--  2.0 unx    22977 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/mip_tp_planner.py
--rw-r--r--  2.0 unx     3471 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/topology.py
--rw-r--r--  2.0 unx    26926 b- defN 24-Jan-17 06:24 atorch/auto/opt_lib/shard_planners/utils.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/common/__init__.py
--rw-r--r--  2.0 unx     3383 b- defN 23-Dec-20 06:58 atorch/common/constants.py
--rw-r--r--  2.0 unx     3340 b- defN 23-Dec-20 06:58 atorch/common/log_utils.py
--rw-r--r--  2.0 unx     6077 b- defN 23-Dec-20 06:58 atorch/common/util_func.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/common/file/__init__.py
--rw-r--r--  2.0 unx      845 b- defN 23-Dec-21 03:00 atorch/common/file/file_io.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/common/file/file_system/__init__.py
--rw-r--r--  2.0 unx     4991 b- defN 23-Dec-20 06:58 atorch/common/file/file_system/file_system.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/common/file/file_system/pangu/__init__.py
--rw-r--r--  2.0 unx    13710 b- defN 23-Dec-20 06:58 atorch/common/file/file_system/pangu/fsspec_instance.py
--rw-r--r--  2.0 unx    17043 b- defN 23-Dec-20 06:58 atorch/common/file/file_system/pangu/pangu_file_system.py
--rw-r--r--  2.0 unx      633 b- defN 24-Jan-22 05:55 atorch/data/__init__.py
--rw-r--r--  2.0 unx    17310 b- defN 23-Dec-20 06:58 atorch/data/coworker_dataset.py
--rw-r--r--  2.0 unx     1347 b- defN 24-Apr-10 08:59 atorch/data/data_utils.py
--rw-r--r--  2.0 unx    13694 b- defN 23-Dec-21 03:00 atorch/data/elastic_dataloader.py
--rw-r--r--  2.0 unx     4771 b- defN 23-Dec-20 06:58 atorch/data/elastic_dataset.py
--rw-r--r--  2.0 unx     6113 b- defN 23-Dec-20 06:58 atorch/data/preloader.py
--rw-r--r--  2.0 unx    27904 b- defN 23-Dec-20 06:58 atorch/data/shm_context.py
--rw-r--r--  2.0 unx    10185 b- defN 24-Apr-10 08:59 atorch/data/shm_dataloader.py
--rw-r--r--  2.0 unx     3396 b- defN 23-Dec-20 06:58 atorch/data/unordered_dataloader.py
--rw-r--r--  2.0 unx     1425 b- defN 23-Dec-20 06:58 atorch/data/unshuffled_batch_dataloader.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/data_parallel/__init__.py
--rw-r--r--  2.0 unx    25559 b- defN 23-Dec-20 06:58 atorch/data_parallel/adp.py
--rw-r--r--  2.0 unx    13332 b- defN 23-Dec-20 06:58 atorch/data_parallel/auto_wrap.py
--rw-r--r--  2.0 unx     3562 b- defN 23-Dec-20 06:58 atorch/data_parallel/wrapper.py
--rw-r--r--  2.0 unx    25890 b- defN 23-Dec-20 06:58 atorch/data_parallel/zero_ddp_mix_112.py
--rw-r--r--  2.0 unx      261 b- defN 23-Dec-20 06:58 atorch/distributed/__init__.py
--rw-r--r--  2.0 unx    28079 b- defN 24-Apr-10 08:59 atorch/distributed/distributed.py
--rw-r--r--  2.0 unx      465 b- defN 23-Dec-20 06:58 atorch/distributed/elastic_controller.py
--rw-r--r--  2.0 unx     3405 b- defN 23-Dec-20 06:58 atorch/distributed/elastic_trainer.py
--rw-r--r--  2.0 unx     1253 b- defN 23-Dec-21 03:00 atorch/distributed/hooks.py
--rw-r--r--  2.0 unx    19071 b- defN 23-Dec-21 03:00 atorch/distributed/launch.py
--rw-r--r--  2.0 unx    12424 b- defN 24-Apr-10 08:59 atorch/distributed/run.py
--rw-r--r--  2.0 unx       68 b- defN 23-Dec-20 06:58 atorch/fault_tolerance/__init__.py
--rw-r--r--  2.0 unx     4825 b- defN 23-Dec-20 06:58 atorch/fault_tolerance/api.py
--rw-r--r--  2.0 unx     8293 b- defN 23-Dec-20 06:58 atorch/fault_tolerance/custom_agent.py
--rw-r--r--  2.0 unx     5659 b- defN 23-Dec-20 06:58 atorch/fault_tolerance/hanging_detector.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:32 atorch/modules/__init__.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/__init__.py
--rw-r--r--  2.0 unx    14763 b- defN 24-Apr-10 08:59 atorch/modules/distributed_modules/activation_checkpointing.py
--rw-r--r--  2.0 unx     5688 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/cross_entropy.py
--rw-r--r--  2.0 unx    29411 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/layers.py
--rw-r--r--  2.0 unx    16790 b- defN 24-Apr-10 08:59 atorch/modules/distributed_modules/mappings.py
--rw-r--r--  2.0 unx     7633 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/mappings_registry.py
--rw-r--r--  2.0 unx     1269 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/materialize_modules.py
--rw-r--r--  2.0 unx    54608 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/modules_registry.py
--rw-r--r--  2.0 unx     5436 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/randomizer.py
--rw-r--r--  2.0 unx    75800 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/transformer.py
--rw-r--r--  2.0 unx     7551 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/utils.py
--rw-r--r--  2.0 unx      147 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/__init__.py
--rw-r--r--  2.0 unx    36537 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/pipe_compiler/PipelineStage.py
--rw-r--r--  2.0 unx     3976 b- defN 24-Apr-10 08:59 atorch/modules/distributed_modules/compilers/pipe_compiler/StageInterleaver.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/pipe_compiler/__init__.py
--rw-r--r--  2.0 unx    20974 b- defN 24-Apr-10 08:59 atorch/modules/distributed_modules/compilers/pipe_compiler/distributed_pippy_compiler.py
--rw-r--r--  2.0 unx    25818 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/pipe_compiler/utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/tp_compiler/__init__.py
--rw-r--r--  2.0 unx      222 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/tp_compiler/dtensor_compiler.py
--rw-r--r--  2.0 unx     7707 b- defN 24-Jan-17 06:32 atorch/modules/distributed_modules/compilers/tp_compiler/tp_compiler.py
--rw-r--r--  2.0 unx       80 b- defN 24-Jan-17 06:32 atorch/modules/distributed_transformer/__init__.py
--rw-r--r--  2.0 unx     3173 b- defN 24-Jan-17 06:32 atorch/modules/distributed_transformer/commu_utils.py
--rw-r--r--  2.0 unx    14623 b- defN 24-Jan-17 06:32 atorch/modules/distributed_transformer/distributed_attention.py
--rw-r--r--  2.0 unx      295 b- defN 24-Jan-17 06:32 atorch/modules/moe/__init__.py
--rw-r--r--  2.0 unx    16005 b- defN 24-Apr-10 08:59 atorch/modules/moe/ddp.py
--rw-r--r--  2.0 unx     4291 b- defN 24-Jan-17 06:32 atorch/modules/moe/inject.py
--rw-r--r--  2.0 unx    25005 b- defN 24-Jan-17 06:32 atorch/modules/moe/moe_layer.py
--rw-r--r--  2.0 unx     6683 b- defN 24-Jan-17 06:32 atorch/modules/moe/switch_gating.py
--rw-r--r--  2.0 unx     5799 b- defN 24-Jan-17 06:32 atorch/modules/moe/topk_gating.py
--rw-r--r--  2.0 unx       37 b- defN 24-Jan-17 06:32 atorch/modules/transformer/__init__.py
--rw-r--r--  2.0 unx     5210 b- defN 24-Jan-17 06:32 atorch/modules/transformer/_fa_api_compat_patch
--rw-r--r--  2.0 unx    13580 b- defN 24-Jan-17 06:32 atorch/modules/transformer/cross_entropy.py
--rw-r--r--  2.0 unx     8248 b- defN 24-Jan-18 02:35 atorch/modules/transformer/inject.py
--rw-r--r--  2.0 unx    67467 b- defN 24-Apr-10 08:59 atorch/modules/transformer/layers.py
--rw-r--r--  2.0 unx     2682 b- defN 24-Jan-17 06:32 atorch/modules/transformer/linear.py
--rw-r--r--  2.0 unx      374 b- defN 24-Apr-10 08:59 atorch/modules/transformer/losses.py
--rw-r--r--  2.0 unx      244 b- defN 24-Apr-10 08:59 atorch/mup/__init__.py
--rw-r--r--  2.0 unx     4232 b- defN 24-Apr-10 08:59 atorch/mup/infshape.py
--rw-r--r--  2.0 unx     8553 b- defN 24-Apr-10 08:59 atorch/mup/init.py
--rw-r--r--  2.0 unx    11021 b- defN 24-Apr-10 08:59 atorch/mup/module.py
--rw-r--r--  2.0 unx     5867 b- defN 24-Apr-10 08:59 atorch/mup/optim.py
--rw-r--r--  2.0 unx     7971 b- defN 24-Apr-10 08:59 atorch/mup/shape.py
--rw-r--r--  2.0 unx      455 b- defN 23-Dec-20 06:58 atorch/normalization/__init__.py
--rw-r--r--  2.0 unx     9000 b- defN 24-Apr-10 08:59 atorch/normalization/layernorm.py
--rw-r--r--  2.0 unx     2681 b- defN 24-Apr-10 08:59 atorch/npu/__init__.py
--rw-r--r--  2.0 unx     6090 b- defN 24-Apr-10 08:59 atorch/npu/layers.py
--rw-r--r--  2.0 unx     7676 b- defN 24-Apr-10 08:59 atorch/npu/optim.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/ops/__init__.py
--rw-r--r--  2.0 unx      950 b- defN 23-Dec-20 06:58 atorch/ops/git_version_info.py
--rw-r--r--  2.0 unx      347 b- defN 24-Apr-12 06:05 atorch/ops/git_version_info_installed.py
--rw-r--r--  2.0 unx      271 b- defN 23-Dec-20 06:58 atorch/ops/accelerator/__init__.py
--rw-r--r--  2.0 unx     4732 b- defN 23-Dec-20 06:58 atorch/ops/accelerator/abstract_accelerator.py
--rw-r--r--  2.0 unx     8910 b- defN 23-Dec-20 06:58 atorch/ops/accelerator/cuda_accelerator.py
--rw-r--r--  2.0 unx     2478 b- defN 23-Dec-20 06:58 atorch/ops/accelerator/real_accelerator.py
--rw-r--r--  2.0 unx    12017 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/conversion_utils.h
--rw-r--r--  2.0 unx     7001 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/dequantization_utils.h
--rw-r--r--  2.0 unx     1202 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/kernel_utils.h
--rw-r--r--  2.0 unx    31857 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/memory_access_utils.h
--rw-r--r--  2.0 unx     1838 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/quantization.h
--rw-r--r--  2.0 unx     1884 b- defN 23-Dec-21 03:00 atorch/ops/csrc/includes/quantization_optimizer.h
--rw-r--r--  2.0 unx    16931 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/quantization_utils.h
--rw-r--r--  2.0 unx      411 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/quantizer.h
--rw-r--r--  2.0 unx    17562 b- defN 23-Dec-20 06:58 atorch/ops/csrc/includes/reduction_utils.h
--rw-r--r--  2.0 unx     3048 b- defN 23-Dec-20 06:58 atorch/ops/csrc/quantization/dequantize.cu
--rw-r--r--  2.0 unx     8061 b- defN 23-Dec-20 06:58 atorch/ops/csrc/quantization/pt_binding.cpp
--rw-r--r--  2.0 unx     9192 b- defN 23-Dec-20 06:58 atorch/ops/csrc/quantization/quant_reduce.cu
--rw-r--r--  2.0 unx     2791 b- defN 23-Dec-21 03:00 atorch/ops/csrc/quantization/quantization_optimizer.cc
--rw-r--r--  2.0 unx    24575 b- defN 23-Dec-21 03:00 atorch/ops/csrc/quantization/quantization_optimizer.cu
--rw-r--r--  2.0 unx     6418 b- defN 23-Dec-20 06:58 atorch/ops/csrc/quantization/quantize.cu
--rw-r--r--  2.0 unx     7576 b- defN 23-Dec-20 06:58 atorch/ops/csrc/quantization/swizzled_quantize.cu
--rw-r--r--  2.0 unx     2091 b- defN 23-Dec-20 06:58 atorch/ops/op_builder/__init__.py
--rw-r--r--  2.0 unx     1271 b- defN 23-Dec-20 06:58 atorch/ops/op_builder/all_ops.py
--rw-r--r--  2.0 unx    25650 b- defN 23-Dec-20 06:58 atorch/ops/op_builder/builder.py
--rw-r--r--  2.0 unx      846 b- defN 23-Dec-21 03:00 atorch/ops/op_builder/quantization_optimizer.py
--rw-r--r--  2.0 unx      920 b- defN 23-Dec-20 06:58 atorch/ops/op_builder/quantizer.py
--rw-r--r--  2.0 unx     2401 b- defN 23-Dec-20 06:58 atorch/ops/quantizer/__init__.py
--rw-r--r--  2.0 unx       93 b- defN 23-Dec-20 06:58 atorch/optimizers/__init__.py
--rw-r--r--  2.0 unx    13353 b- defN 23-Dec-21 03:00 atorch/optimizers/adam_offload.py
--rw-r--r--  2.0 unx     6808 b- defN 24-Apr-10 08:59 atorch/optimizers/agd.py
--rw-r--r--  2.0 unx    11915 b- defN 23-Dec-20 06:58 atorch/optimizers/bf16_optimizer.py
--rw-r--r--  2.0 unx      625 b- defN 23-Dec-20 06:58 atorch/optimizers/utils.py
--rw-r--r--  2.0 unx     5375 b- defN 23-Dec-21 03:00 atorch/optimizers/wsam.py
--rw-r--r--  2.0 unx       55 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/__init__.py
--rw-r--r--  2.0 unx      626 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/config.py
--rw-r--r--  2.0 unx    19476 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/functional.py
--rw-r--r--  2.0 unx      118 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/__init__.py
--rw-r--r--  2.0 unx    10365 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/q_adafactor.py
--rw-r--r--  2.0 unx     7123 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/q_adamw.py
--rw-r--r--  2.0 unx     9927 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/q_agd.py
--rw-r--r--  2.0 unx    10023 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/q_came.py
--rw-r--r--  2.0 unx     7034 b- defN 23-Dec-21 03:00 atorch/optimizers/low_bit/optim/q_optimizer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/protos/__init__.py
--rw-r--r--  2.0 unx    19348 b- defN 24-Apr-12 06:05 atorch/protos/acceleration_pb2.py
--rw-r--r--  2.0 unx     4574 b- defN 24-Apr-12 06:05 atorch/protos/acceleration_pb2_grpc.py
--rw-r--r--  2.0 unx     5993 b- defN 24-Apr-12 06:05 atorch/protos/coworker_pb2.py
--rw-r--r--  2.0 unx     6714 b- defN 24-Apr-12 06:05 atorch/protos/coworker_pb2_grpc.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/__init__.py
--rw-r--r--  2.0 unx     7661 b- defN 24-Apr-10 08:59 atorch/rl/config.py
--rw-r--r--  2.0 unx      849 b- defN 24-Apr-10 08:59 atorch/rl/main.py
--rw-r--r--  2.0 unx       39 b- defN 24-Apr-10 08:59 atorch/rl/data/__init__.py
--rw-r--r--  2.0 unx     6390 b- defN 24-Apr-10 08:59 atorch/rl/data/data_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/__init__.py
--rw-r--r--  2.0 unx    15390 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/ds_hook.py
--rw-r--r--  2.0 unx    16621 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/hybrid_engine.py
--rw-r--r--  2.0 unx     7738 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/initialize.py
--rw-r--r--  2.0 unx      235 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/replace_policy.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/module_inject/__init__.py
--rw-r--r--  2.0 unx      632 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/module_inject/utils.py
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/module_inject/containers/__init__.py
--rw-r--r--  2.0 unx     6707 b- defN 24-Apr-10 08:59 atorch/rl/ds_hybrid_engine/module_inject/containers/llama.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/inference_backend/__init__.py
--rw-r--r--  2.0 unx     1682 b- defN 24-Apr-10 08:59 atorch/rl/inference_backend/vllm_backend.py
--rw-r--r--  2.0 unx       56 b- defN 24-Apr-10 08:59 atorch/rl/model_engine/__init__.py
--rw-r--r--  2.0 unx    21156 b- defN 24-Apr-10 08:59 atorch/rl/model_engine/model_engine.py
--rw-r--r--  2.0 unx     1138 b- defN 24-Apr-10 08:59 atorch/rl/model_engine/strategy.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/model_utils/__init__.py
--rw-r--r--  2.0 unx     6372 b- defN 24-Apr-10 08:59 atorch/rl/model_utils/llama2_utils.py
--rw-r--r--  2.0 unx     6291 b- defN 24-Apr-10 08:59 atorch/rl/model_utils/load_init_model.py
--rw-r--r--  2.0 unx    12237 b- defN 24-Apr-10 08:59 atorch/rl/model_utils/model_util.py
--rw-r--r--  2.0 unx     2144 b- defN 24-Apr-10 08:59 atorch/rl/model_utils/redis_util.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-10 08:59 atorch/rl/ppo_utils/__init__.py
--rw-r--r--  2.0 unx     6842 b- defN 24-Apr-10 08:59 atorch/rl/ppo_utils/ppo_util.py
--rw-r--r--  2.0 unx       40 b- defN 24-Apr-10 08:59 atorch/rl/replay_buffer/__init__.py
--rw-r--r--  2.0 unx     1795 b- defN 24-Apr-10 08:59 atorch/rl/replay_buffer/replay_buffer.py
--rw-r--r--  2.0 unx       34 b- defN 24-Apr-10 08:59 atorch/rl/trainer/__init__.py
--rw-r--r--  2.0 unx      274 b- defN 24-Apr-10 08:59 atorch/rl/trainer/ppo_trainer.py
--rw-r--r--  2.0 unx     3190 b- defN 24-Apr-10 08:59 atorch/rl/trainer/rl_trainer.py
--rw-r--r--  2.0 unx        0 b- defN 23-Dec-20 06:58 atorch/service/__init__.py
--rw-r--r--  2.0 unx     2208 b- defN 23-Dec-20 06:58 atorch/service/coworker_data_service.py
--rw-r--r--  2.0 unx     1924 b- defN 23-Dec-20 06:58 atorch/service/data_info_service.py
--rw-r--r--  2.0 unx     3238 b- defN 23-Dec-20 09:08 atorch/service/rpc_clients.py
--rw-r--r--  2.0 unx      103 b- defN 24-Jan-17 06:33 atorch/trainer/__init__.py
--rw-r--r--  2.0 unx    10651 b- defN 24-Apr-10 08:59 atorch/trainer/atorch_args.py
--rw-r--r--  2.0 unx    98297 b- defN 24-Apr-10 08:59 atorch/trainer/atorch_trainer.py
--rw-r--r--  2.0 unx       63 b- defN 24-Jan-17 06:27 atorch/utils/__init__.py
--rw-r--r--  2.0 unx     8524 b- defN 24-Jan-17 06:27 atorch/utils/ds_pipe_utils.py
--rw-r--r--  2.0 unx     7784 b- defN 24-Apr-10 08:59 atorch/utils/fsdp_async_ckpt_util.py
--rw-r--r--  2.0 unx    14062 b- defN 24-Apr-10 08:59 atorch/utils/fsdp_init_util.py
--rw-r--r--  2.0 unx    41878 b- defN 24-Apr-10 08:59 atorch/utils/fsdp_save_util.py
--rw-r--r--  2.0 unx     2706 b- defN 24-Apr-10 08:59 atorch/utils/grad_scaler.py
--rw-r--r--  2.0 unx     5644 b- defN 24-Jan-17 06:27 atorch/utils/graph_transform_utils.py
--rw-r--r--  2.0 unx     1021 b- defN 24-Apr-10 08:59 atorch/utils/hooks.py
--rw-r--r--  2.0 unx     6940 b- defN 24-Jan-17 06:27 atorch/utils/ib_monitor.py
--rw-r--r--  2.0 unx     1428 b- defN 24-Apr-10 08:59 atorch/utils/import_util.py
--rw-r--r--  2.0 unx    10381 b- defN 24-Jan-18 02:35 atorch/utils/manual_tp_utils.py
--rw-r--r--  2.0 unx    34986 b- defN 24-Jan-18 02:35 atorch/utils/meta_model_utils.py
--rw-r--r--  2.0 unx    11593 b- defN 24-Jan-17 06:27 atorch/utils/meta_overrides.py
--rw-r--r--  2.0 unx     2267 b- defN 24-Jan-17 06:27 atorch/utils/metric_util.py
--rw-r--r--  2.0 unx     5781 b- defN 24-Apr-10 08:59 atorch/utils/numberic_checker.py
--rw-r--r--  2.0 unx     9514 b- defN 24-Jan-17 06:27 atorch/utils/parse_fsdp_mapping.py
--rw-r--r--  2.0 unx    10451 b- defN 24-Apr-10 08:59 atorch/utils/parse_trace_json.py
--rw-r--r--  2.0 unx     3487 b- defN 24-Jan-17 06:27 atorch/utils/patch_fairscale.py
--rw-r--r--  2.0 unx     4875 b- defN 24-Apr-10 08:59 atorch/utils/patch_te.py
--rw-r--r--  2.0 unx     4188 b- defN 24-Jan-17 06:27 atorch/utils/pipe_file_utils.py
--rw-r--r--  2.0 unx    46954 b- defN 24-Apr-10 08:59 atorch/utils/prof.py
--rw-r--r--  2.0 unx     2839 b- defN 24-Jan-17 06:27 atorch/utils/shape_prop.py
--rw-r--r--  2.0 unx     4281 b- defN 24-Jan-17 06:27 atorch/utils/sharding_spec.py
--rw-r--r--  2.0 unx     2547 b- defN 24-Jan-17 06:27 atorch/utils/sparse.py
--rw-r--r--  2.0 unx     6342 b- defN 24-Jan-17 06:27 atorch/utils/spec_prop.py
--rw-r--r--  2.0 unx     2797 b- defN 24-Jan-17 06:27 atorch/utils/timer.py
--rw-r--r--  2.0 unx    24365 b- defN 24-Jan-17 06:27 atorch/utils/tracer.py
--rw-r--r--  2.0 unx     2244 b- defN 24-Jan-18 02:35 atorch/utils/trainer_utils.py
--rw-r--r--  2.0 unx     1441 b- defN 24-Jan-17 06:27 atorch/utils/version.py
--rw-r--r--  2.0 unx     1046 b- defN 23-Dec-20 06:58 atorch-0.1.8.data/data/acceleration.proto
--rw-r--r--  2.0 unx      224 b- defN 24-Apr-10 08:59 atorch-0.1.8.data/data/build_proto.sh
--rw-r--r--  2.0 unx      455 b- defN 23-Dec-20 06:58 atorch-0.1.8.data/data/coworker.proto
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-10 08:59 atorch-0.1.8.data/data/requirements.txt
--rw-r--r--  2.0 unx     1155 b- defN 24-Apr-12 06:05 atorch-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-12 06:05 atorch-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx        7 b- defN 24-Apr-12 06:05 atorch-0.1.8.dist-info/top_level.txt
--rw-rw-r--  2.0 unx    27323 b- defN 24-Apr-12 06:06 atorch-0.1.8.dist-info/RECORD
-289 files, 2182310 bytes uncompressed, 534458 bytes compressed:  75.5%
+Zip file size: 596064 bytes, number of entries: 295
+-rw-r--r--  2.0 unx      958 b- defN 24-Apr-26 08:47 atorch/__init__.py
+-rw-r--r--  2.0 unx      255 b- defN 24-Apr-26 08:47 atorch/amp/__init__.py
+-rw-r--r--  2.0 unx     3412 b- defN 24-Apr-26 08:47 atorch/amp/amp.py
+-rw-r--r--  2.0 unx      868 b- defN 24-Apr-26 08:47 atorch/amp/hook.py
+-rw-r--r--  2.0 unx    12488 b- defN 24-Apr-26 08:47 atorch/amp/pipe_amp.py
+-rw-r--r--  2.0 unx       83 b- defN 24-Apr-26 08:47 atorch/auto/__init__.py
+-rw-r--r--  2.0 unx    28847 b- defN 24-Apr-26 08:47 atorch/auto/accelerate.py
+-rw-r--r--  2.0 unx     1095 b- defN 24-Apr-26 08:47 atorch/auto/auto_accelerate_context.py
+-rw-r--r--  2.0 unx    13550 b- defN 24-Apr-26 08:47 atorch/auto/clip_grad_norm.py
+-rw-r--r--  2.0 unx     6456 b- defN 24-Apr-26 08:47 atorch/auto/device_context.py
+-rw-r--r--  2.0 unx     2480 b- defN 24-Apr-26 08:47 atorch/auto/engine_client.py
+-rw-r--r--  2.0 unx    38252 b- defN 24-May-06 03:03 atorch/auto/model_context.py
+-rw-r--r--  2.0 unx     4803 b- defN 24-Apr-26 08:47 atorch/auto/strategy.py
+-rw-r--r--  2.0 unx      468 b- defN 24-Apr-26 08:47 atorch/auto/task.py
+-rw-r--r--  2.0 unx       31 b- defN 24-Apr-26 08:47 atorch/auto/analyser/__init__.py
+-rw-r--r--  2.0 unx    12008 b- defN 24-Apr-26 08:47 atorch/auto/analyser/analyser.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/dry_runner/__init__.py
+-rw-r--r--  2.0 unx     6435 b- defN 24-Apr-26 08:47 atorch/auto/dry_runner/dry_runner.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/__init__.py
+-rw-r--r--  2.0 unx     3241 b- defN 24-Apr-26 08:47 atorch/auto/engine/acceleration_engine.py
+-rw-r--r--  2.0 unx      948 b- defN 24-Apr-26 08:47 atorch/auto/engine/analyser_result.py
+-rw-r--r--  2.0 unx     3064 b- defN 24-Apr-26 08:47 atorch/auto/engine/client.py
+-rw-r--r--  2.0 unx    11304 b- defN 24-Apr-26 08:47 atorch/auto/engine/executor.py
+-rw-r--r--  2.0 unx     6810 b- defN 24-Apr-26 08:47 atorch/auto/engine/optimization_method.py
+-rw-r--r--  2.0 unx     4587 b- defN 24-Apr-26 08:47 atorch/auto/engine/planner.py
+-rw-r--r--  2.0 unx     3035 b- defN 24-Apr-26 08:47 atorch/auto/engine/servicer.py
+-rw-r--r--  2.0 unx     6306 b- defN 24-Apr-26 08:47 atorch/auto/engine/strategy.py
+-rw-r--r--  2.0 unx     1693 b- defN 24-Apr-26 08:47 atorch/auto/engine/task.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/__init__.py
+-rw-r--r--  2.0 unx     5713 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/bayes_opt_sg.py
+-rw-r--r--  2.0 unx     2271 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/combination_sg.py
+-rw-r--r--  2.0 unx      896 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/sg_algo_lib.py
+-rw-r--r--  2.0 unx      886 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/sg_algorithm.py
+-rw-r--r--  2.0 unx    14213 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/utils.py
+-rw-r--r--  2.0 unx      150 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/acq_optimizers/__init__.py
+-rw-r--r--  2.0 unx     5851 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/acq_optimizers/evolution_optimizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/acquisitions/__init__.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/acquisitions/acq.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/design_space/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/design_space/categorical_param.py
+-rw-r--r--  2.0 unx     3119 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/design_space/design_space.py
+-rw-r--r--  2.0 unx     1063 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/design_space/param.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/__init__.py
+-rw-r--r--  2.0 unx     2105 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/base_model.py
+-rw-r--r--  2.0 unx      666 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/layers.py
+-rw-r--r--  2.0 unx      598 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/model_factory.py
+-rw-r--r--  2.0 unx      541 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/util.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/gauss_process/__init__.py
+-rw-r--r--  2.0 unx     4516 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/gauss_process/gpy_wgp.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/random_forest/__init__.py
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/models/random_forest/rf.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/optimizers/__init__.py
+-rw-r--r--  2.0 unx     1174 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/optimizers/abstract_optimizer.py
+-rw-r--r--  2.0 unx     8272 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/optimizers/hebo.py
+-rw-r--r--  2.0 unx     1608 b- defN 24-Apr-26 08:47 atorch/auto/engine/sg_algo/hebo/optimizers/util.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/__init__.py
+-rw-r--r--  2.0 unx    16692 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/amp_optimization.py
+-rw-r--r--  2.0 unx    10362 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/checkpoint_optimization.py
+-rw-r--r--  2.0 unx     7195 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/ds_3d_parallel_optimization.py
+-rw-r--r--  2.0 unx      356 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/dynamo_backends.py
+-rw-r--r--  2.0 unx     2639 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/dynamo_optimization.py
+-rw-r--r--  2.0 unx     1856 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/half_optimization.py
+-rw-r--r--  2.0 unx    13786 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/mixed_parallel_optimization.py
+-rw-r--r--  2.0 unx     7426 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/module_replace_optimization.py
+-rw-r--r--  2.0 unx    10892 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/optimization.py
+-rw-r--r--  2.0 unx     2921 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/optimization_library.py
+-rw-r--r--  2.0 unx     2112 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/parallel_mode_optimization.py
+-rw-r--r--  2.0 unx    11721 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/pipeline_parallel_optimization.py
+-rw-r--r--  2.0 unx    10728 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/selective_offloading_checkpoint.py
+-rw-r--r--  2.0 unx     4955 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/sequence_parallel_optimization.py
+-rw-r--r--  2.0 unx     7992 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/tensor_parallel_optimization.py
+-rw-r--r--  2.0 unx     6182 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/utils.py
+-rw-r--r--  2.0 unx    23126 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/zero_optimization.py
+-rw-r--r--  2.0 unx      241 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/__init__.py
+-rw-r--r--  2.0 unx     5145 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/base_stage_planner.py
+-rw-r--r--  2.0 unx     9408 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/base_tp_planner.py
+-rw-r--r--  2.0 unx     8974 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/dim_planner.py
+-rw-r--r--  2.0 unx    22977 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/mip_tp_planner.py
+-rw-r--r--  2.0 unx     3471 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/topology.py
+-rw-r--r--  2.0 unx    26926 b- defN 24-Apr-26 08:47 atorch/auto/opt_lib/shard_planners/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/common/__init__.py
+-rw-r--r--  2.0 unx     3383 b- defN 24-Apr-26 08:47 atorch/common/constants.py
+-rw-r--r--  2.0 unx     3340 b- defN 24-Apr-26 08:47 atorch/common/log_utils.py
+-rw-r--r--  2.0 unx     6072 b- defN 24-Apr-26 08:47 atorch/common/util_func.py
+-rw-r--r--  2.0 unx      633 b- defN 24-Apr-26 08:47 atorch/data/__init__.py
+-rw-r--r--  2.0 unx    17310 b- defN 24-Apr-26 08:47 atorch/data/coworker_dataset.py
+-rw-r--r--  2.0 unx     1347 b- defN 24-Apr-26 08:47 atorch/data/data_utils.py
+-rw-r--r--  2.0 unx    13694 b- defN 24-Apr-26 08:47 atorch/data/elastic_dataloader.py
+-rw-r--r--  2.0 unx     4771 b- defN 24-Apr-26 08:47 atorch/data/elastic_dataset.py
+-rw-r--r--  2.0 unx     6113 b- defN 24-Apr-26 08:47 atorch/data/preloader.py
+-rw-r--r--  2.0 unx    27904 b- defN 24-Apr-26 08:47 atorch/data/shm_context.py
+-rw-r--r--  2.0 unx    10185 b- defN 24-Apr-26 08:47 atorch/data/shm_dataloader.py
+-rw-r--r--  2.0 unx     3396 b- defN 24-Apr-26 08:47 atorch/data/unordered_dataloader.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-26 08:47 atorch/data/unshuffled_batch_dataloader.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/data_parallel/__init__.py
+-rw-r--r--  2.0 unx    25559 b- defN 24-Apr-26 08:47 atorch/data_parallel/adp.py
+-rw-r--r--  2.0 unx    13332 b- defN 24-Apr-26 08:47 atorch/data_parallel/auto_wrap.py
+-rw-r--r--  2.0 unx     3562 b- defN 24-Apr-26 08:47 atorch/data_parallel/wrapper.py
+-rw-r--r--  2.0 unx    25890 b- defN 24-Apr-26 08:47 atorch/data_parallel/zero_ddp_mix_112.py
+-rw-r--r--  2.0 unx      473 b- defN 24-Apr-26 08:47 atorch/distributed/__init__.py
+-rw-r--r--  2.0 unx    30705 b- defN 24-Apr-26 08:47 atorch/distributed/distributed.py
+-rw-r--r--  2.0 unx      465 b- defN 24-Apr-26 08:47 atorch/distributed/elastic_controller.py
+-rw-r--r--  2.0 unx     3563 b- defN 24-Apr-26 08:47 atorch/distributed/elastic_trainer.py
+-rw-r--r--  2.0 unx     1253 b- defN 24-Apr-26 08:47 atorch/distributed/hooks.py
+-rw-r--r--  2.0 unx    19071 b- defN 24-Apr-26 08:47 atorch/distributed/launch.py
+-rw-r--r--  2.0 unx    12424 b- defN 24-Apr-26 08:47 atorch/distributed/run.py
+-rw-r--r--  2.0 unx       68 b- defN 24-Apr-26 08:47 atorch/fault_tolerance/__init__.py
+-rw-r--r--  2.0 unx     4825 b- defN 24-Apr-26 08:47 atorch/fault_tolerance/api.py
+-rw-r--r--  2.0 unx     8293 b- defN 24-Apr-26 08:47 atorch/fault_tolerance/custom_agent.py
+-rw-r--r--  2.0 unx     5659 b- defN 24-Apr-26 08:47 atorch/fault_tolerance/hanging_detector.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/local_sgd/__init__.py
+-rw-r--r--  2.0 unx     1579 b- defN 24-Apr-26 08:47 atorch/local_sgd/HSDP/__init__.py
+-rw-r--r--  2.0 unx    13452 b- defN 24-Apr-26 08:47 atorch/local_sgd/HSDP/_init_utils.py
+-rw-r--r--  2.0 unx    21594 b- defN 24-Apr-26 08:47 atorch/local_sgd/HSDP/_runtime_utils.py
+-rw-r--r--  2.0 unx    22339 b- defN 24-Apr-26 08:47 atorch/local_sgd/HSDP/_state_dict_utils.py
+-rw-r--r--  2.0 unx       86 b- defN 24-Apr-26 08:47 atorch/local_sgd/reduce_methods/__init__.py
+-rw-r--r--  2.0 unx     1054 b- defN 24-Apr-26 08:47 atorch/local_sgd/reduce_methods/base.py
+-rw-r--r--  2.0 unx     3503 b- defN 24-Apr-26 08:47 atorch/local_sgd/reduce_methods/generalized_task_arithmetic.py
+-rw-r--r--  2.0 unx     1034 b- defN 24-Apr-26 08:47 atorch/local_sgd/reduce_methods/linear.py
+-rw-r--r--  2.0 unx     1815 b- defN 24-Apr-26 08:47 atorch/local_sgd/reduce_methods/sparsify.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/modules/__init__.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/__init__.py
+-rw-r--r--  2.0 unx    14763 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/activation_checkpointing.py
+-rw-r--r--  2.0 unx     5688 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/cross_entropy.py
+-rw-r--r--  2.0 unx    29411 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/layers.py
+-rw-r--r--  2.0 unx    16790 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/mappings.py
+-rw-r--r--  2.0 unx     7633 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/mappings_registry.py
+-rw-r--r--  2.0 unx     1269 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/materialize_modules.py
+-rw-r--r--  2.0 unx    54608 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/modules_registry.py
+-rw-r--r--  2.0 unx     5436 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/randomizer.py
+-rw-r--r--  2.0 unx    75800 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/transformer.py
+-rw-r--r--  2.0 unx     7551 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/utils.py
+-rw-r--r--  2.0 unx      147 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/__init__.py
+-rw-r--r--  2.0 unx    36537 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/pipe_compiler/PipelineStage.py
+-rw-r--r--  2.0 unx     3976 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/pipe_compiler/StageInterleaver.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/pipe_compiler/__init__.py
+-rw-r--r--  2.0 unx    20974 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/pipe_compiler/distributed_pippy_compiler.py
+-rw-r--r--  2.0 unx    25818 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/pipe_compiler/utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/tp_compiler/__init__.py
+-rw-r--r--  2.0 unx      222 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/tp_compiler/dtensor_compiler.py
+-rw-r--r--  2.0 unx     7707 b- defN 24-Apr-26 08:47 atorch/modules/distributed_modules/compilers/tp_compiler/tp_compiler.py
+-rw-r--r--  2.0 unx       80 b- defN 24-Apr-26 08:47 atorch/modules/distributed_transformer/__init__.py
+-rw-r--r--  2.0 unx     3173 b- defN 24-Apr-26 08:47 atorch/modules/distributed_transformer/commu_utils.py
+-rw-r--r--  2.0 unx    14623 b- defN 24-Apr-26 08:47 atorch/modules/distributed_transformer/distributed_attention.py
+-rw-r--r--  2.0 unx      295 b- defN 24-Apr-26 08:47 atorch/modules/moe/__init__.py
+-rw-r--r--  2.0 unx    16005 b- defN 24-Apr-26 08:47 atorch/modules/moe/ddp.py
+-rw-r--r--  2.0 unx     4707 b- defN 24-Apr-26 08:47 atorch/modules/moe/grouped_gemm_moe.py
+-rw-r--r--  2.0 unx     4291 b- defN 24-Apr-26 08:47 atorch/modules/moe/inject.py
+-rw-r--r--  2.0 unx    25005 b- defN 24-Apr-26 08:47 atorch/modules/moe/moe_layer.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-26 08:47 atorch/modules/moe/ops.py
+-rw-r--r--  2.0 unx     6683 b- defN 24-Apr-26 08:47 atorch/modules/moe/switch_gating.py
+-rw-r--r--  2.0 unx     5799 b- defN 24-Apr-26 08:47 atorch/modules/moe/topk_gating.py
+-rw-r--r--  2.0 unx       37 b- defN 24-Apr-26 08:47 atorch/modules/transformer/__init__.py
+-rw-r--r--  2.0 unx     5210 b- defN 24-Apr-26 08:47 atorch/modules/transformer/_fa_api_compat_patch
+-rw-r--r--  2.0 unx    13580 b- defN 24-Apr-26 08:47 atorch/modules/transformer/cross_entropy.py
+-rw-r--r--  2.0 unx     8248 b- defN 24-Apr-26 08:47 atorch/modules/transformer/inject.py
+-rw-r--r--  2.0 unx    67409 b- defN 24-Apr-26 08:47 atorch/modules/transformer/layers.py
+-rw-r--r--  2.0 unx     2682 b- defN 24-Apr-26 08:47 atorch/modules/transformer/linear.py
+-rw-r--r--  2.0 unx      374 b- defN 24-Apr-26 08:47 atorch/modules/transformer/losses.py
+-rw-r--r--  2.0 unx      244 b- defN 24-Apr-26 08:47 atorch/mup/__init__.py
+-rw-r--r--  2.0 unx     4232 b- defN 24-Apr-26 08:47 atorch/mup/infshape.py
+-rw-r--r--  2.0 unx     8553 b- defN 24-Apr-26 08:47 atorch/mup/init.py
+-rw-r--r--  2.0 unx    11021 b- defN 24-Apr-26 08:47 atorch/mup/module.py
+-rw-r--r--  2.0 unx     5867 b- defN 24-Apr-26 08:47 atorch/mup/optim.py
+-rw-r--r--  2.0 unx     7971 b- defN 24-Apr-26 08:47 atorch/mup/shape.py
+-rw-r--r--  2.0 unx      455 b- defN 24-Apr-26 08:47 atorch/normalization/__init__.py
+-rw-r--r--  2.0 unx     9000 b- defN 24-Apr-26 08:47 atorch/normalization/layernorm.py
+-rw-r--r--  2.0 unx     2681 b- defN 24-Apr-26 08:47 atorch/npu/__init__.py
+-rw-r--r--  2.0 unx     6090 b- defN 24-Apr-26 08:47 atorch/npu/layers.py
+-rw-r--r--  2.0 unx     7676 b- defN 24-Apr-26 08:47 atorch/npu/optim.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/ops/__init__.py
+-rw-r--r--  2.0 unx      950 b- defN 24-Apr-26 08:47 atorch/ops/git_version_info.py
+-rw-r--r--  2.0 unx      355 b- defN 24-May-07 03:07 atorch/ops/git_version_info_installed.py
+-rw-r--r--  2.0 unx      271 b- defN 24-Apr-26 08:47 atorch/ops/accelerator/__init__.py
+-rw-r--r--  2.0 unx     4732 b- defN 24-Apr-26 08:47 atorch/ops/accelerator/abstract_accelerator.py
+-rw-r--r--  2.0 unx     8910 b- defN 24-Apr-26 08:47 atorch/ops/accelerator/cuda_accelerator.py
+-rw-r--r--  2.0 unx     2478 b- defN 24-Apr-26 08:47 atorch/ops/accelerator/real_accelerator.py
+-rw-r--r--  2.0 unx    12017 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/conversion_utils.h
+-rw-r--r--  2.0 unx     7001 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/dequantization_utils.h
+-rw-r--r--  2.0 unx     1202 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/kernel_utils.h
+-rw-r--r--  2.0 unx    31857 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/memory_access_utils.h
+-rw-r--r--  2.0 unx     1838 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/quantization.h
+-rw-r--r--  2.0 unx     1884 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/quantization_optimizer.h
+-rw-r--r--  2.0 unx    16931 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/quantization_utils.h
+-rw-r--r--  2.0 unx      411 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/quantizer.h
+-rw-r--r--  2.0 unx    17562 b- defN 24-Apr-26 08:47 atorch/ops/csrc/includes/reduction_utils.h
+-rw-r--r--  2.0 unx     3048 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/dequantize.cu
+-rw-r--r--  2.0 unx     8061 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/pt_binding.cpp
+-rw-r--r--  2.0 unx     9192 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/quant_reduce.cu
+-rw-r--r--  2.0 unx     2791 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/quantization_optimizer.cc
+-rw-r--r--  2.0 unx    24575 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/quantization_optimizer.cu
+-rw-r--r--  2.0 unx     6418 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/quantize.cu
+-rw-r--r--  2.0 unx     7576 b- defN 24-Apr-26 08:47 atorch/ops/csrc/quantization/swizzled_quantize.cu
+-rw-r--r--  2.0 unx     2091 b- defN 24-Apr-26 08:47 atorch/ops/op_builder/__init__.py
+-rw-r--r--  2.0 unx     1271 b- defN 24-Apr-26 08:47 atorch/ops/op_builder/all_ops.py
+-rw-r--r--  2.0 unx    25650 b- defN 24-Apr-26 08:47 atorch/ops/op_builder/builder.py
+-rw-r--r--  2.0 unx      846 b- defN 24-Apr-26 08:47 atorch/ops/op_builder/quantization_optimizer.py
+-rw-r--r--  2.0 unx      920 b- defN 24-Apr-26 08:47 atorch/ops/op_builder/quantizer.py
+-rw-r--r--  2.0 unx     2401 b- defN 24-Apr-26 08:47 atorch/ops/quantizer/__init__.py
+-rw-r--r--  2.0 unx       93 b- defN 24-Apr-26 08:47 atorch/optimizers/__init__.py
+-rw-r--r--  2.0 unx    13353 b- defN 24-Apr-26 08:47 atorch/optimizers/adam_offload.py
+-rw-r--r--  2.0 unx     6808 b- defN 24-Apr-26 08:47 atorch/optimizers/agd.py
+-rw-r--r--  2.0 unx    11915 b- defN 24-Apr-26 08:47 atorch/optimizers/bf16_optimizer.py
+-rw-r--r--  2.0 unx      625 b- defN 24-Apr-26 08:47 atorch/optimizers/utils.py
+-rw-r--r--  2.0 unx     5375 b- defN 24-Apr-26 08:47 atorch/optimizers/wsam.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/__init__.py
+-rw-r--r--  2.0 unx      626 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/config.py
+-rw-r--r--  2.0 unx    19476 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/functional.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/__init__.py
+-rw-r--r--  2.0 unx    10365 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/q_adafactor.py
+-rw-r--r--  2.0 unx     7123 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/q_adamw.py
+-rw-r--r--  2.0 unx     9927 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/q_agd.py
+-rw-r--r--  2.0 unx    10023 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/q_came.py
+-rw-r--r--  2.0 unx     7034 b- defN 24-Apr-26 08:47 atorch/optimizers/low_bit/optim/q_optimizer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/protos/__init__.py
+-rw-r--r--  2.0 unx     3199 b- defN 24-May-07 03:07 atorch/protos/acceleration_pb2.py
+-rw-r--r--  2.0 unx     4574 b- defN 24-May-07 03:07 atorch/protos/acceleration_pb2_grpc.py
+-rw-r--r--  2.0 unx     1869 b- defN 24-May-07 03:07 atorch/protos/coworker_pb2.py
+-rw-r--r--  2.0 unx     6714 b- defN 24-May-07 03:07 atorch/protos/coworker_pb2_grpc.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/__init__.py
+-rw-r--r--  2.0 unx     7661 b- defN 24-Apr-26 08:47 atorch/rl/config.py
+-rw-r--r--  2.0 unx      849 b- defN 24-Apr-26 08:47 atorch/rl/main.py
+-rw-r--r--  2.0 unx       39 b- defN 24-Apr-26 08:47 atorch/rl/data/__init__.py
+-rw-r--r--  2.0 unx     6390 b- defN 24-Apr-26 08:47 atorch/rl/data/data_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/__init__.py
+-rw-r--r--  2.0 unx    15390 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/ds_hook.py
+-rw-r--r--  2.0 unx    16621 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/hybrid_engine.py
+-rw-r--r--  2.0 unx     7738 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/initialize.py
+-rw-r--r--  2.0 unx      235 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/replace_policy.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/module_inject/__init__.py
+-rw-r--r--  2.0 unx      632 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/module_inject/utils.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/module_inject/containers/__init__.py
+-rw-r--r--  2.0 unx     6707 b- defN 24-Apr-26 08:47 atorch/rl/ds_hybrid_engine/module_inject/containers/llama.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/inference_backend/__init__.py
+-rw-r--r--  2.0 unx     1682 b- defN 24-Apr-26 08:47 atorch/rl/inference_backend/vllm_backend.py
+-rw-r--r--  2.0 unx       56 b- defN 24-Apr-26 08:47 atorch/rl/model_engine/__init__.py
+-rw-r--r--  2.0 unx    21156 b- defN 24-Apr-26 08:47 atorch/rl/model_engine/model_engine.py
+-rw-r--r--  2.0 unx     1138 b- defN 24-Apr-26 08:47 atorch/rl/model_engine/strategy.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/model_utils/__init__.py
+-rw-r--r--  2.0 unx     6372 b- defN 24-Apr-26 08:47 atorch/rl/model_utils/llama2_utils.py
+-rw-r--r--  2.0 unx     6291 b- defN 24-Apr-26 08:47 atorch/rl/model_utils/load_init_model.py
+-rw-r--r--  2.0 unx    12237 b- defN 24-Apr-26 08:47 atorch/rl/model_utils/model_util.py
+-rw-r--r--  2.0 unx     2144 b- defN 24-Apr-26 08:47 atorch/rl/model_utils/redis_util.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/rl/ppo_utils/__init__.py
+-rw-r--r--  2.0 unx     6842 b- defN 24-Apr-26 08:47 atorch/rl/ppo_utils/ppo_util.py
+-rw-r--r--  2.0 unx       40 b- defN 24-Apr-26 08:47 atorch/rl/replay_buffer/__init__.py
+-rw-r--r--  2.0 unx     1795 b- defN 24-Apr-26 08:47 atorch/rl/replay_buffer/replay_buffer.py
+-rw-r--r--  2.0 unx       34 b- defN 24-Apr-26 08:47 atorch/rl/trainer/__init__.py
+-rw-r--r--  2.0 unx      274 b- defN 24-Apr-26 08:47 atorch/rl/trainer/ppo_trainer.py
+-rw-r--r--  2.0 unx     3190 b- defN 24-Apr-26 08:47 atorch/rl/trainer/rl_trainer.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-26 08:47 atorch/service/__init__.py
+-rw-r--r--  2.0 unx     2208 b- defN 24-Apr-26 08:47 atorch/service/coworker_data_service.py
+-rw-r--r--  2.0 unx     1924 b- defN 24-Apr-26 08:47 atorch/service/data_info_service.py
+-rw-r--r--  2.0 unx     3238 b- defN 24-Apr-26 08:47 atorch/service/rpc_clients.py
+-rw-r--r--  2.0 unx      103 b- defN 24-Apr-26 08:47 atorch/trainer/__init__.py
+-rw-r--r--  2.0 unx    11648 b- defN 24-Apr-26 08:47 atorch/trainer/atorch_args.py
+-rw-r--r--  2.0 unx   113391 b- defN 24-Apr-26 08:47 atorch/trainer/atorch_trainer.py
+-rw-r--r--  2.0 unx       63 b- defN 24-Apr-26 08:47 atorch/utils/__init__.py
+-rw-r--r--  2.0 unx     8524 b- defN 24-Apr-26 08:47 atorch/utils/ds_pipe_utils.py
+-rw-r--r--  2.0 unx     7784 b- defN 24-Apr-26 08:47 atorch/utils/fsdp_async_ckpt_util.py
+-rw-r--r--  2.0 unx    23843 b- defN 24-Apr-26 08:47 atorch/utils/fsdp_init_util.py
+-rw-r--r--  2.0 unx    47379 b- defN 24-Apr-26 08:47 atorch/utils/fsdp_save_util.py
+-rw-r--r--  2.0 unx     2706 b- defN 24-Apr-26 08:47 atorch/utils/grad_scaler.py
+-rw-r--r--  2.0 unx     5644 b- defN 24-Apr-26 08:47 atorch/utils/graph_transform_utils.py
+-rw-r--r--  2.0 unx     1021 b- defN 24-Apr-26 08:47 atorch/utils/hooks.py
+-rw-r--r--  2.0 unx     6940 b- defN 24-Apr-26 08:47 atorch/utils/ib_monitor.py
+-rw-r--r--  2.0 unx     1428 b- defN 24-Apr-26 08:47 atorch/utils/import_util.py
+-rw-r--r--  2.0 unx     6956 b- defN 24-Apr-26 08:47 atorch/utils/loss_spike_utils.py
+-rw-r--r--  2.0 unx    10381 b- defN 24-Apr-26 08:47 atorch/utils/manual_tp_utils.py
+-rw-r--r--  2.0 unx    34986 b- defN 24-Apr-26 08:47 atorch/utils/meta_model_utils.py
+-rw-r--r--  2.0 unx    11593 b- defN 24-Apr-26 08:47 atorch/utils/meta_overrides.py
+-rw-r--r--  2.0 unx     2267 b- defN 24-Apr-26 08:47 atorch/utils/metric_util.py
+-rw-r--r--  2.0 unx     5781 b- defN 24-Apr-26 08:47 atorch/utils/numberic_checker.py
+-rw-r--r--  2.0 unx    10451 b- defN 24-Apr-26 08:47 atorch/utils/parse_trace_json.py
+-rw-r--r--  2.0 unx     3487 b- defN 24-Apr-26 08:47 atorch/utils/patch_fairscale.py
+-rw-r--r--  2.0 unx     4918 b- defN 24-Apr-26 08:47 atorch/utils/patch_te.py
+-rw-r--r--  2.0 unx     4188 b- defN 24-Apr-26 08:47 atorch/utils/pipe_file_utils.py
+-rw-r--r--  2.0 unx    46954 b- defN 24-Apr-26 08:47 atorch/utils/prof.py
+-rw-r--r--  2.0 unx     2839 b- defN 24-Apr-26 08:47 atorch/utils/shape_prop.py
+-rw-r--r--  2.0 unx     4281 b- defN 24-Apr-26 08:47 atorch/utils/sharding_spec.py
+-rw-r--r--  2.0 unx     2547 b- defN 24-Apr-26 08:47 atorch/utils/sparse.py
+-rw-r--r--  2.0 unx     6342 b- defN 24-Apr-26 08:47 atorch/utils/spec_prop.py
+-rw-r--r--  2.0 unx     2797 b- defN 24-Apr-26 08:47 atorch/utils/timer.py
+-rw-r--r--  2.0 unx    24365 b- defN 24-Apr-26 08:47 atorch/utils/tracer.py
+-rw-r--r--  2.0 unx     2244 b- defN 24-Apr-26 08:47 atorch/utils/trainer_utils.py
+-rw-r--r--  2.0 unx     1649 b- defN 24-Apr-26 08:47 atorch/utils/version.py
+-rw-r--r--  2.0 unx     1046 b- defN 24-Apr-26 08:47 atorch-0.1.9.data/data/acceleration.proto
+-rw-r--r--  2.0 unx      224 b- defN 24-Apr-11 08:03 atorch-0.1.9.data/data/build_proto.sh
+-rw-r--r--  2.0 unx      455 b- defN 24-Apr-26 08:47 atorch-0.1.9.data/data/coworker.proto
+-rw-r--r--  2.0 unx      287 b- defN 24-May-07 03:05 atorch-0.1.9.data/data/requirements.txt
+-rw-r--r--  2.0 unx     1197 b- defN 24-May-07 03:07 atorch-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-07 03:07 atorch-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx        7 b- defN 24-May-07 03:07 atorch-0.1.9.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx    27885 b- defN 24-May-07 03:07 atorch-0.1.9.dist-info/RECORD
+295 files, 2240046 bytes uncompressed, 551208 bytes compressed:  75.4%
```

## zipnote {}

```diff
@@ -204,14 +204,17 @@
 
 Filename: atorch/auto/opt_lib/pipeline_parallel_optimization.py
 Comment: 
 
 Filename: atorch/auto/opt_lib/selective_offloading_checkpoint.py
 Comment: 
 
+Filename: atorch/auto/opt_lib/sequence_parallel_optimization.py
+Comment: 
+
 Filename: atorch/auto/opt_lib/tensor_parallel_optimization.py
 Comment: 
 
 Filename: atorch/auto/opt_lib/utils.py
 Comment: 
 
 Filename: atorch/auto/opt_lib/zero_optimization.py
@@ -246,35 +249,14 @@
 
 Filename: atorch/common/log_utils.py
 Comment: 
 
 Filename: atorch/common/util_func.py
 Comment: 
 
-Filename: atorch/common/file/__init__.py
-Comment: 
-
-Filename: atorch/common/file/file_io.py
-Comment: 
-
-Filename: atorch/common/file/file_system/__init__.py
-Comment: 
-
-Filename: atorch/common/file/file_system/file_system.py
-Comment: 
-
-Filename: atorch/common/file/file_system/pangu/__init__.py
-Comment: 
-
-Filename: atorch/common/file/file_system/pangu/fsspec_instance.py
-Comment: 
-
-Filename: atorch/common/file/file_system/pangu/pangu_file_system.py
-Comment: 
-
 Filename: atorch/data/__init__.py
 Comment: 
 
 Filename: atorch/data/coworker_dataset.py
 Comment: 
 
 Filename: atorch/data/data_utils.py
@@ -345,14 +327,44 @@
 
 Filename: atorch/fault_tolerance/custom_agent.py
 Comment: 
 
 Filename: atorch/fault_tolerance/hanging_detector.py
 Comment: 
 
+Filename: atorch/local_sgd/__init__.py
+Comment: 
+
+Filename: atorch/local_sgd/HSDP/__init__.py
+Comment: 
+
+Filename: atorch/local_sgd/HSDP/_init_utils.py
+Comment: 
+
+Filename: atorch/local_sgd/HSDP/_runtime_utils.py
+Comment: 
+
+Filename: atorch/local_sgd/HSDP/_state_dict_utils.py
+Comment: 
+
+Filename: atorch/local_sgd/reduce_methods/__init__.py
+Comment: 
+
+Filename: atorch/local_sgd/reduce_methods/base.py
+Comment: 
+
+Filename: atorch/local_sgd/reduce_methods/generalized_task_arithmetic.py
+Comment: 
+
+Filename: atorch/local_sgd/reduce_methods/linear.py
+Comment: 
+
+Filename: atorch/local_sgd/reduce_methods/sparsify.py
+Comment: 
+
 Filename: atorch/modules/__init__.py
 Comment: 
 
 Filename: atorch/modules/distributed_modules/__init__.py
 Comment: 
 
 Filename: atorch/modules/distributed_modules/activation_checkpointing.py
@@ -423,20 +435,26 @@
 
 Filename: atorch/modules/moe/__init__.py
 Comment: 
 
 Filename: atorch/modules/moe/ddp.py
 Comment: 
 
+Filename: atorch/modules/moe/grouped_gemm_moe.py
+Comment: 
+
 Filename: atorch/modules/moe/inject.py
 Comment: 
 
 Filename: atorch/modules/moe/moe_layer.py
 Comment: 
 
+Filename: atorch/modules/moe/ops.py
+Comment: 
+
 Filename: atorch/modules/moe/switch_gating.py
 Comment: 
 
 Filename: atorch/modules/moe/topk_gating.py
 Comment: 
 
 Filename: atorch/modules/transformer/__init__.py
@@ -780,14 +798,17 @@
 
 Filename: atorch/utils/ib_monitor.py
 Comment: 
 
 Filename: atorch/utils/import_util.py
 Comment: 
 
+Filename: atorch/utils/loss_spike_utils.py
+Comment: 
+
 Filename: atorch/utils/manual_tp_utils.py
 Comment: 
 
 Filename: atorch/utils/meta_model_utils.py
 Comment: 
 
 Filename: atorch/utils/meta_overrides.py
@@ -795,17 +816,14 @@
 
 Filename: atorch/utils/metric_util.py
 Comment: 
 
 Filename: atorch/utils/numberic_checker.py
 Comment: 
 
-Filename: atorch/utils/parse_fsdp_mapping.py
-Comment: 
-
 Filename: atorch/utils/parse_trace_json.py
 Comment: 
 
 Filename: atorch/utils/patch_fairscale.py
 Comment: 
 
 Filename: atorch/utils/patch_te.py
@@ -837,32 +855,32 @@
 
 Filename: atorch/utils/trainer_utils.py
 Comment: 
 
 Filename: atorch/utils/version.py
 Comment: 
 
-Filename: atorch-0.1.8.data/data/acceleration.proto
+Filename: atorch-0.1.9.data/data/acceleration.proto
 Comment: 
 
-Filename: atorch-0.1.8.data/data/build_proto.sh
+Filename: atorch-0.1.9.data/data/build_proto.sh
 Comment: 
 
-Filename: atorch-0.1.8.data/data/coworker.proto
+Filename: atorch-0.1.9.data/data/coworker.proto
 Comment: 
 
-Filename: atorch-0.1.8.data/data/requirements.txt
+Filename: atorch-0.1.9.data/data/requirements.txt
 Comment: 
 
-Filename: atorch-0.1.8.dist-info/METADATA
+Filename: atorch-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: atorch-0.1.8.dist-info/WHEEL
+Filename: atorch-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: atorch-0.1.8.dist-info/top_level.txt
+Filename: atorch-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: atorch-0.1.8.dist-info/RECORD
+Filename: atorch-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## atorch/auto/model_context.py

```diff
@@ -17,29 +17,30 @@
 
 import atorch
 from atorch.auto.device_context import get_device_context
 from atorch.auto.opt_lib.utils import _propose_leaf_modules, _propose_wrap_cls, to_module_class_by_name
 from atorch.common.log_utils import default_logger as logger
 from atorch.data import ShmDataloader, expand_batch_dim, get_sample_batch
 from atorch.distributed.distributed import (
+    get_sequence_parallel_size,
     local_rank,
     parallel_group_and_ranks,
     parallel_group_size,
     parallel_rank,
     rank,
 )
 from atorch.modules.distributed_modules.materialize_modules import materialize_modules_to_device
 from atorch.optimizers import BF16Optimizer
 from atorch.utils.graph_transform_utils import map_aggregate
 from atorch.utils.version import torch_version
 
 try:
     from pippy.IR import LossWrapper
 except ImportError:
-    LossWrapper = None
+    LossWrapper = type(object())
 
 from atorch.amp.pipe_amp import _hack_pipe_amp_optimizer, scale_backward_wrapper
 
 try:
     torch.fx.wrap("scale_backward_wrapper")
 except ImportError:
     logger.info("FX not supported, some features may be available")
@@ -84,24 +85,35 @@
     if group_size > 1:
         return rank0_global_rank, rank, group_size
 
     return None, None, None
 
 
 def get_data_partition_rank_and_size():
+    # data, zero are all data parallel and can be mixed used.
     data_size = parallel_group_size("data")
     drank = parallel_rank("data")
     if data_size is None:
         data_size = 1
         drank = 0
     zero_size = parallel_group_size("zero")
     if zero_size is not None:
         zrank = parallel_rank("zero")
         drank = drank * zero_size + zrank
         data_size *= zero_size
+    sp_size = get_sequence_parallel_size()
+    # If sequence parallel used, it is a sequence sharding in data.
+    # Thus, every sp_size ranks share a same training data batch.
+    if sp_size > 1:
+        if data_size % sp_size != 0:
+            logger.error(
+                "data parallel size {} should be divisible by sequence parallel size {}!".format(data_size, sp_size)
+            )
+        data_size = data_size // sp_size
+        drank = drank // sp_size
 
     return drank, data_size
 
 
 def get_mc_default_args():
     args = {"use_optim_backward": False, "requires_set_gradient_accumulation_boundary": False}
     return args
@@ -202,17 +214,14 @@
             )
 
             self.model = loss_wrapper
 
         return isinstance(self.model, LossWrapper)
 
     def _check_loss_wrapper(self):
-        # import pippy internally
-        from pippy.IR import LossWrapper
-
         return isinstance(self.model, LossWrapper)
 
     def _dynamo_capture_graph(self, input_batch):
         import torch._dynamo as dynamo
 
         lowered_device = next(self.model.parameters()).device
 
@@ -328,14 +337,15 @@
                 if total_batchsize != ori_batchsize:
                     logger.warning(
                         "Batchsize={} is not a multiple of data parallel size {}, adjusted to {}.".format(
                             ori_batchsize, ddp_size, total_batchsize
                         )
                     )
 
+        # TODO: if sequence parallel is used, supports only one rank reads/processes data.
         rank0_global_rank, rank, group_size = if_use_shm_dataloader()
         if rank0_global_rank is not None:
             dataloader_args = args
             dataloader_args["sampler"] = sampler
             dataloader_args["num_workers"] = min(dataloader_args["num_workers"] * group_size, 36)
             dataloader_args["drop_last"] = True  # not support different batch size for now.
             io_timeout = int(os.getenv("SHM_DATALOADER_IO_TIMEOUT", 30))
@@ -695,15 +705,15 @@
                 amp_wrapper = self.post_wrappers.pop("amp_native")
                 amp_config = amp_wrapper[1] or None
                 from atorch.modules.distributed_modules.activation_checkpointing import _insert_amp_config_for_tp_ckpt
 
                 _insert_amp_config_for_tp_ckpt(amp_config)
 
         # adjust pre_wrapper order
-        order_wrapper_name = ["half", "module_replace", "fp8", "fsdp", "native_dynamo"]
+        order_wrapper_name = ["half", "module_replace", "sequence_parallel", "fp8", "fsdp", "native_dynamo"]
         match_names = []
         for name in self.pre_wrappers:
             if name in order_wrapper_name:
                 match_names.append(name)
         if len(order_wrapper_name) > 1:
             ordered_wrappers = {}
             for name in self.pre_wrappers:
```

## atorch/auto/opt_lib/module_replace_optimization.py

```diff
@@ -11,14 +11,15 @@
     CLIPAttentionFA,
     GPT2AttentionFA,
     LlamaAttentionFA,
     MultiheadAttentionFA,
 )
 from atorch.normalization import LayerNorm as ApexLayerNorm
 from atorch.utils.meta_model_utils import empty_param, recursive_empty_param
+from atorch.utils.version import package_version_smaller_than
 
 # supported replacement pairs, default replace_configs and supported dtypes for module replace optimization
 # in format of {pair_name: (src_module_cls, target_cls, kwargs, supported_dtypes)}
 REPLACEMENT_PAIRS = dict()
 
 
 def register_replace_pair(
@@ -65,15 +66,17 @@
 register_replace_pair("LayerNorm_Apex", kwargs={"init_from_attr": True}, pair_cls=(LayerNorm, ApexLayerNorm))
 
 # decorator mode register. Not doing this in cls definition
 # because importing `register_replace_pair` there incurs circular import
 register_replace_pair("HF_BertAttention_FA", supported_dtypes={torch.float16, torch.bfloat16})(BertAttentionFA)
 register_replace_pair("HF_CLIPAttention_FA", supported_dtypes={torch.float16, torch.bfloat16})(CLIPAttentionFA)
 register_replace_pair("MultiheadAttention_FA", supported_dtypes={torch.float16, torch.bfloat16})(MultiheadAttentionFA)
-register_replace_pair("HF_LlamaAttention_FA", supported_dtypes={torch.float16, torch.bfloat16})(LlamaAttentionFA)
+if package_version_smaller_than("transformers", "4.38.0"):
+    # transformers 4.38.0 changed LlamaAttention interface, so check version first.
+    register_replace_pair("HF_LlamaAttention_FA", supported_dtypes={torch.float16, torch.bfloat16})(LlamaAttentionFA)
 register_replace_pair("HF_GPT2Attention_FA", supported_dtypes={torch.float16, torch.bfloat16})(GPT2AttentionFA)
 
 
 def _check_model_params_device(model):
     devices = set()
 
     for param in model.parameters():
```

## atorch/auto/opt_lib/optimization_library.py

```diff
@@ -3,14 +3,15 @@
 from atorch.auto.opt_lib.ds_3d_parallel_optimization import DeepSpeed3DParallelOptimization
 from atorch.auto.opt_lib.dynamo_optimization import NativeDynamoOptimization
 from atorch.auto.opt_lib.half_optimization import HalfOptimization
 from atorch.auto.opt_lib.mixed_parallel_optimization import MixedParallelOptimization
 from atorch.auto.opt_lib.module_replace_optimization import ModuleReplaceOptimization
 from atorch.auto.opt_lib.parallel_mode_optimization import ParallelModeOptimization
 from atorch.auto.opt_lib.pipeline_parallel_optimization import PipelineParallelOptimization
+from atorch.auto.opt_lib.sequence_parallel_optimization import SequenceParallelOptimization
 from atorch.auto.opt_lib.tensor_parallel_optimization import TensorParallelOptimization
 from atorch.auto.opt_lib.zero_optimization import FSDPOptimization, Zero1Optimization, Zero2Optimization
 from atorch.common.log_utils import default_logger as logger
 
 SEMIAUTO_STRATEGIES = ("tensor_parallel", "mixed_parallel", "pipeline_parallel")
 
 
@@ -46,14 +47,15 @@
             Fp8Optimization,
             TensorParallelOptimization,
             ModuleReplaceOptimization,
             CheckpointOptimization,
             NativeDynamoOptimization,
             PipelineParallelOptimization,
             MixedParallelOptimization,
+            SequenceParallelOptimization,
             HalfOptimization,
             DeepSpeed3DParallelOptimization,
         ]
         for opt in opt_list:
             opt_instance = opt()
             self.register_opt(opt_instance)
```

## atorch/auto/opt_lib/zero_optimization.py

```diff
@@ -390,27 +390,35 @@
             else:
                 # pytorch version >= (2, 0), use fsdp HYBRID_SHARD
                 from torch.distributed.fsdp.api import ShardingStrategy
 
                 extra_config["sharding_strategy"] = ShardingStrategy.HYBRID_SHARD
                 pg = (parallel_group("zero"), parallel_group("data"))
 
-        if wrapper_config.pop("parse_fsdp", None) is not None:
-            cb = wrapper_config.pop("parse_cb", None)
-            from atorch.utils.parse_fsdp_mapping import ParseFSDP
-
-            fsdp_clz = ParseFSDP(fsdp_clz, fsdp_clz is FSDP, cb)
-
         extra_config["process_group"] = pg
         wrapper_config.update(extra_config)
         if wrap_trainable_outmost:
             fsdp_clz = functools.partial(
                 fsdp_wrap_trainable_outmost, outmost_sharding_strategy=outmost_sharding_strategy
             )
 
+        # support local sgd
+        use_local_sgd = wrapper_config.get("use_local_sgd", None)
+        if use_local_sgd is not None:
+            if not hybrid_with_ddp:
+                raise RuntimeError("use_local_sgd requires hybrid sharding strategy.")
+            elif torch_version() < (2, 1, 0):
+                raise RuntimeError("use_local_sgd requires torch version >= 2.1.0.")
+            elif fsdp_clz is not FSDP:
+                raise RuntimeError("use_local_sgd only supports basic FSDP class.")
+            else:
+                from atorch.local_sgd.HSDP import patch_local_sgd_to_fsdp
+
+                patch_local_sgd_to_fsdp()
+
         model_context.model = fsdp_clz(
             model_context.model,
             **wrapper_config,
         )
         if torch_version() < (1, 12, 0):
             model_context.model.to(local_rank())
```

## atorch/common/util_func.py

```diff
@@ -1,10 +1,10 @@
 import socket
 import time
-from collections.abc import Mapping, Sequence
+from collections.abc import Mapping
 from contextlib import AbstractContextManager
 from operator import attrgetter
 
 import grpc
 import torch
 
 
@@ -83,15 +83,15 @@
             {
                 k: recursively_apply(
                     func, v, *args, test_type=test_type, error_on_other_type=error_on_other_type, **kwargs
                 )
                 for k, v in data.items()
             }
         )
-    elif isinstance(data, Sequence):
+    elif isinstance(data, (tuple, list)):
         return type(data)(
             [
                 recursively_apply(
                     func, v, *args, test_type=test_type, error_on_other_type=error_on_other_type, **kwargs
                 )
                 for v in data
             ]
```

## atorch/distributed/__init__.py

```diff
@@ -1,14 +1,21 @@
 from .distributed import (
     coworker_local_rank,
     coworker_num_per_node,
+    create_sequence_parallel_group,
+    destroy_sequence_parallel_group,
+    get_sequence_parallel_group,
+    get_sequence_parallel_rank,
+    get_sequence_parallel_size,
+    init_distributed,
     is_coworker,
     is_distributed,
     local_rank,
     node_size,
     nproc_per_node,
     rank,
+    seq_all_to_all,
     use_coworker,
     worker_local_rank,
     worker_num_per_node,
     world_size,
 )
```

## atorch/distributed/distributed.py

```diff
@@ -9,14 +9,16 @@
 from torch.distributed.constants import default_pg_timeout
 from torch.distributed.distributed_c10d import _get_default_group
 
 from atorch.common.log_utils import default_logger as logger
 from atorch.common.util_func import find_free_port, get_ip_address, wait_for_server_started
 from atorch.utils.import_util import is_torch_npu_available
 
+_SP_NAME = "_ATORCH_SEQUENCE_PARALLEL"
+
 
 class _DistributedContext:
     LOCAL_RANK = None
     RANK = None
     WORLD_SIZE = None
     BACKEND = None
     INITIALIZED = False
@@ -377,37 +379,42 @@
         _DistributedContext.PARALLEL_GROUP_SIZE[_prefix_pg_name(name)] = size
         _DistributedContext.PARALLEL_RANK[_prefix_pg_name(name)] = rank()
         _DistributedContext.PARALLEL_GROUP[_prefix_pg_name(name)] = _get_default_group()
         if name == "pipe":
             has_pipe = True
     else:
         all_pg_ranks = get_pg_ranks(slicing_dim, rank_order)
-        if _DistributedContext.PARALLEL_GROUPS_AND_RANKS is None:
-            _DistributedContext.PARALLEL_GROUPS_AND_RANKS = {}
         for (name, size) in slicing_dim:
             if name == "pipe":
                 has_pipe = True
-            _DistributedContext.PARALLEL_GROUP_SIZE[_prefix_pg_name(name)] = size
 
-            group_and_ranks = []
-            for idx in range(instance_num):
-                named_ranks = all_pg_ranks[idx][name]
-                for ranks in named_ranks:
-                    group = dist.new_group(ranks)
-                    group_and_ranks.append((group, ranks))
-                    if rank() in ranks:
-                        _DistributedContext.PARALLEL_GROUP[_prefix_pg_name(name)] = group
-                        _DistributedContext.PARALLEL_RANK[_prefix_pg_name(name)] = ranks.index(rank())
-            _DistributedContext.PARALLEL_GROUPS_AND_RANKS[_prefix_pg_name(name)] = group_and_ranks
+            named_ranks = [ranks for idx in range(instance_num) for ranks in all_pg_ranks[idx][name]]
+            _create_named_groups(name, size, named_ranks)
 
     if has_pipe:
         # initialize rpc for pipeline execution
         _build_pippy_rpc_networks()
 
 
+def _create_named_groups(name, size, ranks_list):
+    if _DistributedContext.PARALLEL_GROUPS_AND_RANKS is None:
+        _DistributedContext.PARALLEL_GROUPS_AND_RANKS = {}
+
+    pname = _prefix_pg_name(name)
+    group_and_ranks = []
+    for ranks in ranks_list:
+        group = dist.new_group(ranks)
+        group_and_ranks.append((group, ranks))
+        if rank() in ranks:
+            _DistributedContext.PARALLEL_GROUP[pname] = group
+            _DistributedContext.PARALLEL_RANK[pname] = ranks.index(rank())
+    _DistributedContext.PARALLEL_GROUPS_AND_RANKS[pname] = group_and_ranks
+    _DistributedContext.PARALLEL_GROUP_SIZE[pname] = size
+
+
 def destroy_parallel_group(destroy_rpc=True):
     """
     Delete groups created for mixed parallel and reset parallel mode info
     """
     # must destroy rpc first, since pipe training might depend on this to block and synchronize
     if _DistributedContext.PIPE_RPC_INIT == 1 and destroy_rpc:
         _destroy_pippy_rpc_network()
@@ -421,14 +428,83 @@
     _DistributedContext.PARALLEL_GROUP = None
     _DistributedContext.PARALLEL_GROUPS_AND_RANKS = None
     _DistributedContext.PARALLEL_CONFIG = None
     _DistributedContext.PARALLEL_INSTANCE_NUM = None
     _DistributedContext.PARALLEL_INSTANCE_INDEX = None
 
 
+def create_sequence_parallel_group(sp_size):
+    if sp_size <= 1:
+        return None
+    if world_size() % sp_size != 0:
+        logger.error(f"World size {world_size()} is not divisible by sequence parallel size {sp_size}!")
+    all_ranks = list(range(world_size()))
+    ranks_list = [all_ranks[i : i + sp_size] for i in range(0, world_size(), sp_size)]
+    _create_named_groups(_SP_NAME, sp_size, ranks_list)
+
+
+def destroy_sequence_parallel_group():
+    pname = _prefix_pg_name(_SP_NAME)
+    if (
+        _DistributedContext.PARALLEL_GROUPS_AND_RANKS is not None
+        and pname in _DistributedContext.PARALLEL_GROUPS_AND_RANKS
+    ):
+        for (group, _) in _DistributedContext.PARALLEL_GROUPS_AND_RANKS[pname]:
+            dist.destroy_process_group(group)
+        del _DistributedContext.PARALLEL_GROUPS_AND_RANK[pname]
+        del _DistributedContext.PARALLEL_GROUP[pname]
+        del _DistributedContext.PARALLEL_RANK[pname]
+        del _DistributedContext.PARALLEL_SIZE[pname]
+
+
+def get_sequence_parallel_group():
+    return parallel_group(_SP_NAME)
+
+
+def get_sequence_parallel_size():
+    return parallel_group_size(_SP_NAME) if parallel_group_size(_SP_NAME) is not None else 1
+
+
+def get_sequence_parallel_rank():
+    return parallel_rank(_SP_NAME) if parallel_rank(_SP_NAME) is not None else 0
+
+
+# Sequence  all_to_all implementation is from
+# https://github.com/microsoft/DeepSpeed/blob/master/deepspeed/sequence/layer.py.
+# TODO: use all_to_all_single and custom op to support arbitary scatter_idx/gather_idx.
+class _SeqAllToAll(torch.autograd.Function):
+    @staticmethod
+    def forward(ctx, input, scatter_idx, gather_idx, group=None, sp_size=None):
+        if sp_size is None:
+            sp_size = dist.get_world_size(group)
+        ctx.group = group
+        ctx.sp_size = sp_size
+        ctx.scatter_idx = scatter_idx
+        ctx.gather_idx = gather_idx
+
+        input_list = [t.contiguous() for t in torch.tensor_split(input, sp_size, scatter_idx)]
+        output_list = [torch.empty_like(input_list[0]) for _ in range(sp_size)]
+        dist.all_to_all(output_list, input_list, group=group)
+        return torch.cat(output_list, dim=gather_idx).contiguous()
+
+    @staticmethod
+    def backward(ctx, *grad_output):
+        return (
+            _SeqAllToAll.apply(*grad_output, ctx.gather_idx, ctx.scatter_idx, ctx.group, ctx.sp_size),
+            None,
+            None,
+            None,
+            None,
+        )
+
+
+def seq_all_to_all(input, scatter_idx, gather_idx, group=None, group_size=None):
+    return _SeqAllToAll.apply(input, scatter_idx, gather_idx, group, group_size)
+
+
 def _build_pippy_rpc_networks(num_worker_threads=64, rpc_timeout=1800, init_method="env://"):
     def _has_efa():
         try:
             import subprocess
 
             return (
                 subprocess.run(
```

## atorch/distributed/elastic_controller.py

```diff
@@ -1,13 +1,13 @@
 from atorch.common.log_utils import default_logger as logger
 
 try:
     from elasticai_api.pytorch.DDP_controller import DDPController
 except ImportError:
-    logger.warning("Please import elasticai_api  >= 1.2.0 .")
+    logger.warning("Please install elasticai_api >= 1.4.2 .")
 
 
 class ElasticController(DDPController):
     def __init__(self, data_shard_service):
         super(ElasticController, self).__init__(data_shard_service)
```

## atorch/distributed/elastic_trainer.py

```diff
@@ -1,10 +1,16 @@
 import torch
-from elasticai_api.common.data_shard_service import RecordIndexService
-from elasticai_api.pytorch.DDP_controller import DDPController
+
+from atorch.common.log_utils import default_logger as logger
+
+try:
+    from elasticai_api.common.data_shard_service import RecordIndexService
+    from elasticai_api.pytorch.DDP_controller import DDPController
+except ImportError:
+    logger.warning("Please install elasticai_api >= 1.4.2 .")
 
 from atorch.common.log_utils import default_logger as logger
 from atorch.data.elastic_dataset import ElasticDataset
 
 
 class ElasticTrainer(object):
     def __init__(
```

## atorch/modules/transformer/layers.py

```diff
@@ -72,16 +72,15 @@
     for fn_name in fn_names:
         new_fa_fn = _cast_fa_fn(getattr(flash_attn.flash_attn_interface, fn_name))
         setattr(flash_attn.flash_attn_interface, fn_name, new_fa_fn)
 
     _flash_attn_version = packaging.version.Version(version("flash-attn"))
     try:
         from flash_attn.flash_attention import FlashMHA  # cuda version
-    except (ImportError, ModuleNotFoundError) as e:
-        logger.error(f"Import FlashMHA failed. {e}")
+    except (ImportError, ModuleNotFoundError):
         assert _flash_attn_version >= packaging.version.Version(
             "2"
         ), "FlashMHA is deleted in 2.0 release, but FA1 should has FlashMHA."
         patch_src = Path(__file__).parent.resolve() / "_fa_api_compat_patch"
         patch_dst = Path(flash_attn.__file__).parent.resolve() / "flash_attention.py"
         shutil.copy(patch_src, patch_dst)
         from flash_attn.flash_attention import FlashMHA
```

## atorch/ops/git_version_info_installed.py

```diff
@@ -1,6 +1,6 @@
-version = '0.1.8+1ce9b881'
-git_hash = '1ce9b881'
-git_branch = 'master'
+version = '0.1.9+dc54a95b'
+git_hash = 'dc54a95b'
+git_branch = 'update_20240426'
 installed_ops = {'quantization_optimizer': False, 'quantizer': False}
 compatible_ops = {'quantization_optimizer': True, 'quantizer': True, 'atorch_not_implemented': False}
-torch_info = {'version': '1.13', 'bf16_support': False, 'cuda_version': '11.6', 'nccl_version': '2.14'}
+torch_info = {'version': '2.1', 'bf16_support': False, 'cuda_version': '12.1', 'nccl_version': '2.18'}
```

## atorch/protos/acceleration_pb2.py

```diff
@@ -1,438 +1,39 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: atorch/protos/acceleration.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='atorch/protos/acceleration.proto',
-  package='proto',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n atorch/protos/acceleration.proto\x12\x05proto\x1a\x1bgoogle/protobuf/empty.proto\"4\n\x1eGetAutoAccelerationTaskRequest\x12\x12\n\nprocess_id\x18\x01 \x01(\x05\"C\n\x12OptimizationMethod\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x02 \x01(\x0c\x12\x0f\n\x07tunable\x18\x03 \x01(\x08\"2\n\x08Strategy\x12&\n\x03opt\x18\x01 \x03(\x0b\x32\x19.proto.OptimizationMethod\"\x1f\n\x0e\x41nalysisMethod\x12\r\n\x05names\x18\x01 \x03(\t\"\xe7\x01\n\x14\x41utoAccelerationTask\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x14\n\x0cprocess_mode\x18\x03 \x01(\t\x12#\n\x08strategy\x18\x04 \x01(\x0b\x32\x0f.proto.StrategyH\x00\x12\x30\n\x0f\x61nalysis_method\x18\x05 \x01(\x0b\x32\x15.proto.AnalysisMethodH\x00\x12\x1d\n\x13parallel_group_info\x18\x06 \x01(\x0cH\x00\x12\x12\n\ntime_limit\x18\x07 \x01(\x05\x42\x0b\n\ttask_info\"\xc2\x01\n\x1a\x41utoAccelerationTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x12\n\nprocess_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x08\x12#\n\x08strategy\x18\x04 \x01(\x0b\x32\x0f.proto.StrategyH\x00\x12\x14\n\nmodel_meta\x18\x05 \x01(\x0cH\x00\x12\x17\n\rdryrun_result\x18\x06 \x01(\x0cH\x00\x12\x11\n\ttask_type\x18\x07 \x01(\tB\x08\n\x06result2\xba\x01\n\x17\x41utoAccelerationService\x12N\n\x08get_task\x12%.proto.GetAutoAccelerationTaskRequest\x1a\x1b.proto.AutoAccelerationTask\x12O\n\x12report_task_result\x12!.proto.AutoAccelerationTaskResult\x1a\x16.google.protobuf.Emptyb\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
-
-
-
-
-_GETAUTOACCELERATIONTASKREQUEST = _descriptor.Descriptor(
-  name='GetAutoAccelerationTaskRequest',
-  full_name='proto.GetAutoAccelerationTaskRequest',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='process_id', full_name='proto.GetAutoAccelerationTaskRequest.process_id', index=0,
-      number=1, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=72,
-  serialized_end=124,
-)
-
-
-_OPTIMIZATIONMETHOD = _descriptor.Descriptor(
-  name='OptimizationMethod',
-  full_name='proto.OptimizationMethod',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='name', full_name='proto.OptimizationMethod.name', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='config', full_name='proto.OptimizationMethod.config', index=1,
-      number=2, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='tunable', full_name='proto.OptimizationMethod.tunable', index=2,
-      number=3, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=126,
-  serialized_end=193,
-)
-
-
-_STRATEGY = _descriptor.Descriptor(
-  name='Strategy',
-  full_name='proto.Strategy',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='opt', full_name='proto.Strategy.opt', index=0,
-      number=1, type=11, cpp_type=10, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=195,
-  serialized_end=245,
-)
-
-
-_ANALYSISMETHOD = _descriptor.Descriptor(
-  name='AnalysisMethod',
-  full_name='proto.AnalysisMethod',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='names', full_name='proto.AnalysisMethod.names', index=0,
-      number=1, type=9, cpp_type=9, label=3,
-      has_default_value=False, default_value=[],
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=247,
-  serialized_end=278,
-)
-
-
-_AUTOACCELERATIONTASK = _descriptor.Descriptor(
-  name='AutoAccelerationTask',
-  full_name='proto.AutoAccelerationTask',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='task_id', full_name='proto.AutoAccelerationTask.task_id', index=0,
-      number=1, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_type', full_name='proto.AutoAccelerationTask.task_type', index=1,
-      number=2, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='process_mode', full_name='proto.AutoAccelerationTask.process_mode', index=2,
-      number=3, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='strategy', full_name='proto.AutoAccelerationTask.strategy', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='analysis_method', full_name='proto.AutoAccelerationTask.analysis_method', index=4,
-      number=5, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='parallel_group_info', full_name='proto.AutoAccelerationTask.parallel_group_info', index=5,
-      number=6, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='time_limit', full_name='proto.AutoAccelerationTask.time_limit', index=6,
-      number=7, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-    _descriptor.OneofDescriptor(
-      name='task_info', full_name='proto.AutoAccelerationTask.task_info',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-  ],
-  serialized_start=281,
-  serialized_end=512,
-)
-
-
-_AUTOACCELERATIONTASKRESULT = _descriptor.Descriptor(
-  name='AutoAccelerationTaskResult',
-  full_name='proto.AutoAccelerationTaskResult',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='task_id', full_name='proto.AutoAccelerationTaskResult.task_id', index=0,
-      number=1, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='process_id', full_name='proto.AutoAccelerationTaskResult.process_id', index=1,
-      number=2, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='status', full_name='proto.AutoAccelerationTaskResult.status', index=2,
-      number=3, type=8, cpp_type=7, label=1,
-      has_default_value=False, default_value=False,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='strategy', full_name='proto.AutoAccelerationTaskResult.strategy', index=3,
-      number=4, type=11, cpp_type=10, label=1,
-      has_default_value=False, default_value=None,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='model_meta', full_name='proto.AutoAccelerationTaskResult.model_meta', index=4,
-      number=5, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='dryrun_result', full_name='proto.AutoAccelerationTaskResult.dryrun_result', index=5,
-      number=6, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='task_type', full_name='proto.AutoAccelerationTaskResult.task_type', index=6,
-      number=7, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-    _descriptor.OneofDescriptor(
-      name='result', full_name='proto.AutoAccelerationTaskResult.result',
-      index=0, containing_type=None,
-      create_key=_descriptor._internal_create_key,
-    fields=[]),
-  ],
-  serialized_start=515,
-  serialized_end=709,
-)
-
-_STRATEGY.fields_by_name['opt'].message_type = _OPTIMIZATIONMETHOD
-_AUTOACCELERATIONTASK.fields_by_name['strategy'].message_type = _STRATEGY
-_AUTOACCELERATIONTASK.fields_by_name['analysis_method'].message_type = _ANALYSISMETHOD
-_AUTOACCELERATIONTASK.oneofs_by_name['task_info'].fields.append(
-  _AUTOACCELERATIONTASK.fields_by_name['strategy'])
-_AUTOACCELERATIONTASK.fields_by_name['strategy'].containing_oneof = _AUTOACCELERATIONTASK.oneofs_by_name['task_info']
-_AUTOACCELERATIONTASK.oneofs_by_name['task_info'].fields.append(
-  _AUTOACCELERATIONTASK.fields_by_name['analysis_method'])
-_AUTOACCELERATIONTASK.fields_by_name['analysis_method'].containing_oneof = _AUTOACCELERATIONTASK.oneofs_by_name['task_info']
-_AUTOACCELERATIONTASK.oneofs_by_name['task_info'].fields.append(
-  _AUTOACCELERATIONTASK.fields_by_name['parallel_group_info'])
-_AUTOACCELERATIONTASK.fields_by_name['parallel_group_info'].containing_oneof = _AUTOACCELERATIONTASK.oneofs_by_name['task_info']
-_AUTOACCELERATIONTASKRESULT.fields_by_name['strategy'].message_type = _STRATEGY
-_AUTOACCELERATIONTASKRESULT.oneofs_by_name['result'].fields.append(
-  _AUTOACCELERATIONTASKRESULT.fields_by_name['strategy'])
-_AUTOACCELERATIONTASKRESULT.fields_by_name['strategy'].containing_oneof = _AUTOACCELERATIONTASKRESULT.oneofs_by_name['result']
-_AUTOACCELERATIONTASKRESULT.oneofs_by_name['result'].fields.append(
-  _AUTOACCELERATIONTASKRESULT.fields_by_name['model_meta'])
-_AUTOACCELERATIONTASKRESULT.fields_by_name['model_meta'].containing_oneof = _AUTOACCELERATIONTASKRESULT.oneofs_by_name['result']
-_AUTOACCELERATIONTASKRESULT.oneofs_by_name['result'].fields.append(
-  _AUTOACCELERATIONTASKRESULT.fields_by_name['dryrun_result'])
-_AUTOACCELERATIONTASKRESULT.fields_by_name['dryrun_result'].containing_oneof = _AUTOACCELERATIONTASKRESULT.oneofs_by_name['result']
-DESCRIPTOR.message_types_by_name['GetAutoAccelerationTaskRequest'] = _GETAUTOACCELERATIONTASKREQUEST
-DESCRIPTOR.message_types_by_name['OptimizationMethod'] = _OPTIMIZATIONMETHOD
-DESCRIPTOR.message_types_by_name['Strategy'] = _STRATEGY
-DESCRIPTOR.message_types_by_name['AnalysisMethod'] = _ANALYSISMETHOD
-DESCRIPTOR.message_types_by_name['AutoAccelerationTask'] = _AUTOACCELERATIONTASK
-DESCRIPTOR.message_types_by_name['AutoAccelerationTaskResult'] = _AUTOACCELERATIONTASKRESULT
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-GetAutoAccelerationTaskRequest = _reflection.GeneratedProtocolMessageType('GetAutoAccelerationTaskRequest', (_message.Message,), {
-  'DESCRIPTOR' : _GETAUTOACCELERATIONTASKREQUEST,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.GetAutoAccelerationTaskRequest)
-  })
-_sym_db.RegisterMessage(GetAutoAccelerationTaskRequest)
-
-OptimizationMethod = _reflection.GeneratedProtocolMessageType('OptimizationMethod', (_message.Message,), {
-  'DESCRIPTOR' : _OPTIMIZATIONMETHOD,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.OptimizationMethod)
-  })
-_sym_db.RegisterMessage(OptimizationMethod)
-
-Strategy = _reflection.GeneratedProtocolMessageType('Strategy', (_message.Message,), {
-  'DESCRIPTOR' : _STRATEGY,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.Strategy)
-  })
-_sym_db.RegisterMessage(Strategy)
-
-AnalysisMethod = _reflection.GeneratedProtocolMessageType('AnalysisMethod', (_message.Message,), {
-  'DESCRIPTOR' : _ANALYSISMETHOD,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.AnalysisMethod)
-  })
-_sym_db.RegisterMessage(AnalysisMethod)
-
-AutoAccelerationTask = _reflection.GeneratedProtocolMessageType('AutoAccelerationTask', (_message.Message,), {
-  'DESCRIPTOR' : _AUTOACCELERATIONTASK,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.AutoAccelerationTask)
-  })
-_sym_db.RegisterMessage(AutoAccelerationTask)
-
-AutoAccelerationTaskResult = _reflection.GeneratedProtocolMessageType('AutoAccelerationTaskResult', (_message.Message,), {
-  'DESCRIPTOR' : _AUTOACCELERATIONTASKRESULT,
-  '__module__' : 'atorch.protos.acceleration_pb2'
-  # @@protoc_insertion_point(class_scope:proto.AutoAccelerationTaskResult)
-  })
-_sym_db.RegisterMessage(AutoAccelerationTaskResult)
-
-
-
-_AUTOACCELERATIONSERVICE = _descriptor.ServiceDescriptor(
-  name='AutoAccelerationService',
-  full_name='proto.AutoAccelerationService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=712,
-  serialized_end=898,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='get_task',
-    full_name='proto.AutoAccelerationService.get_task',
-    index=0,
-    containing_service=None,
-    input_type=_GETAUTOACCELERATIONTASKREQUEST,
-    output_type=_AUTOACCELERATIONTASK,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='report_task_result',
-    full_name='proto.AutoAccelerationService.report_task_result',
-    index=1,
-    containing_service=None,
-    input_type=_AUTOACCELERATIONTASKRESULT,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_AUTOACCELERATIONSERVICE)
-
-DESCRIPTOR.services_by_name['AutoAccelerationService'] = _AUTOACCELERATIONSERVICE
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n atorch/protos/acceleration.proto\x12\x05proto\x1a\x1bgoogle/protobuf/empty.proto\"4\n\x1eGetAutoAccelerationTaskRequest\x12\x12\n\nprocess_id\x18\x01 \x01(\x05\"C\n\x12OptimizationMethod\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x0e\n\x06\x63onfig\x18\x02 \x01(\x0c\x12\x0f\n\x07tunable\x18\x03 \x01(\x08\"2\n\x08Strategy\x12&\n\x03opt\x18\x01 \x03(\x0b\x32\x19.proto.OptimizationMethod\"\x1f\n\x0e\x41nalysisMethod\x12\r\n\x05names\x18\x01 \x03(\t\"\xe7\x01\n\x14\x41utoAccelerationTask\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x11\n\ttask_type\x18\x02 \x01(\t\x12\x14\n\x0cprocess_mode\x18\x03 \x01(\t\x12#\n\x08strategy\x18\x04 \x01(\x0b\x32\x0f.proto.StrategyH\x00\x12\x30\n\x0f\x61nalysis_method\x18\x05 \x01(\x0b\x32\x15.proto.AnalysisMethodH\x00\x12\x1d\n\x13parallel_group_info\x18\x06 \x01(\x0cH\x00\x12\x12\n\ntime_limit\x18\x07 \x01(\x05\x42\x0b\n\ttask_info\"\xc2\x01\n\x1a\x41utoAccelerationTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\x05\x12\x12\n\nprocess_id\x18\x02 \x01(\x05\x12\x0e\n\x06status\x18\x03 \x01(\x08\x12#\n\x08strategy\x18\x04 \x01(\x0b\x32\x0f.proto.StrategyH\x00\x12\x14\n\nmodel_meta\x18\x05 \x01(\x0cH\x00\x12\x17\n\rdryrun_result\x18\x06 \x01(\x0cH\x00\x12\x11\n\ttask_type\x18\x07 \x01(\tB\x08\n\x06result2\xba\x01\n\x17\x41utoAccelerationService\x12N\n\x08get_task\x12%.proto.GetAutoAccelerationTaskRequest\x1a\x1b.proto.AutoAccelerationTask\x12O\n\x12report_task_result\x12!.proto.AutoAccelerationTaskResult\x1a\x16.google.protobuf.Emptyb\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'atorch.protos.acceleration_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _globals['_GETAUTOACCELERATIONTASKREQUEST']._serialized_start=72
+  _globals['_GETAUTOACCELERATIONTASKREQUEST']._serialized_end=124
+  _globals['_OPTIMIZATIONMETHOD']._serialized_start=126
+  _globals['_OPTIMIZATIONMETHOD']._serialized_end=193
+  _globals['_STRATEGY']._serialized_start=195
+  _globals['_STRATEGY']._serialized_end=245
+  _globals['_ANALYSISMETHOD']._serialized_start=247
+  _globals['_ANALYSISMETHOD']._serialized_end=278
+  _globals['_AUTOACCELERATIONTASK']._serialized_start=281
+  _globals['_AUTOACCELERATIONTASK']._serialized_end=512
+  _globals['_AUTOACCELERATIONTASKRESULT']._serialized_start=515
+  _globals['_AUTOACCELERATIONTASKRESULT']._serialized_end=709
+  _globals['_AUTOACCELERATIONSERVICE']._serialized_start=712
+  _globals['_AUTOACCELERATIONSERVICE']._serialized_end=898
 # @@protoc_insertion_point(module_scope)
```

## atorch/protos/coworker_pb2.py

```diff
@@ -1,181 +1,33 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
 # source: atorch/protos/coworker.proto
 """Generated protocol buffer code."""
 from google.protobuf import descriptor as _descriptor
-from google.protobuf import message as _message
-from google.protobuf import reflection as _reflection
+from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
+from google.protobuf.internal import builder as _builder
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import empty_pb2 as google_dot_protobuf_dot_empty__pb2
 
 
-DESCRIPTOR = _descriptor.FileDescriptor(
-  name='atorch/protos/coworker.proto',
-  package='protos',
-  syntax='proto3',
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_pb=b'\n\x1c\x61torch/protos/coworker.proto\x12\x06protos\x1a\x1bgoogle/protobuf/empty.proto\"\x19\n\tBatchData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"4\n\x08\x44\x61taInfo\x12\x15\n\rcoworker_addr\x18\x01 \x01(\t\x12\x11\n\tbatch_num\x18\x02 \x01(\x05\x32Q\n\x12\x43oworkerRpcService\x12;\n\x0eget_batch_data\x12\x16.google.protobuf.Empty\x1a\x11.protos.BatchData2\x8a\x01\n\x0f\x44\x61taInfoService\x12<\n\x10report_data_info\x12\x10.protos.DataInfo\x1a\x16.google.protobuf.Empty\x12\x39\n\rget_data_info\x12\x16.google.protobuf.Empty\x1a\x10.protos.DataInfob\x06proto3'
-  ,
-  dependencies=[google_dot_protobuf_dot_empty__pb2.DESCRIPTOR,])
-
-
-
-
-_BATCHDATA = _descriptor.Descriptor(
-  name='BatchData',
-  full_name='protos.BatchData',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='data', full_name='protos.BatchData.data', index=0,
-      number=1, type=12, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"",
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=69,
-  serialized_end=94,
-)
-
-
-_DATAINFO = _descriptor.Descriptor(
-  name='DataInfo',
-  full_name='protos.DataInfo',
-  filename=None,
-  file=DESCRIPTOR,
-  containing_type=None,
-  create_key=_descriptor._internal_create_key,
-  fields=[
-    _descriptor.FieldDescriptor(
-      name='coworker_addr', full_name='protos.DataInfo.coworker_addr', index=0,
-      number=1, type=9, cpp_type=9, label=1,
-      has_default_value=False, default_value=b"".decode('utf-8'),
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-    _descriptor.FieldDescriptor(
-      name='batch_num', full_name='protos.DataInfo.batch_num', index=1,
-      number=2, type=5, cpp_type=1, label=1,
-      has_default_value=False, default_value=0,
-      message_type=None, enum_type=None, containing_type=None,
-      is_extension=False, extension_scope=None,
-      serialized_options=None, file=DESCRIPTOR,  create_key=_descriptor._internal_create_key),
-  ],
-  extensions=[
-  ],
-  nested_types=[],
-  enum_types=[
-  ],
-  serialized_options=None,
-  is_extendable=False,
-  syntax='proto3',
-  extension_ranges=[],
-  oneofs=[
-  ],
-  serialized_start=96,
-  serialized_end=148,
-)
-
-DESCRIPTOR.message_types_by_name['BatchData'] = _BATCHDATA
-DESCRIPTOR.message_types_by_name['DataInfo'] = _DATAINFO
-_sym_db.RegisterFileDescriptor(DESCRIPTOR)
-
-BatchData = _reflection.GeneratedProtocolMessageType('BatchData', (_message.Message,), {
-  'DESCRIPTOR' : _BATCHDATA,
-  '__module__' : 'atorch.protos.coworker_pb2'
-  # @@protoc_insertion_point(class_scope:protos.BatchData)
-  })
-_sym_db.RegisterMessage(BatchData)
-
-DataInfo = _reflection.GeneratedProtocolMessageType('DataInfo', (_message.Message,), {
-  'DESCRIPTOR' : _DATAINFO,
-  '__module__' : 'atorch.protos.coworker_pb2'
-  # @@protoc_insertion_point(class_scope:protos.DataInfo)
-  })
-_sym_db.RegisterMessage(DataInfo)
-
-
-
-_COWORKERRPCSERVICE = _descriptor.ServiceDescriptor(
-  name='CoworkerRpcService',
-  full_name='protos.CoworkerRpcService',
-  file=DESCRIPTOR,
-  index=0,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=150,
-  serialized_end=231,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='get_batch_data',
-    full_name='protos.CoworkerRpcService.get_batch_data',
-    index=0,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_BATCHDATA,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_COWORKERRPCSERVICE)
-
-DESCRIPTOR.services_by_name['CoworkerRpcService'] = _COWORKERRPCSERVICE
-
-
-_DATAINFOSERVICE = _descriptor.ServiceDescriptor(
-  name='DataInfoService',
-  full_name='protos.DataInfoService',
-  file=DESCRIPTOR,
-  index=1,
-  serialized_options=None,
-  create_key=_descriptor._internal_create_key,
-  serialized_start=234,
-  serialized_end=372,
-  methods=[
-  _descriptor.MethodDescriptor(
-    name='report_data_info',
-    full_name='protos.DataInfoService.report_data_info',
-    index=0,
-    containing_service=None,
-    input_type=_DATAINFO,
-    output_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-  _descriptor.MethodDescriptor(
-    name='get_data_info',
-    full_name='protos.DataInfoService.get_data_info',
-    index=1,
-    containing_service=None,
-    input_type=google_dot_protobuf_dot_empty__pb2._EMPTY,
-    output_type=_DATAINFO,
-    serialized_options=None,
-    create_key=_descriptor._internal_create_key,
-  ),
-])
-_sym_db.RegisterServiceDescriptor(_DATAINFOSERVICE)
-
-DESCRIPTOR.services_by_name['DataInfoService'] = _DATAINFOSERVICE
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x1c\x61torch/protos/coworker.proto\x12\x06protos\x1a\x1bgoogle/protobuf/empty.proto\"\x19\n\tBatchData\x12\x0c\n\x04\x64\x61ta\x18\x01 \x01(\x0c\"4\n\x08\x44\x61taInfo\x12\x15\n\rcoworker_addr\x18\x01 \x01(\t\x12\x11\n\tbatch_num\x18\x02 \x01(\x05\x32Q\n\x12\x43oworkerRpcService\x12;\n\x0eget_batch_data\x12\x16.google.protobuf.Empty\x1a\x11.protos.BatchData2\x8a\x01\n\x0f\x44\x61taInfoService\x12<\n\x10report_data_info\x12\x10.protos.DataInfo\x1a\x16.google.protobuf.Empty\x12\x39\n\rget_data_info\x12\x16.google.protobuf.Empty\x1a\x10.protos.DataInfob\x06proto3')
 
+_globals = globals()
+_builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'atorch.protos.coworker_pb2', _globals)
+if _descriptor._USE_C_DESCRIPTORS == False:
+
+  DESCRIPTOR._options = None
+  _globals['_BATCHDATA']._serialized_start=69
+  _globals['_BATCHDATA']._serialized_end=94
+  _globals['_DATAINFO']._serialized_start=96
+  _globals['_DATAINFO']._serialized_end=148
+  _globals['_COWORKERRPCSERVICE']._serialized_start=150
+  _globals['_COWORKERRPCSERVICE']._serialized_end=231
+  _globals['_DATAINFOSERVICE']._serialized_start=234
+  _globals['_DATAINFOSERVICE']._serialized_end=372
 # @@protoc_insertion_point(module_scope)
```

## atorch/trainer/atorch_args.py

```diff
@@ -96,14 +96,15 @@
         default=None,
         metadata={
             "help": (
                 "The format in which the input data is passed to the model."
                 "If model_input_format=None, data is passed to model by `model(data)`."
                 "If model_input_format='unpack_sequence', `model(*data)`."
                 "If model_input_format='unpack_dict', `model(**data)`."
+                "It is invalid to set `model_input_format`, which is legacy in AtorchTrainer."
             )
         },
     )
     distributed_sampler_cls: Optional[Callable] = field(
         default=None,
         metadata={
             "help": "if not None, custom distributed sampler with same interface as pytorch's DistributedSampler."
@@ -172,14 +173,27 @@
         metadata={
             "help": (
                 "The maximum size for a checkpoint before being sharded. " "Used on PreTrainedModel.save_pretrained()."
             )
         },
     )
 
+    logit_names: Optional[List[str]] = field(
+        default=None, metadata={"help": "The list of keys in your dictionary of outputs that correspond to the logits."}
+    )
+    logit_index: int = field(
+        default=-1,
+        metadata={
+            "help": (
+                "If isinstance(model's output, Tuple) and logit_index>=0, "
+                "use the corresponding part of the output as the logits."
+            )
+        },
+    )
+
     @cached_property
     def _setup_devices(self) -> "torch.device":
         logger.info("PyTorch: setting up devices")
 
         if not torch.distributed.is_initialized():
             atorch.init_distributed(
                 os.getenv("TORCH_DISTRIBUTED_BACKEND", "nccl"), timeout=timedelta(seconds=self.ddp_timeout)
@@ -235,8 +249,18 @@
 
         if self.atorch_wrap_cls is not None and not isinstance(self.atorch_wrap_cls, tuple):
             raise ValueError(f"atorch_wrap_cls has {type(self.atorch_wrap_cls)} type, required tuple type.")
 
         if self.atorch_checkpoint_cls is not None and not isinstance(self.atorch_checkpoint_cls, tuple):
             raise ValueError(f"atorch_checkpoint_cls has {type(self.atorch_checkpoint_cls)} type, required tuple type.")
 
+        if self.model_input_format is not None:
+            logger.warning(
+                "It is invalid to set `model_input_format`, which is used in auto_accelerate()'s dryrun "
+                "and will be deprecated in AtorchTrainer."
+            )
+
         Seq2SeqTrainingArguments.__post_init__(self)
+
+        if self.use_legacy_prediction_loop:
+            logger.warning("`use_legacy_prediction_loop` is deprecated and does not have any effect.")
+            self.use_legacy_prediction_loop = False
```

## atorch/trainer/atorch_trainer.py

```diff
@@ -69,36 +69,43 @@
     TrainerState,
 )
 from transformers.trainer_pt_utils import (
     IterableDatasetShard,
     LengthGroupedSampler,
     distributed_broadcast_scalars,
     distributed_concat,
+    find_batch_size,
+    nested_concat,
+    nested_detach,
+    nested_numpify,
     reissue_pt_warnings,
 )
 from transformers.trainer_utils import (
     PREFIX_CHECKPOINT_DIR,
+    EvalLoopOutput,
     EvalPrediction,
     IntervalStrategy,
     PredictionOutput,
     RemoveColumnsCollator,
     TrainOutput,
+    denumpify_detensorize,
     get_last_checkpoint,
     has_length,
     seed_worker,
     speed_metrics,
 )
 from transformers.utils import (
     ADAPTER_SAFE_WEIGHTS_NAME,
     ADAPTER_WEIGHTS_NAME,
     CONFIG_NAME,
     SAFE_WEIGHTS_INDEX_NAME,
     SAFE_WEIGHTS_NAME,
     WEIGHTS_INDEX_NAME,
     WEIGHTS_NAME,
+    can_return_loss,
     find_labels,
     is_datasets_available,
     is_peft_available,
 )
 
 if TYPE_CHECKING:
     import optuna
@@ -144,15 +151,19 @@
         **kwargs,
     ):
         if args is None:
             output_dir = "tmp_atorch_trainer"
             logger.info(f"No `AtorchArguments` passed, using `output_dir={output_dir}`.")
             args = AtorchArguments(output_dir=output_dir)  # type: ignore[call-arg]
 
-        if len(args.sharded_ddp) > 0 or len(args.fsdp) > 0 or args.deepspeed is not None:
+        if (
+            (hasattr(args, "sharded_ddp") and len(args.sharded_ddp) > 0)
+            or len(args.fsdp) > 0
+            or args.deepspeed is not None
+        ):
             logger.warning(
                 "--sharded_ddp, --fsdp, --deepspeed in `TrainingArguments` is invalid when using `AtorchArguments`."
             )
 
         self.args = args
         self.kwargs = kwargs
         self.model = model
@@ -165,14 +176,16 @@
 
         if self.atorch_fsdp and torch_version() < (2, 0, 0):  # type: ignore
             raise ValueError("Greater than version 2.0 of PyTorch is necessary for FSDP.")
 
         if args.save_load_by_streaming and not self.atorch_fsdp:
             raise ValueError("--atorch_opt fsdp is needed when using --save_load_by_streaming.")
 
+        self.is_in_train = False
+
         # create accelerator object
         self.accelerator = Accelerator()
 
         # force device and distributed setup init explicitly
         args._setup_devices
 
         self.data_collator = None
@@ -184,21 +197,25 @@
         self.train_dataset = train_dataset
         self.eval_dataset = eval_dataset
         self.tokenizer = tokenizer
 
         self.model_init = model_init
         self.compute_metrics = compute_metrics
         self.preprocess_logits_for_metrics = preprocess_logits_for_metrics
+        if self.compute_metrics is not None and args.eval_accumulation_steps is None:
+            raise ValueError(
+                "Use custom compute_metrics() function may cause extra high GPU memory footprint during evaluation, "
+                "so eval_accumulation_steps should be set explicitly. If you are unsure of what size to set it to, it's"
+                " recommended to set it to 1."
+            )
 
         self.optimizer, self.lr_scheduler = optimizers
         # Check optimizer and lr_scheduler
         if self.optimizer is not None and not isinstance(self.optimizer, torch.optim.Optimizer):
             raise ValueError("`optimizer` must be the torch.optim.Optimizer type.")
-        if self.lr_scheduler is not None and not isinstance(self.lr_scheduler, torch.optim.lr_scheduler.LambdaLR):
-            raise ValueError("`lr_scheduler` must be the torch.optim.lr_scheduler.LambdaLR type.")
 
         report_callbacks = [TensorBoardCallback]
         # Add additional tensorboard callback.
         if additional_tensorboard_hook is not None and len(additional_tensorboard_hook) > 0:
             report_callbacks.append(additional_tensorboard_hook[0])
         default_callbacks = DEFAULT_CALLBACKS + report_callbacks
         callbacks = default_callbacks if callbacks is None else default_callbacks + callbacks
@@ -254,15 +271,17 @@
 
         self.control = TrainerControl()
         # Internal variable to count flos in each process, will be accumulated in `self.state.total_flos` then
         # returned to 0 every time flos need to be logged
         self.current_flos = 0
         default_label_names = find_labels(self.model.__class__)
         self.label_names = default_label_names if self.args.label_names is None else self.args.label_names
+        self.logit_names = ["logits"] if self.args.logit_names is None else self.args.logit_names
         self.model_forward_args = list(inspect.signature(self.model.forward).parameters.keys())
+        self.can_return_loss = can_return_loss(self.model.__class__)
 
         # Set ATorch Parameters
         self.atorch_wrap_cls = args.atorch_wrap_cls
         self.prepare_input = args.prepare_input
         self.optim_func = args.optim_func
         self.optim_args = args.optim_args
         self.optim_param_func = args.optim_param_func
@@ -358,15 +377,15 @@
         if not status:
             raise TypeError("Unsupported load_strategy, please check your load_strategy.")
 
         # The listed methods will not change the model parameters, while other methods will.
         optim_methods_to_check = ["parallel_mode", "amp_native", "checkpoint"]
 
         if self.optimizer is not None:
-            for (opt_name, config, tunable) in self.load_strategy:
+            for opt_name, config, tunable in self.load_strategy:
                 if opt_name not in optim_methods_to_check:
                     raise ValueError(
                         f"If you're using optimization methods outside of {optim_methods_to_check}, passing"
                         " `optimizers=(xxx,xxx)` when creating a trainer is not supported because auto_accelerate()"
                         " will change the model parameters. Please set `optimizers` via `args.optim_func` instead."
                     )
 
@@ -427,15 +446,15 @@
             signature = inspect.signature(self.model.forward)
             self._signature_columns = list(signature.parameters.keys())
             # Labels may be named label or label_ids, the default data collator handles that.
             self._signature_columns += list(
                 set(["labels", "label", "label_ids"] + self.label_names + self.model_forward_args)
             )
 
-    def _remove_unused_columns(self, dataset: "datasets.Dataset", description: Optional[str] = None):
+    def _remove_unused_columns(self, dataset, description: Optional[str] = None):
         if not self.args.remove_unused_columns:
             return dataset
         self._set_signature_columns_if_needed()
         signature_columns = self._signature_columns
 
         ignored_columns = list(set(dataset.column_names) - set(signature_columns))
         if len(ignored_columns) > 0:
@@ -445,15 +464,15 @@
                 f"`{self.model.__class__.__name__}.forward` and have been ignored: {', '.join(ignored_columns)}."
                 f" If {', '.join(ignored_columns)} are not expected by `{self.model.__class__.__name__}.forward`, "
                 " you can safely ignore this message."
             )
 
         columns = [k for k in signature_columns if k in dataset.column_names]  # type: ignore[attr-defined]
 
-        if version.parse(datasets.__version__) < version.parse("1.4.0"):
+        if version.parse(datasets.__version__) < version.parse("1.4.0"):  # type: ignore[attr-defined]
             dataset.set_format(
                 type=dataset.format["type"], columns=columns, format_kwargs=dataset.format["format_kwargs"]
             )
             return dataset
         else:
             return dataset.remove_columns(ignored_columns)
 
@@ -477,15 +496,17 @@
 
     def _get_train_sampler(self) -> Optional[torch.utils.data.Sampler]:
         if self.train_dataset is None or not has_length(self.train_dataset):
             return None
 
         # Build the sampler.
         if self.args.group_by_length:
-            if is_datasets_available() and isinstance(self.train_dataset, datasets.Dataset):
+            if is_datasets_available() and isinstance(
+                self.train_dataset, datasets.Dataset  # type: ignore[attr-defined]
+            ):
                 lengths = (
                     self.train_dataset[self.args.length_column_name]
                     if self.args.length_column_name in self.train_dataset.column_names
                     else None
                 )
             else:
                 lengths = None
@@ -510,15 +531,15 @@
         Subclass and override this method if you want to inject some custom behavior.
         """
         if self.train_dataset is None:
             raise ValueError("Trainer: training requires a train_dataset.")
 
         train_dataset = self.train_dataset
         data_collator = self.data_collator
-        if is_datasets_available() and isinstance(train_dataset, datasets.Dataset):
+        if is_datasets_available() and isinstance(train_dataset, datasets.Dataset):  # type: ignore[attr-defined]
             train_dataset = self._remove_unused_columns(train_dataset, description="training")
         elif data_collator is not None:
             data_collator = self._get_collator_with_removed_columns(data_collator, description="training")
 
         dataloader_params = {
             "batch_size": self._train_batch_size,
             "num_workers": self.args.dataloader_num_workers,
@@ -553,15 +574,15 @@
         """
         if eval_dataset is None and self.eval_dataset is None:
             raise ValueError("Trainer: evaluation requires an eval_dataset.")
 
         eval_dataset = eval_dataset if eval_dataset is not None else self.eval_dataset
         data_collator = self.data_collator
 
-        if is_datasets_available() and isinstance(eval_dataset, datasets.Dataset):
+        if is_datasets_available() and isinstance(eval_dataset, datasets.Dataset):  # type: ignore[attr-defined]
             eval_dataset = self._remove_unused_columns(eval_dataset, description="evaluation")
         elif data_collator is not None:
             data_collator = self._get_collator_with_removed_columns(data_collator, description="evaluation")
 
         dataloader_params = {
             "batch_size": self.args.eval_batch_size,
             "num_workers": self.args.dataloader_num_workers,
@@ -583,16 +604,36 @@
         Subclass and override this method if you want to inject some custom behavior.
 
         Args:
             test_dataset (`torch.utils.data.Dataset`, *optional*):
                 The test dataset to use. If it is a [`~datasets.Dataset`], columns not accepted by the
                 `model.forward()` method are automatically removed. It must implement `__len__`.
         """
-        # Do Atorch get test dataloader
-        raise NotImplementedError("`get_test_dataloader` is not implemented.")
+        data_collator = self.data_collator
+
+        if is_datasets_available() and isinstance(test_dataset, datasets.Dataset):  # type: ignore[attr-defined]
+            test_dataset = self._remove_unused_columns(test_dataset, description="test")
+        elif data_collator is not None:
+            data_collator = self._get_collator_with_removed_columns(data_collator, description="test")
+
+        dataloader_params = {
+            "batch_size": self.args.eval_batch_size,
+            "collate_fn": data_collator,
+            "num_workers": self.args.dataloader_num_workers,
+            "pin_memory": self.args.dataloader_pin_memory,
+        }
+        if data_collator is not None:
+            dataloader_params["collate_fn"] = data_collator
+
+        if not isinstance(test_dataset, torch.utils.data.IterableDataset):
+            dataloader_params["sampler"] = self._get_eval_sampler(test_dataset)
+            dataloader_params["drop_last"] = self.args.dataloader_drop_last
+
+        # We use the same batch_size as for eval.
+        return self.accelerator.prepare(DataLoader(test_dataset, **dataloader_params))
 
     def create_optimizer(self):
         """
         Setup the optimizer.
 
         We provide a reasonable default that works well. If you want to use something else, you can pass a tuple in the
         Trainer's init through `optimizers`, or subclass and override this method in a subclass.
@@ -607,17 +648,19 @@
 
         Args:
             num_training_steps (int): The number of training steps to do.
         """
         # Do atorch create scheduler
         if self.lr_scheduler is None:
             self.lr_scheduler = get_scheduler(
-                self.args.atorch_lr_scheduler_type
-                if self.args.atorch_lr_scheduler_type is not None
-                else self.args.lr_scheduler_type,
+                (
+                    self.args.atorch_lr_scheduler_type
+                    if self.args.atorch_lr_scheduler_type is not None
+                    else self.args.lr_scheduler_type
+                ),
                 optimizer=self.optimizer if optimizer is None else optimizer,
                 num_warmup_steps=self.args.get_warmup_steps(num_training_steps),
                 num_training_steps=num_training_steps,
             )
         return self.lr_scheduler
 
     def train(
@@ -867,18 +910,17 @@
                 self.current_flos += float(self.floating_point_ops(inputs))
 
                 is_last_step_and_steps_less_than_grad_acc = (
                     steps_in_epoch <= args.gradient_accumulation_steps and (step + 1) == steps_in_epoch
                 )
 
                 if (
-                    total_batched_samples % args.gradient_accumulation_steps == 0
-                    or  # noqa: W504
                     # last step in epoch but step is always smaller than gradient_accumulation_steps
-                    is_last_step_and_steps_less_than_grad_acc
+                    total_batched_samples % args.gradient_accumulation_steps == 0
+                    or is_last_step_and_steps_less_than_grad_acc
                 ):
                     # Gradient clipping
                     if args.max_grad_norm is not None and args.max_grad_norm > 0:
                         if self.do_grad_scaling:
                             # AMP: gradients need unscaling
                             self.scaler.unscale_(self.optimizer)
 
@@ -1491,15 +1533,15 @@
                         max_shard_size=self.args.max_shard_size,
                     ):
                         return False
             else:
                 logger.info("Trainer.model is not a `PreTrainedModel`, only saving its state dict.")
                 if self.args.save_safetensors:
                     if not self._write_safely(
-                        safetensors.torch.save_file,
+                        safetensors.torch.save_file,  # type: ignore[attr-defined]
                         state_dict,
                         os.path.join(output_dir, SAFE_WEIGHTS_NAME),
                     ):
                         return False
                 else:
                     if not self._write_safely(torch.save, state_dict, os.path.join(output_dir, WEIGHTS_NAME)):
                         return False
@@ -1723,38 +1765,42 @@
                 An optional prefix to be used as the metrics key prefix. For example the metrics "bleu" will be named
                 "eval_bleu" if the prefix is "eval" (default)
 
         Returns:
             A dictionary containing the evaluation loss and the potential metrics computed from the predictions. The
             dictionary also contains the epoch number which comes from the training state.
         """
-        self.eval_dataloader = self.get_eval_dataloader(eval_dataset)
-        logger.info("Start evaluation")
-        self.model.eval()
-        losses = []
-        for step, batch in enumerate(self.eval_dataloader):
-            with torch.no_grad():
-                batch = {k: v.to(self.args.device) for k, v in batch.items()}
-                with self.autocast_smart_context_manager():
-                    loss = self.compute_loss(self.model, batch)
-                repeated_loss = loss.repeat(self.args.per_device_eval_batch_size)
-                if repeated_loss.ndim == 0:
-                    repeated_loss = repeated_loss[None]
-                output_tensors = [repeated_loss for _ in range(self.args.world_size)]
-                torch.distributed.all_gather(output_tensors, repeated_loss)
-                losses.append(torch.cat([t.detach().cpu() for t in output_tensors], dim=0))
-
-        losses = torch.cat(losses)
-        losses = losses[: len(self.eval_dataset)]
-        mean_loss = torch.mean(losses).item()
-        metrics = {"eval_loss": mean_loss, "step": self.state.global_step}
-        self.log(metrics)
-        self.control = self.callback_handler.on_evaluate(self.args, self.state, self.control, metrics)
+        eval_dataloader = self.get_eval_dataloader(eval_dataset)
+        start_time = time.time()
 
-        return metrics
+        output = self.evaluation_loop(
+            eval_dataloader,
+            description="Evaluation",
+            # No point gathering the predictions if there are no metrics, otherwise we defer to
+            # self.args.prediction_loss_only
+            prediction_loss_only=True if self.compute_metrics is None else None,
+            ignore_keys=ignore_keys,
+            metric_key_prefix=metric_key_prefix,
+        )
+
+        total_batch_size = self.args.eval_batch_size * self.args.world_size
+        output.metrics.update(
+            speed_metrics(
+                metric_key_prefix,
+                start_time,
+                num_samples=output.num_samples,
+                num_steps=math.ceil(output.num_samples / total_batch_size),
+            )
+        )
+
+        self.log(output.metrics)
+
+        self.control = self.callback_handler.on_evaluate(self.args, self.state, self.control, output.metrics)
+
+        return output.metrics
 
     def predict(
         self, test_dataset: Dataset, ignore_keys: Optional[List[str]] = None, metric_key_prefix: str = "test"
     ) -> PredictionOutput:
         """
         Run prediction and returns predictions and potential metrics.
 
@@ -1783,16 +1829,220 @@
         Returns: *NamedTuple* A namedtuple with the following keys:
 
             - predictions (`np.ndarray`): The predictions on `test_dataset`.
             - label_ids (`np.ndarray`, *optional*): The labels (if the dataset contained some).
             - metrics (`Dict[str, float]`, *optional*): The potential dictionary of metrics (if the dataset contained
               labels).
         """
-        # Do Atorch predict
-        raise NotImplementedError("`predict` is not implemented.")
+
+        test_dataloader = self.get_test_dataloader(test_dataset)
+        start_time = time.time()
+
+        output = self.evaluation_loop(
+            test_dataloader, description="Prediction", ignore_keys=ignore_keys, metric_key_prefix=metric_key_prefix
+        )
+        total_batch_size = self.args.eval_batch_size * self.args.world_size
+        output.metrics.update(
+            speed_metrics(
+                metric_key_prefix,
+                start_time,
+                num_samples=output.num_samples,
+                num_steps=math.ceil(output.num_samples / total_batch_size),
+            )
+        )
+
+        self.control = self.callback_handler.on_predict(self.args, self.state, self.control, output.metrics)
+
+        return PredictionOutput(predictions=output.predictions, label_ids=output.label_ids, metrics=output.metrics)
+
+    def evaluation_loop(
+        self,
+        dataloader: DataLoader,
+        description: str,
+        prediction_loss_only: Optional[bool] = None,
+        ignore_keys: Optional[List[str]] = None,
+        metric_key_prefix: str = "eval",
+    ) -> EvalLoopOutput:
+        """
+        Prediction/evaluation loop, shared by `Trainer.evaluate()` and `Trainer.predict()`.
+
+        Works both with or without labels.
+        """
+        args = self.args
+
+        prediction_loss_only = prediction_loss_only if prediction_loss_only is not None else args.prediction_loss_only
+
+        model = self.model
+
+        # if full fp16 or bf16 eval is wanted and this ``evaluation`` or ``predict`` isn't called
+        # while ``train`` is running, cast it to the right dtype first and then put on device
+        if not self.is_in_train:
+            if args.fp16_full_eval:
+                model = model.to(dtype=torch.float16, device=args.device)
+            elif args.bf16_full_eval:
+                model = model.to(dtype=torch.bfloat16, device=args.device)
+
+        batch_size = self.args.eval_batch_size
+
+        logger.info(f"***** Running {description} *****")
+        if has_length(dataloader):
+            logger.info(f"  Num examples = {self.num_examples(dataloader)}")
+        else:
+            logger.info("  Num examples: Unknown")
+        logger.info(f"  Batch size = {batch_size}")
+
+        model.eval()
+
+        self.callback_handler.eval_dataloader = dataloader
+        # Do this before wrapping.
+        eval_dataset = getattr(dataloader, "dataset", None)
+
+        if args.past_index >= 0:
+            self._past = None
+
+        # Initialize containers
+        # losses/preds/labels on GPU/TPU (accumulated for eval_accumulation_steps)
+        losses_host = None
+        preds_host = None
+        labels_host = None
+        inputs_host = None
+
+        # losses/preds/labels on CPU (final containers)
+        all_losses = None
+        all_preds = None
+        all_labels = None
+        all_inputs = None
+        # Will be useful when we have an iterable dataset so don't know its length.
+
+        observed_num_examples = 0
+        # Main evaluation loop
+        for step, inputs in enumerate(dataloader):
+            # Update the observed num examples
+            observed_batch_size = find_batch_size(inputs)
+            if observed_batch_size is not None:
+                observed_num_examples += observed_batch_size
+                # For batch samplers, batch_size is not known by the dataloader in advance.
+                if batch_size is None:
+                    batch_size = observed_batch_size
+
+            # Prediction step
+            loss, logits, labels = self.prediction_step(model, inputs, prediction_loss_only, ignore_keys=ignore_keys)
+            inputs_decode = self._prepare_input(inputs["input_ids"]) if args.include_inputs_for_metrics else None
+
+            # Update containers on host
+            if loss is not None:
+                losses = self.accelerator.gather_for_metrics((loss.repeat(batch_size)))
+                losses_host = losses if losses_host is None else nested_concat(losses_host, losses, padding_index=-100)
+            if labels is not None:
+                labels = self.accelerator.pad_across_processes(labels, dim=1, pad_index=-100)
+            if inputs_decode is not None:
+                inputs_decode = self.accelerator.pad_across_processes(inputs_decode, dim=1, pad_index=-100)
+                inputs_decode = self.accelerator.gather_for_metrics((inputs_decode))
+                inputs_host = (
+                    inputs_decode
+                    if inputs_host is None
+                    else nested_concat(inputs_host, inputs_decode, padding_index=-100)
+                )
+            if logits is not None:
+                logits = self.accelerator.pad_across_processes(logits, dim=1, pad_index=-100)
+                if self.preprocess_logits_for_metrics is not None:
+                    logits = self.preprocess_logits_for_metrics(logits, labels)
+                logits = self.accelerator.gather_for_metrics((logits))
+                preds_host = logits if preds_host is None else nested_concat(preds_host, logits, padding_index=-100)
+
+            if labels is not None:
+                labels = self.accelerator.gather_for_metrics((labels))
+                labels_host = labels if labels_host is None else nested_concat(labels_host, labels, padding_index=-100)
+
+            self.control = self.callback_handler.on_prediction_step(args, self.state, self.control)
+
+            # Gather all tensors and put them back on the CPU if we have done enough accumulation steps.
+            if (
+                args.eval_accumulation_steps is not None
+                and step % args.eval_accumulation_steps == 0
+                and self.accelerator.sync_gradients
+            ):
+                if losses_host is not None:
+                    losses = nested_numpify(losses_host)
+                    all_losses = losses if all_losses is None else np.concatenate((all_losses, losses), axis=0)
+                if preds_host is not None:
+                    logits = nested_numpify(preds_host)
+                    all_preds = logits if all_preds is None else nested_concat(all_preds, logits, padding_index=-100)
+                if inputs_host is not None:
+                    inputs_decode = nested_numpify(inputs_host)
+                    all_inputs = (
+                        inputs_decode
+                        if all_inputs is None
+                        else nested_concat(all_inputs, inputs_decode, padding_index=-100)
+                    )
+                if labels_host is not None:
+                    labels = nested_numpify(labels_host)
+                    all_labels = labels if all_labels is None else nested_concat(all_labels, labels, padding_index=-100)
+
+                # Set back to None to begin a new accumulation
+                losses_host, preds_host, inputs_host, labels_host = None, None, None, None
+
+        if args.past_index and hasattr(self, "_past"):
+            # Clean the state at the end of the evaluation loop
+            delattr(self, "_past")
+
+        # Gather all remaining tensors and put them back on the CPU
+        if losses_host is not None:
+            losses = nested_numpify(losses_host)
+            all_losses = losses if all_losses is None else np.concatenate((all_losses, losses), axis=0)
+        if preds_host is not None:
+            logits = nested_numpify(preds_host)
+            all_preds = logits if all_preds is None else nested_concat(all_preds, logits, padding_index=-100)
+        if inputs_host is not None:
+            inputs_decode = nested_numpify(inputs_host)
+            all_inputs = (
+                inputs_decode if all_inputs is None else nested_concat(all_inputs, inputs_decode, padding_index=-100)
+            )
+        if labels_host is not None:
+            labels = nested_numpify(labels_host)
+            all_labels = labels if all_labels is None else nested_concat(all_labels, labels, padding_index=-100)
+
+        # Number of samples
+        if has_length(eval_dataset):
+            num_samples = len(eval_dataset)
+        # The instance check is weird and does not actually check for the type, but whether the dataset has the right
+        # methods. Therefore we need to make sure it also has the attribute.
+        elif isinstance(eval_dataset, IterableDatasetShard) and getattr(eval_dataset, "num_examples", 0) > 0:
+            num_samples = eval_dataset.num_examples
+        else:
+            if has_length(dataloader):
+                num_samples = self.num_examples(dataloader)
+            else:  # both len(dataloader.dataset) and len(dataloader) fail
+                num_samples = observed_num_examples
+        if num_samples == 0 and observed_num_examples > 0:
+            num_samples = observed_num_examples
+
+        # Metrics!
+        if self.compute_metrics is not None and all_preds is not None and all_labels is not None:
+            if args.include_inputs_for_metrics:
+                metrics = self.compute_metrics(
+                    EvalPrediction(predictions=all_preds, label_ids=all_labels, inputs=all_inputs)
+                )
+            else:
+                metrics = self.compute_metrics(EvalPrediction(predictions=all_preds, label_ids=all_labels))
+        else:
+            metrics = {}
+
+        # To be JSON-serializable, we need to remove numpy types or zero-d tensors
+        metrics = denumpify_detensorize(metrics)
+
+        if all_losses is not None:
+            metrics[f"{metric_key_prefix}_loss"] = all_losses.mean().item()
+
+        # Prefix all keys with metric_key_prefix + '_'
+        for key in list(metrics.keys()):
+            if not key.startswith(f"{metric_key_prefix}_"):
+                metrics[f"{metric_key_prefix}_{key}"] = metrics.pop(key)
+
+        return EvalLoopOutput(predictions=all_preds, label_ids=all_labels, metrics=metrics, num_samples=num_samples)
 
     def training_step(self, model: nn.Module, inputs: Dict[str, Union[torch.Tensor, Any]]) -> torch.Tensor:
         """
         Perform a training step on a batch of inputs.
 
         Subclass and override to inject custom behavior.
 
@@ -1825,14 +2075,103 @@
         if self.do_grad_scaling:
             self.scaler.scale(loss).backward()
         else:
             loss.backward()
 
         return loss.detach() / self.args.gradient_accumulation_steps
 
+    def prediction_step(
+        self,
+        model: nn.Module,
+        inputs: Dict[str, Union[torch.Tensor, Any]],
+        prediction_loss_only: bool,
+        ignore_keys: Optional[List[str]] = None,
+    ) -> Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]:
+        """
+        Perform an evaluation step on `model` using `inputs`.
+
+        Subclass and override to inject custom behavior.
+
+        Args:
+            model (`nn.Module`):
+                The model to evaluate.
+            inputs (`Dict[str, Union[torch.Tensor, Any]]`):
+                The inputs and targets of the model.
+
+                The dictionary will be unpacked before being fed to the model. Most models expect the targets under the
+                argument `labels`. Check your model's documentation for all accepted arguments.
+            prediction_loss_only (`bool`):
+                Whether or not to return the loss only.
+            ignore_keys (`List[str]`, *optional*):
+                A list of keys in the output of your model (if it is a dictionary) that should be ignored when
+                gathering predictions.
+
+        Return:
+            Tuple[Optional[torch.Tensor], Optional[torch.Tensor], Optional[torch.Tensor]]: A tuple with the loss,
+            logits and labels (each being optional).
+        """
+        has_labels = False if len(self.label_names) == 0 else all(inputs.get(k) is not None for k in self.label_names)
+        # For CLIP-like models capable of returning loss values.
+        # If `return_loss` is not specified or being `None` in `inputs`, we check if the default value of `return_loss`
+        # is `True` in `model.forward`.
+        return_loss = inputs.get("return_loss", None)
+        if return_loss is None:
+            return_loss = self.can_return_loss
+        loss_without_labels = True if len(self.label_names) == 0 and return_loss else False
+
+        inputs = (
+            self.prepare_input(inputs, self.args.device)
+            if self.prepare_input is not None
+            else self._prepare_inputs(inputs)
+        )
+        if ignore_keys is None:
+            unwrapped_model = unwrap_model(self.model)
+            if hasattr(unwrapped_model, "config"):
+                ignore_keys = getattr(unwrapped_model.config, "keys_to_ignore_at_inference", [])
+            else:
+                ignore_keys = []
+
+        # labels may be popped when computing the loss (label smoothing for instance) so we grab them first.
+        if has_labels or loss_without_labels:
+            labels = nested_detach(tuple(inputs.get(name) for name in self.label_names))
+            if len(labels) == 1:
+                labels = labels[0]
+        else:
+            labels = None
+
+        with torch.no_grad():
+            if has_labels or loss_without_labels:
+                with self.autocast_smart_context_manager():
+                    loss, outputs = self.compute_loss(model, inputs, return_outputs=True)
+                loss = loss.mean().detach()
+
+            else:
+                loss = None
+                with self.autocast_smart_context_manager():
+                    outputs = model(**inputs)
+                # TODO: this needs to be fixed and made cleaner later.
+                if self.args.past_index >= 0:
+                    self._past = outputs[self.args.past_index - 1]
+
+            logits = None
+            if isinstance(outputs, dict):
+                logits = tuple(outputs.get(name) for name in self.logit_names)
+            else:
+                if self.args.logit_index >= 0:
+                    logits = (outputs[self.args.logit_index],)
+
+        if prediction_loss_only:
+            return (loss, None, None)
+
+        logits = nested_detach(logits)
+        if len(logits) == 1:
+            logits = logits[0]
+
+        return (loss, logits, labels)
+
     def _prepare_input(self, data: Union[torch.Tensor, Any]) -> Union[torch.Tensor, Any]:
         """
         Prepares one `data` before feeding it to the model, be it a tensor or a nested list/dictionary of tensors.
         """
         if isinstance(data, Mapping):
             return type(data)({k: self._prepare_input(v) for k, v in data.items()})  # type: ignore[call-arg]
         elif isinstance(data, (tuple, list)):
```

## atorch/utils/fsdp_init_util.py

```diff
@@ -1,22 +1,24 @@
 """This file is used to restore FlatParameter from flat ckpt."""
 import collections
 from dataclasses import dataclass
+from functools import partial
+from pathlib import Path
 from typing import Callable, List, Optional, Sequence, Tuple, Type, Union, no_type_check
 
 import torch
 from torch import nn
 from torch.distributed.fsdp import _init_utils, flat_param
 from torch.distributed.fsdp import fully_sharded_data_parallel as FSDP
 from torch.distributed.fsdp._common_utils import clean_tensor_name
 from torch.distributed.utils import _p_assert
 
 from atorch.common.log_utils import default_logger as logger
 from atorch.distributed.distributed import local_rank, rank, world_size
-from atorch.utils.fsdp_save_util import ErrorCode, FlatCkptError, ShardTensorUtil
+from atorch.utils.fsdp_save_util import _FLAT_PARAM_PADDING_VALUE, ErrorCode, FlatCkptError, ShardTensorUtil, TensorDict
 from atorch.utils.meta_model_utils import _find_tied_weights, _retie_weights
 
 OriginFlatParamHandle: Type[flat_param.FlatParamHandle] = flat_param.FlatParamHandle
 origin_init_param_handle_from_module = _init_utils._init_param_handle_from_module
 
 
 def patch_fsdp_init(ckpt_path, wrap_class, top_model, check_module=True, ignore_ckpt_version=False):
@@ -50,14 +52,20 @@
         _init_utils.FlatParamHandle = RestoreFlatParamHandle
     else:
         raise FlatCkptError(
             "Torch git version must equal 7bcf7da3a268b435777fe87c7794c382f444e86d(2.1.0)", ErrorCode.NOT_SUPPORT
         )
 
 
+def reset_hooks():
+    global _init_utils, FSDP
+    _init_utils.FlatParamHandle = OriginFlatParamHandle
+    FSDP._init_param_handle_from_module = origin_init_param_handle_from_module
+
+
 @dataclass
 class RestoreFlatParamHandleInjectConfig:
     """We inherit `FlatParamHandle` from FSDP, as we don't want to change any function signature of
     origin `FlatParamHandle`, so we use this to inject for configuring RestoreFlatParamHandle.
     All `RestoreFlatParamHandle` objects use same instance of `RestoreFlatParamHandleInjectConfig`.
 
     ckpt_path: flat ckpt path
@@ -230,24 +238,60 @@
             load_buffer()
             if orig_storage._size() > 0:
                 orig_storage._resize_(0)
         if self._use_orig_params:
             self._use_sharded_views()
 
 
+def _check_weight_is_init(module_name: str, module: nn.Module) -> None:
+    """
+    Check first param is 42 or not.
+    """
+    for name, p in module.named_parameters():
+        if p.view(-1)[0] == _FLAT_PARAM_PADDING_VALUE:
+            raise FlatCkptError(f"lora weight {module_name}.{name} is not init", ErrorCode.LORA_WEIGHT_INIT_ERROR)
+
+
+def _reset_lora_param(module: nn.Module, lora_cls: Tuple[type]) -> None:
+    """
+    Reset all lora params before FSDP init, this function is called in `FSDP._init_param_handle_from_module`.
+    This function is called after `FSDP.param_init_fn`.
+
+    It's useful when base model and lora model are init on meta device. We can load base model from ckpt, but
+    lora weights are maybe training from scratch, at this time, we do not know how them initialize. Peft offers
+    reset function in lora, but other lora method are not tested.
+    """
+
+    for name, m in module.named_modules():
+        if isinstance(m, lora_cls):
+            try:
+                m.reset_lora_parameters(m.active_adapter)  # type: ignore[attr-defined]
+            except Exception as e:
+                import peft
+
+                raise FlatCkptError(
+                    f"Reset lora weights error, your version of peft is {peft.__version}. Check the origin call stack",
+                    ErrorCode.LORA_RESET_WEIGHT_ERROR,
+                ) from e
+            _check_weight_is_init(name, m)
+
+
 @no_type_check
 def mock_init_param_handle_from_module_pt210(
     state: _init_utils._FSDPState,
     fully_sharded_module: nn.Module,
     device_id: Optional[Union[int, torch.device]],
     param_init_fn: Optional[Callable[[nn.Module], None]],
     sync_module_states: bool,
+    **atorch_hook_kwargs,
 ) -> _init_utils._FSDPState:
     """
-    We only add tie_weights after `materialize_meta_module`. Others are same with original function.
+    We two things, others are same with original function.
+        1. add tie_weights after `materialize_meta_module`.
+        2. add lora reset parameters
     """
     tie_weights = {}
     tie_weights = _find_tied_weights(fully_sharded_module)
 
     _init_utils._check_single_device_module(fully_sharded_module, state._ignored_params, device_id)
     device_from_device_id = _init_utils._get_device_from_device_id(device_id, state.rank)
     is_meta_module, is_torchdistX_deferred_init = _init_utils._need_to_materialize_module(
@@ -268,12 +312,191 @@
     state.compute_device = _init_utils._get_compute_device(
         fully_sharded_module,
         state._ignored_params,
         device_from_device_id,
         state.rank,
     )
 
+    wrap_cls = atorch_hook_kwargs.get("atorch_wrap_cls", int)
+    restore_lora = atorch_hook_kwargs.get("restore_lora", False)
+
+    if not restore_lora and isinstance(fully_sharded_module, wrap_cls):
+        # wrap cls fsdp unit
+        lora_cls = atorch_hook_kwargs.get("lora_cls", None)
+        _reset_lora_param(fully_sharded_module, lora_cls)
+
     managed_params = list(_init_utils._get_orig_params(fully_sharded_module, state._ignored_params))
+
+    if "atorch_wrap_cls" in atorch_hook_kwargs:
+        # check sync_module_states, and any param is 42
+        if not sync_module_states:
+            raise ValueError("FSDP lora on meta init must set `sync_module_states`", ErrorCode.LORA_WEIGHT_INIT_ERROR)
+        for p in managed_params:
+            if p.view(-1)[0] != _FLAT_PARAM_PADDING_VALUE:
+                continue
+            for name, param in fully_sharded_module.named_parameters():
+                if param is p:
+                    raise FlatCkptError(f"Weight {name} is not init", ErrorCode.LORA_WEIGHT_INIT_ERROR)
     if sync_module_states:
         _init_utils._sync_module_params_and_buffers(fully_sharded_module, managed_params, state.process_group)
     _init_utils._init_param_handle_from_params(state, managed_params, fully_sharded_module)
     return state
+
+
+@dataclass
+class FSDPCkptConfig:
+    """
+    This is use for meta init and use `param_init_fn` of FSDP to init params.
+    This object has three str:
+        1. flat_ckpt_path, dir of flat ckpt
+        2. lora_ckpt_path, dir of lora ckpt
+        3. lora_prefix, prefix of lora, 'base_model.model' as usually.
+        4. lora_cls, lora linear class, defaults to peft.tuners.lorr.Linear
+
+    """
+
+    flat_ckpt_path: Optional[str] = None
+    lora_ckpt_path: Optional[str] = None
+    lora_prefix: Optional[str] = None
+    lora_cls: Optional[List[type]] = None
+    lora_weight_name: Optional[str] = None
+
+
+class FSDPInitFn:
+    """
+    param_init_fn of FSDP.
+    """
+
+    def __init__(self, top_model: nn.Module, rank: int, fsdp_ckpt_config: FSDPCkptConfig, wrap_cls: Tuple[type]):
+        if not isinstance(wrap_cls, tuple):
+            raise FlatCkptError("kwarg `wrap_clas` of FSDPInitFn must be tuple of class", ErrorCode.COMMON_ERROR)
+        self._set_global_name_for_params_and_buffers(top_model)
+        self.rank = rank
+        self.fsdp_ckpt_config = fsdp_ckpt_config
+        self._prepare_ckpt()
+        self.wrap_cls = wrap_cls
+        self.restore_lora = fsdp_ckpt_config.lora_ckpt_path is not None
+
+        if rank == 0:
+            FSDP._init_param_handle_from_module = partial(
+                mock_init_param_handle_from_module_pt210,
+                atorch_wrap_cls=wrap_cls,
+                restore_lora=self.restore_lora,
+                lora_cls=self._prepare_lora_cls_check_list(),
+            )
+        else:
+            FSDP._init_param_handle_from_module = mock_init_param_handle_from_module_pt210
+
+    def _prepare_lora_cls_check_list(self):
+        """
+        We need to call `reset_lora_parameters` from class `LoraLinear`, maybe user will implement `lora` by
+        their own, so we pass lora class to filter which object can do `reset_lora_parameters`. defaults to
+        `peft.tuners.lorr.Linear`
+        """
+        from peft.tuners.lora import Linear as LoraLinear
+
+        self.lora_cls = [LoraLinear]
+        config_lora_cls = self.fsdp_ckpt_config.lora_cls
+        if config_lora_cls is not None:
+            self.lora_cls.extend(config_lora_cls)
+        self.lora_cls = tuple(self.lora_cls)
+        return self.lora_cls
+
+    def _prepare_ckpt(self):
+        """
+        Parse all ckpts
+        """
+        flat_ckpt_path = self.fsdp_ckpt_config.flat_ckpt_path
+        lora_ckpt_path = self.fsdp_ckpt_config.lora_ckpt_path
+        lora_prefix = self.fsdp_ckpt_config.lora_prefix
+
+        # we striped prefix which is created by lora, usually, it's  `base_model.model.`
+        self.base_model_weights = ShardTensorUtil(
+            flat_ckpt_path,
+            0,
+            1,
+            name_mapping_func_or_dict=lambda x: f"{x[len(lora_prefix)+1:]}" if lora_prefix else x,
+            device="cpu",
+        )
+        self.lora_weights = self._parse_lora_param(lora_ckpt_path)
+
+    def _get_param_buffer_from_flat(self, name) -> Optional[torch.Tensor]:
+        """
+        Get param or buffer from flat ckpt, if found return tensor, otherwise return None.
+        """
+        return self.base_model_weights.load_tensor_by_name(name, strict=False)
+
+    def _parse_lora_param(self, path: Optional[str]) -> TensorDict:
+        """
+        If we set path, it will find `lora_weight` in path.
+        If not found, raise error.
+        """
+        if path is None:
+            return {}
+        lora_weight_name = self.fsdp_ckpt_config.lora_weight_name or "lora_weight"
+        posix_path = Path(path) / lora_weight_name
+        if not posix_path.exists():
+            raise FlatCkptError(f"lora weights not found, path is {str(posix_path)}", ErrorCode.CHECKPOINT_NOT_FOUND)
+        return torch.load(posix_path)
+
+    def _set_global_name_for_params_and_buffers(self, top_model):
+        """
+        Set extra attr `_atorch_global_name` to record global name of each module.
+        It's useful when we iter on submodule.
+        """
+        for name, param in top_model.named_parameters():
+            param._atorch_global_name = name
+        for name, buf in top_model.named_buffers():
+            buf._atorch_global_name = name
+
+    def __call__(self, module: nn.Module) -> None:
+        """
+        Real param_init_fn at FSDP's initializing. FSDP must set `sync_module_states`.
+
+        For non root rank, empty init each module, and wait broadcasting from root rank.
+        For root rank, there are two cases:
+            1.  Lora weights will init from ckpt, in this case, if we not found key in lora_weight dict,
+                We raise error.
+            2.  Lora weights will init from scratch, in this case, we call `reset_lora_parameters` in peft,
+                `wrap_cls` will not be None, so we fill 42 on every param. Before broadcasting, check is any
+                param is 42 and raise error.
+        """
+        if self.rank != 0:
+            module.to_empty(device=torch.device("cuda"), recurse=False)
+            return
+        with torch.no_grad():
+            global_names = {name: param._atorch_global_name for name, param in module.named_parameters(recurse=False)}
+            global_names.update({name: buf._atorch_global_name for name, buf in module.named_buffers(recurse=False)})
+            module.to_empty(device=torch.device("cuda"), recurse=False)
+            for name, param in module.named_parameters(recurse=False):
+                full_param_name = global_names[name]
+                # lookup on flat ckpt
+                src_tensor = self._get_param_buffer_from_flat(full_param_name)
+                if src_tensor is not None:
+                    orig_storage = param._typed_storage()
+                    param.set_(src_tensor.cuda().contiguous())
+                    if orig_storage._size() > 0:
+                        orig_storage._resize_(0)
+                # lookup of lora ckpt
+                elif full_param_name in self.lora_weights:
+                    orig_storage = param._typed_storage()
+                    param.set_(self.lora_weights[full_param_name].cuda().contiguous())
+                    if orig_storage._size() > 0:
+                        orig_storage._resize_(0)
+                elif self.restore_lora:
+                    raise FlatCkptError(f"Missing lora weight {full_param_name}", ErrorCode.LORA_WEIGHT_INIT_ERROR)
+                else:
+                    # mark not initialized
+                    param.fill_(_FLAT_PARAM_PADDING_VALUE)
+
+            for name, buf in module.named_buffers(recurse=False):
+                full_param_name = global_names[name]
+                src_tensor = self._get_param_buffer_from_flat(full_param_name)
+                # lookup on flat ckpt
+                if src_tensor is not None:
+                    orig_storage = buf._typed_storage()
+                    if orig_storage._size() > 0:
+                        orig_storage._resize_(0)
+                    buf.set_(src_tensor.contiguous().cuda().to(buf.dtype))
+                else:
+                    # mark not initialized
+                    buf.fill_(_FLAT_PARAM_PADDING_VALUE)
```

## atorch/utils/fsdp_save_util.py

```diff
@@ -2,15 +2,15 @@
 import json
 import pickle
 import struct
 from collections import OrderedDict, defaultdict, deque
 from collections.abc import Mapping
 from enum import Enum, auto, unique
 from pathlib import Path
-from typing import Any, DefaultDict, Dict, List, Tuple
+from typing import Any, DefaultDict, Dict, List, Set, Tuple
 
 import safetensors
 import torch
 import torch.distributed as dist
 from packaging.version import Version
 from safetensors.torch import _SIZE, _TYPES, _tobytes, safe_open
 from torch.distributed.fsdp import FullyShardedDataParallel as FSDP
@@ -28,21 +28,27 @@
 
 from atorch.common.log_utils import default_logger as logger
 from atorch.distributed.distributed import local_rank, nproc_per_node, parallel_group
 
 TYPES_TO_STR = {v: k for k, v in _TYPES.items()}
 CKPT_VERSION = 1
 
+TensorDict = Dict[str, torch.Tensor]
+ListFSDP = List[FSDP]
+
 
 @unique
 class ErrorCode(Enum):
     NOT_SUPPORT = auto()
     CHECKPOINT_NOT_FOUND = auto()
     CHECKPOINT_CORRUPTION = auto()
     CHECKPOINT_WRAP_CLASS_MISMATCH = auto()
+    LORA_WEIGHT_INIT_ERROR = auto()
+    LORA_RESET_WEIGHT_ERROR = auto()
+    COMMON_ERROR = auto()
     UNKNOWN = auto()
 
     def __str__(self):
         return (
             f"{self.name} (Code: {self.value}), "
             "check https://yuque.antfin.com/ai-infra/atorch-doc/axb2ce53hitd72kg#fDGSW"
         )
@@ -234,32 +240,147 @@
             'flat_numel': 26806272
         }
     """
     params, buffers, metas, ckpt_meta = get_flat_model_param(model)
     _persist_flat_model_param(path, params, buffers, metas, ckpt_meta)
 
 
-def get_flat_model_param(model):
+def _get_fsdp_units_for_saving(model) -> Tuple[ListFSDP, Set]:
+    """
+    Get all fsdp units which is requires_grad. return units and module name.
+    """
+    check_is_support(model)
+    fsdp_units = [
+        m
+        for m in model.named_modules()
+        if isinstance(m[1], torch.distributed.fsdp.fully_sharded_data_parallel.FullyShardedDataParallel)
+    ]
+    requires_grad_params = set()
+
+    has_grad_fsdp_units = []
+    for fsdp_name, fsdp_unit in fsdp_units:
+        fsdp_flat_handle = get_handle(fsdp_unit)
+        flat_param = fsdp_flat_handle.flat_param
+        if not flat_param.requires_grad:
+            continue
+        for name, param in fsdp_unit.named_parameters():
+            if param.requires_grad:
+                requires_grad_params.add(f"{clean_tensor_name(fsdp_name)}.{clean_tensor_name(name)}")
+        has_grad_fsdp_units.append((fsdp_name, fsdp_unit))
+    return has_grad_fsdp_units, requires_grad_params
+
+
+def get_lora_param(model) -> Tuple[TensorDict, Dict]:
+    """
+    Parse lora param from flat param.
+    Return param and shape info in dict.
+    """
+    metas: Dict[str, torch.Size] = {}
+    params: Dict[str, torch.Tensor] = {}
+    has_grad_fsdp_units, requires_grad_params = _get_fsdp_units_for_saving(model)
+    for fsdp_name, fsdp_unit in has_grad_fsdp_units:
+        fsdp_flat_handle = get_handle(fsdp_unit)
+        meta = fsdp_flat_handle.shard_metadata()
+        flat_param = fsdp_flat_handle.flat_param
+        name = f"{clean_tensor_name(fsdp_name)}" if fsdp_name else ""
+        keys, items = list(zip(*meta._asdict().items()))
+        items = list(zip(*items))
+        data = list(dict(zip(keys, i)) for i in items)
+        shard_info_in_this_rank = [i for i in flat_param._shard_param_infos if i.in_shard]
+        if len(shard_info_in_this_rank) != len(data):
+            raise ValueError("flat param mismatch")
+        for shard_info, each in zip(shard_info_in_this_rank, data):
+            global_name_each = (
+                [name, clean_tensor_name(each["param_names"])] if name else [clean_tensor_name(each["param_names"])]
+            )
+            global_name = ".".join(global_name_each)
+            if global_name in requires_grad_params:
+                s = slice(shard_info.offset_in_shard, shard_info.offset_in_shard + shard_info.numel_in_shard)
+                params[global_name] = flat_param[s].detach().clone().cpu()
+                metas[global_name] = each["param_shapes"]
+    return params, metas
+
+
+def _post_processing_lora_weight(path, lora_weight_name=None) -> None:
+    """
+    Merge all lora_weight shards into single file, and delete all shard files.
+    Final weight file is called `lora_weight`, name of shard's pattern is lora_weight_shard.rank-world_size.
+    ckpt
+    ├── lora_weight
+    ├── lora_weight_shard.00000-00004
+    ├── lora_weight_shard.00001-00004
+    ├── lora_weight_shard.00002-00004
+    └── lora_weight_shard.00003-00004
+    """
+    weight_files = sorted(glob.glob(f"{path}/lora_weight_shard*"))
+    weight_meta_files = sorted(glob.glob(f"{path}/lora_meta*"))
+    weights = [torch.load(i) for i in weight_files]
+    weight_metas = [torch.load(i) for i in weight_meta_files]
+    merged_weights = defaultdict(list)
+    merged_meta = {}
+    for weight, meta in zip(weights, weight_metas):
+        for name, w in weight.items():
+            merged_weights[name].append(w)
+            if name in meta:
+                merged_meta[name] = meta[name]
+    final_weight = {k: torch.cat(v).reshape(merged_meta[k]) for k, v in merged_weights.items()}
+    lora_weight = lora_weight_name or "lora_weight"
+    torch.save(final_weight, f"{path}/{lora_weight}")
+    for f in weight_files + weight_meta_files:
+        Path(f).unlink(missing_ok=True)
+    dist.barrier()
+
+
+def save_lora_param(model, path, lora_weight_name=None) -> None:
+    """
+    Each rank save part of lora weights, and merge into single weights.
+    Dues size of lora is small, we do not save lora weight in sharding format.
+    """
+    d = Path(path)
+    d.mkdir(parents=True, exist_ok=True)
+    params, metas = get_lora_param(model)
+    data_group = parallel_group("data")
+    rank = dist.get_rank(data_group)
+    world_size = dist.get_world_size()
+    torch.save(params, f"{path}/lora_weight_shard.{str(rank).zfill(5)}-{str(world_size).zfill(5)}")
+    torch.save(metas, f"{path}/lora_meta.{str(rank).zfill(5)}-{str(world_size).zfill(5)}")
+    dist.barrier()
+    if rank == 0:
+        _post_processing_lora_weight(path, lora_weight_name)
+    else:
+        dist.barrier()
+
+
+def save_lora_optim_param(model, optimizer, path, lora_weight_name=None) -> None:
+    """
+    Optim of lora is small too, we save full optim state.
+    """
+    optim_state = FSDP.full_optim_state_dict(model, optimizer)
+    d = Path(path)
+    d.mkdir(parents=True, exist_ok=True)
+    data_group = parallel_group("data")
+    rank = dist.get_rank(data_group)
+    if rank == 0:
+        lora_weight = lora_weight_name or "lora_optim"
+        torch.save(optim_state, f"{path}/{lora_weight}")
+
+
+def get_flat_model_param(model) -> Tuple[TensorDict, TensorDict, Dict, Dict]:
     """
     Get flat param and meta info of each fsdp units.
     This is only working on `use_orig_param` is True.
 
     Returns:
         params (dict[str, flat_param]): the parameters of FSDP units.
         buffers (dict): from model.named_buffers().
         metas (dict): contains flat_param_meta and param_meta.
         ckpt_meta: the meta of checkpoint contains the version and the world size.
     """
-    check_is_support(model)
-    fsdp_units = [
-        m
-        for m in model.named_modules()
-        if isinstance(m[1], torch.distributed.fsdp.fully_sharded_data_parallel.FullyShardedDataParallel)
-    ]
-    metas = {"flat_param_meta": {}, "param_meta": {}}
+    fsdp_units, _ = _get_fsdp_units_for_saving(model)
+    metas: Dict[str, dict] = {"flat_param_meta": {}, "param_meta": {}}
     param_meta = metas["param_meta"]
     flat_param_meta = metas["flat_param_meta"]
     params = {}
     data_group = parallel_group("data")
     buffers = {clean_tensor_name(k): v for k, v in model.named_buffers()}
     wrap_class = set()
     for fsdp_name, fsdp_unit in fsdp_units:
@@ -279,18 +400,18 @@
         each_flat["numels"] = flat_param._numels
         each_flat["flat_numel"] = flat_param.numel()
         each_flat["numels_with_padding"] = flat_param._numels_with_padding
         each_flat["is_padding_mask"] = flat_param._is_padding_mask
         flat_param_meta[name] = each_flat
         for shard_info, each in zip(shard_info_in_this_rank, data):
 
-            global_name = (
+            global_name_each = (
                 [name, clean_tensor_name(each["param_names"])] if name else [clean_tensor_name(each["param_names"])]
             )
-            global_name = ".".join(global_name)
+            global_name = ".".join(global_name_each)
             each["pad"] = pad
             each["rank"] = dist.get_rank(data_group)
             each["striped_fsdp_name"] = name
             each["param_offsets"] = (shard_info.offset_in_shard, shard_info.offset_in_shard + shard_info.numel_in_shard)
 
             param_meta[global_name] = each
         params[name] = flat_param
@@ -932,7 +1053,17 @@
         torch.cuda.synchronize(torch.cuda.current_device())
         tensor = torch.cat(shards)
         return tensor.reshape(ori_shape)
 
     def __del__(self):
         for g in self.local_gpus_groups:
             dist.destroy_process_group(g)
+
+
+def ConvertFlatParam(ckpt_path) -> Dict[str, TensorDict]:
+    """
+    Convert flat ckpt to single dict.
+    """
+    util = ShardTensorUtil(ckpt_path, 0, 1, device="cpu")
+    buffers = {i: util.load_tensor_by_name(i) for i in util.buffers.keys()}
+    params = {i: util.load_tensor_by_name(i) for i in util.param_meta.keys()}
+    return {"params": params, "buffers": buffers}
```

## atorch/utils/patch_te.py

```diff
@@ -1,23 +1,24 @@
 # mypy: ignore-errors
-from importlib import metadata
 from typing import Any, Callable, Dict, Tuple, Union
 
 import torch
 from transformer_engine.pytorch.constants import dist_group_type
 from transformer_engine.pytorch.distributed import (
     CheckpointFunction,
     _set_cuda_rng_state,
     activation_recompute_forward,
     detach_variable,
     gather_split_1d_tensor,
     safely_set_viewless_tensor_data,
     split_tensor_into_1d_equal_chunks,
 )
 
+from atorch.utils.version import package_version_smaller_than
+
 
 def te_checkpoint_forward(
     ctx,
     run_function: Callable,
     distribute_saved_activations: bool,
     get_cuda_rng_tracker: Callable,
     tp_group: dist_group_type,
@@ -125,10 +126,10 @@
     torch.autograd.backward(outputs_with_grad, args_with_grad)
     grads = tuple(inp.grad if isinstance(inp, torch.Tensor) else None for inp in detached_inputs)
     return (None, None, None, None, None) + grads
 
 
 def patch_te_if_needed():
     # patch checkpoint if te version < 1.3
-    if metadata.version("transformer_engine") < "1.3":
+    if package_version_smaller_than("transformer_engine", "1.3"):
         CheckpointFunction.forward = te_checkpoint_forward
         CheckpointFunction.backward = te_checkpoint_backward
```

## atorch/utils/version.py

```diff
@@ -1,12 +1,14 @@
 import logging
 import re
+from importlib import metadata
 from typing import List, Tuple, Union
 
 import torch
+from packaging.version import Version
 
 __all__: List[str] = ["torch_version"]
 
 
 # Adopted from Fairscale
 def torch_version(
     version: str = torch.__version__, return_dev: bool = False
@@ -41,7 +43,12 @@
 
 def get_version(package):
     version = package.__version__
     numbering = version.split(".")
     vs = [get_digit_part(x) for x in numbering]
     digits = [int(x) if x != "" else "" for x in vs]
     return tuple(digits)
+
+
+def package_version_smaller_than(pkg_name, version):
+    pkg_v = metadata.version(pkg_name)
+    return Version(pkg_v) < Version(version)
```

## Comparing `atorch-0.1.8.data/data/acceleration.proto` & `atorch-0.1.9.data/data/acceleration.proto`

 * *Files identical despite different names*

## Comparing `atorch-0.1.8.dist-info/METADATA` & `atorch-0.1.9.dist-info/METADATA`

 * *Files 19% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: atorch
-Version: 0.1.8
+Version: 0.1.9
 Summary: A pytorch extension for efficient deep learning.
 Home-page: https://github.com/intelligent-machine-learning/dlrover/tree/master/atorch
 Author: Ant Group
 Requires-Python: >=3.8
 Requires-Dist: fairscale ==0.4.1
 Requires-Dist: apex
 Requires-Dist: flash-attn
-Requires-Dist: deepspeed ==0.10.0
-Requires-Dist: transformers ==4.31.0
+Requires-Dist: deepspeed ==0.10.3
+Requires-Dist: transformers >=4.31.0
 Requires-Dist: networkx
 Requires-Dist: pyomo
 Requires-Dist: pynvml ==11.4.1
-Requires-Dist: grpcio ==1.34.1
-Requires-Dist: grpcio-tools ==1.34.1
-Requires-Dist: fsspec ==2023.10.0
+Requires-Dist: fsspec
+Requires-Dist: grpcio ==1.62.1
+Requires-Dist: grpcio-tools ==1.58.0
 Requires-Dist: pyarrow ==12.0.0
 Requires-Dist: pandas ==2.0.1
-Requires-Dist: tensorboard ==2.11.0
-Requires-Dist: dlrover[torch] ==0.4.0
-Requires-Dist: protobuf ==3.20.3
+Requires-Dist: tensorboard ==2.14.0
+Requires-Dist: dlrover[torch] ==0.3.6
+Requires-Dist: protobuf ==4.25.3
 Requires-Dist: safetensors
 Requires-Dist: GPy
 Requires-Dist: pymoo ==0.5.0
+Requires-Dist: grouped-gemm
+Requires-Dist: megablocks
 
 ATorch supports efficient and easy-to-use model training experience. ATorch provides performance optimizations in aspects such as I/O, preprocessing, computation, and communication (including automatic optimization), and has supported large-scale pretraining and finetuning of LLMs with over 100 billion parameters and thousands of advanced GPUs.
```

## Comparing `atorch-0.1.8.dist-info/RECORD` & `atorch-0.1.9.dist-info/RECORD`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 atorch/amp/pipe_amp.py,sha256=ky_0Yi4jKLHo97CZw4UpPcwydziG6jq1kUXoOcM2SuY,12488
 atorch/auto/__init__.py,sha256=5GppCkqhC0MXbVndBHGKCk0XhHr6vFvBXwsA1EcBylM,83
 atorch/auto/accelerate.py,sha256=n6AWTUs6LbDOZE9HjC1evQ7S6PGbFIKTYF0yUpIyDj4,28847
 atorch/auto/auto_accelerate_context.py,sha256=vGul6an9wE6lAh2WXx9aamVjpSmC-1bcwL-XWE5JkPs,1095
 atorch/auto/clip_grad_norm.py,sha256=sPw4Jv0DTdRIZiI1oWe13usjxmXl5_6aa1wtkiTVjX8,13550
 atorch/auto/device_context.py,sha256=HOiizEAEhHFZIHvJK0JPCasyNmutanmd_nLCL9CJhuw,6456
 atorch/auto/engine_client.py,sha256=2L3rBUDPLFGZJx4nYjm2Sx3t-Dkzu-q4pO8DpYbAeGo,2480
-atorch/auto/model_context.py,sha256=J7qzhy4zXq_ITxQ7Ejvbhl6eZZofOO7-_lym8f3anso,37647
+atorch/auto/model_context.py,sha256=a0dOo9Q960EMohZVONQOaYnPXlX6QPbcXGpPH3_yvgo,38252
 atorch/auto/strategy.py,sha256=BTDVlv_hNgZX0rZ0-_ouZkGVpV6VG0AWAAI7qVEvUQo,4803
 atorch/auto/task.py,sha256=tTf8f8FJB4klUgKGbAFM7mEz3FuvZ-Mgg_bjy3TdNbI,468
 atorch/auto/analyser/__init__.py,sha256=4C4jMmmfnkX-s4eyoK_SuOUpTwNwABJ__9wHjaNips8,31
 atorch/auto/analyser/analyser.py,sha256=wtJryeGZqLe17UyUeBeuDf8Cu4OAUhyfVTCSOWNkmw0,12008
 atorch/auto/dry_runner/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/auto/dry_runner/dry_runner.py,sha256=m4Pq0sq9p0YzimoVv_4V8zCCOGsS0N9A4ulCnneQieM,6435
 atorch/auto/engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -58,41 +58,35 @@
 atorch/auto/opt_lib/amp_optimization.py,sha256=GIDWzeOTmmgIgIALTZKcSqwhIiPungNCgVJo6USAoOY,16692
 atorch/auto/opt_lib/checkpoint_optimization.py,sha256=tVAkRpxh0f7RZxZ-7-_RdRvlerM9jZYrFyfxfSTIULI,10362
 atorch/auto/opt_lib/ds_3d_parallel_optimization.py,sha256=kt6LltZWUGewT00MlwrFuKZN07dO0dKeZf-r6pyCpSE,7195
 atorch/auto/opt_lib/dynamo_backends.py,sha256=nASqKJuDiGzaHH1rsYrHA8TJv7oUA-8ozKb-nSPRJLs,356
 atorch/auto/opt_lib/dynamo_optimization.py,sha256=i4G91wNn-VzTSb27uVqe1vhftkvTTxvgE43AHHf9eyA,2639
 atorch/auto/opt_lib/half_optimization.py,sha256=O18VK70CTD03olzJm568DDaECG7i1shDHHjL_FVxrZ4,1856
 atorch/auto/opt_lib/mixed_parallel_optimization.py,sha256=T7EsDOzMX86ZuPb7GtDDwz6Wc-BGHFPeb0fZq_IrDTM,13786
-atorch/auto/opt_lib/module_replace_optimization.py,sha256=MHGTFm2UsUojaAz6LIHqEMSTDXehvwGjmHWun_PAxlY,7217
+atorch/auto/opt_lib/module_replace_optimization.py,sha256=ThENHetqSBFGzzx4ilAyiTSv6wSANVbwVdwSPVhq5ZM,7426
 atorch/auto/opt_lib/optimization.py,sha256=OKO5uf_W8mvj0xzeRLJws4PxeTm07Te06N9z1n7-Qp8,10892
-atorch/auto/opt_lib/optimization_library.py,sha256=6khls3p-kyzb4KcMHASVVri9zf9BB0iffhHZAYoOoZg,2787
+atorch/auto/opt_lib/optimization_library.py,sha256=fQbkzbLP_XnZV4In9pGGb_wu8to8gCNFGmn4noyCtNI,2921
 atorch/auto/opt_lib/parallel_mode_optimization.py,sha256=f-UylUODH1tpEXQvZNB55N773nIjRfMN8XnxoyrjJHo,2112
 atorch/auto/opt_lib/pipeline_parallel_optimization.py,sha256=062_oAxSiCv9vXE6UEHfV90wb2KCeo4QWWs19EJhgjs,11721
 atorch/auto/opt_lib/selective_offloading_checkpoint.py,sha256=6hskQusHkWk1WaehMQUb-QUT2sRlOEc6nvRyrw0qaQs,10728
+atorch/auto/opt_lib/sequence_parallel_optimization.py,sha256=xZgbuEOGTjrujQURROIHf4AUo7nQAk-xbc3onqCl4H8,4955
 atorch/auto/opt_lib/tensor_parallel_optimization.py,sha256=uD4hkk8zzTuBTrJoM0IXVqqExIPrKfUfTQ1OHEDeGI8,7992
 atorch/auto/opt_lib/utils.py,sha256=7Ghc12Oduc4jTkl_LSMDIdUsgBCu2av9CYr_t0cN9ZU,6182
-atorch/auto/opt_lib/zero_optimization.py,sha256=jcvxpIRI--SzSeM87-UyIczgRK21PLfk14Q9AQM5k90,22731
+atorch/auto/opt_lib/zero_optimization.py,sha256=PHnpixBVSDDvfgmiWBRns9JKK-Jm9fUZmdNCAk7dCg0,23126
 atorch/auto/opt_lib/shard_planners/__init__.py,sha256=TbUvdmFvOAKiwJrh36y9G6tkW9N8TWOVyWt3vHnbxAg,241
 atorch/auto/opt_lib/shard_planners/base_stage_planner.py,sha256=EhgthFiK1PuCu24mJJ9TIp90Q6GjYgSkAFcdpZm676Q,5145
 atorch/auto/opt_lib/shard_planners/base_tp_planner.py,sha256=TX6Z-R3C_nI_OHF5R1KDo5ooeVWNMX7oL3PzyF4pHnE,9408
 atorch/auto/opt_lib/shard_planners/dim_planner.py,sha256=ORKrzIWX0NsRgbpuHS5rEVDfYhFcDGxjcqMayCVW_eU,8974
 atorch/auto/opt_lib/shard_planners/mip_tp_planner.py,sha256=tv53ovNNDQF5dm6yAm5Y9cxeWzGi9r4KnFwSAiDBQ4M,22977
 atorch/auto/opt_lib/shard_planners/topology.py,sha256=cUR8kaHlZu00CjEmQ3UYf1Qkuj_sRU2eFwT3WSW53WM,3471
 atorch/auto/opt_lib/shard_planners/utils.py,sha256=msJUuzpGHqQZxjNbNLh3zFuGWGaHhK2oYqKNdlf7b4c,26926
 atorch/common/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/common/constants.py,sha256=1vsxKPDJ4QDw9jEvtBQDSY39cM2PwTpKNuWVc_UjISI,3383
 atorch/common/log_utils.py,sha256=GKPY2F5HX58PHH3h8ytZPTELN9gc_HUTFsAt_m6ZixU,3340
-atorch/common/util_func.py,sha256=6Qea8NDi-mLOc3Qbd-ysVlGUqeBvsvRxf2mP4KS2F0s,6077
-atorch/common/file/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atorch/common/file/file_io.py,sha256=9BgUxdh7o9KEGnuFguhLkIt-lsfJxdRmJNs6BPJOZ-g,845
-atorch/common/file/file_system/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atorch/common/file/file_system/file_system.py,sha256=DPbmj-JhiwS83YBo1pVIuoymzqf_VPW06134Scdwmxg,4991
-atorch/common/file/file_system/pangu/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atorch/common/file/file_system/pangu/fsspec_instance.py,sha256=VzfKkeMjMZLSRjRdU_dkNqlGXtMXbkcGY3DP7SMHukY,13710
-atorch/common/file/file_system/pangu/pangu_file_system.py,sha256=EgPDOkdpoOBBI71MA4qXWXm3AR2A_DOpUzU98RDKT8U,17043
+atorch/common/util_func.py,sha256=dJGO3ZpB2ZYkQ3BQVs3324o6sO8sUZU9XpugooGR64o,6072
 atorch/data/__init__.py,sha256=mHv0gvkEvucRaZmC8KmzTabD4Tz-OIScrEgAr57hqG4,633
 atorch/data/coworker_dataset.py,sha256=b4iPlNloD0IAXEmIF7IJ5Y5hCly2HeVokeGcgNMy-R8,17310
 atorch/data/data_utils.py,sha256=yBhMkvUusMKQ29evN1bM1_EXUj0B2sxcgLmD8pZpUfc,1347
 atorch/data/elastic_dataloader.py,sha256=mrSDrWTLxehdCRnzhqokNGBB794zAKjZUQiQ-Dd9Qzk,13694
 atorch/data/elastic_dataset.py,sha256=xOU70QiUwvtrExfgoKF4dXwcofEtNg4IiolOO9xrTNM,4771
 atorch/data/preloader.py,sha256=hkYVHJ22dE7bPV9TNOO6ihmDWVqPkPtRw3_mi87rUXQ,6113
 atorch/data/shm_context.py,sha256=iUwp3xcoXknGf-CLizR0qkVFy4xcPx3SqdDFHUFx3HE,27904
@@ -100,25 +94,35 @@
 atorch/data/unordered_dataloader.py,sha256=fMRrCPK5tzEPEFsVl7glxKjav6k5rKtRp1t4HYFfwy4,3396
 atorch/data/unshuffled_batch_dataloader.py,sha256=-mYLnymYcnoWdWovRNkfSW_96yK6GgTdz8285tenzsc,1425
 atorch/data_parallel/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/data_parallel/adp.py,sha256=-lw6ABlDyPiRePMZ_7s6dG09rNW6ewGImQaIaIk4bGU,25559
 atorch/data_parallel/auto_wrap.py,sha256=720Ewtqw07xI4g1CxRsnof0WmyOydXPfeDqqXpG-_Sg,13332
 atorch/data_parallel/wrapper.py,sha256=oarEzeRLlcMWpWidiZaiOifZINUqWwEIeSQabxNKcx4,3562
 atorch/data_parallel/zero_ddp_mix_112.py,sha256=-THdMHvXANJgGq0EeVBbf1_wQdzVfuScx4VCeQvTboo,25890
-atorch/distributed/__init__.py,sha256=VzPm1UfPpoMP6_XMZHNK-PblQcOg6egxEacU8BgISf8,261
-atorch/distributed/distributed.py,sha256=A7N7yJX62YOlkmYhZ6DVzCUSfKdmskXYtJJ0V-G2gvo,28079
-atorch/distributed/elastic_controller.py,sha256=qyy8BHCOIhtHIje-a6d_O-BkRYL31M251WT1DVqB9NQ,465
-atorch/distributed/elastic_trainer.py,sha256=V8KJdKdHuiEe_BRoMEdbVXE38cCpO0j9aMRGr9dqujY,3405
+atorch/distributed/__init__.py,sha256=NA5CrUsHZeEthl7-Sr-xmexiqaVL_ISOLcIFfs4JgQ0,473
+atorch/distributed/distributed.py,sha256=_46YHGxsm9FzXxyYBRrC2ALJnXHrmYZ5GC2Xj3oD2DM,30705
+atorch/distributed/elastic_controller.py,sha256=pH6LZJHcHFlAvpLEoW6Ofr-n_ZZS7yFrLAEdRIGDqTQ,465
+atorch/distributed/elastic_trainer.py,sha256=qVTb-_UEpVnSi8ZsOQ77Eblj9soahrVyG6FNZuja0TM,3563
 atorch/distributed/hooks.py,sha256=7KQNyYtDU6XrekztrKQQz31S-JagyPjZ8OA-6BVNWNA,1253
 atorch/distributed/launch.py,sha256=sAWY0P5AMxOz2cQSg8Niuhe1tY3BtVSjw4CCPaISClw,19071
 atorch/distributed/run.py,sha256=llXERdpqNg2YBdp6tDMdnHNKmaEF9Z1Nq3ATnb_iWIo,12424
 atorch/fault_tolerance/__init__.py,sha256=4upTsfblcbQZxgCnUYEpvA3ALhjPqUkkGEcqkzNnjpg,68
 atorch/fault_tolerance/api.py,sha256=wLXxCJRm8dkPEAjZbarGh2pldfOxdnpMvqOwr2SlBes,4825
 atorch/fault_tolerance/custom_agent.py,sha256=x_PpQGG4Hvopic2W9y78rtrBmsb8MI86F1mKln27XQI,8293
 atorch/fault_tolerance/hanging_detector.py,sha256=tYFGtHKAgZN-BBRG09QbsUCLEBndDK5UuludpFYpecw,5659
+atorch/local_sgd/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
+atorch/local_sgd/HSDP/__init__.py,sha256=QYtmPPCku5-zesjp4UpynD4s1LXRrfSQoDsk_jsh160,1579
+atorch/local_sgd/HSDP/_init_utils.py,sha256=EEc4-nJHKXtvQpUIfAGsIr3Kihj_RelGkLqddC1RTac,13452
+atorch/local_sgd/HSDP/_runtime_utils.py,sha256=ThiOZSBQCb7hnz47jw2-y2KWZzzP7kkmbhADfujLLjA,21594
+atorch/local_sgd/HSDP/_state_dict_utils.py,sha256=SjthyeD7elYtAzv-1nkCXraoBHh9WD3ZHf4qKBKwNyw,22339
+atorch/local_sgd/reduce_methods/__init__.py,sha256=WJ-hXV_ptXks0o2I_Dk9okkiXmRFi6QSzdyzitJ-qDc,86
+atorch/local_sgd/reduce_methods/base.py,sha256=liz4Ej8h9uGSq4Z-HMShYXZnrZBjC0_ZLOkixBfVu3I,1054
+atorch/local_sgd/reduce_methods/generalized_task_arithmetic.py,sha256=7R5PLQv6MggbyurvpuRbJPaOAc0rVkliJGeZu2ZdmKI,3503
+atorch/local_sgd/reduce_methods/linear.py,sha256=TeSfJBFty92Obit2M5Lj-7aDUw3hWwOs4PKm_K05_IU,1034
+atorch/local_sgd/reduce_methods/sparsify.py,sha256=MBx3Q-p_duEnss12739Hlgiikg9UE4lY6dBBTZNfJkk,1815
 atorch/modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/modules/distributed_modules/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/modules/distributed_modules/activation_checkpointing.py,sha256=DtKP5ByzmZ4Qv5Lf0XUo-eeVElVgtodR6Sk-TE0Lt7U,14763
 atorch/modules/distributed_modules/cross_entropy.py,sha256=2vO4JXfsaNly-car7z7oAVQwkjlHBQ7u5maz0ohtS5I,5688
 atorch/modules/distributed_modules/layers.py,sha256=Gmy1QAASienm74iSrKfzK91EFCZjhKwfmdtkuVCfER4,29411
 atorch/modules/distributed_modules/mappings.py,sha256=9BQH-Sf5ZaXWQ8_Vg6B3Oe-7O2czC1KCCG42TW1tIE0,16790
 atorch/modules/distributed_modules/mappings_registry.py,sha256=j2a56W0lOQxwchJVM3n6gMPZgDkFym2NGP92UCsP8OA,7633
@@ -137,23 +141,25 @@
 atorch/modules/distributed_modules/compilers/tp_compiler/dtensor_compiler.py,sha256=wIw4OrXfdHMKDHizVkXOM8nRUycdWIWptehJIniihNI,222
 atorch/modules/distributed_modules/compilers/tp_compiler/tp_compiler.py,sha256=M5uymcUECFf-fkd1-BYjmLyY1bQpOgFQW8QVmP37gsI,7707
 atorch/modules/distributed_transformer/__init__.py,sha256=LVuyK4aCir9zRsde-RvMFRNUSb-zTeGN5fcS36nt460,80
 atorch/modules/distributed_transformer/commu_utils.py,sha256=ljzY1lpNjdEzwfCg3GbO6x4IyCJejlawXAKwWXOh4hI,3173
 atorch/modules/distributed_transformer/distributed_attention.py,sha256=LCMkkcsmvRCdPhnmWJGSAJ6t8rmGQO6JPcmbA3ghl8E,14623
 atorch/modules/moe/__init__.py,sha256=ddTRkRFLvmEws66--QiOx-dKT4mdKd_8-Q3TxBjjwBM,295
 atorch/modules/moe/ddp.py,sha256=xhYn6xEzkzkoEY1g8hS8zYNj_U-OkAb9orx5xPzSgvA,16005
+atorch/modules/moe/grouped_gemm_moe.py,sha256=QFrLz7avLJea9U0vrvHIa_D8DEcTd3mG7vt22-1Qfsc,4707
 atorch/modules/moe/inject.py,sha256=njrdSMjILOL1WJZwZFJxROaHNoSiuF7R4tlU1yQyHfM,4291
 atorch/modules/moe/moe_layer.py,sha256=PQ4eIZx81JcUO-D-UbLnIpQAmpSJuzpje4FhFUhUJvA,25005
+atorch/modules/moe/ops.py,sha256=RQVU_EXYwt8tFPB--OdNqCcoh7r6D6x872yhYMGb9wQ,4512
 atorch/modules/moe/switch_gating.py,sha256=1OfKZFJ9YrfvQKJCUUnoqiHAblM1sAavRka8uzzRmkk,6683
 atorch/modules/moe/topk_gating.py,sha256=BTScyg2dkt3WcX5w_ojzTBgvaDbsiT7mSKr7tKw0B4o,5799
 atorch/modules/transformer/__init__.py,sha256=8jGPBsMO4Yc-rsAO2CfZ_dn9kIu_8faBo4b3lTE7rm4,37
 atorch/modules/transformer/_fa_api_compat_patch,sha256=iOfGTPpaTarJ4hVaS6VoQKK7iDpn7N2LUwgAhlASn78,5210
 atorch/modules/transformer/cross_entropy.py,sha256=Xv32RhMM53jCLrhu12MEEShzwY9-9YpzJwElZoqAqZA,13580
 atorch/modules/transformer/inject.py,sha256=0AVocffvENX0ppvXV8EarYhvmRw8yQiUKtAeK2qVSfE,8248
-atorch/modules/transformer/layers.py,sha256=ua6S8q-rT8EALWypxOJITAod4zmO4l07pLl-MgWHJ3o,67467
+atorch/modules/transformer/layers.py,sha256=t7LKTuW9T-IKIQUbCBlgNp0b-0tw3Bo50NChWl2vlpw,67409
 atorch/modules/transformer/linear.py,sha256=p2bu3WT-dyvwWxdIYhpFlTxuFeV-cqQrUgs-y7zEk0o,2682
 atorch/modules/transformer/losses.py,sha256=sbMsYmzqZFArbHFIGh-1EOhzjXEBZJQTvk7q7Yh2cow,374
 atorch/mup/__init__.py,sha256=T5q60GRUstHUYwNSsoIsGsDOVcs7C5UlDLborv5CpTE,244
 atorch/mup/infshape.py,sha256=QOolFbJkTInt-Mr77RzrRHOIjFx6sCJLE5VBT9tTBUQ,4232
 atorch/mup/init.py,sha256=QZKlSX8YIWNyHc_3KmjyahAfbAA27gSk-nZbM0_w0tk,8553
 atorch/mup/module.py,sha256=5vLI9NGAVO-S3D8-ZI54W2svq70sYwRN_w7Aq5_WAhM,11021
 atorch/mup/optim.py,sha256=X4SdpBKh7588kLWEnEXM7DXVNVl3-14tFY-4CMTNDbw,5867
@@ -161,15 +167,15 @@
 atorch/normalization/__init__.py,sha256=jS_nSmlS1t03tY1Kvt84e-XU6aURJf2xMqWOAnsWorI,455
 atorch/normalization/layernorm.py,sha256=YlQ9TP3yN5289T6CauqgkmxPQqq7YkmJxpVn9JiEF9I,9000
 atorch/npu/__init__.py,sha256=j9kJhxhFccrmIpJYN_5rUUWawVArR0KLtcVWZ7qNOVA,2681
 atorch/npu/layers.py,sha256=H-d9jQlA67nbh0XpzFUMH_Nm0CjNwFc1nv8jknPDyhc,6090
 atorch/npu/optim.py,sha256=1lbnfV1xiEb55091M9Hyhi3SqISs1KbtNr-gGjdMtZg,7676
 atorch/ops/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/ops/git_version_info.py,sha256=0UWHC_5zh71LNENaFWCacCsC4PsbHi3gKOihQBLmzeM,950
-atorch/ops/git_version_info_installed.py,sha256=M5V245OTobrxnMBjsmJsFieeKSSlD_JPq6DVv-jWztM,347
+atorch/ops/git_version_info_installed.py,sha256=a3P6kGdY8eh_HaXKBA_tYD862S--S5vWt0zGSm2JgIc,355
 atorch/ops/accelerator/__init__.py,sha256=gWQg_tMCqUv4mjGYxXV-C314BDS4IEdLEV4rGPwfXUI,271
 atorch/ops/accelerator/abstract_accelerator.py,sha256=Bz7eo_CCRCr_V3eO_8xw7aL1WqVftUU-M5cd5e6qzHQ,4732
 atorch/ops/accelerator/cuda_accelerator.py,sha256=LFvghhqUrL-Z9rRnWZXfouPy4ZNNjB1uyrLbaRBc7b8,8910
 atorch/ops/accelerator/real_accelerator.py,sha256=jWxYWBNNWbDpL6Vhk_4_ySLCV3rHyT-GdcylseRMvZU,2478
 atorch/ops/csrc/includes/conversion_utils.h,sha256=Rj9QBKdYTLrkCovxMI03IKQKb153SrtgE9WYJS_PnLs,12017
 atorch/ops/csrc/includes/dequantization_utils.h,sha256=q9gZ4uSR9Kq1nU9bFu7oFMkWUV9kflzX78ZiyUQdXuo,7001
 atorch/ops/csrc/includes/kernel_utils.h,sha256=iZ1AAiQL8ipcNdSEN4itVH8xPIXiAI4XWrnpz6lGfVg,1202
@@ -204,17 +210,17 @@
 atorch/optimizers/low_bit/optim/__init__.py,sha256=EDq0eIKpAk2IYcgg8XiZhBTJ2J-na7XAXZ2QR0ralH8,118
 atorch/optimizers/low_bit/optim/q_adafactor.py,sha256=Sd_SbyZ4LGBCr5Itm1KzcFinJxpz0Hnenx-DrEHCw9Y,10365
 atorch/optimizers/low_bit/optim/q_adamw.py,sha256=8IXD8fFu0H8VqrsPCFQorLH_AVfQ5R_Vs0h5F7qz5iI,7123
 atorch/optimizers/low_bit/optim/q_agd.py,sha256=xsVBCQ4HgkekOwbjoX_KdiXfFVuxcGODZoYVBHgMniQ,9927
 atorch/optimizers/low_bit/optim/q_came.py,sha256=SToF6Bws8wTa1qS7-5Fwnqzx5BT68nbJ6kdwqg-5sYs,10023
 atorch/optimizers/low_bit/optim/q_optimizer.py,sha256=tFOQbRfjgN3sb7xJvHp5RgdqU_Dj7J6ZqS9B3rb5g4Y,7034
 atorch/protos/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-atorch/protos/acceleration_pb2.py,sha256=njaQFtIRpb-rnHO6FzqBtCuUiinyUQh550Y7F4RQKDs,19348
+atorch/protos/acceleration_pb2.py,sha256=4jDGv8Cs4H_s2YqkR-QQThxZBZGrSC0PtAsP7cWk7rc,3199
 atorch/protos/acceleration_pb2_grpc.py,sha256=zuznfu_tehpKMLI35pyfB1XqMHMH6czvPRjPBgEN2dw,4574
-atorch/protos/coworker_pb2.py,sha256=E-RcveDUbrH0N-vJoLFiuLi8e_Tj4RC8o_92bhIvCS8,5993
+atorch/protos/coworker_pb2.py,sha256=BtCErbiuMRg7hTbmLvutNyuKt4ZkWPu_xCnUkHhX1tY,1869
 atorch/protos/coworker_pb2_grpc.py,sha256=X29YrfA028EACXZnjTTxZBqugKc_CoozIJC3k91HHqU,6714
 atorch/rl/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/rl/config.py,sha256=ctu2t1_XuFW6--QbpCmxT86_DIoT7WIZoMQdq0Ij9IM,7661
 atorch/rl/main.py,sha256=SWg2e2Y5fa5yvdUv7w_72sulX4R1sO1T0hgKToVV_2c,849
 atorch/rl/data/__init__.py,sha256=BJhzBkR6f8S99fjMr3MhfZZL2QDHkf8Ovj3PDQlS4a8,39
 atorch/rl/data/data_utils.py,sha256=p43-c-pVMzHQxj3pHSgh17CR5A5aF7xpfHBHVFha5qY,6390
 atorch/rl/ds_hybrid_engine/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
@@ -244,46 +250,46 @@
 atorch/rl/trainer/ppo_trainer.py,sha256=u30GMOz6PAxBFF3D5hGnSBU-ooKwyFSZ_mzC6ddrSv8,274
 atorch/rl/trainer/rl_trainer.py,sha256=S_ccwiN2YwwOk4wFwNd_Yrpus1PLN2RwYn45BboKxnc,3190
 atorch/service/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 atorch/service/coworker_data_service.py,sha256=0mkkj9vHibS6X9wQVoEk3CIwd323Vkr5WqtZG6iWYog,2208
 atorch/service/data_info_service.py,sha256=3mRykB5OMBnfIpi8M27peh-XmQY-vLe1Q37kRDj6ng8,1924
 atorch/service/rpc_clients.py,sha256=4tKfDLeWqa9zWEUGYpkfgdvmx-d7IFv8m459oFoR6eE,3238
 atorch/trainer/__init__.py,sha256=IeqSgO7h3mVQX6TrvFFPjlxsIkrQB939g4W_JVuRRFU,103
-atorch/trainer/atorch_args.py,sha256=JfxFggF07xytT7osKDn4R8tdGTusirT-kQ9mFGLafcg,10651
-atorch/trainer/atorch_trainer.py,sha256=7yXAhnkk4Q3wrmovIBiD1XQN2O9zQszSDvNgZIWOGeE,98297
+atorch/trainer/atorch_args.py,sha256=zmS4dU7Dc4KU65Pcv8v8bZA_5KePDsC9YIYwuphi0hU,11648
+atorch/trainer/atorch_trainer.py,sha256=lr0sZp1pfoUJ3hVwmaUdLwvsrI9SNyLwGbF5OFOLFvQ,113391
 atorch/utils/__init__.py,sha256=XdOjdSUeFYAxmhjAHSUqeoLsKkcTSu6e_m3Mw20p_3U,63
 atorch/utils/ds_pipe_utils.py,sha256=kb5wBRNrBCnSt7xRGq3PjizjHalJbvebBLramwVvT58,8524
 atorch/utils/fsdp_async_ckpt_util.py,sha256=FpczDvGyqt9wRFfTgFkZ234v-atsAEs-kVCE_ISTOTo,7784
-atorch/utils/fsdp_init_util.py,sha256=jcJBUuEfAxNBrA2MWmW1hQr1veuVYZQRG-CxUJmCKyk,14062
-atorch/utils/fsdp_save_util.py,sha256=E_eWDDGA0jnRzRJ6iVDRua5SYOFDIXe-1K7O9_Fz7Wk,41878
+atorch/utils/fsdp_init_util.py,sha256=gwvR00_0Ge22993Iv-Gv7jUx4y3pESHvsees94XcCdA,23843
+atorch/utils/fsdp_save_util.py,sha256=-Eu7fjpg-3XfYsvAu7wlSThhD8vPlcCvmJO5NjMClBM,47379
 atorch/utils/grad_scaler.py,sha256=VXkj2R7wQjewbioRtcNLFnCvZa8XBJep4nGnisiO9tw,2706
 atorch/utils/graph_transform_utils.py,sha256=9xm6n8ekjUbvyP-HC0tkhFYF5f_r_tiznozBQRWyXrc,5644
 atorch/utils/hooks.py,sha256=WDCvgA_Q43_ySZLPczqSnxx9a9DTMjXeLTYGgDbSBww,1021
 atorch/utils/ib_monitor.py,sha256=9X6n3T7mzZ2vDRATz90E3VVmSzZTKkbSuMRGfInQpJw,6940
 atorch/utils/import_util.py,sha256=qMGtsKMrN2wqmm0_IAMTUooaq1ZjP9x4oalldKPr7I0,1428
+atorch/utils/loss_spike_utils.py,sha256=OQwO3Y-PFTZtzaU3K4Eu7iK7dN-ptBWR8nQ3A54wiBo,6956
 atorch/utils/manual_tp_utils.py,sha256=Kg8sWEZqrPciK7zt8t49OqfdZqg2bED9Tgpc8y5VdcA,10381
 atorch/utils/meta_model_utils.py,sha256=j1i4OkEacMF-904cv7RGuCqztMS3hgoPR2i6GoAunLk,34986
 atorch/utils/meta_overrides.py,sha256=nkaTKZ6siJ1b0J1FziJcn6b0hZ8f9oDDzU8Jacrkb98,11593
 atorch/utils/metric_util.py,sha256=aPCo5GqG7do-h_AH1PoOYZtpOJ8EYdnw7KSZRukpgcU,2267
 atorch/utils/numberic_checker.py,sha256=JlvqWzDjAbhMnnhElNDHaJLJ5Eoid2f5mNyms8ZCQwo,5781
-atorch/utils/parse_fsdp_mapping.py,sha256=5WsCSPFHMTDsJFdH6zDwv04wxoi2tflNAWrTDwOAFDc,9514
 atorch/utils/parse_trace_json.py,sha256=rGdUgPQ6I34SXtQGBcw25JE-d0s7tKTBnDo_MC-XJQo,10451
 atorch/utils/patch_fairscale.py,sha256=xnHugClneeeaW407fJvj2BS65WuSdo_JZX-vIir_H-M,3487
-atorch/utils/patch_te.py,sha256=mb0KUoCvcX3x0y3LqbQwXPEWGxitKOIK-etQ_UwjSD8,4875
+atorch/utils/patch_te.py,sha256=xstS7kRrJWnxMhbjPQG1__UoVEnoYb92k5jC8D4zAik,4918
 atorch/utils/pipe_file_utils.py,sha256=dEKBb-YLRNBZc2Qzp039zn8s-VM9hUVlJpBTxn3hqnA,4188
 atorch/utils/prof.py,sha256=FfH4w8h-JB7xHdF7zdD-m98bxcWUi5TcIQEy8Onl8cU,46954
 atorch/utils/shape_prop.py,sha256=J6qIbDc5TZgCFLCLdu_WTDybLW07GoIZyUerAA0kHm8,2839
 atorch/utils/sharding_spec.py,sha256=wLWHcIRM_OjB1H3sQZluOtUfmMFxz7VETlOYPBS9aS4,4281
 atorch/utils/sparse.py,sha256=ek0trMwZbdGQRo7v9g9UgAjESczZZxDDvC8X02GWCfI,2547
 atorch/utils/spec_prop.py,sha256=S9OEHpoXVOZQMEMaqKB6LhwsAOQEa5borPAh5F5lQoI,6342
 atorch/utils/timer.py,sha256=4_pZda7ZT_7vQ5cRBz4e-ZpYU9qaSivKxSZtGUbl1XM,2797
 atorch/utils/tracer.py,sha256=6VWBeLtW_BNyRBYVO3Q1HvbnFstg30qmdXYoguRoggo,24365
 atorch/utils/trainer_utils.py,sha256=gd4XcPGEDgzQ6VslrHGZBdTcI8CbBZm-x6lv7a5gd5M,2244
-atorch/utils/version.py,sha256=i71v6eiVb_IXQdDlWOwYWnyMok9j29nzLGh83Vjic5Y,1441
-atorch-0.1.8.data/data/acceleration.proto,sha256=spmYAqmckmV29X1XkmOSwajWgKMGrj7pn1nraL3TnW0,1046
-atorch-0.1.8.data/data/build_proto.sh,sha256=sbTOt_HHt_F-DyfgHY74m755redknL6nHeZwIUjswD4,224
-atorch-0.1.8.data/data/coworker.proto,sha256=hezllszC0XadStrgrgi6J9pmlZLJj2E50uTi9aqVamE,455
-atorch-0.1.8.data/data/requirements.txt,sha256=6EcK-CwiZRCpwxiU3srZyvlvLESn0fF_NK8Xr2aj3JQ,273
-atorch-0.1.8.dist-info/METADATA,sha256=qDqP74juQzP0sbkOqvxT3HKN-nqSghepThIKl1t_mIo,1155
-atorch-0.1.8.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
-atorch-0.1.8.dist-info/top_level.txt,sha256=64BT5ChWxA_sdfYF3xxVLu_I8jhTEfSSOlK5WQ4zcH0,7
-atorch-0.1.8.dist-info/RECORD,,
+atorch/utils/version.py,sha256=7Cq-WDsyFUFyeg3HeRAlYt1JKUuu7FUMliSipCEcOsg,1649
+atorch-0.1.9.data/data/acceleration.proto,sha256=spmYAqmckmV29X1XkmOSwajWgKMGrj7pn1nraL3TnW0,1046
+atorch-0.1.9.data/data/build_proto.sh,sha256=sbTOt_HHt_F-DyfgHY74m755redknL6nHeZwIUjswD4,224
+atorch-0.1.9.data/data/coworker.proto,sha256=hezllszC0XadStrgrgi6J9pmlZLJj2E50uTi9aqVamE,455
+atorch-0.1.9.data/data/requirements.txt,sha256=Lf8nuoICh3r7BQS7AvHQ0_AfgNfybm2PHz618BFKkiQ,287
+atorch-0.1.9.dist-info/METADATA,sha256=l0Q10pu-UCUQX_hIacmih9HP8I0v6ZGrFwyA_LXVh_4,1197
+atorch-0.1.9.dist-info/WHEEL,sha256=yQN5g4mg4AybRjkgi-9yy4iQEFibGQmlz78Pik5Or-A,92
+atorch-0.1.9.dist-info/top_level.txt,sha256=64BT5ChWxA_sdfYF3xxVLu_I8jhTEfSSOlK5WQ4zcH0,7
+atorch-0.1.9.dist-info/RECORD,,
```

