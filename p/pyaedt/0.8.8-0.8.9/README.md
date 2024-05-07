# Comparing `tmp/pyaedt-0.8.8.tar.gz` & `tmp/pyaedt-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyaedt-0.8.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "pyaedt-0.8.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `pyaedt-0.8.8.tar` & `pyaedt-0.8.9.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0     1111 2023-12-31 17:45:46.144704 pyaedt-0.8.8/LICENSE
--rw-r--r--   0        0        0    10530 2024-03-18 17:32:41.568450 pyaedt-0.8.8/README.md
--rw-r--r--   0        0        0     3483 2024-04-16 19:20:04.036426 pyaedt-0.8.8/pyaedt/__init__.py
--rw-r--r--   0        0        0    33008 2024-03-26 16:57:20.066432 pyaedt-0.8.8/pyaedt/aedt_logger.py
--rw-r--r--   0        0        0     6966 2023-11-15 14:48:51.126062 pyaedt-0.8.8/pyaedt/application/AEDT_File_Management.py
--rw-r--r--   0        0        0    92484 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/application/Analysis.py
--rw-r--r--   0        0        0    56669 2024-04-16 16:03:45.141509 pyaedt-0.8.8/pyaedt/application/Analysis3D.py
--rw-r--r--   0        0        0    11645 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/application/Analysis3DLayout.py
--rw-r--r--   0        0        0     3225 2024-02-29 11:54:54.087433 pyaedt-0.8.8/pyaedt/application/AnalysisMaxwellCircuit.py
--rw-r--r--   0        0        0    13652 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/application/AnalysisNexxim.py
--rw-r--r--   0        0        0     4655 2024-03-26 16:57:20.066432 pyaedt-0.8.8/pyaedt/application/AnalysisRMxprt.py
--rw-r--r--   0        0        0     4889 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/application/AnalysisTwinBuilder.py
--rw-r--r--   0        0        0   141100 2024-04-12 06:21:23.624898 pyaedt-0.8.8/pyaedt/application/Design.py
--rw-r--r--   0        0        0     6194 2023-11-15 14:48:51.126062 pyaedt-0.8.8/pyaedt/application/JobManager.py
--rw-r--r--   0        0        0    80899 2024-03-29 15:34:31.534043 pyaedt-0.8.8/pyaedt/application/Variables.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.141075 pyaedt-0.8.8/pyaedt/application/__init__.py
--rw-r--r--   0        0        0    13127 2024-03-26 16:57:20.082054 pyaedt-0.8.8/pyaedt/application/aedt_objects.py
--rw-r--r--   0        0        0    14049 2024-04-08 07:26:14.718804 pyaedt-0.8.8/pyaedt/application/analysis_hf.py
--rw-r--r--   0        0        0    38458 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/application/design_solutions.py
--rw-r--r--   0        0        0    80398 2024-04-16 16:03:45.141509 pyaedt-0.8.8/pyaedt/circuit.py
--rw-r--r--   0        0        0    10845 2024-04-05 14:27:59.009689 pyaedt-0.8.8/pyaedt/common_rpc.py
--rw-r--r--   0        0        0    93993 2024-04-16 16:03:45.141509 pyaedt-0.8.8/pyaedt/desktop.py
--rw-r--r--   0        0        0    26397 2024-04-16 16:33:03.403200 pyaedt-0.8.8/pyaedt/downloads.py
--rw-r--r--   0        0        0      210 2024-02-23 10:39:15.272359 pyaedt-0.8.8/pyaedt/edb.py
--rw-r--r--   0        0        0    11388 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/emit.py
--rw-r--r--   0        0        0     6102 2024-01-31 07:08:42.610124 pyaedt-0.8.8/pyaedt/emit_core/Couplings.py
--rw-r--r--   0        0        0     3762 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/emit_core/__init__.py
--rw-r--r--   0        0        0     2664 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/emit_core/emit_constants.py
--rw-r--r--   0        0        0        2 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/emit_core/results/__init__.py
--rw-r--r--   0        0        0     7406 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/emit_core/results/results.py
--rw-r--r--   0        0        0    30406 2024-04-12 06:22:12.847095 pyaedt-0.8.8/pyaedt/emit_core/results/revision.py
--rw-r--r--   0        0        0     9836 2024-01-08 11:44:37.567605 pyaedt-0.8.8/pyaedt/generic/Ansys.png
--rw-r--r--   0        0        0      761 2024-02-02 17:51:14.912475 pyaedt-0.8.8/pyaedt/generic/AnsysTemplate.json
--rw-r--r--   0        0        0    15961 2024-04-12 06:21:23.624898 pyaedt-0.8.8/pyaedt/generic/DataHandlers.py
--rw-r--r--   0        0        0    16551 2024-04-12 06:21:23.624898 pyaedt-0.8.8/pyaedt/generic/LoadAEDTFile.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/generic/__init__.py
--rw-r--r--   0        0        0     1413 2023-11-15 14:48:51.281530 pyaedt-0.8.8/pyaedt/generic/ami.json
--rw-r--r--   0        0        0     3347 2024-03-26 16:57:20.082054 pyaedt-0.8.8/pyaedt/generic/clr_module.py
--rw-r--r--   0        0        0        0 2024-04-05 14:27:59.009689 pyaedt-0.8.8/pyaedt/generic/com_parameters.py
--rw-r--r--   0        0        0    37863 2024-04-12 06:22:12.847095 pyaedt-0.8.8/pyaedt/generic/compliance.py
--rw-r--r--   0        0        0    91065 2024-04-16 16:03:45.141509 pyaedt-0.8.8/pyaedt/generic/configurations.py
--rw-r--r--   0        0        0    28707 2024-03-18 17:32:41.568450 pyaedt-0.8.8/pyaedt/generic/constants.py
--rw-r--r--   0        0        0    73888 2024-04-15 11:56:45.704733 pyaedt-0.8.8/pyaedt/generic/design_types.py
--rw-r--r--   0        0        0      190 2024-04-16 16:03:45.141509 pyaedt-0.8.8/pyaedt/generic/desktop_sessions.py
--rw-r--r--   0        0        0     3934 2024-03-26 16:57:20.082054 pyaedt-0.8.8/pyaedt/generic/filesystem.py
--rw-r--r--   0        0        0    68771 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/generic/general_methods.py
--rw-r--r--   0        0        0     9430 2024-03-26 16:57:20.082054 pyaedt-0.8.8/pyaedt/generic/grpc_plugin.py
--rw-r--r--   0        0        0     3473 2023-12-13 11:29:08.166076 pyaedt-0.8.8/pyaedt/generic/grpc_plugin_dll.py
--rw-r--r--   0        0        0    44398 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/generic/ibis_reader.py
--rw-r--r--   0        0        0     2776 2024-01-02 08:48:34.102194 pyaedt-0.8.8/pyaedt/generic/ibis_v7.json
--rw-r--r--   0        0        0     7029 2023-11-15 14:48:51.297153 pyaedt-0.8.8/pyaedt/generic/near_field_import.py
--rw-r--r--   0        0        0    21938 2024-04-05 14:27:59.009689 pyaedt-0.8.8/pyaedt/generic/pdf.py
--rw-r--r--   0        0        0    65524 2024-04-04 20:41:59.615015 pyaedt-0.8.8/pyaedt/generic/plot.py
--rw-r--r--   0        0        0    20256 2023-11-15 14:48:51.297153 pyaedt-0.8.8/pyaedt/generic/python_optimizers.py
--rw-r--r--   0        0        0     3536 2023-11-15 14:48:51.297153 pyaedt-0.8.8/pyaedt/generic/report_file_parser.py
--rw-r--r--   0        0        0    17709 2024-04-05 13:12:25.411540 pyaedt-0.8.8/pyaedt/generic/settings.py
--rw-r--r--   0        0        0    25263 2024-04-05 14:27:59.009689 pyaedt-0.8.8/pyaedt/generic/spisim.py
--rw-r--r--   0        0        0    20374 2024-03-28 11:32:30.107010 pyaedt-0.8.8/pyaedt/generic/touchstone_parser.py
--rw-r--r--   0        0        0   253753 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/hfss.py
--rw-r--r--   0        0        0    84193 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/hfss3dlayout.py
--rw-r--r--   0        0        0   278413 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/icepak.py
--rw-r--r--   0        0        0   130037 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/maxwell.py
--rw-r--r--   0        0        0     7953 2024-03-26 16:57:20.097680 pyaedt-0.8.8/pyaedt/maxwellcircuit.py
--rw-r--r--   0        0        0    24791 2024-04-15 11:56:45.720413 pyaedt-0.8.8/pyaedt/mechanical.py
--rw-r--r--   0        0        0     3642 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/Console.py_build
--rw-r--r--   0        0        0     2230 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/Job_Settings.areg
--rw-r--r--   0        0        0     3394 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/Jupyter.py_build
--rw-r--r--   0        0        0     4125 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/Run_PyAEDT_Script.py_build
--rw-r--r--   0        0        0     3526 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
--rw-r--r--   0        0        0      202 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/__init__.py
--rw-r--r--   0        0        0    10796 2024-03-26 16:57:20.097680 pyaedt-0.8.8/pyaedt/misc/aedtlib_personalib_install.py
--rw-r--r--   0        0        0    19870 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/amat.xml
--rw-r--r--   0        0        0     2620 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/ansys_cloud.areg
--rw-r--r--   0        0        0     2013 2024-01-03 08:09:17.894973 pyaedt-0.8.8/pyaedt/misc/config.schema.json
--rw-r--r--   0        0        0     3554 2024-01-31 07:08:42.610124 pyaedt-0.8.8/pyaedt/misc/console_setup.py
--rw-r--r--   0        0        0       48 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/create_remote_dir.py
--rw-r--r--   0        0        0    15250 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/images/gallery/PyAEDT.png
--rw-r--r--   0        0        0      855 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/images/large/pyansys.png
--rw-r--r--   0        0        0     5630 2024-03-08 10:07:44.551028 pyaedt-0.8.8/pyaedt/misc/install_extra_toolkits.py
--rw-r--r--   0        0        0     1728 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/jupyter_template.ipynb
--rw-r--r--   0        0        0     2700 2024-03-26 16:57:20.097680 pyaedt-0.8.8/pyaedt/misc/misc.py
--rw-r--r--   0        0        0   771467 2023-11-15 14:48:51.312829 pyaedt-0.8.8/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
--rw-r--r--   0        0        0   502580 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
--rw-r--r--   0        0        0   162026 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
--rw-r--r--   0        0        0   134414 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
--rw-r--r--   0        0        0      289 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/pyaedt.runtimeconfig.json
--rw-r--r--   0        0        0      960 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/pyaedt_local_config.acf
--rw-r--r--   0        0        0    16550 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/pyansys-logo-black-cropped.png
--rw-r--r--   0        0        0       61 2024-03-20 11:35:09.070685 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/__init__.py
--rw-r--r--   0        0        0     5192 2024-03-20 11:35:09.070685 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
--rw-r--r--   0        0        0     5153 2024-03-20 11:35:09.070685 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
--rw-r--r--   0        0        0     5155 2024-03-20 11:35:09.070685 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
--rw-r--r--   0        0        0    12280 2024-03-21 13:12:02.821738 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
--rw-r--r--   0        0        0    15308 2024-03-20 11:35:09.070685 pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
--rw-r--r--   0        0        0      868 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/misc/template.acf
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/modeler/__init__.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/__init__.py
--rw-r--r--   0        0        0    14073 2024-02-09 10:59:25.236001 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/actors.py
--rw-r--r--   0        0        0    20019 2024-02-09 10:59:25.236001 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/multiparts.py
--rw-r--r--   0        0        0    18513 2023-11-15 14:48:51.328409 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/oms.py
--rw-r--r--   0        0        0    16676 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/parts.py
--rw-r--r--   0        0        0   126296 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/modeler/advanced_cad/stackup_3d.py
--rw-r--r--   0        0        0    80031 2024-04-16 16:03:45.157131 pyaedt-0.8.8/pyaedt/modeler/cad/Modeler.py
--rw-r--r--   0        0        0   335948 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/Primitives.py
--rw-r--r--   0        0        0    14603 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/Primitives2D.py
--rw-r--r--   0        0        0   144677 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/Primitives3D.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.344085 pyaedt-0.8.8/pyaedt/modeler/cad/__init__.py
--rw-r--r--   0        0        0    29696 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/component_array.py
--rw-r--r--   0        0        0    41884 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/components_3d.py
--rw-r--r--   0        0        0    49374 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/elements3d.py
--rw-r--r--   0        0        0    59455 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/object3d.py
--rw-r--r--   0        0        0    53212 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/cad/polylines.py
--rw-r--r--   0        0        0    12604 2023-11-15 14:48:51.344085 pyaedt-0.8.8/pyaedt/modeler/calculators.py
--rw-r--r--   0        0        0    44326 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesCircuit.py
--rw-r--r--   0        0        0    39329 2024-04-12 06:22:12.847095 pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesEmit.py
--rw-r--r--   0        0        0     8514 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
--rw-r--r--   0        0        0    68319 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesNexxim.py
--rw-r--r--   0        0        0    15130 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.344085 pyaedt-0.8.8/pyaedt/modeler/circuits/__init__.py
--rw-r--r--   0        0        0    34524 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/circuits/object3dcircuit.py
--rw-r--r--   0        0        0    68299 2024-04-15 14:11:58.269561 pyaedt-0.8.8/pyaedt/modeler/geometry_operators.py
--rw-r--r--   0        0        0     6929 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/modeler2d.py
--rw-r--r--   0        0        0    66190 2024-04-16 16:03:45.172811 pyaedt-0.8.8/pyaedt/modeler/modeler3d.py
--rw-r--r--   0        0        0    33272 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modeler/modelerpcb.py
--rw-r--r--   0        0        0    52444 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modeler/pcb/Primitives3DLayout.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.359653 pyaedt-0.8.8/pyaedt/modeler/pcb/__init__.py
--rw-r--r--   0        0        0    66436 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modeler/pcb/object3dlayout.py
--rw-r--r--   0        0        0    23856 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modeler/schematic.py
--rw-r--r--   0        0        0    51557 2024-04-15 11:56:45.720413 pyaedt-0.8.8/pyaedt/modules/AdvancedPostProcessing.py
--rw-r--r--   0        0        0   169925 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/Boundary.py
--rw-r--r--   0        0        0    71749 2024-04-05 14:27:59.025313 pyaedt-0.8.8/pyaedt/modules/CableModeling.py
--rw-r--r--   0        0        0    16319 2023-11-15 14:48:51.359653 pyaedt-0.8.8/pyaedt/modules/CircuitTemplates.py
--rw-r--r--   0        0        0    56829 2024-04-12 06:21:23.656143 pyaedt-0.8.8/pyaedt/modules/DesignXPloration.py
--rw-r--r--   0        0        0    40453 2024-04-12 06:21:23.656143 pyaedt-0.8.8/pyaedt/modules/LayerStackup.py
--rw-r--r--   0        0        0   105895 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/Material.py
--rw-r--r--   0        0        0    33683 2024-03-26 16:57:20.128932 pyaedt-0.8.8/pyaedt/modules/MaterialLib.py
--rw-r--r--   0        0        0    55020 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/Mesh.py
--rw-r--r--   0        0        0    12354 2024-04-09 09:33:35.792297 pyaedt-0.8.8/pyaedt/modules/Mesh3DLayout.py
--rw-r--r--   0        0        0    49218 2024-04-10 06:18:36.719407 pyaedt-0.8.8/pyaedt/modules/MeshIcepak.py
--rw-r--r--   0        0        0     4437 2023-11-15 14:48:51.359653 pyaedt-0.8.8/pyaedt/modules/OptimetricsTemplates.py
--rw-r--r--   0        0        0   211693 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/PostProcessor.py
--rw-r--r--   0        0        0    72048 2024-03-08 11:06:27.183697 pyaedt-0.8.8/pyaedt/modules/SetupTemplates.py
--rw-r--r--   0        0        0   147699 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/SolveSetup.py
--rw-r--r--   0        0        0    32997 2024-04-15 11:56:45.720413 pyaedt-0.8.8/pyaedt/modules/SolveSweeps.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/modules/__init__.py
--rw-r--r--   0        0        0    31386 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/modules/monitor_icepak.py
--rw-r--r--   0        0        0   137795 2024-04-16 10:41:18.667222 pyaedt-0.8.8/pyaedt/modules/report_templates.py
--rw-r--r--   0        0        0   135852 2024-04-15 11:56:45.735987 pyaedt-0.8.8/pyaedt/modules/solutions.py
--rw-r--r--   0        0        0    97896 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/q3d.py
--rw-r--r--   0        0        0    10722 2024-04-15 11:56:45.735987 pyaedt-0.8.8/pyaedt/rmxprt.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/rpc/__init__.py
--rw-r--r--   0        0        0      415 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/rpc/local_server.py
--rw-r--r--   0        0        0    42608 2024-04-16 16:03:45.188385 pyaedt-0.8.8/pyaedt/rpc/rpyc_services.py
--rw-r--r--   0        0        0        0 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/__init__.py
--rw-r--r--   0        0        0     9463 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/hdm_parser.py
--rw-r--r--   0        0        0     2096 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/hdm_utils.py
--rw-r--r--   0        0        0     2607 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/HdmObject.m
--rw-r--r--   0        0        0       97 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/README.md
--rw-r--r--   0        0        0      735 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/SbrBounceType.m
--rw-r--r--   0        0        0     2886 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/StopWatch.m
--rw-r--r--   0        0        0     1402 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/add_3dlight.m
--rw-r--r--   0        0        0      340 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/amp2db.m
--rw-r--r--   0        0        0    36837 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/draw_rays1.m
--rw-r--r--   0        0        0     4322 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/draw_wfobj.m
--rw-r--r--   0        0        0    31414 2023-11-15 14:48:51.375283 pyaedt-0.8.8/pyaedt/sbrplus/matlab/filter_rays1.m
--rw-r--r--   0        0        0     1504 2023-11-15 14:48:51.390911 pyaedt-0.8.8/pyaedt/sbrplus/matlab/filtered_tracks.m
--rw-r--r--   0        0        0    20853 2023-11-15 14:48:51.390911 pyaedt-0.8.8/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
--rw-r--r--   0        0        0    14781 2023-11-15 14:48:51.390911 pyaedt-0.8.8/pyaedt/sbrplus/matlab/ld_wfobj.m
--rw-r--r--   0        0        0      318 2023-11-15 14:48:51.390911 pyaedt-0.8.8/pyaedt/sbrplus/matlab/pwr2db.m
--rw-r--r--   0        0        0     2607 2023-11-15 14:48:51.390911 pyaedt-0.8.8/pyaedt/sbrplus/matlab/validate_sfields.m
--rw-r--r--   0        0        0     7621 2024-03-26 16:57:20.144566 pyaedt-0.8.8/pyaedt/sbrplus/plot.py
--rw-r--r--   0        0        0    21529 2024-04-15 11:56:45.735987 pyaedt-0.8.8/pyaedt/twinbuilder.py
--rw-r--r--   0        0        0     6768 2024-04-16 10:43:22.619068 pyaedt-0.8.8/pyproject.toml
--rw-r--r--   0        0        0    16490 1970-01-01 00:00:00.000000 pyaedt-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0     1111 2024-01-08 19:14:30.151334 pyaedt-0.8.9/LICENSE
+-rw-r--r--   0        0        0    10530 2024-03-18 17:51:52.716931 pyaedt-0.8.9/README.md
+-rw-r--r--   0        0        0     3483 2024-04-20 18:31:25.985325 pyaedt-0.8.9/pyaedt/__init__.py
+-rw-r--r--   0        0        0    33134 2024-04-18 10:46:52.634008 pyaedt-0.8.9/pyaedt/aedt_logger.py
+-rw-r--r--   0        0        0     6966 2023-11-15 14:48:55.940401 pyaedt-0.8.9/pyaedt/application/AEDT_File_Management.py
+-rw-r--r--   0        0        0    92906 2024-04-19 11:54:25.539394 pyaedt-0.8.9/pyaedt/application/Analysis.py
+-rw-r--r--   0        0        0    56829 2024-04-19 11:13:06.273295 pyaedt-0.8.9/pyaedt/application/Analysis3D.py
+-rw-r--r--   0        0        0    11793 2024-04-18 13:42:58.079510 pyaedt-0.8.9/pyaedt/application/Analysis3DLayout.py
+-rw-r--r--   0        0        0     3225 2024-02-29 13:41:13.886891 pyaedt-0.8.9/pyaedt/application/AnalysisMaxwellCircuit.py
+-rw-r--r--   0        0        0    13652 2024-04-15 11:56:47.798989 pyaedt-0.8.9/pyaedt/application/AnalysisNexxim.py
+-rw-r--r--   0        0        0     4655 2024-03-26 18:55:40.973822 pyaedt-0.8.9/pyaedt/application/AnalysisRMxprt.py
+-rw-r--r--   0        0        0     4889 2024-04-15 11:56:47.798989 pyaedt-0.8.9/pyaedt/application/AnalysisTwinBuilder.py
+-rw-r--r--   0        0        0   142914 2024-04-18 13:42:58.079510 pyaedt-0.8.9/pyaedt/application/Design.py
+-rw-r--r--   0        0        0     6194 2023-11-15 14:48:55.940401 pyaedt-0.8.9/pyaedt/application/JobManager.py
+-rw-r--r--   0        0        0    80912 2024-04-19 16:05:23.675083 pyaedt-0.8.9/pyaedt/application/Variables.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:55.940401 pyaedt-0.8.9/pyaedt/application/__init__.py
+-rw-r--r--   0        0        0    13127 2024-03-26 18:55:40.973822 pyaedt-0.8.9/pyaedt/application/aedt_objects.py
+-rw-r--r--   0        0        0    14049 2024-04-08 07:26:19.042029 pyaedt-0.8.9/pyaedt/application/analysis_hf.py
+-rw-r--r--   0        0        0    38458 2024-04-15 11:56:47.798989 pyaedt-0.8.9/pyaedt/application/design_solutions.py
+-rw-r--r--   0        0        0    81061 2024-04-19 10:41:23.663533 pyaedt-0.8.9/pyaedt/circuit.py
+-rw-r--r--   0        0        0    10845 2024-04-05 14:28:19.087164 pyaedt-0.8.9/pyaedt/common_rpc.py
+-rw-r--r--   0        0        0    94120 2024-04-18 12:07:48.942838 pyaedt-0.8.9/pyaedt/desktop.py
+-rw-r--r--   0        0        0    26482 2024-04-19 08:40:11.152072 pyaedt-0.8.9/pyaedt/downloads.py
+-rw-r--r--   0        0        0      210 2024-02-23 10:20:46.907198 pyaedt-0.8.9/pyaedt/edb.py
+-rw-r--r--   0        0        0    11388 2024-04-15 11:56:47.798989 pyaedt-0.8.9/pyaedt/emit.py
+-rw-r--r--   0        0        0     6102 2024-01-31 08:29:55.307606 pyaedt-0.8.9/pyaedt/emit_core/Couplings.py
+-rw-r--r--   0        0        0     3762 2024-02-06 15:33:49.564252 pyaedt-0.8.9/pyaedt/emit_core/__init__.py
+-rw-r--r--   0        0        0     2664 2023-11-15 14:48:56.128198 pyaedt-0.8.9/pyaedt/emit_core/emit_constants.py
+-rw-r--r--   0        0        0        2 2023-11-15 14:48:56.128198 pyaedt-0.8.9/pyaedt/emit_core/results/__init__.py
+-rw-r--r--   0        0        0     7406 2023-11-15 14:48:56.128198 pyaedt-0.8.9/pyaedt/emit_core/results/results.py
+-rw-r--r--   0        0        0    30406 2024-04-12 06:22:14.182014 pyaedt-0.8.9/pyaedt/emit_core/results/revision.py
+-rw-r--r--   0        0        0     9836 2024-01-08 11:44:42.739939 pyaedt-0.8.9/pyaedt/generic/Ansys.png
+-rw-r--r--   0        0        0      761 2024-02-02 17:43:33.722695 pyaedt-0.8.9/pyaedt/generic/AnsysTemplate.json
+-rw-r--r--   0        0        0    15961 2024-04-12 06:21:24.852374 pyaedt-0.8.9/pyaedt/generic/DataHandlers.py
+-rw-r--r--   0        0        0    16551 2024-04-12 06:21:24.852374 pyaedt-0.8.9/pyaedt/generic/LoadAEDTFile.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.128198 pyaedt-0.8.9/pyaedt/generic/__init__.py
+-rw-r--r--   0        0        0     1413 2023-11-15 14:48:56.128198 pyaedt-0.8.9/pyaedt/generic/ami.json
+-rw-r--r--   0        0        0     3347 2024-03-26 18:55:40.989446 pyaedt-0.8.9/pyaedt/generic/clr_module.py
+-rw-r--r--   0        0        0        0 2024-04-05 14:28:19.087164 pyaedt-0.8.9/pyaedt/generic/com_parameters.py
+-rw-r--r--   0        0        0    37863 2024-04-12 06:22:14.182014 pyaedt-0.8.9/pyaedt/generic/compliance.py
+-rw-r--r--   0        0        0    91063 2024-04-18 16:52:37.739026 pyaedt-0.8.9/pyaedt/generic/configurations.py
+-rw-r--r--   0        0        0    28707 2024-03-19 11:00:02.376642 pyaedt-0.8.9/pyaedt/generic/constants.py
+-rw-r--r--   0        0        0    74044 2024-04-18 13:42:58.095124 pyaedt-0.8.9/pyaedt/generic/design_types.py
+-rw-r--r--   0        0        0      190 2024-04-16 16:33:04.957996 pyaedt-0.8.9/pyaedt/generic/desktop_sessions.py
+-rw-r--r--   0        0        0     3934 2024-03-26 18:55:40.989446 pyaedt-0.8.9/pyaedt/generic/filesystem.py
+-rw-r--r--   0        0        0    68771 2024-04-17 18:23:08.705993 pyaedt-0.8.9/pyaedt/generic/general_methods.py
+-rw-r--r--   0        0        0     9430 2024-03-26 18:55:40.989446 pyaedt-0.8.9/pyaedt/generic/grpc_plugin.py
+-rw-r--r--   0        0        0     3473 2024-02-06 15:33:49.564252 pyaedt-0.8.9/pyaedt/generic/grpc_plugin_dll.py
+-rw-r--r--   0        0        0    44288 2024-04-18 16:52:37.739026 pyaedt-0.8.9/pyaedt/generic/ibis_reader.py
+-rw-r--r--   0        0        0     2776 2024-01-02 08:48:38.514823 pyaedt-0.8.9/pyaedt/generic/ibis_v7.json
+-rw-r--r--   0        0        0     7029 2023-11-15 14:48:56.143712 pyaedt-0.8.9/pyaedt/generic/near_field_import.py
+-rw-r--r--   0        0        0    21938 2024-04-05 14:28:19.102805 pyaedt-0.8.9/pyaedt/generic/pdf.py
+-rw-r--r--   0        0        0    65524 2024-04-04 19:07:08.904699 pyaedt-0.8.9/pyaedt/generic/plot.py
+-rw-r--r--   0        0        0    20256 2023-11-15 14:48:56.143712 pyaedt-0.8.9/pyaedt/generic/python_optimizers.py
+-rw-r--r--   0        0        0     3536 2024-02-06 15:33:49.564252 pyaedt-0.8.9/pyaedt/generic/report_file_parser.py
+-rw-r--r--   0        0        0    17709 2024-04-05 13:12:30.970116 pyaedt-0.8.9/pyaedt/generic/settings.py
+-rw-r--r--   0        0        0    25263 2024-04-05 14:28:19.102805 pyaedt-0.8.9/pyaedt/generic/spisim.py
+-rw-r--r--   0        0        0    20384 2024-04-18 16:52:37.739026 pyaedt-0.8.9/pyaedt/generic/touchstone_parser.py
+-rw-r--r--   0        0        0   252594 2024-04-18 16:52:37.739026 pyaedt-0.8.9/pyaedt/hfss.py
+-rw-r--r--   0        0        0    86223 2024-04-19 11:13:06.273295 pyaedt-0.8.9/pyaedt/hfss3dlayout.py
+-rw-r--r--   0        0        0   278343 2024-04-18 16:52:37.754695 pyaedt-0.8.9/pyaedt/icepak.py
+-rw-r--r--   0        0        0   130077 2024-04-18 16:52:37.754695 pyaedt-0.8.9/pyaedt/maxwell.py
+-rw-r--r--   0        0        0     7953 2024-03-26 18:55:41.005072 pyaedt-0.8.9/pyaedt/maxwellcircuit.py
+-rw-r--r--   0        0        0    24715 2024-04-19 11:13:06.289079 pyaedt-0.8.9/pyaedt/mechanical.py
+-rw-r--r--   0        0        0     3642 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/Console.py_build
+-rw-r--r--   0        0        0     2230 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/Job_Settings.areg
+-rw-r--r--   0        0        0     3394 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/Jupyter.py_build
+-rw-r--r--   0        0        0     4125 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/Run_PyAEDT_Script.py_build
+-rw-r--r--   0        0        0     3526 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build
+-rw-r--r--   0        0        0      202 2023-11-15 14:48:56.159371 pyaedt-0.8.9/pyaedt/misc/__init__.py
+-rw-r--r--   0        0        0    10796 2024-03-26 18:55:41.005072 pyaedt-0.8.9/pyaedt/misc/aedtlib_personalib_install.py
+-rw-r--r--   0        0        0    19870 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/amat.xml
+-rw-r--r--   0        0        0     2620 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/ansys_cloud.areg
+-rw-r--r--   0        0        0     2013 2024-01-03 08:09:11.617311 pyaedt-0.8.9/pyaedt/misc/config.schema.json
+-rw-r--r--   0        0        0     3554 2024-01-31 08:29:55.323250 pyaedt-0.8.9/pyaedt/misc/console_setup.py
+-rw-r--r--   0        0        0       48 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/create_remote_dir.py
+-rw-r--r--   0        0        0    15250 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/images/gallery/PyAEDT.png
+-rw-r--r--   0        0        0      855 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/images/large/pyansys.png
+-rw-r--r--   0        0        0     5630 2024-03-08 09:52:28.386458 pyaedt-0.8.9/pyaedt/misc/install_extra_toolkits.py
+-rw-r--r--   0        0        0     1728 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/jupyter_template.ipynb
+-rw-r--r--   0        0        0     2700 2024-03-26 18:55:41.005072 pyaedt-0.8.9/pyaedt/misc/misc.py
+-rw-r--r--   0        0        0   771467 2023-11-15 14:48:56.174972 pyaedt-0.8.9/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json
+-rw-r--r--   0        0        0   502580 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json
+-rw-r--r--   0        0        0   162026 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib
+-rw-r--r--   0        0        0   134414 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib
+-rw-r--r--   0        0        0      289 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/pyaedt.runtimeconfig.json
+-rw-r--r--   0        0        0      960 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/pyaedt_local_config.acf
+-rw-r--r--   0        0        0    16550 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/pyansys-logo-black-cropped.png
+-rw-r--r--   0        0        0       61 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/__init__.py
+-rw-r--r--   0        0        0     5192 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json
+-rw-r--r--   0        0        0     5153 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_93_8.json
+-rw-r--r--   0        0        0     5155 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_94_17.json
+-rw-r--r--   0        0        0    12280 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_parameters.py
+-rw-r--r--   0        0        0    15308 2024-03-22 10:54:58.740472 pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py
+-rw-r--r--   0        0        0      868 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/misc/template.acf
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/modeler/__init__.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/__init__.py
+-rw-r--r--   0        0        0    14073 2024-02-09 10:07:59.429453 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/actors.py
+-rw-r--r--   0        0        0    20019 2024-02-09 10:07:59.429453 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/multiparts.py
+-rw-r--r--   0        0        0    18513 2023-11-15 14:48:56.190611 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/oms.py
+-rw-r--r--   0        0        0    16694 2024-04-18 16:52:37.754695 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/parts.py
+-rw-r--r--   0        0        0   126161 2024-04-18 18:30:05.847066 pyaedt-0.8.9/pyaedt/modeler/advanced_cad/stackup_3d.py
+-rw-r--r--   0        0        0    80218 2024-04-18 16:52:37.754695 pyaedt-0.8.9/pyaedt/modeler/cad/Modeler.py
+-rw-r--r--   0        0        0   341163 2024-04-19 11:54:25.539394 pyaedt-0.8.9/pyaedt/modeler/cad/Primitives.py
+-rw-r--r--   0        0        0    14615 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/Primitives2D.py
+-rw-r--r--   0        0        0   145579 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/Primitives3D.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.206131 pyaedt-0.8.9/pyaedt/modeler/cad/__init__.py
+-rw-r--r--   0        0        0    29755 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/component_array.py
+-rw-r--r--   0        0        0    41999 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/components_3d.py
+-rw-r--r--   0        0        0    49431 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/elements3d.py
+-rw-r--r--   0        0        0    60382 2024-04-19 11:54:25.539394 pyaedt-0.8.9/pyaedt/modeler/cad/object3d.py
+-rw-r--r--   0        0        0    52803 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/cad/polylines.py
+-rw-r--r--   0        0        0    12604 2023-11-15 14:48:56.206131 pyaedt-0.8.9/pyaedt/modeler/calculators.py
+-rw-r--r--   0        0        0    43854 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesCircuit.py
+-rw-r--r--   0        0        0    39329 2024-04-12 06:22:14.197637 pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesEmit.py
+-rw-r--r--   0        0        0     8509 2024-04-18 16:52:37.770311 pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py
+-rw-r--r--   0        0        0    68054 2024-04-20 11:56:57.906165 pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesNexxim.py
+-rw-r--r--   0        0        0    15154 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.221789 pyaedt-0.8.9/pyaedt/modeler/circuits/__init__.py
+-rw-r--r--   0        0        0    34497 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/circuits/object3dcircuit.py
+-rw-r--r--   0        0        0    68299 2024-04-15 14:41:20.463366 pyaedt-0.8.9/pyaedt/modeler/geometry_operators.py
+-rw-r--r--   0        0        0     6949 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/modeler2d.py
+-rw-r--r--   0        0        0    66016 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/modeler3d.py
+-rw-r--r--   0        0        0    33126 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/modelerpcb.py
+-rw-r--r--   0        0        0    51427 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/pcb/Primitives3DLayout.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.221789 pyaedt-0.8.9/pyaedt/modeler/pcb/__init__.py
+-rw-r--r--   0        0        0    66142 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/pcb/object3dlayout.py
+-rw-r--r--   0        0        0    23878 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modeler/schematic.py
+-rw-r--r--   0        0        0    51557 2024-04-15 11:56:47.814636 pyaedt-0.8.9/pyaedt/modules/AdvancedPostProcessing.py
+-rw-r--r--   0        0        0   169948 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modules/Boundary.py
+-rw-r--r--   0        0        0    71749 2024-04-05 14:28:19.102805 pyaedt-0.8.9/pyaedt/modules/CableModeling.py
+-rw-r--r--   0        0        0    16319 2023-11-15 14:48:56.237302 pyaedt-0.8.9/pyaedt/modules/CircuitTemplates.py
+-rw-r--r--   0        0        0    56843 2024-04-19 11:54:25.539394 pyaedt-0.8.9/pyaedt/modules/DesignXPloration.py
+-rw-r--r--   0        0        0    40485 2024-04-18 16:52:37.785949 pyaedt-0.8.9/pyaedt/modules/LayerStackup.py
+-rw-r--r--   0        0        0   105999 2024-04-18 18:30:05.847066 pyaedt-0.8.9/pyaedt/modules/Material.py
+-rw-r--r--   0        0        0    33743 2024-04-18 18:30:05.847066 pyaedt-0.8.9/pyaedt/modules/MaterialLib.py
+-rw-r--r--   0        0        0    54992 2024-04-18 16:52:37.801540 pyaedt-0.8.9/pyaedt/modules/Mesh.py
+-rw-r--r--   0        0        0    12354 2024-04-09 15:05:58.103918 pyaedt-0.8.9/pyaedt/modules/Mesh3DLayout.py
+-rw-r--r--   0        0        0    49289 2024-04-18 12:07:48.958449 pyaedt-0.8.9/pyaedt/modules/MeshIcepak.py
+-rw-r--r--   0        0        0     4437 2023-11-15 14:48:56.237302 pyaedt-0.8.9/pyaedt/modules/OptimetricsTemplates.py
+-rw-r--r--   0        0        0   220742 2024-04-19 11:56:25.289183 pyaedt-0.8.9/pyaedt/modules/PostProcessor.py
+-rw-r--r--   0        0        0    72048 2024-03-08 11:06:30.309390 pyaedt-0.8.9/pyaedt/modules/SetupTemplates.py
+-rw-r--r--   0        0        0   147980 2024-04-19 16:05:23.675083 pyaedt-0.8.9/pyaedt/modules/SolveSetup.py
+-rw-r--r--   0        0        0    32997 2024-04-15 11:56:47.830268 pyaedt-0.8.9/pyaedt/modules/SolveSweeps.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/modules/__init__.py
+-rw-r--r--   0        0        0    31325 2024-04-18 16:52:37.801540 pyaedt-0.8.9/pyaedt/modules/monitor_icepak.py
+-rw-r--r--   0        0        0   137795 2024-04-16 10:25:44.004063 pyaedt-0.8.9/pyaedt/modules/report_templates.py
+-rw-r--r--   0        0        0   136275 2024-04-18 15:41:51.581857 pyaedt-0.8.9/pyaedt/modules/solutions.py
+-rw-r--r--   0        0        0    96011 2024-04-19 10:41:23.663533 pyaedt-0.8.9/pyaedt/q3d.py
+-rw-r--r--   0        0        0    10722 2024-04-15 11:56:47.830268 pyaedt-0.8.9/pyaedt/rmxprt.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/rpc/__init__.py
+-rw-r--r--   0        0        0      415 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/rpc/local_server.py
+-rw-r--r--   0        0        0    42608 2024-04-17 12:00:57.657032 pyaedt-0.8.9/pyaedt/rpc/rpyc_services.py
+-rw-r--r--   0        0        0        0 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/__init__.py
+-rw-r--r--   0        0        0     9463 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/hdm_parser.py
+-rw-r--r--   0        0        0     2096 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/hdm_utils.py
+-rw-r--r--   0        0        0     2607 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/matlab/HdmObject.m
+-rw-r--r--   0        0        0       97 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/matlab/README.md
+-rw-r--r--   0        0        0      735 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/matlab/SbrBounceType.m
+-rw-r--r--   0        0        0     2886 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/matlab/StopWatch.m
+-rw-r--r--   0        0        0     1402 2023-11-15 14:48:56.252956 pyaedt-0.8.9/pyaedt/sbrplus/matlab/add_3dlight.m
+-rw-r--r--   0        0        0      340 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/amp2db.m
+-rw-r--r--   0        0        0    36837 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/draw_rays1.m
+-rw-r--r--   0        0        0     4322 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/draw_wfobj.m
+-rw-r--r--   0        0        0    31414 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/filter_rays1.m
+-rw-r--r--   0        0        0     1504 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/filtered_tracks.m
+-rw-r--r--   0        0        0    20853 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/ld_sbrplushdm.m
+-rw-r--r--   0        0        0    14781 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/ld_wfobj.m
+-rw-r--r--   0        0        0      318 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/pwr2db.m
+-rw-r--r--   0        0        0     2607 2023-11-15 14:48:56.268468 pyaedt-0.8.9/pyaedt/sbrplus/matlab/validate_sfields.m
+-rw-r--r--   0        0        0     7621 2024-03-26 18:55:41.067597 pyaedt-0.8.9/pyaedt/sbrplus/plot.py
+-rw-r--r--   0        0        0    21565 2024-04-19 11:13:06.289079 pyaedt-0.8.9/pyaedt/twinbuilder.py
+-rw-r--r--   0        0        0     6768 2024-04-20 08:56:12.060663 pyaedt-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0    16490 1970-01-01 00:00:00.000000 pyaedt-0.8.9/PKG-INFO
```

### Comparing `pyaedt-0.8.8/LICENSE` & `pyaedt-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/README.md` & `pyaedt-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/__init__.py` & `pyaedt-0.8.9/pyaedt/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
 
 deprecation_warning()
 
 #
 
 pyaedt_path = os.path.dirname(__file__)
-__version__ = "0.8.8"
+__version__ = "0.8.9"
 version = __version__
 
 #
 
 import pyaedt.downloads as downloads
 from pyaedt.generic import constants
 import pyaedt.generic.DataHandlers as data_handler
```

### Comparing `pyaedt-0.8.8/pyaedt/aedt_logger.py` & `pyaedt-0.8.9/pyaedt/aedt_logger.py`

 * *Files 1% similar despite different names*

```diff
@@ -575,28 +575,28 @@
 
         if not des_name:
             des_name = ""
 
         if not level:
             level = "Design"
 
-        assert level in message_levels, "Message level must be `Design', 'Project', or 'Global'."
+        if level not in message_levels:
+            raise ValueError("Message level must be 'Design', 'Project', or 'Global'.")
 
         if self._log_on_desktop and self._desktop:
             if not proj_name and message_levels[level] > 0:
                 proj_name = self.project_name
             if not des_name and message_levels[level] > 1:
                 des_name = self.design_name
             if des_name and ";" in des_name:
                 des_name = des_name[des_name.find(";") + 1 :]
             try:
                 self._desktop.AddMessage(proj_name, des_name, message_type, message_text)
-
             except Exception:  # pragma: no cover
-                pass
+                self._global.info("Failed to add desktop message.")
 
     def _log_on_handler(self, message_type, message_text, *args, **kwargs):
         message_text = str(message_text)
         if args:
             try:
                 msg1 = message_text % tuple(str(i) for i in args)
             except TypeError:
@@ -656,15 +656,15 @@
         if proj_name is None:
             proj_name = self.project_name
         if des_name is None:
             des_name = self.design_name
         try:
             self._desktop.ClearMessages(proj_name, des_name, level)
         except Exception:  # pragma: no cover
-            pass
+            self._global.info("Failed to clear desktop messages.")
 
     @property
     def non_graphical(self):
         """Check if desktop is graphical or not.
 
         Returns
         -------
```

### Comparing `pyaedt-0.8.8/pyaedt/application/AEDT_File_Management.py` & `pyaedt-0.8.9/pyaedt/application/AEDT_File_Management.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/Analysis.py` & `pyaedt-0.8.9/pyaedt/application/Analysis.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,17 @@
 from pyaedt.modules.SolveSetup import SetupHFSSAuto
 from pyaedt.modules.SolveSetup import SetupMaxwell
 from pyaedt.modules.SolveSetup import SetupQ3D
 from pyaedt.modules.SolveSetup import SetupSBR
 from pyaedt.modules.SolveSweeps import SetupProps
 
 if is_linux and is_ironpython:
-    import subprocessdotnet as subprocess
+    import subprocessdotnet as subprocess  # nosec
 else:
-    import subprocess
+    import subprocess  # nosec
 
 
 class Analysis(Design, object):
     """Contains all common analysis functions.
 
     This class is inherited in the caller application and is accessible through it ( eg. ``hfss.method_name``).
 
@@ -83,14 +83,17 @@
     close_on_exit : bool
         Whether to release  AEDT on exit.
     student_version : bool
         Whether to enable the student version of AEDT.
     aedt_process_id : int, optional
         Only used when ``new_desktop_session = False``, specifies by process ID which instance
         of Electronics Desktop to point PyAEDT at.
+    ic_mode : bool, optional
+        Whether to set the design to IC mode. The default is ``False``.
+        This parameter applies only to HFSS 3D Layout.
 
     """
 
     def __init__(
         self,
         application,
         projectname,
@@ -101,14 +104,15 @@
         non_graphical,
         new_desktop_session,
         close_on_exit,
         student_version,
         machine="",
         port=0,
         aedt_process_id=None,
+        ic_mode=False,
     ):
         Design.__init__(
             self,
             application,
             projectname,
             designname,
             solution_type,
@@ -116,14 +120,15 @@
             non_graphical,
             new_desktop_session,
             close_on_exit,
             student_version,
             machine,
             port,
             aedt_process_id,
+            ic_mode,
         )
         self._excitation_objects = {}
         self._setup = None
         if setup_name:
             self.active_setup = setup_name
         self._materials = None
         self._available_variations = self.AvailableVariations(self)
@@ -281,18 +286,19 @@
             self._setup = None
             return self._setup
 
     @active_setup.setter
     def active_setup(self, setup_name):
         setup_list = self.existing_analysis_setups
         if setup_list:
-            assert setup_name in setup_list, "Invalid setup name {}".format(setup_name)
+            if setup_name not in setup_list:
+                raise ValueError("Setup name {} is invalid.".format(setup_name))
             self._setup = setup_name
         else:
-            raise AttributeError("No setup defined")
+            raise AttributeError("No setup is defined.")
 
     @property
     def existing_analysis_sweeps(self):
         """Existing analysis sweeps.
 
         Returns
         -------
@@ -702,15 +708,15 @@
             export_path = os.path.join(
                 export_folder, "{0}_{1}_{2}.csv".format(self.project_name, self.design_name, name_no_space)
             )
             try:
                 self.post.oreportsetup.ExportToFile(str(report_name), export_path)
                 self.logger.info("Export Data: {}".format(export_path))
             except Exception:
-                pass
+                self.logger.info("Failed to export to file.")
             exported_files.append(export_path)
 
         if touchstone_format == "MagPhase":
             touchstone_format_value = 0
         elif touchstone_format == "RealImag":
             touchstone_format_value = 1
         elif touchstone_format == "DbPhase":
@@ -941,27 +947,26 @@
             data_vals = self.design_properties["ModelSetup"]["GeometryCore"]["GeometryOperations"][
                 "SubModelDefinitions"
             ]["NativeComponentDefinition"]
             if not isinstance(data_vals, list) and isinstance(data_vals, (OrderedDict, dict)):
                 data_vals = [data_vals]
             for ds in data_vals:
                 try:
+                    component_name = "undefined"
                     if isinstance(ds, (OrderedDict, dict)):
-                        boundaries.append(
-                            NativeComponentObject(
-                                self,
-                                ds["NativeComponentDefinitionProvider"]["Type"],
-                                ds["BasicComponentInfo"]["ComponentName"],
-                                ds,
-                            )
-                        )
+                        component_type = ds["NativeComponentDefinitionProvider"]["Type"]
+                        component_name = ds["BasicComponentInfo"]["ComponentName"]
+                        native_component_object = NativeComponentObject(self, component_type, component_name, ds)
+                        boundaries.append(native_component_object)
                 except Exception:
-                    pass
+                    msg = "Failed to add native component object."
+                    msg_end = "." if component_name == "undefined" else "(named {}).".format(component_name)
+                    self.logger.debug(msg + msg_end)
         except Exception:
-            pass
+            self.logger.debug("Failed to add native component object.")
         return boundaries
 
     class AvailableVariations(object):
         def __init__(self, app):
             """Contains available variations.
 
             Parameters
@@ -1495,15 +1500,16 @@
 
         References
         ----------
 
         >>> oDesign.GetNominalVariation
         >>> oModule.GetOutputVariableValue
         """
-        assert variable in self.output_variables, "Output variable {} does not exist.".format(variable)
+        if variable not in self.output_variables:
+            raise KeyError("Output variable {} does not exist.".format(variable))
         nominal_variation = self.odesign.GetNominalVariation()
         if solution is None:
             solution = self.existing_analysis_sweeps[0]
         value = self.ooutput_variable.GetOutputVariableValue(
             variable, nominal_variation, solution, self.solution_type, []
         )
         return value
@@ -1546,42 +1552,43 @@
                 dict[entry] = mat_props._props
             else:
                 dict[entry] = {}
                 for prop_name in prop_names:
                     dict[entry][prop_name] = mat_props._props[prop_name]
         return dict
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(setup_name="name", num_cores="cores", num_tasks="tasks", num_gpu="gpus")
     def analyze(
         self,
-        setup_name=None,
-        num_cores=4,
-        num_tasks=1,
-        num_gpu=1,
+        name=None,
+        cores=4,
+        tasks=1,
+        gpus=1,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
         revert_to_initial_mesh=False,
         blocking=True,
     ):
         """Solve the active design.
 
         Parameters
         ----------
-        setup_name : str, optional
-            Setup to analyze. Default is ``None`` which solves all the setups.
-        num_cores : int, optional
+        name : str, optional
+            Setup to analyze. The default is ``None``, in which case all
+            setups are solved.
+        cores : int, optional
             Number of simulation cores. Default is ``4`` which is the number of cores available in license.
-        num_tasks : int, optional
-            Number of simulation tasks. Default is ``1``.
-            In bach solve, set num_tasks to ``-1`` to apply auto settings and distributed mode.
-        num_gpu : int, optional
-            Number of simulation graphic processing units to use. Default is ``0``.
+        tasks : int, optional
+            Number of simulation tasks. The default is ``1``.
+            In bach solve, set ``tasks`` to ``-1`` to apply auto settings and distributed mode.
+        gpus : int, optional
+            Number of simulation graphic processing units to use. The default is ``0``.
         acf_file : str, optional
             Full path to the custom ACF file.
         use_auto_settings : bool, optional
             Set ``True`` to use automatic settings for HPC. The option is only considered for setups
             that support automatic settings.
         solve_in_batch : bool, optional
             Whether to solve the project in batch or not.
@@ -1608,59 +1615,59 @@
         >>> oDesign.Analyze
         """
         if solve_in_batch:
             return self.solve_in_batch(
                 filename=None,
                 machine=machine,
                 run_in_thread=run_in_thread,
-                num_cores=num_cores,
-                num_tasks=num_tasks,
+                cores=cores,
+                tasks=tasks,
                 revert_to_initial_mesh=revert_to_initial_mesh,
             )
         else:
             return self.analyze_setup(
-                setup_name,
-                num_cores,
-                num_tasks,
-                num_gpu,
+                name,
+                cores,
+                tasks,
+                gpus,
                 acf_file,
                 use_auto_settings,
                 revert_to_initial_mesh=revert_to_initial_mesh,
                 blocking=blocking,
             )
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(num_cores="cores", num_tasks="tasks", num_gpu="gpus")
     def analyze_setup(
         self,
         name=None,
-        num_cores=4,
-        num_tasks=1,
-        num_gpu=0,
+        cores=4,
+        tasks=1,
+        gpus=0,
         acf_file=None,
         use_auto_settings=True,
         num_variations_to_distribute=None,
         allowed_distribution_types=None,
         revert_to_initial_mesh=False,
         blocking=True,
     ):
         """Analyze a design setup.
 
         Parameters
         ----------
         name : str, optional
             Name of the setup, which can be an optimetric setup or a simple setup.
-            If ``None`` all setups will be solved.
-        num_cores : int, optional
-            Number of simulation cores.  Default is ``1``.
-        num_tasks : int, optional
-            Number of simulation tasks.  Default is ``1``.
-        num_gpu : int, optional
-            Number of simulation graphics processing units.  Default is ``0``.
+            The default is ``None``, in which case all setups are solved.
+        cores : int, optional
+            Number of simulation cores.  The default is ``1``.
+        tasks : int, optional
+            Number of simulation tasks.  The default is ``1``.
+        gpus : int, optional
+            Number of simulation graphics processing units.  The default is ``0``.
         acf_file : str, optional
-            Full path to custom ACF file. The default is ``None.``
+            Full path to the custom ACF file. The default is ``None``.
         use_auto_settings : bool, optional
             Either if use or not auto settings in task/cores. It is not supported by all Setup.
         num_variations_to_distribute : int, optional
             Number of variations to distribute. For this to take effect ``use_auto_settings`` must be set to ``True``.
         allowed_distribution_types : list, optional
             List of strings. Each string represents a distribution type. The default value ``None`` does nothing.
             An empty list ``[]`` disables all types.
@@ -1689,20 +1696,18 @@
             with open_file(acf_file, "r") as f:
                 lines = f.readlines()
                 for line in lines:
                     if "ConfigName" in line:
                         name = line.strip().split("=")[1]
                         break
             if name:
-                try:
-                    self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, name)
+                success = self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, name)
+                if success:
                     set_custom_dso = True
-                except Exception:
-                    pass
-        elif num_gpu or num_tasks or num_cores:
+        elif gpus or tasks or cores:
             config_name = "pyaedt_config"
             source_name = os.path.join(self.pyaedt_dir, "misc", "pyaedt_local_config.acf")
             if settings.remote_rpc_session:
                 target_name = os.path.join(tempfile.gettempdir(), generate_unique_name("config") + ".acf")
             else:
                 target_name = (
                     os.path.join(self.working_directory, config_name + ".acf").replace("\\", "/")
@@ -1721,22 +1726,22 @@
                 self.logger.error("Permission denied.")
                 skip_files = True
             # For other errors
             except Exception:
                 self.logger.error("Error occurred while copying file.")
                 skip_files = True
             if not skip_files:
-                if num_cores:
-                    succeeded = update_hpc_option(target_name, "NumCores", num_cores, False)
+                if cores:
+                    succeeded = update_hpc_option(target_name, "NumCores", cores, False)
                     skip_files = True if not succeeded else skip_files
-                if num_gpu:
-                    succeeded = update_hpc_option(target_name, "NumGPUs", num_gpu, False)
+                if gpus:
+                    succeeded = update_hpc_option(target_name, "NumGPUs", gpus, False)
                     skip_files = True if not succeeded else skip_files
-                if num_tasks:
-                    succeeded = update_hpc_option(target_name, "NumEngines", num_tasks, False)
+                if tasks:
+                    succeeded = update_hpc_option(target_name, "NumEngines", tasks, False)
                     skip_files = True if not succeeded else skip_files
                 succeeded = update_hpc_option(target_name, "ConfigName", config_name, True)
                 skip_files = True if not succeeded else skip_files
                 succeeded = update_hpc_option(target_name, "DesignType", self.design_type, True)
                 skip_files = True if not succeeded else skip_files
                 if self.design_type == "Icepak":
                     use_auto_settings = False
@@ -1767,18 +1772,18 @@
                 target_name = remote_name
             if not skip_files:
                 try:
                     self._desktop.SetRegistryFromFile(target_name)
                     self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, config_name)
                     set_custom_dso = True
                 except Exception:
-                    pass
+                    self.logger.info("Failed to set registry from file {}.".format(target_name))
         if not name:
             try:
-                self.logger.info("Solving all design setups")
+                self.logger.info("Solving all design setups.")
                 if self.desktop_class.aedt_version_id > "2023.1":
                     self.odesign.AnalyzeAll(blocking)
                 else:
                     self.odesign.AnalyzeAll()
             except Exception:
                 if set_custom_dso:
                     self.set_registry_key(r"Desktop/ActiveDSOConfigurations/" + self.design_type, active_config)
@@ -1854,23 +1859,23 @@
         Returns
         -------
         str
 
         """
         return self.desktop_class.stop_simulations(clean_stop=clean_stop)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(numcores="cores", num_tasks="tasks", setup_name="setup")
     def solve_in_batch(
         self,
         filename=None,
         machine="localhost",
         run_in_thread=False,
-        num_cores=4,
-        num_tasks=1,
-        setup_name=None,
+        cores=4,
+        tasks=1,
+        setup=None,
         revert_to_initial_mesh=False,
     ):  # pragma: no cover
         """Analyze a design setup in batch mode.
 
         .. note::
            To use this function, the project must be closed.
 
@@ -1880,22 +1885,24 @@
             Name of the setup. The default is ``None``, which means that the active project
             is to be solved.
         machine : str, optional
             Name of the machine if remote.  The default is ``"localhost"``.
         run_in_thread : bool, optional
             Whether to submit the batch command as a thread. The default is
             ``False``.
-        num_cores : int, optional
-            Number of cores to use in simulation.
-        num_tasks : int, optional
-            Number of tasks to use in simulation. Set num_tasks to ``-1`` to apply auto settings and distributed mode.
-        setup_name : str
-            Name of the setup, which can be an optimetric setup or a simple setup. If ``None`` all setup will be solved.
+        cores : int, optional
+            Number of cores to use in the simulation.
+        tasks : int, optional
+            Number of tasks to use in the simulation.
+            Set ``num_tasks`` to ``-1`` to apply auto settings and distributed mode.
+        setup : str
+            Name of the setup, which can be an optimetric setup or a simple setup.
+            The default is ``None``, in which case all setups are solved.
         revert_to_initial_mesh : bool, optional
-            Whether to revert to initial mesh before solving or not. Default is ``False``.
+            Whether to revert to the initial mesh before solving. The default is ``False``.
 
         Returns
         -------
          bool
            ``True`` when successful, ``False`` when failed.
         """
         inst_dir = self.desktop_install_dir
@@ -1915,61 +1922,50 @@
         queue_file = filename + ".q"
         queue_file_completed = filename + ".q.completed"
         if os.path.exists(queue_file):
             os.unlink(queue_file)
         if os.path.exists(queue_file_completed):
             os.unlink(queue_file_completed)
 
-        if is_linux and settings.use_lsf_scheduler:
-            options = [
-                "-ng",
-                "-BatchSolve",
-                "-machinelist",
-                "list={}:{}:{}:90%:1".format(machine, num_tasks, num_cores),
-                "-Monitor",
-            ]
-            if num_tasks == -1:
-                options.append("-distributed")
-                options.append("-auto")
-        else:
-            options = [
-                "-ng",
-                "-BatchSolve",
-                "-machinelist",
-                "list={}:{}:{}:90%:1".format(machine, num_tasks, num_cores),
-                "-Monitor",
-            ]
-        if setup_name and design_name:
+        options = [
+            "-ng",
+            "-BatchSolve",
+            "-machinelist",
+            "list={}:{}:{}:90%:1".format(machine, tasks, cores),
+            "-Monitor",
+        ]
+        if is_linux and settings.use_lsf_scheduler and tasks == -1:
+            options.append("-distributed")
+            options.append("-auto")
+        if setup and design_name:
             options.append(
-                "{}:{}:{}".format(
-                    design_name, "Nominal" if setup_name in self.setup_names else "Optimetrics", setup_name
-                )
+                "{}:{}:{}".format(design_name, "Nominal" if setup in self.setup_names else "Optimetrics", setup)
             )
         if is_linux and not settings.use_lsf_scheduler:
             batch_run = [inst_dir + "/ansysedt"]
         elif is_linux and settings.use_lsf_scheduler:  # pragma: no cover
             if settings.lsf_queue:
                 batch_run = [
                     "bsub",
                     "-n",
-                    str(num_cores),
+                    str(cores),
                     "-R",
-                    "span[ptile={}]".format(num_cores),
+                    "span[ptile={}]".format(cores),
                     "-R",
                     "rusage[mem={}]".format(settings.lsf_ram),
                     "-queue {}".format(settings.lsf_queue),
                     settings.lsf_aedt_command,
                 ]
             else:
                 batch_run = [
                     "bsub",
                     "-n",
-                    str(num_cores),
+                    str(cores),
                     "-R",
-                    "span[ptile={}]".format(num_cores),
+                    "span[ptile={}]".format(cores),
                     "-R",
                     "rusage[mem={}]".format(settings.lsf_ram),
                     settings.lsf_aedt_command,
                 ]
         else:
             batch_run = [inst_dir + "/ansysedt.exe"]
         batch_run.extend(options)
@@ -1979,15 +1975,14 @@
         # don't have old .asol files etc
 
         self.logger.info("Solving model in batch mode on " + machine)
         if run_in_thread and is_windows:
             DETACHED_PROCESS = 0x00000008
             subprocess.Popen(batch_run, creationflags=DETACHED_PROCESS)
             self.logger.info("Batch job launched.")
-
         else:
             subprocess.Popen(batch_run)
             self.logger.info("Batch job finished.")
 
         if machine == "localhost":
             while not os.path.exists(queue_file):
                 time.sleep(0.5)
```

### Comparing `pyaedt-0.8.8/pyaedt/application/Analysis3D.py` & `pyaedt-0.8.9/pyaedt/application/Analysis3D.py`

 * *Files 2% similar despite different names*

```diff
@@ -699,18 +699,18 @@
         --------
         The method :func:`assign_material` is used to assign a material to a list of objects.
 
         Open a design and create the objects.
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> box1 = hfss.modeler.create_box([10, 10, 10], [4, 5, 5])
-        >>> box2 = hfss.modeler.create_box([0, 0, 0], [2, 3, 4])
-        >>> cylinder1 = hfss.modeler.create_cylinder(cs_axis="X", position=[5, 0, 0], radius=1, height=20)
-        >>> cylinder2 = hfss.modeler.create_cylinder(cs_axis="Z", position=[0, 0, 5], radius=1, height=10)
+        >>> box1 = hfss.modeler.create_box([10, 10, 10],[4, 5, 5])
+        >>> box2 = hfss.modeler.create_box([0, 0, 0],[2, 3, 4])
+        >>> cylinder1 = hfss.modeler.create_cylinder(orientation="X",origin=[5, 0, 0],radius=1,height=20)
+        >>> cylinder2 = hfss.modeler.create_cylinder(orientation="Z",origin=[0, 0, 5],radius=1,height=10)
 
         Assign the material ``"copper"`` to all the objects.
 
         >>> objects_list = [box1, box2, cylinder1, cylinder2]
         >>> hfss.assign_material(objects_list, "copper")
 
         The method also accepts a list of object names.
@@ -1031,15 +1031,16 @@
                 for key, val in self.modeler.user_defined_components.items()
                 if val.definition_name not in native_comp_names
             ]
         else:
             if isinstance(component_name, str):
                 component_name = [component_name]
             for cmp in component_name:
-                assert cmp in self.modeler.user_defined_component_names, "Component Definition not found."
+                if cmp not in self.modeler.user_defined_component_names:
+                    raise ValueError("Component definition was not found for '{}'.".format(cmp))
 
         for cmp in component_name:
             comp = self.modeler.user_defined_components[cmp]
             target_cs = self.modeler._create_reference_cs_from_3dcomp(comp, password=password)
             app = comp.edit_definition(password=password)
             for var, val in comp.parameters.items():
                 app[var] = val
@@ -1306,25 +1307,25 @@
             vArg3.append("dest_selected:="), vArg3.append(False)
             vArg3.append("layer_type:="), vArg3.append("signal")
             vArg2.append(vArg3)
         vArg1.append(vArg2)
         self.oeditor.ImportDXF(vArg1)
         return True
 
-    @pyaedt_function_handler
-    def import_gds_3d(self, gds_file, gds_number, unit="um", import_method=1):  # pragma: no cover
+    @pyaedt_function_handler(gds_file="input_file", gds_number="mapping_layers", unit="units")
+    def import_gds_3d(self, input_file, mapping_layers, units="um", import_method=1):  # pragma: no cover
         """Import a GDSII file.
 
         Parameters
         ----------
-        gds_file : str
+        input_file : str
             Path to the GDS file.
-        gds_number : dict
+        mapping_layers : dict
             Dictionary keys are GDS layer numbers, and the value is a tuple with the thickness and elevation.
-        unit : string, optional
+        units : string, optional
             Length unit values. The default is ``"um"``.
         import_method : integer, optional
             GDSII import method. The default is ``1``. Options are:
 
             - ``0`` for script.
             - ``1`` for Parasolid.
 
@@ -1341,31 +1342,31 @@
         --------
         Import a GDS file in an HFSS 3D project.
 
         >>> gds_path = r"C:\\temp\\gds1.gds"
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> gds_number = {7: (100, 10), 9: (110, 5)}
-        >>> hfss.import_gds_3d(gds_path, gds_number, unit="um", import_method=1)
+        >>> hfss.import_gds_3d(gds_path,gds_number,units="um",import_method=1)
 
         """
 
         if self.desktop_class.non_graphical:
             self.logger.error("Method is supported only in graphical mode.")
             return False
-        if not os.path.exists(gds_file):
+        if not os.path.exists(input_file):
             self.logger.error("GDSII file does not exist. No layer is imported.")
             return False
-        if len(gds_number) == 0:
+        if len(mapping_layers) == 0:
             self.logger.error("Dictionary for GDSII layer numbers is empty. No layer is imported.")
             return False
 
         layermap = ["NAME:LayerMap"]
         ordermap = []
-        for i, k in enumerate(gds_number):
+        for i, k in enumerate(mapping_layers):
             layername = "signal" + str(k)
             layermap.append(
                 [
                     "NAME:LayerMapInfo",
                     "LayerNum:=",
                     k,
                     "DestLayer:=",
@@ -1380,28 +1381,28 @@
                     "order:=",
                     i,
                     "layer:=",
                     layername,
                     "LayerNumber:=",
                     k,
                     "Thickness:=",
-                    unit_converter(gds_number[k][1], unit_system="Length", input_units=unit, output_units="meter"),
+                    unit_converter(mapping_layers[k][1], unit_system="Length", input_units=units, output_units="meter"),
                     "Elevation:=",
-                    unit_converter(gds_number[k][0], unit_system="Length", input_units=unit, output_units="meter"),
+                    unit_converter(mapping_layers[k][0], unit_system="Length", input_units=units, output_units="meter"),
                     "Color:=",
                     "color",
                 ],
             ]
             ordermap.extend(ordermap1)
 
         self.oeditor.ImportGDSII(
             [
                 "NAME:options",
                 "FileName:=",
-                gds_file,
+                input_file,
                 "FlattenHierarchy:=",
                 True,
                 "ImportMethod:=",
                 import_method,
                 layermap,
                 "OrderMap:=",
                 ordermap,
```

### Comparing `pyaedt-0.8.8/pyaedt/application/Analysis3DLayout.py` & `pyaedt-0.8.9/pyaedt/application/Analysis3DLayout.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,16 +47,18 @@
         machine. The default is ``False``.
     close_on_exit : bool, optional
         Whether to release AEDT on exit. The default is ``False``.
     student_version : bool, optional
         Whether to enable the student version of AEDT. The default
         is ``False``.
     aedt_process_id : int, optional
-        Only used when ``new_desktop_session = False``, specifies by process ID which instance
-        of Electronics Desktop to point PyAEDT at.
+        Specifies by process ID the instance of AEDT to point PyAEDT at.
+        This parameter is only used when ``new_desktop_session=False``.
+    ic_mode : bool, optional
+        Whether to set the design to IC mode. The default is ``False``.
 
     """
 
     def __init__(
         self,
         application,
         projectname,
@@ -67,14 +69,15 @@
         non_graphical=False,
         new_desktop_session=False,
         close_on_exit=False,
         student_version=False,
         machine="",
         port=0,
         aedt_process_id=None,
+        ic_mode=False,
     ):
         Analysis.__init__(
             self,
             application,
             projectname,
             designname,
             solution_type,
@@ -83,14 +86,15 @@
             non_graphical,
             new_desktop_session,
             close_on_exit,
             student_version,
             machine,
             port,
             aedt_process_id,
+            ic_mode,
         )
         self._modeler = None
         self._mesh = None
         self._post = None
         self._configurations = Configurations3DLayout(self)
         if not settings.lazy_load:
             self._modeler = self.modeler
```

### Comparing `pyaedt-0.8.8/pyaedt/application/AnalysisMaxwellCircuit.py` & `pyaedt-0.8.9/pyaedt/application/AnalysisMaxwellCircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/AnalysisNexxim.py` & `pyaedt-0.8.9/pyaedt/application/AnalysisNexxim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/AnalysisRMxprt.py` & `pyaedt-0.8.9/pyaedt/application/AnalysisRMxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/AnalysisTwinBuilder.py` & `pyaedt-0.8.9/pyaedt/application/AnalysisTwinBuilder.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/Design.py` & `pyaedt-0.8.9/pyaedt/application/Design.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
         Whether to release AEDT on exit. The default is ``False``.
     student_version : bool, optional
         Whether to enable the student version of AEDT. The default
         is ``False``.
     aedt_process_id : int, optional
         Only used when ``new_desktop_session = False``, specifies by process ID which instance
         of Electronics Desktop to point PyAEDT at.
+    ic_mode : bool, optional
+        Whether to set the design to IC mode or not. The default is ``False``. Applicable only to ``Hfss3dLayout``.
 
     """
 
     @property
     def _pyaedt_details(self):
         import platform
 
@@ -195,26 +197,28 @@
         non_graphical=False,
         new_desktop_session=False,
         close_on_exit=False,
         student_version=False,
         machine="",
         port=0,
         aedt_process_id=None,
+        ic_mode=False,
     ):
 
         self.__t = None
         if (
             not is_ironpython
             and project_name
             and os.path.exists(project_name)
             and (os.path.splitext(project_name)[1] == ".aedt" or os.path.splitext(project_name)[1] == ".a3dcomp")
         ):
             self.__t = threading.Thread(target=load_aedt_thread, args=(project_name,), daemon=True)
             self.__t.start()
         self._init_variables()
+        self._ic_mode = ic_mode
         self._design_type = design_type
         self.last_run_log = ""
         self.last_run_job = ""
         self._design_dictionary = None
         # Get Desktop from global Desktop Environment
         self._project_dictionary = OrderedDict()
         self._boundaries = {}
@@ -392,15 +396,15 @@
             else:
                 self._boundaries[boundary] = BoundaryObject(self, boundary, boundarytype=boundarytype)
         try:
             for k, v in zip(current_excitations, current_excitation_types):
                 if k not in self._boundaries:
                     self._boundaries[k] = BoundaryObject(self, k, boundarytype=v)
         except Exception:
-            pass
+            self.logger.info("Failed to design boundary object.")
         return list(self._boundaries.values())
 
     @property
     def boundaries_by_type(self):
         """Design boundaries by type.
 
         Returns
@@ -512,16 +516,17 @@
             and settings.remote_rpc_session
             and settings.remote_rpc_session.filemanager.pathexists(self.project_file)
         ):
             file_path = check_and_download_file(self.project_file)
             try:
                 settings._project_properties[os.path.normpath(self.project_file)] = load_entire_aedt_file(file_path)
             except Exception:
-                pass
-            self._logger.info("aedt file load time {}".format(time.time() - start))
+                self._logger.info("Failed to load AEDT file.")
+            else:
+                self._logger.info("Time to load AEDT file: {}.".format(time.time() - start))
         if os.path.normpath(self.project_file) in settings._project_properties:
             return settings._project_properties[os.path.normpath(self.project_file)]
         return {}
 
     @property
     def design_properties(self):
         """Design properties.
@@ -613,15 +618,16 @@
             timestep = 0.1
             while new_name not in [
                 i.GetName() if ";" not in i.GetName() else i.GetName().split(";")[1]
                 for i in list(self._oproject.GetDesigns())
             ]:
                 time.sleep(timestep)
                 timeout -= timestep
-                assert timeout >= 0
+                if timeout < 0:
+                    raise RuntimeError("Timeout reached while checking design renaming.")
 
     @property
     def design_list(self):
         """Design list.
 
         Returns
         -------
@@ -1062,14 +1068,16 @@
 
             else:
                 self.logger.info(warning_msg)
                 self._insert_design(self._design_type)
                 self.design_solutions._odesign = self.odesign
                 if self._temp_solution_type:
                     self.design_solutions.solution_type = self._temp_solution_type
+        if self.solution_type == "HFSS3DLayout" or self.solution_type == "HFSS 3D Layout Design":
+            self.set_oo_property_value(self.odesign, "Design Settings", "Design Mode/IC", self._ic_mode)
 
     @property
     def oproject(self):
         """Project property.
 
         Returns
         -------
@@ -1118,17 +1126,16 @@
                         project = proj_name[:-5] + ".aedt"
                     if os.path.exists(project) and self.check_if_project_is_loaded(project):
                         pname = self.check_if_project_is_loaded(project)
                         self._oproject = self.odesktop.SetActiveProject(pname)
                         self._add_handler()
                         self.logger.info("Project %s set to active.", pname)
                     elif os.path.exists(project):
-                        assert not is_project_locked(
-                            project
-                        ), "Project is locked. Close or remove the lock before proceeding."
+                        if is_project_locked(project):
+                            raise RuntimeError("Project is locked. Close or remove the lock before proceeding.")
                         self.logger.info("aedt project found. Loading it.")
                         self._oproject = self.odesktop.OpenProject(project)
                         self._add_handler()
                         self.logger.info("Project %s has been opened.", self._oproject.GetName())
                         time.sleep(0.5)
                     else:
                         oTool = self.odesktop.GetTool("ImportExport")
@@ -1144,17 +1151,16 @@
                         )
                 elif self.check_if_project_is_loaded(proj_name):
                     pname = self.check_if_project_is_loaded(proj_name)
                     self._oproject = self.odesktop.SetActiveProject(pname)
                     self._add_handler()
                     self.logger.info("Project %s set to active.", pname)
                 else:
-                    assert not is_project_locked(
-                        proj_name
-                    ), "Project is locked. Close or remove the lock before proceeding."
+                    if is_project_locked(proj_name):
+                        raise RuntimeError("Project is locked. Close or remove the lock before proceeding.")
                     self._oproject = self.odesktop.OpenProject(proj_name)
                     self._add_handler()
                     self.logger.info("Project %s has been opened.", self._oproject.GetName())
                     time.sleep(0.5)
             elif settings.force_error_on_missing_project and ".aedt" in proj_name:
                 raise Exception("Project doesn't exist. Check it and retry.")
             else:
@@ -1292,27 +1298,55 @@
         """Return the Object Oriented AEDT Object Properties.
 
         Parameters
         ----------
         aedt_object : object
             AEDT Object on which search for property. It can be any oProperty (ex. oDesign).
         object_name : str
-            Path to the object list. Example ``"DesignName\\Boundaries"``.
+            Path to the object list. For example, ``"DesignName\\Boundaries"``.
+        prop_name : str
+            Property name.
 
         Returns
         -------
         str, float, bool
-            Values returned by method if any.
+            ``True`` when successful, ``False`` when failed.
         """
         try:
             return aedt_object.GetChildObject(object_name).GetPropValue(prop_name)
         except Exception:
             return None
 
     @pyaedt_function_handler()
+    def set_oo_property_value(self, aedt_object, object_name, prop_name, value):
+        """Change the property value of the object-oriented AEDT object.
+
+        Parameters
+        ----------
+        aedt_object : object
+            AEDT object to search for the property on. It can be any oProperty. For example, oDesign.
+        object_name : str
+            Path to the object list. Example ``"DesignName\\Boundaries"``.
+        prop_name : str
+            Property name.
+        value : str
+            Property value.
+
+        Returns
+        -------
+        bool
+            Values returned by method if any.
+        """
+        try:
+            aedt_object.GetChildObject(object_name).SetPropValue(prop_name, value)
+            return True
+        except Exception:
+            return False
+
+    @pyaedt_function_handler()
     def export_profile(self, setup_name, variation_string="", file_path=None):
         """Export a solution profile to a PROF file.
 
         Parameters
         ----------
         setup_name : str
             Setup name. For example, ``'Setup1'``.
@@ -2208,15 +2242,15 @@
                                     self,
                                     ds,
                                     self.design_properties["BoundarySetup"]["Boundaries"][ds],
                                     self.design_properties["BoundarySetup"]["Boundaries"][ds]["BoundType"],
                                 )
                             )
                 except Exception:
-                    pass
+                    self.logger.debug("Failed to retrieve boundary data from 'BoundarySetup'.")
         if self.design_properties and "MaxwellParameterSetup" in self.design_properties:
             for ds in self.design_properties["MaxwellParameterSetup"]["MaxwellParameters"]:
                 try:
                     param = "MaxwellParameters"
                     setup = "MaxwellParameterSetup"
                     if isinstance(self.design_properties[setup][param][ds], (OrderedDict, dict)):
                         boundaries.append(
@@ -2226,15 +2260,15 @@
                                 self.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds],
                                 self.design_properties["MaxwellParameterSetup"]["MaxwellParameters"][ds][
                                     "MaxwellParameterType"
                                 ],
                             )
                         )
                 except Exception:
-                    pass
+                    self.logger.debug("Failed to retrieve boundary data from 'MaxwellParameterSetup'.")
         if self.design_properties and "ModelSetup" in self.design_properties:
             if "MotionSetupList" in self.design_properties["ModelSetup"]:
                 for ds in self.design_properties["ModelSetup"]["MotionSetupList"]:
                     try:
                         motion_list = "MotionSetupList"
                         setup = "ModelSetup"
                         # check moving part
@@ -2244,15 +2278,15 @@
                                     self,
                                     ds,
                                     self.design_properties["ModelSetup"]["MotionSetupList"][ds],
                                     self.design_properties["ModelSetup"]["MotionSetupList"][ds]["MotionType"],
                                 )
                             )
                     except Exception:
-                        pass
+                        self.logger.debug("Failed to retrieve boundary data from 'ModelSetup'.")
         if self.design_type in ["HFSS 3D Layout Design"]:
             for port in self.oboundary.GetAllPortsList():
                 bound = self._update_port_info(port)
                 if bound:
                     boundaries.append(bound)
         return boundaries
 
@@ -2323,27 +2357,27 @@
         try:
             for ds in self.project_properties["AnsoftProject"]["ProjectDatasets"]["DatasetDefinitions"]:
                 data = self.project_properties["AnsoftProject"]["ProjectDatasets"]["DatasetDefinitions"][ds][
                     "Coordinates"
                 ]
                 datasets[ds] = self._get_ds_data(ds, data)
         except Exception:
-            pass
+            self.logger.debug("Failed to retrieve project data sets.")
         return datasets
 
     @pyaedt_function_handler()
     def _get_design_datasets(self):
         """ """
         datasets = {}
         try:
             for ds in self.design_properties["ModelSetup"]["DesignDatasets"]["DatasetDefinitions"]:
                 data = self.design_properties["ModelSetup"]["DesignDatasets"]["DatasetDefinitions"][ds]["Coordinates"]
                 datasets[ds] = self._get_ds_data(ds, data)
         except Exception:
-            pass
+            self.logger.debug("Failed to retrieve design data sets.")
         return datasets
 
     @pyaedt_function_handler()
     def close_desktop(self):
         """Close AEDT and release it.
 
         Returns
@@ -3260,17 +3294,17 @@
         self._init_design(
             project_name=self.project_name if self.project_name else generate_unique_name("Project"),
             design_name=design_name,
             solution_type=solution_type if solution_type else self.solution_type,
         )
 
     def _insert_design(self, design_type, design_name=None):
-        assert design_type in self.design_solutions.design_types, "Invalid design type for insert: {}".format(
-            design_type
-        )
+        if design_type not in self.design_solutions.design_types:
+            raise ValueError("Design type of insert '{}' is invalid.".format(design_type))
+
         # self.save_project() ## Commented because it saves a Projectxxx.aedt when launched on an empty Desktop
         unique_design_name = self._generate_unique_design_name(design_name)
 
         if design_type == "RMxprtSolution":
             new_design = self._oproject.InsertDesign("RMxprt", unique_design_name, "Inner-Rotor Induction Machine", "")
         elif design_type == "ModelCreation":
             new_design = self._oproject.InsertDesign(
@@ -3667,15 +3701,16 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesktop.DeleteProject
         """
-        assert self.project_name != project_name, "You cannot delete the active project."
+        if self.project_name == project_name:
+            raise ValueError("You cannot delete the active project.")
         self.odesktop.DeleteProject(project_name)
         return True
 
     @pyaedt_function_handler()
     def set_active_design(self, name):
         """Change the active design to another design.
 
@@ -3894,21 +3929,18 @@
 
     @pyaedt_function_handler()
     def _assert_consistent_design_type(self, des_name):
         if des_name in self.design_list:
             self._odesign = self._oproject.SetActiveDesign(des_name)
             dtype = self._odesign.GetDesignType()
             if dtype != "RMxprt":
-                assert dtype == self._design_type, "Error: Specified design is not of type {}.".format(
-                    self._design_type
-                )
-            else:
-                assert ("RMxprtSolution" == self._design_type) or (
-                    "ModelCreation" == self._design_type
-                ), "Error: Specified design is not of type {}.".format(self._design_type)
+                if dtype != self._design_type:
+                    raise ValueError("Specified design is not of type {}.".format(self._design_type))
+            elif self._design_type not in {"RMxprtSolution", "ModelCreation"}:
+                raise ValueError("Specified design is not of type {}.".format(self._design_type))
             return True
         elif ":" in des_name:
             try:
                 self._odesign = self._oproject.SetActiveDesign(des_name)
                 return True
             except Exception:
                 return des_name
```

### Comparing `pyaedt-0.8.8/pyaedt/application/JobManager.py` & `pyaedt-0.8.9/pyaedt/application/JobManager.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/Variables.py` & `pyaedt-0.8.9/pyaedt/application/Variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -2314,35 +2314,35 @@
             self._app._oproject.DeleteDataset(self.name)
             del self._app.project_datasets[self.name]
         else:
             self._app._odesign.DeleteDataset(self.name)
             del self._app.design_datasets[self.name]
         return True
 
-    @pyaedt_function_handler()
-    def export(self, dataset_path=None):
+    @pyaedt_function_handler(dataset_path="output_dir")
+    def export(self, output_dir=None):
         """Export the dataset.
 
         Parameters
         ----------
-        dataset_path : str, optional
+        output_dir : str, optional
             Path to export the dataset to. The default is ``None``, in which
             case the dataset is exported to the working_directory path.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oProject.ExportDataset
         >>> oDesign.ExportDataset
         """
-        if not dataset_path:
-            dataset_path = os.path.join(self._app.working_directory, self.name + ".tab")
+        if not output_dir:
+            output_dir = os.path.join(self._app.working_directory, self.name + ".tab")
         if self.name[0] == "$":
-            self._app._oproject.ExportDataset(self.name, dataset_path)
+            self._app._oproject.ExportDataset(self.name, output_dir)
         else:
-            self._app._odesign.ExportDataset(self.name, dataset_path)
+            self._app._odesign.ExportDataset(self.name, output_dir)
         return True
```

### Comparing `pyaedt-0.8.8/pyaedt/application/aedt_objects.py` & `pyaedt-0.8.9/pyaedt/application/aedt_objects.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/analysis_hf.py` & `pyaedt-0.8.9/pyaedt/application/analysis_hf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/application/design_solutions.py` & `pyaedt-0.8.9/pyaedt/application/design_solutions.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/circuit.py` & `pyaedt-0.8.9/pyaedt/circuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -161,30 +161,30 @@
         value = value.replace("µ", "u")
         try:
             float(value)
             return value
         except Exception:
             return from_rkm_to_aedt(value)
 
-    @pyaedt_function_handler()
-    def create_schematic_from_netlist(self, file_to_import):
+    @pyaedt_function_handler(file_to_import="input_file")
+    def create_schematic_from_netlist(self, input_file):
         """Create a circuit schematic from an HSpice netlist.
 
         Supported currently are:
 
         * R
         * L
         * C
         * Diodes
         * Bjts
         * Discrete components with syntax ``Uxxx net1 net2 ... netn modname``
 
         Parameters
         ----------
-        file_to_import : str
+        input_file : str
             Full path to the HSpice file to import.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -197,15 +197,15 @@
         use_instance = True
         model = []
         self._desktop.CloseAllWindows()
         autosave = False
         if self._desktop.GetAutoSaveEnabled() == 1:
             self._desktop.EnableAutoSave(False)
             autosave = True
-        with open_file(file_to_import, "rb") as f:
+        with open_file(input_file, "rb") as f:
             for line in f:
                 line = line.decode("utf-8")
                 if ".param" in line[:7].lower():
                     try:
                         param_line = " ".join(line[7:].split())
                         param_re = re.split("[ =]", param_line)
 
@@ -223,18 +223,18 @@
             self.modeler.schematic.create_component(
                 None,
                 component_library=None,
                 component_name="Models_Netlist",
                 location=[xpos, 0],
                 global_netlist_list=model,
             )
-            self.modeler.schematic.disable_data_netlist(component_name="Models_Netlist")
+            self.modeler.schematic.disable_data_netlist(assignment="Models_Netlist")
             xpos += 0.0254
         counter = 0
-        with open_file(file_to_import, "rb") as f:
+        with open_file(input_file, "rb") as f:
             for line in f:
                 line = line.decode("utf-8")
                 mycomp = None
                 fields = line.split(" ")
                 name = fields[0].replace(".", "")
 
                 if fields[0][0] == "R":
@@ -303,19 +303,15 @@
                         self.modeler.schematic.create_symbol(parameter, pins)
                         already_exist = False
                         for el in self.modeler.schematic.components:
                             if self.modeler.schematic.components[el].name == parameter:
                                 already_exist = True
                         if not already_exist:
                             self.modeler.schematic.create_new_component_from_symbol(
-                                parameter,
-                                pins,
-                                refbase=fields[0][0],
-                                parameter_list=parameter_list,
-                                parameter_value=parameter_value,
+                                parameter, pins, refbase=fields[0][0], parameters=parameter_list, values=parameter_value
                             )
                         mycomp = self.modeler.schematic.create_component(
                             fields[0],
                             component_library=None,
                             component_name=parameter,
                             location=[xpos, ypos],
                             use_instance_id_netlist=use_instance,
@@ -338,19 +334,15 @@
                     self.modeler.schematic.create_symbol(parameter, pins)
                     already_exist = False
                     for el in self.modeler.schematic.components:
                         if self.modeler.schematic.components[el].name == parameter:
                             already_exist = True
                     if not already_exist:
                         self.modeler.schematic.create_new_component_from_symbol(
-                            parameter,
-                            pins,
-                            refbase=fields[0][0],
-                            parameter_list=parameter_list,
-                            parameter_value=parameter_value,
+                            parameter, pins, refbase=fields[0][0], parameters=parameter_list, values=parameter_value
                         )
                     mycomp = self.modeler.schematic.create_component(
                         fields[0],
                         component_library=None,
                         component_name=parameter,
                         location=[xpos, ypos],
                         use_instance_id_netlist=use_instance,
@@ -418,53 +410,54 @@
                         counter = 0
         if autosave:
             self._desktop.EnableAutoSave(True)
         self.modeler.schematic_units = units
         self.logger.info("Netlist was correctly imported into %s", self.design_name)
         return True
 
-    @pyaedt_function_handler()
-    def get_ibis_model_from_file(self, path, is_ami=False):
+    @pyaedt_function_handler(path="input_file")
+    def get_ibis_model_from_file(self, input_file, is_ami=False):
         """Create an IBIS model based on the data contained in an IBIS file.
 
         Parameters
         ----------
-        path : str
+        input_file : str
             Path of the IBIS file.
         is_ami : bool, optional
-            Whether if import an IBIS or an IBIS AMI.
+            Whether the file to import is an IBIS AMI file. The
+            default is ``False``, in which case it is an IBIS file.
 
         Returns
         -------
         :class:`pyaedt.generic.ibis_reader.Ibis`
             IBIS object exposing all data from the IBIS file.
         """
         if is_ami:
-            reader = ibis_reader.AMIReader(path, self)
+            reader = ibis_reader.AMIReader(input_file, self)
         else:
-            reader = ibis_reader.IbisReader(path, self)
+            reader = ibis_reader.IbisReader(input_file, self)
         reader.parse_ibis_file()
         return reader.ibis_model
 
-    @pyaedt_function_handler()
-    def create_schematic_from_mentor_netlist(self, file_to_import):
+    @pyaedt_function_handler(file_to_import="input_file")
+    def create_schematic_from_mentor_netlist(self, input_file):
         """Create a circuit schematic from a Mentor netlist.
 
         Supported currently are:
 
         * R
         * L
         * C
         * Diodes
         * Bjts
         * Discrete components with syntax ``Uxxx net1 net2get_source_pin_names ... netn modname``
 
         Parameters
         ----------
-        file_to_import : str
+        input_file : str
             Full path to the HSpice file to import.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -472,15 +465,15 @@
         units = self.modeler.schematic_units
         self.modeler.schematic_units = "meter"
         xpos = 0
         ypos = 0
         delta = 0.0508
         use_instance = True
         my_netlist = []
-        with open_file(file_to_import, "r") as f:
+        with open_file(input_file, "r") as f:
             for line in f:
                 my_netlist.append(line.split(" "))
         nets = [i for i in my_netlist if i[0] == "NET"]
         comps = [i for i in my_netlist if i[0] == "COMP:"]
         props = {}
         for el in my_netlist:
             if el[0] == "COMP:":
@@ -582,38 +575,38 @@
                     xpos += delta
                     ypos = 0
 
         self.logger.info("Netlist was correctly imported into %s", self.design_name)
         self.modeler.schematic_units = units
         return True
 
-    @pyaedt_function_handler()
-    def retrieve_mentor_comp(self, refid):
+    @pyaedt_function_handler(refid="reference_id")
+    def retrieve_mentor_comp(self, reference_id):
         """Retrieve the type of the Mentor netlist component for a given reference ID.
 
         Parameters
         ----------
-        refid : int
+        reference_id : list
             Reference ID.
 
         Returns
         -------
         str
             Type of the Mentor netlist component.
 
         """
-        if refid[1] == "R":
+        if reference_id[1] == "R":
             return "resistor:RES."
-        elif refid[1] == "C":
+        elif reference_id[1] == "C":
             return "capacitor:CAP."
-        elif refid[1] == "L":
+        elif reference_id[1] == "L":
             return "inductor:COIL."
-        elif refid[1] == "D":
+        elif reference_id[1] == "D":
             return "diode"
-        elif refid[1] == "Q":
+        elif reference_id[1] == "Q":
             return "transistor:NPN"
         else:
             return ""
 
     @pyaedt_function_handler()
     def get_source_pin_names(
         self, source_design_name, source_project_name=None, source_project_path=None, port_selector=3
@@ -666,50 +659,50 @@
             port = "Circuit Port"
         if not port:
             return False
         pins = list(tmp_oModule.GetExcitationsOfType(port))
         self.logger.info("%s Excitations Pins found.", len(pins))
         return pins
 
-    @pyaedt_function_handler()
-    def import_touchstone_solution(self, filename, solution_name="Imported_Data"):
+    @pyaedt_function_handler(filename="input_file", solution_name="solution")
+    def import_touchstone_solution(self, input_file, solution="Imported_Data"):
         """Import a Touchstone file as the solution.
 
         Parameters
         ----------
-        filename : str
+        input_file : str
             Name of the Touchstone file.
-        solution_name : str, optional
+        solution : str, optional
             Name of the solution. The default is ``"Imported_Data"``.
 
         Returns
         -------
         list
             List of ports.
 
         References
         ----------
 
         >>> oDesign.ImportData
         """
-        if filename[-2:] == "ts":
-            with open_file(filename, "r") as f:
+        if input_file[-2:] == "ts":
+            with open_file(input_file, "r") as f:
                 lines = f.readlines()
                 for i in lines:
                     if "[Number of Ports]" in i:
                         ports = int(i[i.find("]") + 1 :])
                 portnames = [i.split(" = ")[1].strip() for i in lines if "! Port" in i[:9]]
                 if not portnames:
                     portnames = ["Port{}".format(i + 1) for i in range(ports)]
         else:
             re_filename = re.compile(r"\.s(?P<ports>\d+)+p", re.I)
-            m = re_filename.search(filename)
+            m = re_filename.search(input_file)
             ports = int(m.group("ports"))
             portnames = None
-            with open_file(filename, "r") as f:
+            with open_file(input_file, "r") as f:
                 lines = f.readlines()
                 portnames = [i.split(" = ")[1].strip() for i in lines if "Port[" in i]
             if not portnames:
                 portnames = ["Port{}".format(i + 1) for i in range(ports)]
         arg = [
             "NAME:NPortData",
             "Description:=",
@@ -717,15 +710,15 @@
             "ImageFile:=",
             "",
             "SymbolPinConfiguration:=",
             0,
             ["NAME:PortInfoBlk"],
             ["NAME:PortOrderBlk"],
             "filename:=",
-            filename,
+            input_file,
             "numberofports:=",
             ports,
             "sssfilename:=",
             "",
             "sssmodel:=",
             False,
             "PortNames:=",
@@ -733,15 +726,15 @@
             "domain:=",
             "frequency",
             "datamode:=",
             "Link",
             "devicename:=",
             "",
             "SolutionName:=",
-            solution_name,
+            solution,
             "displayformat:=",
             "MagnitudePhase",
             "datatype:=",
             "SMatrix",
             [
                 "NAME:DesignerCustomization",
                 "DCOption:=",
@@ -930,110 +923,112 @@
                 20,
             ],
         )
         self.logger.info("FullWaveSpice correctly exported to %s", filename)
 
         return filename
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        plot_name="name", curvenames="curves", solution_name="solution", variation_dict="variations"
+    )
     def create_touchstone_report(
         self,
-        plot_name,
-        curvenames,
-        solution_name=None,
-        variation_dict=None,
+        name,
+        curves,
+        solution=None,
+        variations=None,
         differential_pairs=False,
         subdesign_id=None,
     ):
         """
         Create a Touchstone plot.
 
         Parameters
         ----------
-        plot_name : str
+        name : str
             Name of the plot.
-        curvenames : list
+        curves : list
             List of names for the curves to plot.
-        solution_name : str, optional
-            Name of the solution. The default value is ``None``.
-        variation_dict : dict, optional
-            Dictionary of variation names. The default value is ``None``.
+        solution : str, optional
+            Name of the solution. The default is ``None``.
+        variations : dict, optional
+            Dictionary of variation names. The default is ``None``.
         differential_pairs : bool, optional
-            Specify if the plot is on differential pairs traces. The default value is ``False``.
+            Whether the plot is on differential pairs traces. The default is ``False``.
         subdesign_id : int, optional
             Specify a subdesign ID to export a Touchstone file of this subdesign. The default value is ``None``.
         Returns
         -------
         bool
            ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.CreateReport
         """
-        if not solution_name:
-            solution_name = self.nominal_sweep
-        variations = {"Freq": ["All"]}
-        if variation_dict:
-            for el in variation_dict:
-                variations[el] = [variation_dict[el]]
+        if not solution:
+            solution = self.nominal_sweep
+        variations_dict = {"Freq": ["All"]}
+        if variations:
+            for el in variations:
+                variations_dict[el] = [variations[el]]
         dif = None
         if differential_pairs:
             dif = "Differential Pairs"
         return self.post.create_report(
-            curvenames, solution_name, variations=variations, context=dif, subdesign_id=subdesign_id
+            curves, solution, variations=variations_dict, context=dif, subdesign_id=subdesign_id, plot_name=name
         )
 
-    @pyaedt_function_handler()
-    def push_excitations(self, instance_name, thevenin_calculation=False, setup_name="LinearFrequency"):
+    @pyaedt_function_handler(instance_name="instance", setup_name="setup")
+    def push_excitations(self, instance, thevenin_calculation=False, setup="LinearFrequency"):
         """Push excitations for a linear frequency setup.
 
         Parameters
         ----------
-        instance_name : str
+        instance : str
             Name of the instance.
         thevenin_calculation : bool, optional
             Whether to perform the Thevenin equivalent calculation. The default is ``False``.
-        setup_name : str, optional
+        setup : str, optional
             Name of the solution setup to push. The default is ``"LinearFrequency"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.PushExcitations
         """
-        arg = ["NAME:options", "CalcThevenin:=", thevenin_calculation, "Sol:=", setup_name]
+        arg = ["NAME:options", "CalcThevenin:=", thevenin_calculation, "Sol:=", setup]
 
-        self.modeler.oeditor.PushExcitations(instance_name, arg)
+        self.modeler.oeditor.PushExcitations(instance, arg)
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(instance_name="instance", setup_name="setup")
     def push_time_excitations(
         self,
-        instance_name,
+        instance,
         start=0.0,
         stop=0.0,
         harmonics=100,
         window_type="Rectangular",
         width_percentage=100.0,
         kaiser=0.0,
         correct_coherent_gain=True,
-        setup_name="NexximTransient",
+        setup="NexximTransient",
     ):
         """Push excitations for a transient setup.
 
         Parameters
         ----------
-        instance_name : str
+        instance : str
             Name of the instance.
         start : float, optional
             Start time in ``seconds``. The default is ``0.0``.
         stop : float, optional
             Stop time in ``seconds``. The default is ``0.0``.
         harmonics : int, optional
             Maximum number of harmonics. The default is ``100``.
@@ -1041,16 +1036,16 @@
             Window type. Available windows are: ``Rectangular``, ``Barlett``, ``Blackman``, ``Hamming``,
             ``Hanning``, ``Kaiser``, ``Welch``, ``Weber``, ``Lanzcos``. The default is ``Rectangular``.
         width_percentage : float, optional
             Width percentage. The default is ``100.0``.
         kaiser : float, optional
             Kaiser value. The default is ``0.0``.
         correct_coherent_gain : bool, optional
-            Enable coherent gain correction. The default is ``True``.
-        setup_name : str, optional
+            Whether to enable the coherent gain correction. The default is ``True``.
+        setup : str, optional
             Name of the solution setup to push. The default is ``"LinearFrequency"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -1075,17 +1070,17 @@
                 width_percentage,
                 "kaiser:=",
                 kaiser,
                 "correctCoherentGain:=",
                 correct_coherent_gain,
             ],
             "Sol:=",
-            setup_name,
+            setup,
         ]
-        self.modeler.oeditor.PushExcitations(instance_name, arg)
+        self.modeler.oeditor.PushExcitations(instance, arg)
         return True
 
     @pyaedt_function_handler()
     def create_source(self, source_type, name=None):
         """Create a source in Circuit.
 
         Parameters
@@ -1214,111 +1209,118 @@
         """
         source_p = self.create_source(source_type="PowerSin")
         for port in ports:
             self.excitation_objects[port].enabled_sources.append(source_p.name)
             self.excitation_objects[port].update()
         return source_p
 
-    @pyaedt_function_handler()
-    def assign_voltage_frequency_dependent_excitation_to_ports(self, ports, filepath):
-        """Assign a frequency dependent excitation to circuit ports from a frequency dependent source (.fds format).
+    @pyaedt_function_handler(filepath="input_file")
+    def assign_voltage_frequency_dependent_excitation_to_ports(self, ports, input_file):
+        """Assign a frequency dependent excitation to circuit ports from a frequency dependent source (FDS format).
 
         Parameters
         ----------
         ports : list
             List of circuit ports to assign to the frequency dependent excitation.
-        filepath : str
+        input_file : str
             Path to the frequency dependent file.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.Source`
             Circuit Source Object.
 
         References
         ----------
 
         >>> oDesign.UpdateSources
         """
-        if not os.path.exists(filepath) or os.path.splitext(filepath)[1] != ".fds":
+        if not os.path.exists(input_file) or os.path.splitext(input_file)[1] != ".fds":
             self.logger.error("Introduced file is not correct. Check path and format.")
             return False
 
         if not all(elem in self.excitations for elem in ports):
             self.logger.error("Defined ports do not exist")
             return False
 
         source_freq = self.create_source(source_type="VoltageFrequencyDependent")
-        source_freq.fds_filename = filepath
+        source_freq.fds_filename = input_file
         for port in ports:
             self.excitation_objects[port].enabled_sources.append(source_freq.name)
             self.excitation_objects[port].update()
         return source_freq
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        positive_terminal="assignment",
+        negative_terminal="reference",
+        common_name="common_mode",
+        diff_name="differential_mode",
+        common_ref="common_reference",
+        diff_ref_z="differential_reference",
+    )
     def set_differential_pair(
         self,
-        positive_terminal,
-        negative_terminal,
-        common_name=None,
-        diff_name=None,
-        common_ref_z=25,
-        diff_ref_z=100,
+        assignment,
+        reference,
+        common_mode=None,
+        differential_mode=None,
+        common_reference=25,
+        differential_reference=100,
         active=True,
     ):
         """Add a differential pair definition.
 
         Parameters
         ----------
-        positive_terminal : str
+        assignment : str
             Name of the terminal to use as the positive terminal.
-        negative_terminal : str
+        reference : str
             Name of the terminal to use as the negative terminal.
-        common_name : str, optional
-            Name for the common mode. Default is ``None`` in which case a unique name is chosen.
-        diff_name : str, optional
-            Name for the differential mode. Default is ``None`` in which case a unique name is chosen.
-        common_ref_z : float, optional
-            Reference impedance for the common mode. Units are Ohm. Default is ``25``.
-        diff_ref_z : float, optional
+        common_mode : str, optional
+            Name for the common mode. The default is ``None``, in which case a unique name is assigned.
+        differential_mode : str, optional
+            Name for the differential mode. The default is ``None``, in which case a unique name is assigned.
+        common_reference : float, optional
+            Reference impedance for the common mode. The units are Ohm. The default is ``25``.
+        differential_reference : float, optional
             Reference impedance for the differential mode. Units are Ohm. Default is ``100``.
         active : bool, optional
-            Set the differential pair as active. Default is ``True``.
+            Whether to set the differential pair as active. The default is ``True``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oDesign.SetDiffPairs
         """
-        if not diff_name:
-            diff_name = generate_unique_name("Diff")
-        if not common_name:
-            common_name = generate_unique_name("Comm")
+        if not differential_mode:
+            differential_mode = generate_unique_name("Diff")
+        if not common_mode:
+            common_mode = generate_unique_name("Comm")
 
         arg1 = [
             "Pos:=",
-            positive_terminal,
+            assignment,
             "Neg:=",
-            negative_terminal,
+            reference,
             "On:=",
             active,
             "matched:=",
             False,
             "Dif:=",
-            diff_name,
+            differential_mode,
             "DfZ:=",
-            [float(diff_ref_z), 0],
+            [float(differential_reference), 0],
             "Com:=",
-            common_name,
+            common_mode,
             "CmZ:=",
-            [float(common_ref_z), 0],
+            [float(common_reference), 0],
         ]
 
         arg = ["NAME:DiffPairs"]
         arg.append("Pair:=")
         arg.append(arg1)
 
         tmpfile1 = os.path.join(self.working_directory, generate_unique_name("tmp"))
@@ -1360,125 +1362,125 @@
 
         try:
             self.odesign.SetDiffPairs(arg)
         except Exception:  # pragma: no cover
             return False
         return True
 
-    @pyaedt_function_handler()
-    def load_diff_pairs_from_file(self, filename):
+    @pyaedt_function_handler(filename="input_file")
+    def load_diff_pairs_from_file(self, input_file):
         """Load differtential pairs definition from a file.
 
-        You can use the ``save_diff_pairs_to_file`` method to obtain the file format.
+        You can use the ``save_diff_pairs_to_file()`` method to obtain the file format.
         New definitions are added only if they are compatible with the existing definitions in the project.
 
         Parameters
         ----------
-        filename : str
+        input_file : str
             Full qualified name of the file containing the differential pairs definition.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oDesign.LoadDiffPairsFromFile
         """
-        if not os.path.isfile(filename):  # pragma: no cover
-            raise ValueError("{}: The specified file could not be found.".format(filename))
+        if not os.path.isfile(input_file):  # pragma: no cover
+            raise ValueError("{}: The specified file could not be found.".format(input_file))
 
         try:
-            new_file = os.path.join(os.path.dirname(filename), generate_unique_name("temp") + ".txt")
-            with open_file(filename, "r") as file:
+            new_file = os.path.join(os.path.dirname(input_file), generate_unique_name("temp") + ".txt")
+            with open_file(input_file, "r") as file:
                 filedata = file.read().splitlines()
             with io.open(new_file, "w", newline="\n") as fh:
                 for line in filedata:
                     fh.write(line + "\n")
 
             self.odesign.LoadDiffPairsFromFile(new_file)
             os.remove(new_file)
         except Exception:  # pragma: no cover
             return False
         return True
 
-    @pyaedt_function_handler()
-    def save_diff_pairs_to_file(self, filename):
-        """Save differtential pairs definition to file.
+    @pyaedt_function_handler(filename="output_file")
+    def save_diff_pairs_to_file(self, output_file):
+        """Save differential pairs definition to a file.
 
         If the file that is specified already exists, it is overwritten.
 
         Parameters
         ----------
-        filename : str
-            Full qualified name of the file containing the differential pairs definition.
+        output_file : str
+            Full qualified name of the file to save the differential pairs definition to.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oDesign.SaveDiffPairsToFile
         """
-        self.odesign.SaveDiffPairsToFile(filename)
+        self.odesign.SaveDiffPairsToFile(output_file)
 
-        return os.path.isfile(filename)
+        return os.path.isfile(output_file)
 
-    @pyaedt_function_handler()
-    def add_netlist_datablock(self, netlist_file, datablock_name=None):
+    @pyaedt_function_handler(netlist_file="input_file", datablock_name="name")
+    def add_netlist_datablock(self, input_file, name=None):
         """Add a new netlist data block to the circuit schematic.
 
         Parameters
         ----------
-        netlist_file : str
+        input_file : str
             Path to the netlist file.
-        datablock_name : str, optional
+        name : str, optional
             Name of the data block.
 
         Returns
         -------
         bool
-            ``True`` if successfully created, ``False`` otherwise.
+            ``True`` when successful, ``False`` when failed.
         """
-        if not os.path.exists(netlist_file):
+        if not os.path.exists(input_file):
             self.logger.error("Netlist File doesn't exists")
             return False
-        if not datablock_name:
-            datablock_name = generate_unique_name("Inc")
+        if not name:
+            name = generate_unique_name("Inc")
 
         tmp_oModule = self.odesign.GetModule("DataBlock")
         tmp_oModule.AddNetlistDataBlock(
-            ["NAME:DataBlock", "name:=", datablock_name, "filename:=", netlist_file, "filelocation:=", 0]
+            ["NAME:DataBlock", "name:=", name, "filename:=", input_file, "filelocation:=", 0]
         )
         return True
 
-    @pyaedt_function_handler()
-    def browse_log_file(self, filepath=None):
-        """Save most recent log file into a new directory.
+    @pyaedt_function_handler(filepath="input_file")
+    def browse_log_file(self, input_file=None):
+        """Save the most recent log file in a new directory.
 
         Parameters
         ----------
-        filepath : str, optional
-            New log file path. The default is the pyaedt folder.
+        input_file : str, optional
+            File path to save the new log file to. The default is the ``pyaedt`` folder.
 
         Returns
         -------
         str
             File Path.
         """
-        if filepath and not os.path.exists(os.path.normpath(filepath)):
+        if input_file and not os.path.exists(os.path.normpath(input_file)):
             self.logger.error("Path does not exist.")
             return None
-        elif not filepath:
-            filepath = os.path.join(os.path.normpath(self.working_directory), "logfile")
-            if not os.path.exists(filepath):
-                os.mkdir(filepath)
+        elif not input_file:
+            input_file = os.path.join(os.path.normpath(self.working_directory), "logfile")
+            if not os.path.exists(input_file):
+                os.mkdir(input_file)
 
         results_path = os.path.join(os.path.normpath(self.results_directory), self.design_name)
         results_temp_path = os.path.join(results_path, "temp")
 
         # Check if .log exist in temp folder
         if os.path.exists(results_temp_path) and search_files(results_temp_path, "*.log"):
             # Check the most recent
@@ -1488,17 +1490,17 @@
             # Check the most recent
             files = search_files(results_path, "*.log")
             latest_file = max(files, key=os.path.getctime)
         else:
             self.logger.error("Design not solved")
             return None
 
-        shutil.copy(latest_file, filepath)
+        shutil.copy(latest_file, input_file)
         filename = os.path.basename(latest_file)
-        return os.path.join(filepath, filename)
+        return os.path.join(input_file, filename)
 
     @pyaedt_function_handler()
     def connect_circuit_models_from_multi_zone_cutout(
         self, project_connections, edb_zones_dict, ports=None, schematic_units="mm", model_inc=50
     ):
         """Connect circuit model from a multizone clipped project.
 
@@ -1537,15 +1539,15 @@
         >>> circ.connect_circuit_models_from_multi_zone_cutout(project_connexions, edb_zones, defined_ports)
         """
         if project_connections and edb_zones_dict:
             self.modeler.schematic_units = schematic_units
             inc = model_inc
             ind = 1
             for edb_file in list(edb_zones_dict.keys()):
-                hfss3d_layout_model = self.import_edb_in_circuit(edb_path=edb_file)
+                hfss3d_layout_model = self.import_edb_in_circuit(input_dir=edb_file)
                 model_position = [ind * inc, 0]
                 hfss3d_layout_model.location = model_position
                 ind += 1
             for connection in project_connections:
                 pin1 = None
                 pin2 = None
                 model1 = next(
@@ -1579,28 +1581,28 @@
                                 model_pin = None
                             if model_pin:
                                 self.modeler.components.create_interface_port(port_name, model_pin.location)
             self.save_project()
             return True
         return False
 
-    @pyaedt_function_handler()
-    def import_edb_in_circuit(self, edb_path):
+    @pyaedt_function_handler(edb_path="input_dir")
+    def import_edb_in_circuit(self, input_dir):
         """Import an EDB design inside a Circuit project.
 
         Parameters
         ----------
-        edb_path : str
+        input_dir : str
             Path of the EDB file to copy.
 
         Returns
         -------
             ``Hfss3DLayout`` component instance.
         """
-        hfss = Hfss3dLayout(edb_path)
+        hfss = Hfss3dLayout(input_dir)
         try:
             hfss.edit_cosim_options(
                 simulate_missing_solution=True,
                 setup_override_name=hfss.setup_names[0],
                 sweep_override_name=hfss.existing_analysis_sweeps[0].split(":")[1].strip(" "),
             )
         except Exception:
@@ -1611,35 +1613,35 @@
         active_project.CopyDesign(hfss.design_name)
         active_project = self.odesktop.SetActiveProject(self.project_name)
         active_project.Paste()
         hfss_3d_layout_model = self.modeler.schematic.add_subcircuit_3dlayout(hfss.design_name)
         hfss.close_project(save_project=False)
         return hfss_3d_layout_model
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(touchstone="input_file")
     def create_tdr_schematic_from_snp(
         self,
-        touchstone,
+        input_file,
         probe_pins,
         probe_ref_pins=None,
         termination_pins=None,
         differential=True,
         rise_time=30,
         use_convolution=True,
         analyze=True,
         design_name="LNA",
     ):
         """Create a schematic from a Touchstone file and automatically setup a TDR transient analysis.
 
         Parameters
         ----------
-        touchstone : str
+        input_file : str
             Full path to the sNp file.
         probe_pins : list
-            Pins to attach to the probe components.
+            List of pins to attach to the probe components.
         probe_ref_pins : list, optional
             Reference pins to attach to probe components. The default is ``None``.
             This parameter is valid only in differential TDR probes.
         termination_pins : list, optional
             Pins to terminate. The default is ``None``.
         differential : bool, optional
             Whether the buffers are differential. The default is ``True``. If ``False``, the
@@ -1658,18 +1660,18 @@
         -------
 
         """
         if design_name in self.design_list:
             self.logger.warning("Design already exists. renaming.")
             design_name = generate_unique_name(design_name)
         self.insert_design(design_name)
-        if isinstance(touchstone, type(Hfss3dLayout)):
-            touchstone_path = touchstone.export_touchstone()
+        if isinstance(input_file, type(Hfss3dLayout)):
+            touchstone_path = input_file.export_touchstone()
         else:
-            touchstone_path = touchstone
+            touchstone_path = input_file
 
         sub = self.modeler.components.create_touchstone_component(touchstone_path)
         center_x = sub.location[0]
         center_y = sub.location[1]
         left = 0
         delta_y = -1 * sub.location[1] - 2000 - 50 * len(probe_pins)
         if differential:
@@ -1747,33 +1749,33 @@
             setup.props["OptionName"] = "Nexxim Options"
         if analyze:
             self.analyze()
             for trace in tdr_probe_names:
                 self.post.create_report(trace)
         return True, tdr_probe_names
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(touchstone="input_file")
     def create_lna_schematic_from_snp(
         self,
-        touchstone,
+        input_file,
         start_frequency=0,
         stop_frequency=30,
         auto_assign_diff_pairs=False,
         separation=".",
         pattern=None,
         analyze=True,
         design_name="LNA",
     ):
         """Create a schematic from a Touchstone file and automatically set up an LNA analysis.
 
         This method optionally assigns differential pairs automatically based on name pattern.
 
         Parameters
         ----------
-        touchstone : str
+        input_file : str
             Full path to the sNp file.
         start_frequency : int, float, optional
             Start frequency in GHz of the LNA setup. The default is ``0``.
         stop_frequency  : int, float, optional
             Stop frequency in GHz of the LNA setup. The default is ``30``.
         auto_assign_diff_pairs : bool
             Whether to automatically assign differential pairs. The default is ``False``.
@@ -1794,18 +1796,18 @@
         """
         if pattern is None:
             pattern = ["component", "pin", "net"]
         if design_name in self.design_list:
             self.logger.warning("Design already exists. renaming.")
             design_name = generate_unique_name(design_name)
         self.insert_design(design_name)
-        if isinstance(touchstone, type(Hfss3dLayout)):
-            touchstone_path = touchstone.export_touchstone()
+        if isinstance(input_file, type(Hfss3dLayout)):
+            touchstone_path = input_file.export_touchstone()
         else:
-            touchstone_path = touchstone
+            touchstone_path = input_file
 
         sub = self.modeler.components.create_touchstone_component(touchstone_path)
 
         ports = []
         center = sub.location[0]
         left = 0
         right = 0
@@ -1819,15 +1821,15 @@
             else:
                 delta = unit_converter(
                     start + right * 200, input_units="mil", output_units=self.modeler.schematic_units
                 )
                 new_loc = [loc[0] + delta, loc[1]]
                 right += 1
             port = self.modeler.components.create_interface_port(name=pin.name, location=new_loc)
-            port.pins[0].connect_to_component(component_pin=pin, use_wire=True)
+            port.pins[0].connect_to_component(assignment=pin, use_wire=True)
             ports.append(port)
         diff_pairs = []
         comm_pairs = []
         if auto_assign_diff_pairs:
             for pin in ports:
                 pin_name = pin.name.split(separation)
                 if pin_name[-1][-1] == "P":
@@ -1837,35 +1839,35 @@
                         neg_pin_name = neg_pin.name.split(separation)
                         component_neg = neg_pin_name[pattern.index("component")]
 
                         net_neg = neg_pin_name[pattern.index("net")]
 
                         if component_neg == component and net_neg != net and net_neg[:-1] == net[:-1]:
                             self.set_differential_pair(
-                                positive_terminal=pin.name,
-                                negative_terminal=neg_pin.name,
-                                common_name="COMMON_{}_{}".format(component, net),
-                                diff_name="{}_{}".format(component, net),
-                                common_ref_z=25,
-                                diff_ref_z=100,
+                                assignment=pin.name,
+                                reference=neg_pin.name,
+                                common_mode="COMMON_{}_{}".format(component, net),
+                                differential_mode="{}_{}".format(component, net),
+                                common_reference=25,
+                                differential_reference=100,
                                 active=True,
                             )
                             diff_pairs.append("{}_{}".format(component, net))
                             comm_pairs.append("COMMON_{}_{}".format(component, net))
                             break
         setup1 = self.create_setup()
         setup1.props["SweepDefinition"]["Data"] = "LINC {}GHz {}GHz 1001".format(start_frequency, stop_frequency)
         if analyze:
             self.analyze()
         return True, diff_pairs, comm_pairs
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(touchstone="input_file")
     def create_ami_schematic_from_snp(
         self,
-        touchstone,
+        input_file,
         ibis_ami,
         component_name,
         tx_buffer_name,
         rx_buffer_name,
         tx_pins,
         tx_refs,
         rx_pins,
@@ -1878,15 +1880,15 @@
         analyze=False,
         design_name="AMI",
     ):
         """Create a schematic from a Touchstone file and automatically set up an IBIS-AMI analysis.
 
         Parameters
         ----------
-        touchstone : str
+        input_file : str
             Full path to the sNp file.
         ibis_ami : str
             Full path to the IBIS file.
         component_name : str
             Component name in the IBIS file to assign to components.
         tx_buffer_name : str
             Transmission buffer name.
@@ -1923,21 +1925,21 @@
         Returns
         -------
         (bool, list, list)
             First argument is ``True`` if successful.
             Second and third arguments are respectively the names of the tx and rx mode probes.
         """
         if design_name in self.design_list:
-            self.logger.warning("Design already exists. renaming.")
+            self.logger.warning("Design already exists. Renaming.")
             design_name = generate_unique_name(design_name)
         self.insert_design(design_name)
-        if isinstance(touchstone, type(Hfss3dLayout)):
-            touchstone_path = touchstone.export_touchstone()
+        if isinstance(input_file, type(Hfss3dLayout)):
+            touchstone_path = input_file.export_touchstone()
         else:
-            touchstone_path = touchstone
+            touchstone_path = input_file
 
         sub = self.modeler.components.create_touchstone_component(touchstone_path)
         center_x = sub.location[0]
         center_y = sub.location[1]
         left = 0
         delta_y = -1 * sub.location[1] - 2000 - 50 * len(tx_pins)
         ibis = self.get_ibis_model_from_file(ibis_ami, is_ami=True)
```

### Comparing `pyaedt-0.8.8/pyaedt/common_rpc.py` & `pyaedt-0.8.9/pyaedt/common_rpc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/desktop.py` & `pyaedt-0.8.9/pyaedt/desktop.py`

 * *Files 0% similar despite different names*

```diff
@@ -941,18 +941,18 @@
                         if port and desktop.GetGrpcServerPort() == port:
                             self.isoutsideDesktop = True
                             self.odesktop = desktop
                             self.aedt_process_id = self.odesktop.GetProcessID()
                             self.is_grpc_api = True
                             last_session.parent_desktop_id.append(self.aedt_process_id)
                             return True
-                    except:
+                    except Exception:
                         messages = desktop.GetMessages("", "", 0)
                         for message in messages:
-                            if " GRPC server running on port: " in message and str(port) in message:
+                            if "gRPC server running on port: " in message and str(port) in message:
                                 self.isoutsideDesktop = True
                                 self.odesktop = desktop
                                 self.aedt_process_id = self.odesktop.GetProcessID()
                                 self.is_grpc_api = True
                                 last_session.parent_desktop_id.append(self.aedt_process_id)
                                 return True
             if new_session:
@@ -1487,14 +1487,17 @@
                     self.odesktop.CloseProject(project)
                 except Exception:  # pragma: no cover
                     self.logger.warning("Failed to close Project {}".format(project))
         result = _close_aedt_application(self, close_on_exit, self.aedt_process_id, self.is_grpc_api)
         if not result:
             self.logger.error("Error releasing desktop.")
             return False
+        self.logger._desktop_class = None
+        self.logger._oproject = None
+        self.logger._odesign = None
         if close_on_exit:
             self.logger.info("Desktop has been released and closed.")
         else:
             self.logger.info("Desktop has been released.")
         del _desktop_sessions[self.aedt_process_id]
         props = [a for a in dir(self) if not a.startswith("__")]
         for a in props:
```

### Comparing `pyaedt-0.8.8/pyaedt/downloads.py` & `pyaedt-0.8.9/pyaedt/downloads.py`

 * *Files 0% similar despite different names*

```diff
@@ -730,29 +730,30 @@
         local_path = os.path.join(destination, os.path.join("twin_builder", file_name))
         if os.path.exists(local_path):
             os.unlink(local_path)
     _download_file("pyaedt/twin_builder", file_name, destination)
     return os.path.join(destination, "twin_builder")
 
 
-@pyaedt_function_handler(filename="name")
-def download_file(directory, name=None, destination=None):
+@pyaedt_function_handler(filename="name", directory="source")
+def download_file(source, name=None, destination=None):
     """
     Download a file or files from the online examples repository.
 
     Files are downloaded from the
     :ref:`example-data<https://github.com/ansys/example-data/tree/master/pyaedt>`_ repository
     to a local destination. If ``name`` is not specified, the full directory path
     will be copied to the local drive.
 
     Parameters
     ----------
-    directory : str
-        Directory name in the Ansys ``example-data`` repository. If the ``pyaed/`` prefix
-        is not part of ``directory`` it will be prepended.
+    source : str
+        Directory name in the Ansys ``example-data`` repository from which the example
+        data is to be retrieved. If the ``pyaedt/`` prefix
+        is not part of ``directory`` the path will be automatically prepended.
     name : str, optional
         File name to download. By default all files in ``directory``
         will be downloaded.
     destination : str, optional
         Path where the files will be saved locally. Default is the user temp folder.
 
     Returns
@@ -766,20 +767,20 @@
 
     >>> import pyaedt
     >>> path = pyaedt.downloads.download_file("motorcad", "IPM_Vweb_Hairpin.mot")
     >>> path
     'C:/Users/user/AppData/local/temp/PyAEDTExamples/motorcad'
     """
     local_paths = []
-    _download_file(directory, name, destination, local_paths)
+    _download_file(source, name, destination, local_paths)
     if name:
         return list(set(local_paths))[0]
     else:
         if not destination:
             destination = EXAMPLES_PATH
-        destination_dir = os.path.join(destination, directory)
+        destination_dir = os.path.join(destination, source)
         return destination_dir
 
 
 def unzip(source_filename, dest_dir):
     with zipfile.ZipFile(source_filename) as zf:
         zf.extractall(dest_dir)
```

### Comparing `pyaedt-0.8.8/pyaedt/emit.py` & `pyaedt-0.8.9/pyaedt/emit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/emit_core/Couplings.py` & `pyaedt-0.8.9/pyaedt/emit_core/Couplings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/emit_core/__init__.py` & `pyaedt-0.8.9/pyaedt/emit_core/__init__.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/emit_core/emit_constants.py` & `pyaedt-0.8.9/pyaedt/emit_core/emit_constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/emit_core/results/results.py` & `pyaedt-0.8.9/pyaedt/emit_core/results/results.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/emit_core/results/revision.py` & `pyaedt-0.8.9/pyaedt/emit_core/results/revision.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/Ansys.png` & `pyaedt-0.8.9/pyaedt/generic/Ansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/AnsysTemplate.json` & `pyaedt-0.8.9/pyaedt/generic/AnsysTemplate.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/DataHandlers.py` & `pyaedt-0.8.9/pyaedt/generic/DataHandlers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/LoadAEDTFile.py` & `pyaedt-0.8.9/pyaedt/generic/LoadAEDTFile.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/ami.json` & `pyaedt-0.8.9/pyaedt/generic/ami.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/clr_module.py` & `pyaedt-0.8.9/pyaedt/generic/clr_module.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/compliance.py` & `pyaedt-0.8.9/pyaedt/generic/compliance.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/configurations.py` & `pyaedt-0.8.9/pyaedt/generic/configurations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1995,15 +1995,15 @@
             old_objs = list(self._app.modeler.user_defined_components.keys())
             if operation_dict["Props"]["Command"] == "Move":
                 obj.move(
                     [decompose_variable_value(operation_dict["Props"]["Move Vector"][2 * i + 1])[0] for i in range(3)]
                 )
             elif operation_dict["Props"]["Command"] == "Rotate":
                 rotation = decompose_variable_value(operation_dict["Props"]["Angle"])
-                obj.rotate(operation_dict["Props"]["Axis"], angle=rotation[0], unit=rotation[1])
+                obj.rotate(operation_dict["Props"]["Axis"], angle=rotation[0], units=rotation[1])
             elif operation_dict["Props"]["Command"] == "Mirror":
                 obj.mirror(
                     [
                         decompose_variable_value(operation_dict["Props"]["Base Position"][2 * i + 1])[0]
                         for i in range(3)
                     ],
                     [
@@ -2016,19 +2016,19 @@
                     [decompose_variable_value(operation_dict["Props"]["Vector"][2 * i + 1])[0] for i in range(3)],
                     nclones=operation_dict["Props"]["Total Number"],
                     attach_object=operation_dict["Props"]["Attach To Original Object"],
                 )
             elif operation_dict["Props"]["Command"] == "DuplicateAroundAxis":
                 rotation = decompose_variable_value(operation_dict["Props"]["Angle"])
                 new_objs = obj.duplicate_around_axis(
-                    operation_dict["Props"]["Axis"], angle=rotation[0], nclones=operation_dict["Props"]["Total Number"]
+                    operation_dict["Props"]["Axis"], angle=rotation[0], clones=operation_dict["Props"]["Total Number"]
                 )
             elif operation_dict["Props"]["Command"] == "DuplicateMirror":
                 new_objs = obj.duplicate_and_mirror(
-                    position=[
+                    origin=[
                         decompose_variable_value(operation_dict["Props"]["Base Position"][2 * i + 1])[0]
                         for i in range(3)
                     ],
                     vector=[
                         decompose_variable_value(operation_dict["Props"]["Normal Position"][2 * i + 1])[0]
                         for i in range(3)
                     ],
```

### Comparing `pyaedt-0.8.8/pyaedt/generic/constants.py` & `pyaedt-0.8.9/pyaedt/generic/constants.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/design_types.py` & `pyaedt-0.8.9/pyaedt/generic/design_types.py`

 * *Files 0% similar despite different names*

```diff
@@ -526,14 +526,15 @@
     non_graphical=False,
     new_desktop_session=False,
     close_on_exit=False,
     student_version=False,
     machine="",
     port=0,
     aedt_process_id=None,
+    ic_mode=False,
 ):
     """Hfss3dLayout Class.
 
     Parameters
     ----------
     projectname : str, optional
         Name of the project to select or the full path to the project
@@ -575,14 +576,16 @@
     port : int, optional
         Port number on which to start the oDesktop communication on an already existing server.
         This parameter is ignored when creating a new server. It works only in 2022 R2 or later.
         The remote server must be up and running with the command `"ansysedt.exe -grpcsrv portnum"`.
     aedt_process_id : int, optional
         Process ID for the instance of AEDT to point PyAEDT at. The default is
         ``None``. This parameter is only used when ``new_desktop_session = False``.
+    ic_mode : bool, optional
+        Whether to set the design to IC mode or not. The default is ``False``.
 
     Returns
     -------
     :class:`pyaedt.hfss3dlayout.Hfss3dLayout`
 
     Examples
     --------
@@ -633,14 +636,15 @@
         non_graphical=non_graphical,
         new_desktop_session=new_desktop_session,
         close_on_exit=close_on_exit,
         student_version=student_version,
         machine=machine,
         port=port,
         aedt_process_id=aedt_process_id,
+        ic_mode=ic_mode,
     )
 
 
 def Maxwell2d(
     projectname=None,
     designname=None,
     solution_type=None,
```

### Comparing `pyaedt-0.8.8/pyaedt/generic/filesystem.py` & `pyaedt-0.8.9/pyaedt/generic/filesystem.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/general_methods.py` & `pyaedt-0.8.9/pyaedt/generic/general_methods.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/grpc_plugin.py` & `pyaedt-0.8.9/pyaedt/generic/grpc_plugin.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/grpc_plugin_dll.py` & `pyaedt-0.8.9/pyaedt/generic/grpc_plugin_dll.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/ibis_reader.py` & `pyaedt-0.8.9/pyaedt/generic/ibis_reader.py`

 * *Files 0% similar despite different names*

```diff
@@ -271,18 +271,15 @@
         -------
         :class:`pyaedt.modeler.Object3d.CircuitComponent`
             Circuit Component Object.
 
         """
 
         return self._circuit.modeler.schematic.create_component(
-            component_library=None,
-            component_name=self.buffer_name,
-            location=[x, y],
-            angle=angle,
+            component_library=None, component_name=self.buffer_name, location=[x, y], angle=angle
         )
 
 
 class DifferentialPin:
     """Provides the differential pin from a component with all its data feature.
 
     Parameters
@@ -411,15 +408,15 @@
                     True,
                     "Data:=",
                     [],
                     "GRef:=",
                     [],
                 ],
             )
-        except:
+        except Exception:
             logger.error("Error adding {} pin component.".format(self.short_name))
             return False
 
     def insert(self, x, y, angle=0.0):
         """Insert a pin at a defined location inside the graphical window.
 
         Parameters
@@ -435,18 +432,15 @@
         -------
         :class:`pyaedt.modeler.Object3d.CircuitComponent`
             Circuit Component Object.
 
         """
 
         return self._circuit.modeler.schematic.create_component(
-            component_library=None,
-            component_name=self.buffer_name,
-            location=[x, y],
-            angle=angle,
+            component_library=None, component_name=self.buffer_name, location=[x, y], angle=angle
         )
 
 
 class Buffer:
     def __init__(self, ibis_name, short_name, circuit):
         self._ibis_name = ibis_name
         self._short_name = short_name
@@ -499,18 +493,15 @@
         -------
         :class:`pyaedt.modeler.Object3d.CircuitComponent`
             Circuit Component Object.
 
         """
 
         return self._circuit.modeler.schematic.create_component(
-            component_library=None,
-            component_name=self.name,
-            location=[x, y],
-            angle=angle,
+            component_library=None, component_name=self.name, location=[x, y], angle=angle
         )
 
 
 class ModelSelector:
     def __init__(self):
         self._model_selector_items = []
         self._name = None
```

### Comparing `pyaedt-0.8.8/pyaedt/generic/ibis_v7.json` & `pyaedt-0.8.9/pyaedt/generic/ibis_v7.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/near_field_import.py` & `pyaedt-0.8.9/pyaedt/generic/near_field_import.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/pdf.py` & `pyaedt-0.8.9/pyaedt/generic/pdf.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/plot.py` & `pyaedt-0.8.9/pyaedt/generic/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/python_optimizers.py` & `pyaedt-0.8.9/pyaedt/generic/python_optimizers.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/report_file_parser.py` & `pyaedt-0.8.9/pyaedt/generic/report_file_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/settings.py` & `pyaedt-0.8.9/pyaedt/generic/settings.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/spisim.py` & `pyaedt-0.8.9/pyaedt/generic/spisim.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/generic/touchstone_parser.py` & `pyaedt-0.8.9/pyaedt/generic/touchstone_parser.py`

 * *Files 1% similar despite different names*

```diff
@@ -251,27 +251,27 @@
 
     @pyaedt_function_handler()
     def get_return_loss_index(self, excitation_name_prefix=""):
         """Get the list of all the Returnloss from a list of exctitations.
 
         If no excitation is provided it will provide a full list of return losses.
 
-        Example: excitation_names ["1","2"] is_touchstone_expression=False output ["S(1,1)",, S(2,2)]
-        Example: excitation_names ["S(1,1)","S(1,2)", S(2,2)] is_touchstone_expression=True output ["S(1,1)",, S(2,2)]
+        Example: excitation_names ["1","2"] is_touchstone_expression=False output ["S(1,1)", S(2,2)]
+        Example: excitation_names ["S(1,1)","S(1,2)", S(2,2)] is_touchstone_expression=True output ["S(1,1)", S(2,2)]
 
         Parameters
         ----------
 
         excitation_name_prefix :
              (Default value = '')
 
         Returns
         -------
         list
-            list of index couples representing Return Losses of excitations
+            List of index couples representing return losses of excitations.
 
         """
         values = []
         if excitation_name_prefix:
             excitation_names = [i for i in self.port_names if excitation_name_prefix.lower() in i.lower()]
         else:
             excitation_names = [i for i in self.port_names]
@@ -541,15 +541,15 @@
             if "Maximum causality" in line and causality:
                 msg_log = line[17:]
                 is_causal = True
                 try:
                     causality_check = float(msg_log.split("Maximum causality error: ")[-1].split("for entry")[0])
                     if not causality_check == 0.0:
                         is_causal = False
-                except:
+                except Exception:
                     is_causal = False
-                    raise Exception("Failed evaluating causality value")
+                    raise Exception("Failed evaluating causality value.")
                 out[snpf].append(["causality", is_causal, msg_log])
             if "Causality check is inconclusive" in line and causality:
                 is_causal = False
                 out[snpf].append(["causality", is_causal, line[17:]])
     return out
```

### Comparing `pyaedt-0.8.8/pyaedt/hfss.py` & `pyaedt-0.8.9/pyaedt/hfss.py`

 * *Files 1% similar despite different names*

```diff
@@ -692,20 +692,16 @@
 
         Create two cylinders in the XY working plane and assign a copper coating of 0.2 mm to the inner cylinder and
         outer face.
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> origin = hfss.modeler.Position(0, 0, 0)
-        >>> inner = hfss.modeler.create_cylinder(
-        ...     hfss.PLANE.XY, origin, 3, 200, 0, "inner"
-        ... )
-        >>> outer = hfss.modeler.create_cylinder(
-        ...     hfss.PLANE.XY, origin, 4, 200, 0, "outer"
-        ... )
+        >>> inner = hfss.modeler.create_cylinder(hfss.PLANE.XY,origin,3,200,0,"inner")
+        >>> outer = hfss.modeler.create_cylinder(hfss.PLANE.XY,origin,4,200,0,"outer")
         >>> coat = hfss.assign_coating(["inner", outer.faces[2].id], "copper", use_thickness=True, thickness="0.2mm")
 
         """
 
         userlst = self.modeler.convert_to_selections(assignment, True)
         lstobj = []
         lstface = []
@@ -885,15 +881,18 @@
         Examples
         --------
 
         Create a setup named ``"LinearCountSetup"`` and use it in a linear count sweep
         named ``"LinearCountSweep"``.
 
         >>> setup = hfss.create_setup("LinearCountSetup")
-        >>> linear_count_sweep = hfss.create_linear_count_sweep(,,,
+        >>> linear_count_sweep = hfss.create_linear_count_sweep(setup="LinearCountSetup",
+        ...                                                     sweep="LinearCountSweep",
+        ...                                                     units="MHz", start_frequency=1.1e3,
+        ...                                                     stop_frequency=1200.1, num_of_freq_points=1658)
         >>> type(linear_count_sweep)
         <class 'pyaedt.modules.SetupTemplates.SweepHFSS'>
 
         """
         if sweep_type in ["Interpolating", "Fast"]:
             if num_of_freq_points == None:
                 num_of_freq_points = 401
@@ -1672,16 +1671,16 @@
             Boundary object.
 
         Examples
         --------
         >>> aedtapp = Hfss()
         >>> aedtapp.insert_design("Design_Terminal_2")
         >>> aedtapp.solution_type = "Terminal"
-        >>> box1 = aedtapp.modeler.create_box([-100, -100, 0], [200, 200, 5], name="gnd2z", matname="copper")
-        >>> box2 = aedtapp.modeler.create_box([-100, -100, 20], [200, 200, 25], name="sig2z", matname="copper")
+        >>> box1 = aedtapp.modeler.create_box([-100, -100, 0],[200, 200, 5],name="gnd2z",material="copper")
+        >>> box2 = aedtapp.modeler.create_box([-100, -100, 20],[200, 200, 25],name="sig2z",material="copper")
         >>> aedtapp.modeler.fit_all()
         >>> portz = aedtapp.create_spiral_lumped_port(box1,box2)
         """
         if not "Terminal" in self.solution_type:
             raise Exception("This method can be used only in Terminal solutions.")
         assignment = self.modeler.convert_to_selections(assignment)
         reference = self.modeler.convert_to_selections(reference)
@@ -1790,36 +1789,36 @@
         elif plane == "Y":
             orient = "X" if (dx < dz) else "Z"
         else:
             orient = "X" if (dx < dy) else "Y"
 
         poly1 = self.modeler.create_polyline(
             p1_down,
+            name=assignment + "_sheet",
             xsection_type="Line",
             xsection_orient=orient,
             xsection_width=closest_distance / 2,
-            name=assignment + "_sheet",
         )
 
         # create second polyline to join spiral with conductor face
         dx = abs(p2_up[0][0] - p2_up[1][0])
         dy = abs(p2_up[0][1] - p2_up[1][1])
         dz = abs(p2_up[0][2] - p2_up[1][2])
         if plane == "X":
             orient = "Y" if (dy < dz) else "Z"
         elif plane == "Y":
             orient = "X" if (dx < dz) else "Z"
         else:
             orient = "X" if (dx < dy) else "Y"
         poly2 = self.modeler.create_polyline(
             p2_up,
+            name=reference + "_sheet",
             xsection_type="Line",
             xsection_orient=orient,
             xsection_width=closest_distance / 2,
-            name=reference + "_sheet",
         )
 
         # assign pec to created polylines
         self.assign_perfecte_to_sheets(poly1, name=assignment)
         self.assign_perfecte_to_sheets(poly2, name=reference)
 
         # create lumped port on spiral
@@ -1862,18 +1861,16 @@
         >>> oModule.AssignVoltage
 
         Examples
         --------
 
         Create two boxes for creating a voltage source named ``'VoltageSource'``.
 
-        >>> box1 = hfss.modeler.create_box([30, 0, 0], [40, 10, 5],
-        ...                                "BoxVolt1", "copper")
-        >>> box2 = hfss.modeler.create_box([30, 0, 10], [40, 10, 5],
-        ...                                "BoxVolt2", "copper")
+        >>> box1 = hfss.modeler.create_box([30, 0, 0],[40, 10, 5],"BoxVolt1","copper")
+        >>> box2 = hfss.modeler.create_box([30, 0, 10],[40, 10, 5],"BoxVolt2","copper")
         >>> v1 = hfss.create_voltage_source_from_objects("BoxVolt1","BoxVolt2",hfss.AxisDir.XNeg,"VoltageSource")
         PyAEDT INFO: Connection Correctly created
         """
 
         if not self.modeler.does_object_exists(assignment) or not self.modeler.does_object_exists(reference):
             self.logger.error("One or both objects doesn't exists. Check and retry")
             return False
@@ -1920,18 +1917,16 @@
         >>> oModule.AssignCurrent
 
         Examples
         --------
 
         Create two boxes for creating a current source named ``'CurrentSource'``.
 
-        >>> box1 = hfss.modeler.create_box([30, 0, 20], [40, 10, 5],
-        ...                                "BoxCurrent1", "copper")
-        >>> box2 = hfss.modeler.create_box([30, 0, 30], [40, 10, 5],
-        ...                                "BoxCurrent2", "copper")
+        >>> box1 = hfss.modeler.create_box([30, 0, 20],[40, 10, 5],"BoxCurrent1","copper")
+        >>> box2 = hfss.modeler.create_box([30, 0, 30],[40, 10, 5],"BoxCurrent2","copper")
         >>> i1 = hfss.create_current_source_from_objects("BoxCurrent1","BoxCurrent2",hfss.AxisDir.XPos,"CurrentSource")
         PyAEDT INFO: Connection created 'CurrentSource' correctly.
         """
 
         if not self.modeler.does_object_exists(assignment) or not self.modeler.does_object_exists(reference):
             self.logger.error("One or both objects do not exist. Check and retry.")
             return False
@@ -2407,18 +2402,16 @@
         >>> oModule.AssignPerfectE
 
         Examples
         --------
 
         Create two boxes for creating a Perfect E named ``'PerfectE'``.
 
-        >>> box1 = hfss.modeler.create_box([0,0,0], [10,10,5],
-        ...                                "perfect1", "Copper")
-        >>> box2 = hfss.modeler.create_box([0, 0, 10], [10, 10, 5],
-        ...                                "perfect2", "copper")
+        >>> box1 = hfss.modeler.create_box([0,0,0],[10,10,5],"perfect1","Copper")
+        >>> box2 = hfss.modeler.create_box([0, 0, 10],[10, 10, 5],"perfect2","copper")
         >>> perfect_e = hfss.create_perfecte_from_objects("perfect1","perfect2",hfss.AxisDir.ZNeg,"PerfectE")
         PyAEDT INFO: Connection Correctly created
         >>> type(perfect_e)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
@@ -2477,18 +2470,16 @@
         >>> oModule.AssignPerfectH
 
         Examples
         --------
 
         Create two boxes for creating a Perfect H named ``'PerfectH'``.
 
-        >>> box1 = hfss.modeler.create_box([0,0,20], [10,10,5],
-        ...                                "perfect1", "Copper")
-        >>> box2 = hfss.modeler.create_box([0, 0, 30], [10, 10, 5],
-        ...                                "perfect2", "copper")
+        >>> box1 = hfss.modeler.create_box([0,0,20],[10,10,5],"perfect1","Copper")
+        >>> box2 = hfss.modeler.create_box([0, 0, 30],[10, 10, 5],"perfect2","copper")
         >>> perfect_h = hfss.create_perfecth_from_objects("perfect1","perfect2",hfss.AxisDir.ZNeg,"Perfect H")
         PyAEDT INFO: Connection Correctly created
         >>> type(perfect_h)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
@@ -2654,18 +2645,16 @@
         >>> oModule.AssignLumpedRLC
 
         Examples
         --------
 
         Create two boxes for creating a lumped RLC named ``'LumpedRLC'``.
 
-        >>> box1 = hfss.modeler.create_box([0, 0, 50], [10, 10, 5],
-        ...                                           "rlc1", "copper")
-        >>> box2 = hfss.modeler.create_box([0, 0, 60], [10, 10, 5],
-        ...                                           "rlc2", "copper")
+        >>> box1 = hfss.modeler.create_box([0, 0, 50],[10, 10, 5],"rlc1","copper")
+        >>> box2 = hfss.modeler.create_box([0, 0, 60],[10, 10, 5],"rlc2","copper")
         >>> rlc = hfss.create_lumped_rlc_between_objects("rlc1","rlc2",hfss.AxisDir.XPos,"Lumped RLC",resistance=50,
         ...                                              inductance=1e-9, capacitance=1e-6)
         PyAEDT INFO: Connection Correctly created
 
         """
 
         if not self.modeler.does_object_exists(assignment) or not self.modeler.does_object_exists(reference):
@@ -2757,18 +2746,16 @@
         >>> oModule.AssignImpedance
 
         Examples
         --------
 
         Create two boxes for creating an impedance named ``'ImpedanceExample'``.
 
-        >>> box1 = hfss.modeler.create_box([0, 0, 70], [10, 10, 5],
-        ...                                           "box1", "copper")
-        >>> box2 = hfss.modeler.create_box([0, 0, 80], [10, 10, 5],
-        ...                                           "box2", "copper")
+        >>> box1 = hfss.modeler.create_box([0, 0, 70],[10, 10, 5],"box1","copper")
+        >>> box2 = hfss.modeler.create_box([0, 0, 80],[10, 10, 5],"box2","copper")
         >>> impedance = hfss.create_impedance_between_objects("box1", "box2", hfss.AxisDir.XPos,
         ...                                                   "ImpedanceExample", 100, 50)
         PyAEDT INFO: Connection Correctly created
 
         """
 
         if not self.modeler.does_object_exists(start_assignment) or not self.modeler.does_object_exists(end_assignment):
@@ -2928,17 +2915,16 @@
         >>> oModule.AssignVoltage
 
         Examples
         --------
 
         Create a sheet and assign to it some voltage.
 
-        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
-        ...                                                  [0, 0, -70], [10, 2], name="VoltageSheet",
-        ...                                                  matname="copper")
+        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,[0, 0, -70],[10, 2],
+        ...                                       name="VoltageSheet",material="copper")
         >>> v1 = hfss.assign_voltage_source_to_sheet(sheet.name,hfss.AxisDir.XNeg,"VoltageSheetExample")
         >>> v2 = hfss.assign_voltage_source_to_sheet(sheet.name,[sheet.bottom_edge_x.midpoint,
         ...                                     sheet.bottom_edge_y.midpoint],50)
 
         """
 
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
@@ -2981,16 +2967,16 @@
         >>> oModule.AssignCurrent
 
         Examples
         --------
 
         Create a sheet and assign some current to it.
 
-        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY, [0, 0, -50],
-        ...                                                  [5, 1], name="CurrentSheet", matname="copper")
+        >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,[0, 0, -50],[5, 1],
+        ...                                       name="CurrentSheet",material="copper")
         >>> hfss.assign_current_source_to_sheet(sheet.name,hfss.AxisDir.XNeg,"CurrentSheetExample")
         'CurrentSheetExample'
         >>> c1 = hfss.assign_current_source_to_sheet(sheet.name,[sheet.bottom_edge_x.midpoint,
         ...                                     sheet.bottom_edge_y.midpoint])
 
         """
 
@@ -3032,15 +3018,15 @@
 
         Examples
         --------
 
         Create a sheet and use it to create a Perfect E.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY, [0, 0, -90],
-        ...                                       [10, 2], name="PerfectESheet", matname="Copper")
+        ...                                       [10, 2], name="PerfectESheet", material="Copper")
         >>> perfect_e_from_sheet = hfss.assign_perfecte_to_sheets(sheet.name,"PerfectEFromSheet")
         >>> type(perfect_e_from_sheet)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
         assignment = self.modeler.convert_to_selections(assignment, True)
         if self.solution_type in ["Modal", "Terminal", "Transient Network", "SBR+", "Eigenmode"]:
@@ -3074,15 +3060,15 @@
 
         Examples
         --------
 
         Create a sheet and use it to create a Perfect H.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY, [0, 0, -90],
-        ...                                       [10, 2], name="PerfectHSheet", matname="Copper")
+        ...                                       [10, 2], name="PerfectHSheet", material="Copper")
         >>> perfect_h_from_sheet = hfss.assign_perfecth_to_sheets(sheet.name,"PerfectHFromSheet")
         >>> type(perfect_h_from_sheet)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         if self.solution_type in ["Modal", "Terminal", "Transient Network", "SBR+", "Eigenmode"]:
@@ -3150,15 +3136,15 @@
         Examples
         --------
 
         Create a sheet and use it to create a lumped RLC.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
         ...                                       [0, 0, -90], [10, 2], name="RLCSheet",
-        ...                                        matname="Copper")
+        ...                                        material="Copper")
         >>> lumped_rlc_to_sheet = hfss.assign_lumped_rlc_to_sheet(sheet.name,hfss.AxisDir.XPos,resistance=50,
         ...                                                       inductance=1e-9,capacitance=1e-6)
         >>> type(lumped_rlc_to_sheet)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
         >>> h2 = hfss.assign_lumped_rlc_to_sheet(sheet.name,[sheet.bottom_edge_x.midpoint,
         ...                                      sheet.bottom_edge_y.midpoint],resistance=50,inductance=1e-9,
         ...                                      capacitance=1e-6)
@@ -3231,15 +3217,15 @@
         Examples
         --------
 
         Create a sheet and use it to create an impedance.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
         ...                                       [0, 0, -90], [10, 2], name="ImpedanceSheet",
-        ...                                        matname="Copper")
+        ...                                        material="Copper")
         >>> impedance_to_sheet = hfss.assign_impedance_to_sheet(sheet.name,"ImpedanceFromSheet",100,50)
         >>> type(impedance_to_sheet)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         if self.solution_type in ["Modal", "Terminal", "Transient Network"]:
@@ -3315,22 +3301,22 @@
         Examples
         --------
 
         Create a sheet and use it to create an impedance.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
         ...                                       [0, 0, -90], [10, 2], name="ImpedanceSheet",
-        ...                                        matname="Copper")
+        ...                                        material="Copper")
         >>> impedance_to_sheet = hfss.assign_impedance_to_sheet(sheet.name,"ImpedanceFromSheet",100,50)
 
         Create a sheet and use it to create an anisotropic impedance.
 
         >>> sheet = hfss.modeler.create_rectangle(hfss.PLANE.XY,
         ...                                       [0, 0, -90], [10, 2], name="ImpedanceSheet",
-        ...                                        matname="Copper")
+        ...                                        material="Copper")
         >>> anistropic_impedance_to_sheet = hfss.assign_impedance_to_sheet(sheet.name,
         ...                                                                "ImpedanceFromSheet",
         ...                                                                [377, 0, 0, 377],
         ...                                                                [0, 50, 0, 0])
 
         """
 
@@ -3753,50 +3739,50 @@
         tol = 1e-6
         ports_ID = {}
         aedt_bounding_box = self.modeler.get_model_bounding_box()
         aedt_bounding_dim = self.modeler.get_bounding_dimension()
         directions = {}
         for el in assignment:
             objID = self.modeler.oeditor.GetFaceIDs(el)
-            faceCenter = self.modeler.oeditor.GetFaceCenter(int(objID[0]))
-            directionfound = False
-            l = min(aedt_bounding_dim) / 2
-            while not directionfound:
+            face_center = self.modeler.oeditor.GetFaceCenter(int(objID[0]))
+            direction_found = False
+            thickness = min(aedt_bounding_dim) / 2
+            while not direction_found:
                 self.modeler.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
-                    ["NAME:SheetThickenParameters", "Thickness:=", str(l) + "mm", "BothSides:=", False],
+                    ["NAME:SheetThickenParameters", "Thickness:=", str(thickness) + "mm", "BothSides:=", False],
                 )
-                # aedt_bounding_box2 = self.oeditor.GetModelBoundingBox()
+
                 aedt_bounding_box2 = self.modeler.get_model_bounding_box()
                 self._odesign.Undo()
                 if aedt_bounding_box != aedt_bounding_box2:
                     directions[el] = "External"
-                    directionfound = True
+                    direction_found = True
                 self.modeler.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
-                    ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(l) + "mm", "BothSides:=", False],
+                    ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(thickness) + "mm", "BothSides:=", False],
                 )
-                # aedt_bounding_box2 = self.oeditor.GetModelBoundingBox()
+
                 aedt_bounding_box2 = self.modeler.get_model_bounding_box()
 
                 self._odesign.Undo()
 
                 if aedt_bounding_box != aedt_bounding_box2:
                     directions[el] = "Internal"
-                    directionfound = True
+                    direction_found = True
                 else:
-                    l = l + min(aedt_bounding_dim) / 2
+                    thickness = thickness + min(aedt_bounding_dim) / 2
         for el in assignment:
             objID = self.modeler.oeditor.GetFaceIDs(el)
             maxarea = 0
             for f in objID:
                 faceArea = self.modeler.get_face_area(int(f))
                 if faceArea > maxarea:
                     maxarea = faceArea
-                    faceCenter = self.modeler.oeditor.GetFaceCenter(int(f))
+                    face_center = self.modeler.oeditor.GetFaceCenter(int(f))
             if directions[el] == "Internal":
                 self.modeler.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                     ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(value) + "mm", "BothSides:=", False],
                 )
             else:
                 self.modeler.oeditor.ThickenSheet(
@@ -3806,16 +3792,16 @@
             if "Vacuum" in el:
                 newfaces = self.modeler.oeditor.GetFaceIDs(el)
                 for f in newfaces:
                     try:
                         fc2 = self.modeler.oeditor.GetFaceCenter(f)
                         fc2 = [float(i) for i in fc2]
                         fa2 = self.modeler.get_face_area(int(f))
-                        faceoriginal = [float(i) for i in faceCenter]
-                        # dist = mat.sqrt(sum([(a*a-b*b) for a,b in zip(faceCenter, fc2)]))
+                        faceoriginal = [float(i) for i in face_center]
+                        # dist = mat.sqrt(sum([(a*a-b*b) for a,b in zip(face_center, fc2)]))
                         if abs(fa2 - maxarea) < tol**2 and (
                             abs(faceoriginal[2] - fc2[2]) > tol
                             or abs(faceoriginal[1] - fc2[1]) > tol
                             or abs(faceoriginal[0] - fc2[0]) > tol
                         ):
                             ports_ID[el] = int(f)
 
@@ -3828,16 +3814,16 @@
                         #     ports_ID[el] = int(f)
                     except Exception:
                         pass
             if extrude_internally:
                 objID2 = self.modeler.oeditor.GetFaceIDs(el)
                 for fid in objID2:
                     try:
-                        faceCenter2 = self.modeler.oeditor.GetFaceCenter(int(fid))
-                        if faceCenter2 == faceCenter:
+                        face_center2 = self.modeler.oeditor.GetFaceCenter(int(fid))
+                        if face_center2 == face_center:
                             self.modeler.oeditor.MoveFaces(
                                 ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                                 [
                                     "NAME:Parameters",
                                     [
                                         "NAME:MoveFacesParameters",
                                         "MoveAlongNormalFlag:=",
@@ -3853,15 +3839,14 @@
                                         "FacesToMove:=",
                                         [int(fid)],
                                     ],
                                 ],
                             )
                     except Exception:
                         self.logger.info("done")
-                        # self.modeler_oproject.ClearMessages()
         return ports_ID
 
     @pyaedt_function_handler(dname="design", ouputdir="ouput_dir")
     def validate_full_design(self, design=None, ouput_dir=None, ports=None):
         """Validate a design based on an expected value and save information to the log file.
 
 
@@ -4146,16 +4131,15 @@
         >>> oModule.AssignRadiation
 
         Examples
         --------
 
         Create a box and assign a radiation boundary to it.
 
-        >>> radiation_box = hfss.modeler.create_box([0, -200, -200], [200, 200, 200],
-        ...                                         name="Radiation_box")
+        >>> radiation_box = hfss.modeler.create_box([0, -200, -200],[200, 200, 200],name="Radiation_box")
         >>> radiation = hfss.assign_radiation_boundary_to_objects("Radiation_box")
         >>> type(radiation)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         object_list = self.modeler.convert_to_selections(assignment, return_list=True)
@@ -4190,16 +4174,15 @@
         >>> oModule.AssignHybridRegion
 
         Examples
         --------
 
         Create a box and assign a hybrid boundary to it.
 
-        >>> box = hfss.modeler.create_box([0, -200, -200], [200, 200, 200],
-        ...                                         name="Radiation_box")
+        >>> box = hfss.modeler.create_box([0, -200, -200],[200, 200, 200],name="Radiation_box")
         >>> sbr_box = hfss.assign_hybrid_region("Radiation_box")
         >>> type(sbr_box)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         object_list = self.modeler.convert_to_selections(assignment, return_list=True)
@@ -4234,16 +4217,15 @@
         >>> oModule.AssignFEBI
 
         Examples
         --------
 
         Create a box and assign an FE-BI boundary to it.
 
-        >>> box = hfss.modeler.create_box([0, -200, -200], [200, 200, 200],
-        ...                                         name="Radiation_box")
+        >>> box = hfss.modeler.create_box([0, -200, -200],[200, 200, 200],name="Radiation_box")
         >>> febi_box = hfss.assign_febi("Radiation_box")
         >>> type(febi_box)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
 
         object_list = self.modeler.convert_to_selections(assignment, return_list=True)
@@ -4278,16 +4260,15 @@
 
         Examples
         --------
 
         Create a box. Select the faces of this box and assign a radiation
         boundary to them.
 
-        >>> radiation_box = hfss.modeler.create_box([0 , -100, 0], [200, 200, 200],
-        ...                                         name="RadiationForFaces")
+        >>> radiation_box = hfss.modeler.create_box([0 , -100, 0],[200, 200, 200],name="RadiationForFaces")
         >>> ids = [i.id for i in hfss.modeler["RadiationForFaces"].faces]
         >>> radiation = hfss.assign_radiation_boundary_to_faces(ids)
         >>> type(radiation)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
         faces_list = self.modeler.convert_to_selections(assignment, True)
@@ -5539,16 +5520,15 @@
         >>> oModule.AssignSymmetry
 
         Examples
         --------
 
         Create a box. Select the faces of this box and assign a symmetry.
 
-        >>> symmetry_box = hfss.modeler.create_box([0 , -100, 0], [200, 200, 200],
-        ...                                         name="SymmetryForFaces")
+        >>> symmetry_box = hfss.modeler.create_box([0 , -100, 0],[200, 200, 200],name="SymmetryForFaces")
         >>> ids = [i.id for i in hfss.modeler["SymmetryForFaces"].faces]
         >>> symmetry = hfss.assign_symmetry(ids)
         >>> type(symmetry)
         <class 'pyaedt.modules.Boundary.BoundaryObject'>
 
         """
         try:
@@ -5591,16 +5571,15 @@
         >>> oModule.ChangeImpedanceMult
 
         Examples
         --------
 
         Create a box. Select the faces of this box and assign a symmetry.
 
-        >>> symmetry_box = hfss.modeler.create_box([0 , -100, 0], [200, 200, 200],
-        ...                                         name="SymmetryForFaces")
+        >>> symmetry_box = hfss.modeler.create_box([0 , -100, 0],[200, 200, 200],name="SymmetryForFaces")
         >>> ids = [i.id for i in hfss.modeler["SymmetryForFaces"].faces]
         >>> symmetry = hfss.assign_symmetry(ids)
         >>> hfss.set_impedance_multiplier(2.0)
 
         """
         try:
             if self.solution_type not in ["Modal"]:
@@ -5856,18 +5835,16 @@
 
         Examples
         --------
 
         Create two boxes that will be used to create a lumped port
         named ``'LumpedPort'``.
 
-        >>> box1 = hfss.modeler.create_box([0, 0, 50], [10, 10, 5],
-        ...                                "BoxLumped1","copper")
-        >>> box2 = hfss.modeler.create_box([0, 0, 60], [10, 10, 5],
-        ...                                "BoxLumped2", "copper")
+        >>> box1 = hfss.modeler.create_box([0, 0, 50],[10, 10, 5],"BoxLumped1","copper")
+        >>> box2 = hfss.modeler.create_box([0, 0, 60],[10, 10, 5],"BoxLumped2","copper")
         >>> hfss.lumped_port("BoxLumped1","BoxLumped2",hfss.AxisDir.XNeg,50,"LumpedPort",True,False)
         PyAEDT INFO: Connection Correctly created
         'LumpedPort'
 
         """
         if create_port_sheet:
             assignment = self.modeler.convert_to_selections(assignment)
@@ -5994,20 +5971,17 @@
         >>> oModule.AssignWavePort
 
         Examples
         --------
 
         Create a wave port supported by a microstrip line.
 
-        >>> ms = hfss.modeler.create_box([4, 5, 0], [1, 100, 0.2],
-        ...                               name="MS1", matname="copper")
-        >>> sub = hfss.modeler.create_box([0, 5, -2], [20, 100, 2],
-        ...                               name="SUB1", matname="FR4_epoxy")
-        >>> gnd = hfss.modeler.create_box([0, 5, -2.2], [20, 100, 0.2],
-        ...                               name="GND1", matname="FR4_epoxy")
+        >>> ms = hfss.modeler.create_box([4, 5, 0],[1, 100, 0.2],name="MS1",material="copper")
+        >>> sub = hfss.modeler.create_box([0, 5, -2],[20, 100, 2],name="SUB1",material="FR4_epoxy")
+        >>> gnd = hfss.modeler.create_box([0, 5, -2.2],[20, 100, 0.2],name="GND1",material="FR4_epoxy")
         >>> port = hfss.wave_port("GND1","MS1",integration_line=1,name="MS1")
         PyAEDT INFO: Connection correctly created.
 
         """
         oname = ""
 
         if create_port_sheet:
```

### Comparing `pyaedt-0.8.8/pyaedt/hfss3dlayout.py` & `pyaedt-0.8.9/pyaedt/hfss3dlayout.py`

 * *Files 7% similar despite different names*

```diff
@@ -69,14 +69,16 @@
     port : int, optional
         Port number on which to start the oDesktop communication on an already existing server.
         This parameter is ignored when creating a new server. It works only in 2022 R2 or later.
         The remote server must be up and running with the command `"ansysedt.exe -grpcsrv portnum"`.
     aedt_process_id : int, optional
         Process ID for the instance of AEDT to point PyAEDT at. The default is
         ``None``. This parameter is only used when ``new_desktop_session = False``.
+    ic_mode : bool, optional
+        Whether to set the design to IC mode or not. The default is ``False``.
 
     Examples
     --------
     Create an ``Hfss3dLayout`` object and connect to an existing HFSS
     design or create a new HFSS design if one does not exist.
 
     >>> from pyaedt import Hfss3dLayout
@@ -124,14 +126,15 @@
         non_graphical=False,
         new_desktop_session=False,
         close_on_exit=False,
         student_version=False,
         machine="",
         port=0,
         aedt_process_id=None,
+        ic_mode=False,
     ):
         FieldAnalysis3DLayout.__init__(
             self,
             "HFSS 3D Layout Design",
             projectname,
             designname,
             solution_type,
@@ -140,144 +143,170 @@
             non_graphical,
             new_desktop_session,
             close_on_exit,
             student_version,
             machine,
             port,
             aedt_process_id,
+            ic_mode,
         )
         ScatteringMethods.__init__(self, self)
 
     def _init_from_design(self, *args, **kwargs):
         self.__init__(*args, **kwargs)
 
-    @pyaedt_function_handler()
+    @property
+    def ic_mode(self):
+        """IC mode of current design.
+
+        Returns
+        -------
+        bool
+        """
+        return self.get_oo_property_value(self.odesign, "Design Settings", "Design Mode/IC")
+
+    @ic_mode.setter
+    def ic_mode(self, value):
+        self.set_oo_property_value(self.odesign, "Design Settings", "Design Mode/IC", value)
+
+    @pyaedt_function_handler(
+        primivitivename="assignment",
+        edgenumber="edge_number",
+        iscircuit="is_circuit_port",
+        iswave="is_wave_port",
+        ref_primitive_name="reference_primitive",
+        ref_edge_number="reference_edge_number",
+    )
     def create_edge_port(
         self,
-        primivitivename,
-        edgenumber,
-        iscircuit=False,
-        iswave=False,
+        assignment,
+        edge_number,
+        is_circuit_port=False,
+        is_wave_port=False,
         wave_horizontal_extension=5,
         wave_vertical_extension=3,
         wave_launcher="1mm",
-        ref_primitive_name=None,
-        ref_edge_number=0,
+        reference_primitive=None,
+        reference_edge_number=0,
     ):
         # type: (str | Line3dLayout,int,bool, bool,float,float, str, str, str | int) -> BoundaryObject3dLayout | bool
         """Create an edge port.
 
         Parameters
         ----------
-        primivitivename : str or :class:`pyaedt.modeler.pcb.object3dlayout.Line3dLayout`
+        assignment : str or :class:`pyaedt.modeler.pcb.object3dlayout.Line3dLayout`
             Name of the primitive to create the edge port on.
-        edgenumber :
+        edge_number :
             Edge number to create the edge port on.
-        iscircuit : bool, optional
+        is_circuit_port : bool, optional
             Whether the edge port is a circuit port. The default is ``False``.
-        iswave : bool, optional
+        is_wave_port : bool, optional
             Whether the edge port is a wave port. The default is ``False``.
         wave_horizontal_extension : float, optional
             Horizontal port extension factor. The default is `5`.
         wave_vertical_extension : float, optional
             Vertical port extension factor. The default is `5`.
         wave_launcher : str, optional
             PEC (perfect electrical conductor) launcher size with units. The
             default is `"1mm"`.
-        ref_primitive_name : str, optional
+        reference_primitive : str, optional
             Name of the reference primitive to place negative edge port terminal.
             The default is ``None``.
-        ref_edge_number : str, int
+        reference_edge_number : str, int
             Edge number of reference primitive. The default is ``0``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject3dLayout`
             Port objcet port when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateEdgePort
         """
-        primivitivename = self.modeler.convert_to_selections(primivitivename, False)
+        assignment = self.modeler.convert_to_selections(assignment, False)
         listp = self.port_list
         self.modeler.oeditor.CreateEdgePort(
             [
                 "NAME:Contents",
                 "edge:=",
-                ["et:=", "pe", "prim:=", primivitivename, "edge:=", edgenumber],
+                ["et:=", "pe", "prim:=", assignment, "edge:=", edge_number],
                 "circuit:=",
-                iscircuit,
+                is_circuit_port,
                 "btype:=",
                 0,
             ]
         )
 
         listnew = self.port_list
         a = [i for i in listnew if i not in listp]
 
-        if ref_primitive_name:
+        if reference_primitive:
             self.modeler.oeditor.AddRefPort(
                 [a[0]],
-                ["NAME:Contents", "edge:=", ["et:=", "pe", "prim:=", ref_primitive_name, "edge:=", ref_edge_number]],
+                [
+                    "NAME:Contents",
+                    "edge:=",
+                    ["et:=", "pe", "prim:=", reference_primitive, "edge:=", reference_edge_number],
+                ],
             )
 
         if len(a) > 0:
-            if iswave:
+            if is_wave_port:
                 self.modeler.change_property(
-                    property_object="Excitations:{}".format(a[0]),
-                    property_name="HFSS Type",
-                    property_value="Wave",
-                    property_tab="EM Design",
+                    assignment="Excitations:{}".format(a[0]),
+                    name="HFSS Type",
+                    value="Wave",
+                    aedt_tab="EM Design",
                 )
                 self.modeler.change_property(
-                    property_object="Excitations:{}".format(a[0]),
-                    property_name="Horizontal Extent Factor",
-                    property_value=str(wave_horizontal_extension),
-                    property_tab="EM Design",
+                    assignment="Excitations:{}".format(a[0]),
+                    name="Horizontal Extent Factor",
+                    value=str(wave_horizontal_extension),
+                    aedt_tab="EM Design",
                 )
                 if "Vertical Extent Factor" in list(
                     self.modeler.oeditor.GetProperties("EM Design", "Excitations:{}".format(a[0]))
                 ):
                     self.modeler.change_property(
-                        property_object="Excitations:{}".format(a[0]),
-                        property_name="Vertical Extent Factor",
-                        property_value=str(wave_vertical_extension),
-                        property_tab="EM Design",
+                        assignment="Excitations:{}".format(a[0]),
+                        name="Vertical Extent Factor",
+                        value=str(wave_vertical_extension),
+                        aedt_tab="EM Design",
                     )
                 self.modeler.change_property(
-                    property_object="Excitations:{}".format(a[0]),
-                    property_name="PEC Launch Width",
-                    property_value=str(wave_launcher),
-                    property_tab="EM Design",
+                    assignment="Excitations:{}".format(a[0]),
+                    name="PEC Launch Width",
+                    value=str(wave_launcher),
+                    aedt_tab="EM Design",
                 )
             bound = self._update_port_info(a[0])
             if bound:
                 self._boundaries[bound.name] = bound
                 return bound
             else:
                 return False
         else:
             return False
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(primitive_name="assignment")
     def create_wave_port(
         self,
-        primivitive_name,
+        assignment,
         edge_number,
         wave_horizontal_extension=5,
         wave_vertical_extension=3,
         wave_launcher="1mm",
     ):
         """Create a single-ended wave port.
 
         Parameters
         ----------
-        primivitive_name : str
+        assignment : str
             Name of the primitive to create the edge port on.
         edge_number : int
             Edge number to create the edge port on.
         wave_horizontal_extension : float, optional
             Horizontal port extension factor. The default is ``5``.
         wave_vertical_extension : float, optional
             Vertical port extension factor. The default is ``5``.
@@ -290,15 +319,15 @@
         :class:`pyaedt.modules.Boundary.BoundaryObject3dLayout`
             Port objcet port when successful, ``False`` when failed.
 
         References
         ----------
         """
         port_name = self.create_edge_port(
-            primivitive_name,
+            assignment,
             edge_number,
             wave_horizontal_extension=wave_horizontal_extension,
             wave_vertical_extension=wave_vertical_extension,
             wave_launcher=wave_launcher,
         )
         if port_name:
             port_name["HFSS Type"] = "Wave"
@@ -306,49 +335,53 @@
             if "Vertical Extent Factor" in list(port_name.props.keys()):
                 port_name["Vertical Extent Factor"] = str(wave_vertical_extension)
             port_name["PEC Launch Width"] = str(wave_launcher)
             return port_name
         else:
             return False
 
-    @pyaedt_function_handler()
-    def create_wave_port_from_two_conductors(self, primivitivenames=[""], edgenumbers=[""]):
+    @pyaedt_function_handler(primivitivenames="assignment", edgenumbers="edge_numbers")
+    def create_wave_port_from_two_conductors(self, assignment=None, edge_numbers=None):
         """Create a wave port.
 
         Parameters
         ----------
-        primivitivenames : list(str)
+        assignment : list, optional
             List of the primitive names to create the wave port on.
             The list must have two entries, one entry for each of the two conductors,
             or the method is not executed.
 
-        edgenumbers :
+        edge_numbers : list, optional
             List of the edge number to create the wave port on.
             The list must have two entries, one entry for each of the two edges,
             or the method is not executed.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject3dLayout`
             Port objcet port when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateEdgePort
         """
-        if len(primivitivenames) == 2 and len(edgenumbers) == 2:
+        if edge_numbers is None:
+            edge_numbers = [""]
+        if assignment is None:
+            assignment = [""]
+        if len(assignment) == 2 and len(edge_numbers) == 2:
             listp = self.port_list
             self.modeler.oeditor.CreateEdgePort(
                 [
                     "NAME:Contents",
                     "edge:=",
-                    ["et:=", "pe", "prim:=", primivitivenames[0], "edge:=", edgenumbers[0]],
+                    ["et:=", "pe", "prim:=", assignment[0], "edge:=", edge_numbers[0]],
                     "edge:=",
-                    ["et:=", "pe", "prim:=", primivitivenames[1], "edge:=", edgenumbers[1]],
+                    ["et:=", "pe", "prim:=", assignment[1], "edge:=", edge_numbers[1]],
                     "external:=",
                     True,
                     "btype:=",
                     0,
                 ]
             )
             listnew = self.port_list
@@ -361,44 +394,44 @@
                 else:
                     return False
             else:
                 return False
         else:
             return False
 
-    @pyaedt_function_handler()
-    def dissolve_component(self, component_name):
+    @pyaedt_function_handler(component_name="component")
+    def dissolve_component(self, component):
         """Dissolve a component and remove it from 3D Layout.
 
         Parameters
         ----------
-        component_name : str
+        component : str
             Name of the component.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
 
         """
-        self.oeditor.DissolveComponents(["NAME:elements", component_name])
+        self.oeditor.DissolveComponents(["NAME:elements", component])
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(component_name="component")
     def create_ports_on_component_by_nets(
         self,
-        component_name,
+        component,
         nets,
     ):
         """Create the ports on a component for a list of nets.
 
         Parameters
         ----------
-        component_name : str
+        component : str
             Component name.
         nets : str, list
             Nets to include.
 
 
         Returns
         -------
@@ -412,37 +445,37 @@
         """
         listp = self.port_list
         if isinstance(nets, list):
             pass
         else:
             nets = [nets]
         net_array = ["NAME:Nets"] + nets
-        self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", component_name], net_array, "Port", "0", "0", "0")
+        self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", component], net_array, "Port", "0", "0", "0")
         listnew = self.port_list
         a = [i for i in listnew if i not in listp]
         ports = []
         if len(a) > 0:
             for port in a:
                 bound = self._update_port_info(port)
                 if bound:
                     self._boundaries[bound.name] = bound
                     ports.append(bound)
         return ports
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(component_name="component")
     def create_pec_on_component_by_nets(
         self,
-        component_name,
+        component,
         nets,
     ):
         """Create a PEC connection on a component for a list of nets.
 
         Parameters
         ----------
-        component_name : str
+        component : str
             Component name.
         nets : str, list
             Nets to include.
 
 
         Returns
         -------
@@ -455,73 +488,73 @@
         >>> oEditor.CreateEdgePort
         """
         if isinstance(nets, list):
             pass
         else:
             nets = [nets]
         net_array = ["NAME:Nets"] + nets
-        self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", component_name], net_array, "PEC", "0", "0", "0")
+        self.oeditor.CreatePortsOnComponentsByNet(["NAME:Components", component], net_array, "PEC", "0", "0", "0")
         return True
 
-    @pyaedt_function_handler()
-    def create_differential_port(self, via_signal, via_reference, port_name, deembed=True):
+    @pyaedt_function_handler(port_name="name")
+    def create_differential_port(self, via_signal, via_reference, name, deembed=True):
         """Create a differential port.
 
         Parameters
         ----------
         via_signal : str
             Signal pin.
         via_reference : float
             Reference pin.
-        port_name : str
+        name : str
             New Port Name.
         deembed : bool, optional
-            Either to deembed parasitics or not. Default is `True`.
+            Whether to deembed parasitics. The default is ``True``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject3dLayout`
             Port Object when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateEdgePort
         """
         listp = self.port_list
-        if port_name in self.port_list:
-            self.logger.error("Port already existing on via {}".format(port_name))
+        if name in self.port_list:
+            self.logger.error("Port already existd on via {}.".format(name))
             return False
         self.oeditor.ToggleViaPin(["NAME:elements", via_signal])
 
         listnew = self.port_list
         a = [i for i in listnew if i not in listp]
         if len(a) > 0:
-            self.modeler.change_property("Excitations:{}".format(a[0]), "Port", port_name, "EM Design")
-            self.modeler.oeditor.AssignRefPort([port_name], via_reference)
+            self.modeler.change_property("Excitations:{}".format(a[0]), "Port", name, "EM Design")
+            self.modeler.oeditor.AssignRefPort([name], via_reference)
             if deembed:
                 self.modeler.change_property(
-                    "Excitations:{}".format(port_name), "DeembedParasiticPortInductance", deembed, "EM Design"
+                    "Excitations:{}".format(name), "DeembedParasiticPortInductance", deembed, "EM Design"
                 )
-            bound = self._update_port_info(port_name)
+            bound = self._update_port_info(name)
             if bound:
                 self._boundaries[bound.name] = bound
                 return bound
             else:
                 return False
         else:
             return False
 
-    @pyaedt_function_handler()
-    def create_coax_port(self, vianame, radial_extent=0.1, layer=None, alignment="lower"):
-        """Create a new coax port.
+    @pyaedt_function_handler(vianame="via")
+    def create_coax_port(self, via, radial_extent=0.1, layer=None, alignment="lower"):
+        """Create a coax port.
 
         Parameters
         ----------
-        vianame : str
+        via : str
             Name of the via to create the port on.
         radial_extent : float
             Radial coax extension.
         layer : str
             Name of the layer to apply the reference to.
         alignment : str, optional
             Port alignment on the layer.
@@ -533,59 +566,55 @@
 
         References
         ----------
 
         >>> oEditor.CreateEdgePort
         """
         listp = self.port_list
-        if vianame in self.port_list:
-            self.logger.error("Port already existing on via {}".format(vianame))
+        if via in self.port_list:
+            self.logger.error("Port already exists on via {}.".format(via))
             return False
-        self.oeditor.ToggleViaPin(["NAME:elements", vianame])
+        self.oeditor.ToggleViaPin(["NAME:elements", via])
 
         listnew = self.port_list
         a = [i for i in listnew if i not in listp]
         if len(a) > 0:
             self.modeler.change_property(
                 "Excitations:{}".format(a[0]), "Radial Extent Factor", str(radial_extent), "EM Design"
             )
             self.modeler.change_property("Excitations:{}".format(a[0]), "Layer Alignment", alignment, "EM Design")
             if layer:
-                self.modeler.change_property(
-                    a[0],
-                    "Pad Port Layer",
-                    layer,
-                )
+                self.modeler.change_property(a[0], "Pad Port Layer", layer)
             bound = self._update_port_info(a[0])
             if bound:
                 self._boundaries[bound.name] = bound
                 return bound
             else:
                 return False
         else:
             return False
 
-    @pyaedt_function_handler()
-    def create_pin_port(self, name, xpos=0, ypos=0, rotation=0, top_layer=None, bot_layer=None):
+    @pyaedt_function_handler(xpos="x", ypos="y", bot_layer="bottom_layer")
+    def create_pin_port(self, name, x=0, y=0, rotation=0, top_layer=None, bottom_layer=None):
         """Create a pin port.
 
         Parameters
         ----------
         name : str
             Name of the pin port.
-        xpos : float, optional
+        x : float, optional
             X-axis position of the pin. The default is ``0``.
-        ypos : float, optional
+        y : float, optional
             Y-axis position of the pin. The default is ``0``.
         rotation : float, optional
             Rotation of the pin in degrees. The default is ``0``.
         top_layer : str, optional
             Top layer of the pin. The default is ``None``, in which case the top
             layer is assigned automatically.
-        bot_layer : str
+        bottom_layer : str
             Bottom layer of the pin. The default is ``None``, in which case the
             bottom layer is assigned automatically.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject3dLayout`
 
@@ -595,107 +624,107 @@
         ----------
 
         >>> oEditor.CreatePin
         """
         layers = self.modeler.layers.all_signal_layers
         if not top_layer:
             top_layer = layers[0].name
-        if not bot_layer:
-            bot_layer = layers[len(layers) - 1].name
+        if not bottom_layer:
+            bottom_layer = layers[len(layers) - 1].name
         self.modeler.oeditor.CreatePin(
             [
                 "NAME:Contents",
                 ["NAME:Port", "Name:=", name],
                 "ReferencedPadstack:=",
                 "Padstacks:NoPad SMT East",
                 "vposition:=",
-                ["x:=", str(xpos) + self.modeler.model_units, "y:=", str(ypos) + self.modeler.model_units],
+                ["x:=", str(x) + self.modeler.model_units, "y:=", str(y) + self.modeler.model_units],
                 "vrotation:=",
                 [str(rotation) + "deg"],
                 "overrides hole:=",
                 False,
                 "hole diameter:=",
                 ["0mm"],
                 "Pin:=",
                 True,
                 "highest_layer:=",
                 top_layer,
                 "lowest_layer:=",
-                bot_layer,
+                bottom_layer,
             ]
         )
         bound = self._update_port_info(name)
         if bound:
             self._boundaries[bound.name] = bound
             return bound
         else:
             return False
 
-    @pyaedt_function_handler()
-    def delete_port(self, portname):
+    @pyaedt_function_handler(portname="name")
+    def delete_port(self, name):
         """Delete a port.
 
         Parameters
         ----------
-        portname : str
+        name : str
             Name of the port.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.Delete
         """
-        self.oexcitation.Delete(portname)
+        self.oexcitation.Delete(name)
         for bound in self.boundaries:
-            if bound.name == portname:
+            if bound.name == name:
                 self.boundaries.remove(bound)
         return True
 
-    @pyaedt_function_handler()
-    def import_edb(self, edb_full_path):
+    @pyaedt_function_handler(edb_full_path="input_folder")
+    def import_edb(self, input_folder):
         """Import EDB.
 
         Parameters
         ----------
-        edb_full_path : str
+        input_folder : str
             Full path to EDB.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportEDB
         """
-        if "edb.def" not in edb_full_path:
-            edb_full_path = os.path.join(edb_full_path, "edb.def")
-        self.oimport_export.ImportEDB(edb_full_path)
+        if "edb.def" not in input_folder:
+            input_folder = os.path.join(input_folder, "edb.def")
+        self.oimport_export.ImportEDB(input_folder)
         self._close_edb()
         project_name = self.odesktop.GetActiveProject().GetName()
         design_name = self.odesktop.GetActiveProject().GetActiveDesign().GetName().split(";")[-1]
         self.__init__(projectname=project_name, designname=design_name)
         return True
 
-    @pyaedt_function_handler()
-    def validate_full_design(self, name=None, outputdir=None, ports=None):
+    @pyaedt_function_handler(outputdir="output_dir")
+    def validate_full_design(self, name=None, output_dir=None, ports=None):
         """Validate the design based on the expected value and save the information in the log file.
 
         Parameters
         ----------
         name : str, optional
             Name of the design to validate. The default is ``None``.
-        outputdir : str, optional
+        output_dir : str, optional
             Output directory to save the log file to. The default is ``None``,
             in which case the file is exported to the working directory.
 
         ports : str, optional
             Number of excitations that are expected. The default is ``None``.
 
         Returns
@@ -706,30 +735,30 @@
         References
         ----------
 
         >>> oDesign.ValidateDesign
         """
         if name is None:
             name = self.design_name
-        if outputdir is None:
-            outputdir = self.working_directory
+        if output_dir is None:
+            output_dir = self.working_directory
 
         self.logger.info("#### Design Validation Checks###")
         #
         # Routine outputs to the validation info to a log file in the project directory and also
         # returns the validation info to be used to update properties.xml file
 
         validation_ok = True
 
         #
         # Write an overall validation log file with all output from all checks
-        # The design validation inside HFSS outputs to a separate log file which we merge into this overall file
+        # The design validation inside HFSS outputs to a separate log file that is merged into this overall file
         #
         val_list = []
-        all_validate = outputdir + "\\all_validation.log"
+        all_validate = output_dir + "\\all_validation.log"
         with open_file(all_validate, "w") as validation:
             # Desktop Messages
             msg = "Desktop Messages:"
             validation.writelines(msg + "\n")
             val_list.append(msg)
             msgs = self._desktop.GetMessages(self.project_name, name, 0)
             # need to check if design name is always this default name HFSSDesign1
@@ -780,23 +809,23 @@
                 msg = "Excitation name: " + str(excitation)
                 self.logger.info(msg)
                 validation.writelines(msg + "\n")
                 val_list.append(msg)
         validation.close()
         return val_list, validation_ok  # return all the info in a list for use later
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(plot_name="plot")
     def create_scattering(
-        self, plot_name="S Parameter Plot Nominal", sweep_name=None, port_names=None, port_excited=None, variations=None
+        self, plot="S Parameter Plot Nominal", sweep_name=None, port_names=None, port_excited=None, variations=None
     ):
         """Create a scattering report.
 
         Parameters
         ----------
-        plot_name : str, optional
+        plot : str, optional
             Name of the plot. The default is ``"S Parameter Plot Nominal"``.
         sweep_name : str, optional
             Name of the sweep. The default is ``None``.
         port_names : str or list, optional
             One or more port names. The default is ``None``.
         port_excited : optional
             The default is ``None``.
@@ -820,19 +849,19 @@
             solution_data = "Terminal Solution Data"
         if not port_names:
             port_names = self.excitations
         if not port_excited:
             port_excited = port_names
         traces = ["dB(S(" + p + "," + q + "))" for p, q in zip(list(port_names), list(port_excited))]
         return self.post.create_report(
-            traces, sweep_name, variations=variations, report_category=solution_data, plot_name=plot_name
+            traces, sweep_name, variations=variations, report_category=solution_data, plot_name=plot
         )
 
-    @pyaedt_function_handler()
-    def set_export_touchstone(self, activate, export_dir=""):
+    @pyaedt_function_handler(export_dir="output_dir")
+    def set_export_touchstone(self, activate, output_dir=""):
         """Export the Touchstone file automatically if the simulation is successful.
 
         Parameters
         ----------
         activate : bool
             Whether to export the Touchstone file after the simulation.
         export_dir str, optional
@@ -850,15 +879,15 @@
         """
         settings = []
         if activate:
             settings.append("NAME:options")
             settings.append("ExportAfterSolve:=")
             settings.append(True)
             settings.append("ExportDir:=")
-            settings.append(export_dir)
+            settings.append(output_dir)
         elif not activate:
             settings.append("NAME:options")
             settings.append("ExportAfterSolve:=")
             settings.append(False)
         self.odesign.DesignOptions(settings, 0)
         return True
 
@@ -1233,24 +1262,26 @@
         if set_as_active:
             self._close_edb()
             self.__init__(project_name)
         if close_active_project:
             self.odesktop.CloseProject(active_project)
         return True
 
-    @pyaedt_function_handler()
-    def import_gds(self, gds_path, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False):
+    @pyaedt_function_handler(gds_path="input_file", aedb_path="output_dir")
+    def import_gds(
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
+    ):
         """Import a GDS file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
-        gds_path : str
+        input_file : str
             Full path to the GDS file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML or TECH file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
             If a TECH file is provided and the layer name starts with ``"v"``, the layer
             is mapped as a via layer.
         set_as_active : bool, optional
             Whether to set the GDS file as active. The default is ``True``.
@@ -1263,26 +1294,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportGDSII
         """
-        return self._import_cad(gds_path, "gds", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "gds", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
-    def import_dxf(self, dxf_path, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False):
+    @pyaedt_function_handler(dxf_path="input_file", aedb_path="output_dir")
+    def import_dxf(
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
+    ):
         """Import a DXF file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
-        dxf_path : str
+        input_file : str
             Full path to the DXF file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML or TECH file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
             If a TECH file is provided and the layer name starts with ``"v"``, the layer
             is mapped as a via layer.
         set_as_active : bool, optional
             Whether to set the DXF file as active. The default is ``True``.
@@ -1295,28 +1328,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportDXF
         """
-        return self._import_cad(dxf_path, "dxf", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "dxf", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(gerber_path="input_file", aedb_path="output_dir")
     def import_gerber(
-        self, gerber_path, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
     ):
         """Import a Gerber zip file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
-        gerber_path : str
+        input_file : str
             Full path to the Gerber zip file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
         set_as_active : bool, optional
             Whether to set the Gerber zip file file as active. The default is ``True``.
         close_active_project : bool, optional
             Whether to close the active project after loading the Gerber zip file file.
@@ -1327,28 +1360,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportGerber
         """
-        return self._import_cad(gerber_path, "gerber", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "gerber", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(aedb_path="output_dir")
     def import_brd(
-        self, input_file, aedb_path=None, set_as_active=True, close_active_project=False, control_file=None
+        self, input_file, output_dir=None, set_as_active=True, close_active_project=False, control_file=None
     ):  # pragma: no cover
         """Import a board file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
         input_file : str
             Full path to the board file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         set_as_active : bool, optional
             Whether to set the board file as active. The default is ``True``.
         close_active_project : bool, optional
             Whether to close the active project after loading the board file.
             The default is ''False``.
         control_file : str, optional
             Path to the XML file with the stackup information. The default is ``None``, in
@@ -1360,28 +1393,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportExtracta
         """
-        return self._import_cad(input_file, "brd", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "brd", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(aedb_path="output_dir")
     def import_awr(
-        self, input_file, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
     ):  # pragma: no cover
         """Import an AWR Microwave Office file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
         input_file : str
             Full path to the AWR Microwave Office file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
         set_as_active : bool, optional
             Whether to set the AWR Microwave Office file as active. The default is ``True``.
         close_active_project : bool, optional
             Whether to close the active project after loading the AWR Microwave Office file.
@@ -1392,28 +1425,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportAWRMicrowaveOffice
         """
-        return self._import_cad(input_file, "awr", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "awr", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(aedb_path="output_dir")
     def import_ipc2581(
-        self, input_file, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
     ):
         """Import an IPC2581 file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
         input_file : str
             Full path to the IPC2581 file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
         set_as_active : bool, optional
             Whether to set the IPC2581 file as active. The default is ``True``.
         close_active_project : bool, optional
             Whether to close the active project after loading the IPC2581 file.
@@ -1424,26 +1457,28 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportAWRMicrowaveOffice
         """
-        return self._import_cad(input_file, "ipc2581", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "ipc2581", output_dir, control_file, set_as_active, close_active_project)
 
-    @pyaedt_function_handler()
-    def import_odb(self, input_file, aedb_path=None, control_file=None, set_as_active=True, close_active_project=False):
+    @pyaedt_function_handler(aedb_path="output_dir")
+    def import_odb(
+        self, input_file, output_dir=None, control_file=None, set_as_active=True, close_active_project=False
+    ):
         """Import an ODB++ file into HFSS 3D Layout and assign the stackup from an XML file if present.
 
         Parameters
         ----------
         input_file : str
             Full path to the ODB++ file.
-        aedb_path : str, optional
-            Full path to the AEDB file.
+        output_dir : str, optional
+            Full path to the AEDB folder. For example, ``"c:\\temp\\test.aedb"``.
         control_file : str, optional
             Path to the XML file with the stackup information. The default is ``None``, in
             which case the stackup is not edited.
         set_as_active : bool, optional
             Whether to set the ODB++ file as active. The default is ``True``.
         close_active_project : bool, optional
             Whether to close the active project after loading the ODB++ file.
@@ -1454,15 +1489,15 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.ImportAWRMicrowaveOffice
         """
-        return self._import_cad(input_file, "odb++", aedb_path, control_file, set_as_active, close_active_project)
+        return self._import_cad(input_file, "odb++", output_dir, control_file, set_as_active, close_active_project)
 
     @pyaedt_function_handler()
     def edit_cosim_options(
         self,
         simulate_missing_solution=True,
         align_ports=True,
         renormalize_ports=True,
@@ -1566,41 +1601,48 @@
         arg.append("Renormalize:=")
         arg.append(renormalize_ports)
         arg.append("RenormImpedance:=")
         arg.append(renorm_impedance)
         self.odesign.EditCoSimulationOptions(arg)
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        positive_terminal="assignment",
+        negative_terminal="reference",
+        common_name="common_mode",
+        diff_name="differential_mode",
+        common_ref="common_reference",
+        diff_ref_z="differential_reference",
+    )
     def set_differential_pair(
         self,
-        positive_terminal,
-        negative_terminal,
-        common_name=None,
-        diff_name=None,
-        common_ref_z=25,
-        diff_ref_z=100,
+        assignment,
+        reference,
+        common_mode=None,
+        differential_mode=None,
+        common_reference=25,
+        differential_reference=100,
         active=True,
         matched=False,
     ):
         """Add a differential pair definition.
 
         Parameters
         ----------
-        positive_terminal : str
+        assignment : str
             Name of the terminal to use as the positive terminal.
-        negative_terminal : str
+        reference : str
             Name of the terminal to use as the negative terminal.
-        common_name : str, optional
+        common_mode : str, optional
             Name for the common mode. The default is ``None``, in which case a unique name is assigned.
-        diff_name : str, optional
+        differential_mode : str, optional
             Name for the differential mode. The default is ``None``, in which case a unique name is assigned.
-        common_ref_z : float, optional
+        common_reference : float, optional
             Reference impedance for the common mode in ohms. The default is ``25``.
-        diff_ref_z : float, optional
+        differential_reference : float, optional
             Reference impedance for the differential mode in ohms. The default is ``100``.
         active : bool, optional
             Whether to set the differential pair as active. The default is ``True``.
         matched : bool, optional
             Whether to set the differential pair as active. The default is ``False``.
 
         Returns
@@ -1608,36 +1650,36 @@
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oModule.SetDiffPairs
         """
-        if not diff_name:
-            diff_name = generate_unique_name("Diff")
-        if not common_name:
-            common_name = generate_unique_name("Comm")
+        if not differential_mode:
+            differential_mode = generate_unique_name("Diff")
+        if not common_mode:
+            common_mode = generate_unique_name("Comm")
 
         arg1 = [
             "Pos:=",
-            positive_terminal,
+            assignment,
             "Neg:=",
-            negative_terminal,
+            reference,
             "On:=",
             active,
             "matched:=",
             matched,
             "Dif:=",
-            diff_name,
+            differential_mode,
             "DfZ:=",
-            [float(diff_ref_z), 0],
+            [float(differential_reference), 0],
             "Com:=",
-            common_name,
+            common_mode,
             "CmZ:=",
-            [float(common_ref_z), 0],
+            [float(common_reference), 0],
         ]
 
         arg = ["NAME:DiffPairs"]
         arg.append("Pair:=")
         arg.append(arg1)
 
         tmpfile1 = os.path.join(self.working_directory, generate_unique_name("tmp"))
@@ -1683,17 +1725,14 @@
         return True
 
     @pyaedt_function_handler()
     def get_differential_pairs(self):
         # type: () -> list
         """Get the list defined differential pairs.
 
-        Parameters
-        ----------
-        None
 
         Returns
         -------
         list
             List of differential pairs.
 
         Examples
@@ -1717,106 +1756,106 @@
             try:
                 os.remove(tmpfile1)
             except Exception:  # pragma: no cover
                 self.logger.warning("ERROR: Cannot remove temp files.")
 
         return list_output
 
-    @pyaedt_function_handler()
-    def load_diff_pairs_from_file(self, filename):
+    @pyaedt_function_handler(filename="input_file")
+    def load_diff_pairs_from_file(self, input_file):
         # type: (str) -> bool
-        """Load differtential pairs definition from file.
+        """Load differential pairs definition from a file.
 
         You can use the ``save_diff_pairs_to_file`` method to obtain the file format.
         The ``File End Of Line`` must be UNIX (LF).
         New definitions are added only if compatible with the existing definition already defined in the project.
 
         Parameters
         ----------
-        filename : str
-            Fully qualified name of the file containing the differential pairs definition.
+        input_file : str
+            Full path to the differential pairs definition file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oModule.LoadDiffPairsFromFile
         """
-        if not os.path.isfile(filename):  # pragma: no cover
-            raise ValueError("{}: unable to find the specified file.".format(filename))
+        if not os.path.isfile(input_file):  # pragma: no cover
+            raise ValueError("{}: Unable to find the specified file.".format(input_file))
 
         try:
-            new_file = os.path.join(os.path.dirname(filename), generate_unique_name("temp") + ".txt")
-            with open_file(filename, "r") as file:
+            new_file = os.path.join(os.path.dirname(input_file), generate_unique_name("temp") + ".txt")
+            with open_file(input_file, "r") as file:
                 filedata = file.read().splitlines()
             with io.open(new_file, "w", newline="\n") as fh:
                 for line in filedata:
                     fh.write(line + "\n")
 
             self.oexcitation.LoadDiffPairsFromFile(new_file)
             os.remove(new_file)
         except Exception:  # pragma: no cover
             return False
         return True
 
-    @pyaedt_function_handler()
-    def save_diff_pairs_to_file(self, filename):
+    @pyaedt_function_handler(filename="output_file")
+    def save_diff_pairs_to_file(self, output_file):
         # type: (str) -> bool
         """Save differtential pairs definition to a file.
 
         If a file with the specified name already exists, it is overwritten.
 
         Parameters
         ----------
-        filename : str
-            Fully qualified name of the file containing the differential pairs definition.
+        output_file : str
+            Full path to the differential pairs definition file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
         >>> oModule.SaveDiffPairsToFile
         """
-        self.oexcitation.SaveDiffPairsToFile(filename)
+        self.oexcitation.SaveDiffPairsToFile(output_file)
 
-        return os.path.isfile(filename)
+        return os.path.isfile(output_file)
 
-    @pyaedt_function_handler()
-    def export_3d_model(self, file_name=None):
+    @pyaedt_function_handler(file_name="output_file")
+    def export_3d_model(self, output_file=None):
         """Export the Ecad model to a 3D file.
 
         Parameters
         ----------
-        file_name : str, optional
-            Full name of the file to export. The default is None, in which case the file name is
+        output_file : str, optional
+            Full name of the file to export. The default is ``None``, in which case the file name is
             set to the design name and saved as a SAT file in the working directory.
-            Extensions available are ``"sat"``, ``"sab"``, and ``"sm3"`` up to AEDT 2022R2 and
+            Extensions available are ``"sat"``, ``"sab"``, and ``"sm3"`` up to AEDT 2022 R2 and
             Parasolid format `"x_t"` from AEDT 2023R1.
 
         Returns
         -------
         str
             File name if successful.
         """
-        if not file_name:
+        if not output_file:
             if settings.aedt_version > "2022.2":
-                file_name = os.path.join(self.working_directory, self.design_name + ".x_t")
-                self.modeler.oeditor.ExportCAD(["NAME:options", "FileName:=", file_name])
+                output_file = os.path.join(self.working_directory, self.design_name + ".x_t")
+                self.modeler.oeditor.ExportCAD(["NAME:options", "FileName:=", output_file])
 
             else:
-                file_name = os.path.join(self.working_directory, self.design_name + ".sat")
-                self.modeler.oeditor.ExportAcis(["NAME:options", "FileName:=", file_name])
+                output_file = os.path.join(self.working_directory, self.design_name + ".sat")
+                self.modeler.oeditor.ExportAcis(["NAME:options", "FileName:=", output_file])
 
-        return file_name
+        return output_file
 
     @pyaedt_function_handler()
     def enable_rigid_flex(self):
         """Turn on or off the rigid flex of a board with bending if available.
 
         This function is the same for both turning on and off rigid flex.
 
@@ -1828,15 +1867,15 @@
         """
         if settings.aedt_version >= "2022.2":
             self.modeler.oeditor.ProcessBentModelCmd()
         if self.desktop_class.non_graphical:
             return True
         return True if self.variable_manager["BendModel"].expression == "1" else False
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def edit_hfss_extents(
         self,
         diel_extent_type=None,
         diel_extent_horizontal_padding=None,
         diel_honor_primitives_on_diel_layers="keep",
         air_extent_type=None,
         air_truncate_model_at_ground_layer="keep",
@@ -1942,39 +1981,41 @@
             if fnmatch.fnmatch(filename, model_name)
         ]
         if out_files:
             out_files.sort(key=lambda x: os.path.getmtime(x))
             return out_files[0]
         return ""
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(source_name="source", file_name="input_file")
     def edit_source_from_file(
         self,
-        source_name,
-        file_name,
+        source,
+        input_file,
         is_time_domain=True,
         x_scale=1,
         y_scale=1,
         impedance=50,
         data_format="Power",
         encoding="utf-8",
         include_post_effects=True,
         incident_voltage=True,
     ):
         """Edit a source from file data.
         File data is a csv containing either frequency data or time domain data that will be converted through FFT.
 
         Parameters
         ----------
-        source_name : str
+        source : str
             Source Name.
-        file_name : str
+        input_file : str
             Full name of the input file.
         is_time_domain : bool, optional
-            Either if the input data is Time based or Frequency Based. Frequency based data are Mag/Phase (deg).
+            Whether the input data is time-based. The defaulti s ``True``. If
+            ``False``, the input data is frequency-based. Frequency-based data
+            is degrees in this format: ``Mag/Phase``.
         x_scale : float, optional
             Scaling factor for x axis.
         y_scale : float, optional
             Scaling factor for y axis.
         impedance : float, optional
             Excitation impedance. Default is `50`.
         data_format : str, optional
@@ -1989,51 +2030,51 @@
 
         Returns
         -------
         bool
         """
         out = "Voltage"
         freq, mag, phase = parse_excitation_file(
-            file_name=file_name,
+            file_name=input_file,
             is_time_domain=is_time_domain,
             x_scale=x_scale,
             y_scale=y_scale,
             impedance=impedance,
             data_format=data_format,
             encoding=encoding,
             out_mag=out,
         )
-        ds_name_mag = "ds_" + source_name.replace(":", "_mode_") + "_Mag"
-        ds_name_phase = "ds_" + source_name.replace(":", "_mode_") + "_Angle"
+        ds_name_mag = "ds_" + source.replace(":", "_mode_") + "_Mag"
+        ds_name_phase = "ds_" + source.replace(":", "_mode_") + "_Angle"
         if self.dataset_exists(ds_name_mag, False):
             self.design_datasets[ds_name_mag].x = freq
             self.design_datasets[ds_name_mag].y = mag
             self.design_datasets[ds_name_mag].update()
         else:
             self.create_dataset1d_design(ds_name_mag, freq, mag, xunit="Hz")
         if self.dataset_exists(ds_name_phase, False):
             self.design_datasets[ds_name_phase].x = freq
             self.design_datasets[ds_name_phase].y = phase
             self.design_datasets[ds_name_phase].update()
 
         else:
             self.create_dataset1d_design(ds_name_phase, freq, phase, xunit="Hz", yunit="deg")
         for p in self.boundaries:
-            if p.name == source_name:
+            if p.name == source:
                 str_val = ["TotalVoltage"]
                 if incident_voltage:
                     str_val = ["IncidentVoltage"]
                 if include_post_effects:
                     str_val.append("IncludePortPostProcess")
                 self.oboundary.EditExcitations(
                     [
                         "NAME:Excitations",
-                        [source_name, "pwl({}, Freq)".format(ds_name_mag), "pwl({}, Freq)".format(ds_name_phase)],
+                        [source, "pwl({}, Freq)".format(ds_name_mag), "pwl({}, Freq)".format(ds_name_phase)],
                     ],
-                    ["NAME:Terminations", [source_name, False, str(impedance) + "ohm", "0ohm"]],
+                    ["NAME:Terminations", [source, False, str(impedance) + "ohm", "0ohm"]],
                     ",".join(str_val),
                     [],
                 )
 
                 self.logger.info("Source Excitation updated with Dataset.")
                 return True
         self.logger.error("Port not found.")
```

### Comparing `pyaedt-0.8.8/pyaedt/icepak.py` & `pyaedt-0.8.9/pyaedt/icepak.py`

 * *Files 1% similar despite different names*

```diff
@@ -420,16 +420,16 @@
         >>> oModule.AssignBlockBoundary
 
         Examples
         --------
 
         Create block boundaries from each box in the list.
 
-        >>> box1 = icepak.modeler.create_box([1, 1, 1], [3, 3, 3], "BlockBox1", "copper")
-        >>> box2 = icepak.modeler.create_box([2, 2, 2], [4, 4, 4], "BlockBox2", "copper")
+        >>> box1 = icepak.modeler.create_box([1, 1, 1],[3, 3, 3],"BlockBox1","copper")
+        >>> box2 = icepak.modeler.create_box([2, 2, 2],[4, 4, 4],"BlockBox2","copper")
         >>> blocks = icepak.create_source_blocks_from_list([["BlockBox1", 2], ["BlockBox2", 4]])
         PyAEDT INFO: Block on ...
         >>> blocks[1].props
         {'Objects': ['BlockBox1'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '2W'}
         >>> blocks[3].props
         {'Objects': ['BlockBox2'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '4W'}
         """
@@ -484,15 +484,15 @@
         ----------
 
         >>> oModule.AssignBlockBoundary
 
         Examples
         --------
 
-        >>> box = icepak.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
+        >>> box = icepak.modeler.create_box([5, 5, 5],[1, 2, 3],"BlockBox3","copper")
         >>> block = icepak.create_source_block("BlockBox3", "1W", False)
         PyAEDT INFO: Block on ...
         >>> block.props
         {'Objects': ['BlockBox3'], 'Block Type': 'Solid', 'Use External Conditions': False, 'Total Power': '1W'}
 
         """
         if assign_material:
@@ -684,15 +684,15 @@
         >>> oModule.AssignSourceBoundary
 
         Examples
         --------
 
         Create two source boundaries from one box, one on the top face and one on the bottom face.
 
-        >>> box = icepak.modeler.create_box([0, 0, 0], [20, 20, 20], name="SourceBox")
+        >>> box = icepak.modeler.create_box([0, 0, 0],[20, 20, 20],name="SourceBox")
         >>> source1 = icepak.create_source_power(box.top_face_z.id, input_power="2W")
         >>> source1.props["Total Power"]
         '2W'
         >>> source2 = icepak.create_source_power(box.bottom_face_z.id,
         ...                                      thermal_condtion="Fixed Temperature",
         ...                                      temperature="28cel")
         >>> source2.props["Temperature"]
@@ -777,15 +777,15 @@
         ----------
 
         >>> oModule.AssignNetworkBoundary
 
         Examples
         --------
 
-        >>> box = icepak.modeler.create_box([4, 5, 6], [5, 5, 5], "NetworkBox1", "copper")
+        >>> box = icepak.modeler.create_box([4, 5, 6],[5, 5, 5],"NetworkBox1","copper")
         >>> block = icepak.create_network_block("NetworkBox1", "2W", 20, 10, 2 , 1.05918)
         >>> block.props["Nodes"]["Internal"][0]
         '2W'
         """
         warnings.warn(
             "This method is deprecated in 0.6.27. Use the create_two_resistor_network_block() method.",
             DeprecationWarning,
@@ -877,16 +877,16 @@
         >>> oModule.AssignNetworkBoundary
 
         Examples
         --------
 
         Create network boundaries from each box in the list.
 
-        >>> box1 = icepak.modeler.create_box([1, 2, 3], [10, 10, 10], "NetworkBox2", "copper")
-        >>> box2 = icepak.modeler.create_box([4, 5, 6], [5, 5, 5], "NetworkBox3", "copper")
+        >>> box1 = icepak.modeler.create_box([1, 2, 3],[10, 10, 10],"NetworkBox2","copper")
+        >>> box2 = icepak.modeler.create_box([4, 5, 6],[5, 5, 5],"NetworkBox3","copper")
         >>> blocks = icepak.create_network_blocks([["NetworkBox2", 20, 10, 3], ["NetworkBox3", 4, 10, 2]],
         ...                                        2, 1.05918, False)
         >>> blocks[0].props["Nodes"]["Internal"]
         ['3W']
         """
         objs = self.modeler.solid_names
         countpow = len(input_list[0]) - 3
@@ -943,16 +943,15 @@
         >>> oModule.AssignFaceMonitor
 
         Examples
         --------
 
         Create a rectangle named ``"Surface1"`` and assign a temperature monitor to that surface.
 
-        >>> surface = icepak.modeler.create_rectangle(icepak.PLANE.XY,
-        ...                                           [0, 0, 0], [10, 20], name="Surface1")
+        >>> surface = icepak.modeler.create_rectangle(icepak.PLANE.XY,[0, 0, 0],[10, 20],name="Surface1")
         >>> icepak.assign_surface_monitor("Surface1", monitor_name="monitor")
         'monitor'
         """
         return self._monitor.assign_surface_monitor(face_name, monitor_quantity=monitor_type, monitor_name=monitor_name)
 
     @pyaedt_function_handler()
     def assign_point_monitor(self, point_position, monitor_type="Temperature", monitor_name=None):
@@ -1014,15 +1013,15 @@
         >>> oModule.AssignPointMonitor
 
         Examples
         --------
 
         Create a box named ``"BlockBox1"`` and assign a temperature monitor point to that object.
 
-        >>> box = icepak.modeler.create_box([1, 1, 1], [3, 3, 3], "BlockBox1", "copper")
+        >>> box = icepak.modeler.create_box([1, 1, 1],[3, 3, 3],"BlockBox1","copper")
         >>> icepak.assign_point_monitor(box.name, monitor_name="monitor2")
         "'monitor2'
         """
         return self._monitor.assign_point_monitor_in_object(
             name, monitor_quantity=monitor_type, monitor_name=monitor_name
         )
 
@@ -1164,15 +1163,15 @@
             self.modeler.oeditor.ChangeProperty(args)
         oBoundingBox = self.modeler.get_model_bounding_box()
         if gravityDir < 3:
             return oBoundingBox[gravityDir + 3]
         else:
             return oBoundingBox[gravityDir - 3]
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(matname="material")
     def create_parametric_fin_heat_sink(
         self,
         hs_height=100,
         hs_width=100,
         hs_basethick=10,
         pitch=20,
         thick=10,
@@ -1181,15 +1180,15 @@
         draftangle=0,
         patternangle=10,
         separation=5,
         symmetric=True,
         symmetric_separation=20,
         numcolumn_perside=2,
         vertical_separation=10,
-        matname="Al-Extruded",
+        material="Al-Extruded",
         center=[0, 0, 0],
         plane_enum=0,
         rotation=0,
         tolerance=1e-3,
     ):
         """Create a parametric heat sink.
 
@@ -1219,15 +1218,15 @@
             Whether the heat sink is symmetric. The default is ``True``.
         symmetric_separation : optional
             The default is ``20``.
         numcolumn_perside : int, optional
             Number of columns per side. The default is ``2``.
         vertical_separation : optional
             The default is ``10``.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``Al-Extruded``.
         center : list, optional
            List of ``[x, y, z]`` coordinates for the center of
            the heatsink. The default is ``[0, 0, 0]``.
         plane_enum : str, int, optional
             Plane for orienting the heat sink.
             :class:`pyaedt.constants.PLANE` Enumerator can be used as input.
@@ -1246,15 +1245,15 @@
         --------
         Create a symmetric fin heat sink.
 
         >>> from pyaedt import Icepak
         >>> icepak = Icepak()
         >>> icepak.insert_design("Heat_Sink_Example")
         >>> icepak.create_parametric_fin_heat_sink(draftangle=1.5, patternangle=8, numcolumn_perside=3,
-        ...                                        vertical_separation=5.5, matname="Steel", center=[10, 0, 0],
+        ...                                        vertical_separation=5.5, material="Steel", center=[10, 0, 0],
         ...                                        plane_enum=icepak.PLANE.XY, rotation=45, tolerance=0.005)
 
         """
         warnings.warn(
             "This method is deprecated in 0.7.12. Use the create_parametric_heatsink_on_face() method.",
             DeprecationWarning,
         )
@@ -1270,20 +1269,20 @@
             draft_angle=draftangle,
             pattern_angle=patternangle,
             separation=separation,
             column_separation=vertical_separation,
             symmetric=symmetric,
             symmetric_separation=symmetric_separation,
             numcolumn_perside=numcolumn_perside,
-            matname=matname,
+            material=material,
         )
         rect.delete()
         return bool(hs)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(matname="material")
     def create_parametric_heatsink_on_face(
         self,
         top_face,
         relative=True,
         hs_basethick=0.1,
         fin_thick=0.05,
         fin_length=0.25,
@@ -1291,15 +1290,15 @@
         draft_angle=0,
         pattern_angle=10,
         separation=0.05,
         column_separation=0.05,
         symmetric=True,
         symmetric_separation=0.05,
         numcolumn_perside=2,
-        matname="Al-Extruded",
+        material="Al-Extruded",
     ):
         """Create a parametric heat sink.
 
         Parameters
         ----------
         top_face : modeler.cad.elements3d.FacePrimitive
             Face to build the heatsink on.
@@ -1333,15 +1332,15 @@
         symmetric : bool, optional
             Whether the heat sink is symmetric. The default is ``True``.
         symmetric_separation : optional
             Separation between the two sides. If ``relative==True``, it is the
             fraction of the ``top_face`` height. The default is ``0.01``.
         numcolumn_perside : int, optional
             Number of columns per side. The default is ``2``.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``Al-Extruded``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             Heatsink created or ``False`` when failed.
         dict
@@ -1349,17 +1348,17 @@
             are the corresponding variables names in Icepak.
 
         Examples
         --------
 
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
-        >>> box = ipk.modeler.create_box([0,0,0], [1,2,3])
+        >>> box = ipk.modeler.create_box([0,0,0],[1,2,3])
         >>> top_face=box.top_face_z
-        >>> ipk.create_parametric_heatsink_on_face(top_face, matname="Al-Extruded")
+        >>> ipk.create_parametric_heatsink_on_face(top_face, material="Al-Extruded")
         """
         all_obj = self.modeler.object_names
         center = top_face.center
         normal = top_face.normal
         ref_edge = top_face.edges[0]
         x_vect = [ref_edge.midpoint[i] - center[i] for i in range(3)]
         y_vect = go.v_cross(normal, x_vect)
@@ -1425,15 +1424,15 @@
             else:
                 self[name_map["SymSeparation"]] = self.modeler._arg_with_dim(symmetric_separation)
 
         hs_base = self.modeler.create_box(
             ["-" + name_map["HSWidth"] + "/2", "-" + name_map["HSHeight"] + "/2", "0"],
             [name_map["HSWidth"], name_map["HSHeight"], name_map["HSBaseThick"]],
             generate_unique_name("HSBase"),
-            matname,
+            material,
         )
         fin_line = []
         fin_line.append(self.Position(0, 0, name_map["HSBaseThick"]))
         fin_line.append(self.Position(0, name_map["FinThickness"], name_map["HSBaseThick"]))
         fin_line.append(
             self.Position(
                 name_map["FinLength"],
@@ -1503,15 +1502,15 @@
                 0,
                 "sin(" + name_map["DraftAngle"] + "*3.14/180)*" + name_map["FinThickness"],
                 name_map["FinHeight"] + "+" + name_map["HSBaseThick"],
             )
         )
         fin_top = self.modeler.create_polyline(fin_line2, cover_surface=True, name=generate_unique_name("Fin_top"))
         self.modeler.connect([fin_base.name, fin_top.name])
-        self.modeler[fin_base.name].material_name = matname
+        self.modeler[fin_base.name].material_name = material
         self[name_map["_num"]] = (
             "nint(("
             + name_map["HSWidth"]
             + "+"
             + name_map["FinLength"]
             + "*sin("
             + name_map["PatternAngle"]
@@ -3419,16 +3418,16 @@
         References
         ----------
 
         >>> oModule.AssignNetworkBoundary
 
         Examples
         --------
-        >>> board = icepak.modeler.create_box([0, 0, 0], [50, 100, 2], "board", "copper")
-        >>> box = icepak.modeler.create_box([20, 20, 2], [10, 10, 3], "network_box1", "copper")
+        >>> board = icepak.modeler.create_box([0, 0, 0],[50, 100, 2],"board","copper")
+        >>> box = icepak.modeler.create_box([20, 20, 2],[10, 10, 3],"network_box1","copper")
         >>> network_block = icepak.create_two_resistor_network_block("network_box1", "board", "5W", 2.5, 5)
         >>> network_block.props["Nodes"]["Internal"][0]
         '5W'
         """
 
         def get_face_normal(obj_face):
             vertex1 = obj_face.vertices[0].position
@@ -3441,15 +3440,15 @@
             return normalized_n
 
         net_handle = self.modeler.get_object_from_name(object_name)
         if pcb in self.modeler.user_defined_component_names:
             part_names = sorted(
                 [
                     pcb_layer
-                    for pcb_layer in self.modeler.get_3d_component_object_list(componentname=pcb)
+                    for pcb_layer in self.modeler.get_3d_component_object_list(name=pcb)
                     if re.search(self.modeler.user_defined_components[pcb].definition_name + r"_\d\d\d.*", pcb_layer)
                 ]
             )
 
             pcb_layers = [part_names[0], part_names[-1]]
             for layer in pcb_layers:
                 x = self.modeler.get_object_from_name(object_name).get_touching_faces(layer)
@@ -4181,15 +4180,15 @@
         >>> oModule.AssignSourceBoundary
 
         Examples
         --------
 
         >>> from pyaedt import Icepak
         >>> app = Icepak()
-        >>> box = app.modeler.create_box([0, 0, 0], [20, 20, 20], name="box")
+        >>> box = app.modeler.create_box([0, 0, 0],[20, 20, 20],name="box")
         >>> ds = app.create_dataset1d_design("Test_DataSet", [1, 2, 3], [3, 4, 5])
         >>> app.solution_type = "Transient"
         >>> b = app.assign_source("box", "Total Power", assignment_value={"Type": "Temp Dep",
         ... "Function": "Piecewise Linear", "Values": "Test_DataSet"})
 
         """
         default_values = {"Total Power": "0W", "Surface Heat": "0irrad_W_per_m2", "Temperature": "AmbientTemp"}
@@ -4326,15 +4325,15 @@
         >>> oModule.AssignNetworkBoundary
 
         Examples
         --------
 
         >>> from pyaedt import Icepak
         >>> app = Icepak()
-        >>> box = app.modeler.create_box([0, 0, 0], [20, 50, 80])
+        >>> box = app.modeler.create_box([0, 0, 0],[20, 50, 80])
         >>> faces_ids = [face.id for face in box.faces][0, 1]
         >>> sources_power = [3, "4mW"]
         >>> matrix = [[0, 0, 0, 0],
         >>>           [1, 0, 0, 0],
         >>>           [0, 3, 0, 0],
         >>>           [1, 2, 4, 0]]
         >>> boundary = app.assign_resistor_network_from_matrix(sources_power, faces_ids, matrix)
@@ -4409,15 +4408,15 @@
         >>> oModule.AssignBlockBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
-        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox3", "copper")
+        >>> box = ipk.modeler.create_box([5, 5, 5],[1, 2, 3],"BlockBox3","copper")
         >>> power_dict = {"Type": "Transient", "Function": "Sinusoidal", "Values": ["0W", 1, 1, "1s"]}
         >>> block = ipk.assign_solid_block("BlockBox3", power_dict)
 
         """
         if ext_temperature != "AmbientTemp" and ext_temperature is not None and not htc:
             self.logger.add_error_message("Set an argument for ``htc`` or remove the ``ext_temperature`` argument.")
             return None
@@ -4519,15 +4518,15 @@
         >>> oModule.AssignBlockBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
-        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBox5", "copper")
+        >>> box = ipk.modeler.create_box([5, 5, 5],[1, 2, 3],"BlockBox5","copper")
         >>> box.solve_inside = False
         >>> temp_dict = {"Type": "Transient", "Function": "Square Wave", "Values": ["1cel", "0s", "1s", "0.5s", "0cel"]}
         >>> block = ipk.assign_hollow_block("BlockBox5", "Heat Transfer Coefficient", "1w_per_m2kel", "Test", temp_dict)
 
         """
         if assignment_value == "Joule Heating" and assignment_type != "Total Power":
             self.logger.add_error_message(
@@ -5101,15 +5100,15 @@
 
         >>> oModule.AssignAdiabaticPlateBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
-        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "Box", "copper")
+        >>> box = ipk.modeler.create_box([5, 5, 5],[1, 2, 3],"Box","copper")
         >>> ad_plate = ipk.assign_adiabatic_plate(box.top_face_x, None, {"RadiateTo": "AllObjects"})
 
         """
         if not isinstance(assignment, list):
             assignment = [assignment]
         if isinstance(assignment[0], str):
             key = "Objects"
@@ -5555,15 +5554,15 @@
         >>> oModule.AssignRecircBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
         >>> ipk.solution_type = "Transient"
-        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBoxEmpty", "copper")
+        >>> box = ipk.modeler.create_box([5, 5, 5],[1, 2, 3],"BlockBoxEmpty","copper")
         >>> box.solve_inside = False
         >>> recirc = ipk.assign_recirculation_opening([box.top_face_x, box.bottom_face_x], box.top_face_x,
         >>>                                          flow_assignment="10kg_per_s_m2")
 
         """
         if not len(face_list) == 2:
             self.logger.error("Recirculation boundary condition must be assigned to two faces.")
@@ -5696,15 +5695,15 @@
 
         >>> oModule.AssignBlowerBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
-        >>> cylinder = self.aedtapp.modeler.create_cylinder(cs_axis="X", position=[0,0,0], radius=10, height=1)
+        >>> cylinder = self.aedtapp.modeler.create_cylinder(orientation="X",origin=[0,0,0],radius=10,height=1)
         >>> curved_face = [f for f in cylinder.faces if not f.is_planar]
         >>> planar_faces = [f for f in cylinder.faces if f.is_planar]
         >>> cylinder.solve_inside=False
         >>> blower = self.aedtapp.assign_blower_type1([f.id for f in curved_face+planar_faces],
         >>>                                           [f.id for f in planar_faces], [10, 5, 0], [0, 2, 4])
 
         """
@@ -5761,15 +5760,15 @@
 
         >>> oModule.AssignBlowerBoundary
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> ipk = Icepak()
-        >>> box = ipk.modeler.create_box([5, 5, 5], [1, 2, 3], "BlockBoxEmpty", "copper")
+        >>> box = ipk.modeler.create_box([5, 5, 5],[1, 2, 3],"BlockBoxEmpty","copper")
         >>> box.solve_inside=False
         >>> blower = self.aedtapp.assign_blower_type2([box.faces[0], box.faces[1]],
         >>>                                           [box.faces[0]], [10, 5, 0], [0, 2, 4])
 
         """
         props = {}
         props["Exhaust Exit Angle"] = exhaust_angle
```

### Comparing `pyaedt-0.8.8/pyaedt/maxwell.py` & `pyaedt-0.8.9/pyaedt/maxwell.py`

 * *Files 0% similar despite different names*

```diff
@@ -688,15 +688,15 @@
         >>> oModule.AssignCurrent
 
         Examples
         --------
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d(solution_type="ElectroDCConduction")
-        >>> cylinder= m3d.modeler.create_cylinder("X", [0,0,0],10, 100, 250)
+        >>> cylinder= m3d.modeler.create_cylinder("X",[0,0,0],10,100,250)
         >>> current = m3d.assign_current(cylinder.top_face_x.id,amplitude="2mA")
         >>> m3d.release_desktop(True, True)
         """
 
         if isinstance(amplitude, (int, float)):
             amplitude = str(amplitude) + "A"
 
@@ -1245,24 +1245,24 @@
         Examples
         --------
 
         Assign virtual force to a magnetic object:
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> iron_object = m3d.modeler.create_box([0, 0, 0], [2, 10, 10], name="iron")
-        >>> magnet_object = m3d.modeler.create_box([10, 0, 0], [2, 10, 10], name="magnet")
+        >>> iron_object = m3d.modeler.create_box([0, 0, 0],[2, 10, 10],name="iron")
+        >>> magnet_object = m3d.modeler.create_box([10, 0, 0],[2, 10, 10],name="magnet")
         >>> m3d.assign_material(iron_object, "iron")
         >>> m3d.assign_material(magnet_object, "NdFe30")
         >>> m3d.assign_force("iron",is_virtual=True,force_name="force_iron")
 
         Assign Lorentz force to a conductor:
 
-        >>> conductor1 = m3d.modeler.create_box([0, 0, 0], [1, 1, 10], name="conductor1")
-        >>> conductor2 = m3d.modeler.create_box([10, 0, 0], [1, 1, 10], name="conductor2")
+        >>> conductor1 = m3d.modeler.create_box([0, 0, 0],[1, 1, 10],name="conductor1")
+        >>> conductor2 = m3d.modeler.create_box([10, 0, 0],[1, 1, 10],name="conductor2")
         >>> m3d.assign_material(conductor1, "copper")
         >>> m3d.assign_material(conductor2, "copper")
         >>> m3d.assign_force("conductor1",is_virtual=False,force_name="force_copper") # conductor, use Lorentz force
         >>> m3d.release_desktop(True, True)
         """
         if self.solution_type not in ["ACConduction", "DCConduction"]:
             assignment = self.modeler.convert_to_selections(assignment, True)
@@ -1670,16 +1670,16 @@
         Examples
         --------
 
         Assign radiation boundary to one box and one face:
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> box1 = m3d.modeler.create_box([0, 0, 0], [2, 10, 10])
-        >>> box2 = m3d.modeler.create_box([10, 0, 0], [2, 10, 10])
+        >>> box1 = m3d.modeler.create_box([0, 0, 0],[2, 10, 10])
+        >>> box2 = m3d.modeler.create_box([10, 0, 0],[2, 10, 10])
         >>> m3d.assign_radiation([box1, box2.faces[0]])
         >>> m3d.release_desktop(True, True)
         """
 
         if self.solution_type in ["EddyCurrent"]:
             if not radiation:
                 radiation = generate_unique_name("Radiation")
@@ -2166,24 +2166,26 @@
         Examples
         --------
 
         Create a box and assign insulating boundary to it.
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> insulated_box = m3d.modeler.create_box([50, 0, 50], [294, 294, 19], name="InsulatedBox")
+        >>> insulated_box = m3d.modeler.create_box([50, 0, 50],[294, 294, 19],name="InsulatedBox")
         >>> insulating_assignment = m3d.assign_insulating(assignment=insulated_box,insulation="InsulatingExample")
         >>> m3d.release_desktop(True, True)
         """
 
         if self.solution_type in [
+            "Magnetostatic",
             "EddyCurrent",
             "Transient",
             "TransientAPhiFormulation",
             "DCConduction",
+            "ACConduction",
             "ElectroDCConduction",
         ]:
             if not insulation:
                 insulation = generate_unique_name("Insulation")
             elif insulation in self.modeler.get_boundaries_name():
                 insulation = generate_unique_name(insulation)
 
@@ -2243,15 +2245,15 @@
         Examples
         --------
 
         Create a box and assign impedance boundary to the faces.
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> shield = m3d.modeler.create_box([-50, -50, -50], [294, 294, 19], name="shield")
+        >>> shield = m3d.modeler.create_box([-50, -50, -50],[294, 294, 19],name="shield")
         >>> shield_faces = m3d.modeler.select_allfaces_fromobjects(["shield"])
         >>> impedance_assignment = m3d.assign_impedance(assignment=shield_faces,impedance="ShieldImpedance")
         >>> m3d.release_desktop(True, True)
         """
 
         if self.solution_type in [
             "EddyCurrent",
@@ -2534,15 +2536,15 @@
         Examples
         --------
 
         Create a box and assign a flux tangential boundary to one of its faces.
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> box = m3d.modeler.create_box([50, 0, 50], [294, 294, 19], name="Box")
+        >>> box = m3d.modeler.create_box([50, 0, 50],[294, 294, 19],name="Box")
         >>> flux_tangential = m3d.assign_flux_tangential(box.faces[0],"FluxExample")
         >>> m3d.release_desktop(True, True)
         """
         if self.solution_type != "TransientAPhiFormulation":
             self.logger.error("Flux tangential boundary can only be assigned to a transient APhi solution type.")
             return False
```

### Comparing `pyaedt-0.8.8/pyaedt/maxwellcircuit.py` & `pyaedt-0.8.9/pyaedt/maxwellcircuit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/mechanical.py` & `pyaedt-0.8.9/pyaedt/mechanical.py`

 * *Files 10% similar despite different names*

```diff
@@ -335,36 +335,36 @@
         if bound.create():
             self._boundaries[bound.name] = bound
             self.logger.info("Thermal conditions are mapped from design %s.", design)
             return bound
 
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
     def assign_uniform_convection(
         self,
-        objects_list,
+        assignment,
         convection_value=1.0,
         convection_unit="w_per_m2kel",
         temperature="AmbientTemp",
-        boundary_name="",
+        name="",
     ):
         """Assign a uniform convection to the face list.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of objects, faces, or both.
         convection_value : float, optional
             Convection value. The default is ``"1.0"``.
         convection_unit : str, optional
             Units for the convection value. The default is ``"w_per_m2kel"``.
         temperature : str, optional
             Temperature. The default is ``"AmbientTemp"``.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``, in which case the default
             name is used.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
@@ -373,48 +373,48 @@
         ----------
 
         >>> oModule.AssignConvection
         """
         assert "Thermal" in self.solution_type, "This method works only in a Mechanical Thermal analysis."
 
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
 
-        if isinstance(objects_list, list):
-            if isinstance(objects_list[0], str):
-                props["Objects"] = objects_list
+        if isinstance(assignment, list):
+            if isinstance(assignment[0], str):
+                props["Objects"] = assignment
             else:
-                props["Faces"] = objects_list
+                props["Faces"] = assignment
 
         props["Temperature"] = temperature
         props["Uniform"] = True
         props["FilmCoeff"] = str(convection_value) + convection_unit
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("Convection")
-        bound = BoundaryObject(self, boundary_name, props, "Convection")
+        if not name:
+            name = generate_unique_name("Convection")
+        bound = BoundaryObject(self, name, props, "Convection")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_uniform_temperature(self, objects_list, temperature="AmbientTemp", boundary_name=""):
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
+    def assign_uniform_temperature(self, assignment, temperature="AmbientTemp", name=""):
         """Assign a uniform temperature boundary.
 
         .. note::
             This method works only in a Mechanical Thermal analysis.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of objects, faces, or both.
         temperature : str, optional.
             Type of the temperature. The default is ``"AmbientTemp"``.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
 
@@ -422,44 +422,44 @@
         ----------
 
         >>> oModule.AssignTemperature
         """
         assert "Thermal" in self.solution_type, "This method works only in a Mechanical Thermal analysis."
 
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
 
-        if isinstance(objects_list, list):
-            if isinstance(objects_list[0], str):
-                props["Objects"] = objects_list
+        if isinstance(assignment, list):
+            if isinstance(assignment[0], str):
+                props["Objects"] = assignment
             else:
-                props["Faces"] = objects_list
+                props["Faces"] = assignment
 
         props["Temperature"] = temperature
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("Temp")
-        bound = BoundaryObject(self, boundary_name, props, "Temperature")
+        if not name:
+            name = generate_unique_name("Temp")
+        bound = BoundaryObject(self, name, props, "Temperature")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_frictionless_support(self, objects_list, boundary_name=""):
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
+    def assign_frictionless_support(self, assignment, name=""):
         """Assign a Mechanical frictionless support.
 
         .. note::
             This method works only in a Mechanical Structural analysis.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of faces to apply to the frictionless support.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``, in which case the
             default name is used.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
@@ -470,42 +470,42 @@
         >>> oModule.AssignFrictionlessSupport
         """
 
         if not (self.solution_type == "Structural" or "Modal" in self.solution_type):
             self.logger.error("This method works only in Mechanical Structural analysis.")
             return False
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
 
-        if type(objects_list) is list:
-            if type(objects_list[0]) is str:
-                props["Objects"] = objects_list
+        if type(assignment) is list:
+            if type(assignment[0]) is str:
+                props["Objects"] = assignment
             else:
-                props["Faces"] = objects_list
+                props["Faces"] = assignment
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("Temp")
-        bound = BoundaryObject(self, boundary_name, props, "Frictionless")
+        if not name:
+            name = generate_unique_name("Temp")
+        bound = BoundaryObject(self, name, props, "Frictionless")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_fixed_support(self, objects_list, boundary_name=""):
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
+    def assign_fixed_support(self, assignment, name=""):
         """Assign a Mechanical fixed support.
 
         .. note::
            This method works only in a Mechanical Structural analysis.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of faces to apply to the fixed support.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``, in which case
             the default name is used.
 
         Returns
         -------
         aedt.modules.Boundary.Boundary
             Boundary object.
@@ -515,22 +515,22 @@
 
         >>> oModule.AssignFixedSupport
         """
         if not (self.solution_type == "Structural" or "Modal" in self.solution_type):
             self.logger.error("This method works only in a Mechanical Structural analysis.")
             return False
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
 
-        if type(objects_list) is list:
-            props["Faces"] = objects_list
+        if type(assignment) is list:
+            props["Faces"] = assignment
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("Temp")
-        bound = BoundaryObject(self, boundary_name, props, "FixedSupport")
+        if not name:
+            name = generate_unique_name("Temp")
+        bound = BoundaryObject(self, name, props, "FixedSupport")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
     @property
     def existing_analysis_sweeps(self):
@@ -548,27 +548,27 @@
         """
         setup_list = self.existing_analysis_setups
         sweep_list = []
         for el in setup_list:
             sweep_list.append(el + " : Solution")
         return sweep_list
 
-    @pyaedt_function_handler()
-    def assign_heat_flux(self, objects_list, heat_flux_type, value, boundary_name=""):
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
+    def assign_heat_flux(self, assignment, heat_flux_type, value, name=""):
         """Assign heat flux boundary condition to an object or face list.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of objects, faces, or both.
         heat_flux_type : str
             Type of the heat flux. Options are ``"Total Power"`` or ``"Surface Flux"``.
         value : str
             Value of heat flux with units.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``, in which case the default
             name is used.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
@@ -577,46 +577,46 @@
         ----------
 
         >>> oModule.AssignHeatFlux
         """
         assert "Thermal" in self.solution_type, "This method works only in a Mechanical Thermal analysis."
 
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
-        if type(objects_list) is list:
-            if type(objects_list[0]) is str:
-                props["Objects"] = objects_list
+        assignment = self.modeler.convert_to_selections(assignment, True)
+        if type(assignment) is list:
+            if type(assignment[0]) is str:
+                props["Objects"] = assignment
             else:
-                props["Faces"] = objects_list
+                props["Faces"] = assignment
 
         if heat_flux_type == "Total Power":
             props["TotalPower"] = value
         else:
             props["SurfaceFlux"] = value
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("HeatFlux")
+        if not name:
+            name = generate_unique_name("HeatFlux")
 
-        bound = BoundaryObject(self, boundary_name, props, "HeatFlux")
+        bound = BoundaryObject(self, name, props, "HeatFlux")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_heat_generation(self, objects_list, value, boundary_name=""):
+    @pyaedt_function_handler(objects_list="assignment", boundary_name="name")
+    def assign_heat_generation(self, assignment, value, name=""):
         """Assign a heat generation boundary condition to an object list.
 
         Parameters
         ----------
-        objects_list : list
+        assignment : list
             List of objects.
         value : str
             Value of heat generation with units.
-        boundary_name : str, optional
+        name : str, optional
             Name of the boundary. The default is ``""``, in which case the default
             name is used.
 
         Returns
         -------
         :class:`aedt.modules.Boundary.Boundary object`
             Boundary object.
@@ -625,24 +625,24 @@
         ----------
 
         >>> oModule.AssignHeatGeneration
         """
         assert "Thermal" in self.solution_type, "This method works only in a Mechanical Thermal analysis."
 
         props = {}
-        objects_list = self.modeler.convert_to_selections(objects_list, True)
-        if type(objects_list) is list:
-            props["Objects"] = objects_list
+        assignment = self.modeler.convert_to_selections(assignment, True)
+        if type(assignment) is list:
+            props["Objects"] = assignment
 
         props["TotalPower"] = value
 
-        if not boundary_name:
-            boundary_name = generate_unique_name("HeatGeneration")
+        if not name:
+            name = generate_unique_name("HeatGeneration")
 
-        bound = BoundaryObject(self, boundary_name, props, "HeatGeneration")
+        bound = BoundaryObject(self, name, props, "HeatGeneration")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler(setupname="name", setuptype="setup_type")
     def create_setup(self, name="MySetupAuto", setup_type=None, **kwargs):
```

### Comparing `pyaedt-0.8.8/pyaedt/misc/Console.py_build` & `pyaedt-0.8.9/pyaedt/misc/Console.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/Job_Settings.areg` & `pyaedt-0.8.9/pyaedt/misc/Job_Settings.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/Jupyter.py_build` & `pyaedt-0.8.9/pyaedt/misc/Jupyter.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/Run_PyAEDT_Script.py_build` & `pyaedt-0.8.9/pyaedt/misc/Run_PyAEDT_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build` & `pyaedt-0.8.9/pyaedt/misc/Run_PyAEDT_Toolkit_Script.py_build`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/aedtlib_personalib_install.py` & `pyaedt-0.8.9/pyaedt/misc/aedtlib_personalib_install.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/amat.xml` & `pyaedt-0.8.9/pyaedt/misc/amat.xml`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/ansys_cloud.areg` & `pyaedt-0.8.9/pyaedt/misc/ansys_cloud.areg`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/config.schema.json` & `pyaedt-0.8.9/pyaedt/misc/config.schema.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/console_setup.py` & `pyaedt-0.8.9/pyaedt/misc/console_setup.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/images/gallery/PyAEDT.png` & `pyaedt-0.8.9/pyaedt/misc/images/gallery/PyAEDT.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/images/large/pyansys.png` & `pyaedt-0.8.9/pyaedt/misc/images/large/pyansys.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/install_extra_toolkits.py` & `pyaedt-0.8.9/pyaedt/misc/install_extra_toolkits.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/jupyter_template.ipynb` & `pyaedt-0.8.9/pyaedt/misc/jupyter_template.ipynb`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/misc.py` & `pyaedt-0.8.9/pyaedt/misc/misc.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json` & `pyaedt-0.8.9/pyaedt/misc/ml_data_file_train_100MHz_1GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json` & `pyaedt-0.8.9/pyaedt/misc/ml_data_file_train_1GHz_10GHz.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib` & `pyaedt-0.8.9/pyaedt/misc/patch_svr_model_100MHz_1GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib` & `pyaedt-0.8.9/pyaedt/misc/patch_svr_model_1GHz_10GHz.joblib`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/pyaedt_local_config.acf` & `pyaedt-0.8.9/pyaedt/misc/pyaedt_local_config.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/pyansys-logo-black-cropped.png` & `pyaedt-0.8.9/pyaedt/misc/pyansys-logo-black-cropped.png`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json` & `pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_120d_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_93_8.json` & `pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_93_8.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_94_17.json` & `pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_94_17.json`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_parameters.py` & `pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_parameters.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py` & `pyaedt-0.8.9/pyaedt/misc/spisim_com_configuration_files/com_settings_mapping.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/misc/template.acf` & `pyaedt-0.8.9/pyaedt/misc/template.acf`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/advanced_cad/actors.py` & `pyaedt-0.8.9/pyaedt/modeler/advanced_cad/actors.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/advanced_cad/multiparts.py` & `pyaedt-0.8.9/pyaedt/modeler/advanced_cad/multiparts.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/advanced_cad/oms.py` & `pyaedt-0.8.9/pyaedt/modeler/advanced_cad/oms.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/advanced_cad/parts.py` & `pyaedt-0.8.9/pyaedt/modeler/advanced_cad/parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -408,18 +408,18 @@
         str
             Name of inserted object.
         """
         aedt_objects = []
         # TODO: Why the inconsistent syntax for cs commands?
         if self._do_offset:
             self.set_relative_cs(app)  # Create coordinate system, if needed.
-            comp_obj = app.modeler.insert_3d_component(self.file_name, targetCS=self.cs_name)
+            comp_obj = app.modeler.insert_3d_component(self.file_name, coordinate_system=self.cs_name)
             aedt_objects.append(comp_obj.name)
         else:
-            comp_obj = app.modeler.insert_3d_component(self.file_name, targetCS=self._multiparts.cs_name)
+            comp_obj = app.modeler.insert_3d_component(self.file_name, coordinate_system=self._multiparts.cs_name)
             aedt_objects.append(comp_obj.name)
         if self._do_rotate:
             self.do_rotate(app, aedt_objects[0])
 
         # Duplication occurs in parent coordinate system.
         app.modeler.set_working_coordinate_system(self._multiparts.cs_name)
         if self["duplicate_vector"]:
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/advanced_cad/stackup_3d.py` & `pyaedt-0.8.9/pyaedt/modeler/advanced_cad/stackup_3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -307,16 +307,15 @@
 
     Examples
     --------
     >>> from pyaedt import Hfss
     >>> from pyaedt.modeler.advanced_cad.stackup_3d import Stackup3D
     >>> hfss = Hfss()
     >>> my_stackup = Stackup3D(hfss, 2.5e9)
-    >>> my_layer = my_stackup.add_layer("my_layer", layer_type="D", material_name="air",
-    >>> thickness=3, fill_material=None)
+    >>> my_layer = my_stackup.add_layer("my_layer")
     >>> gnd = my_stackup.add_ground_layer("gnd")
     >>> diel = my_stackup.add_dielectric_layer("diel1", thickness=1.5, material="Duroid (tm)")
     >>> top = my_stackup.add_signal_layer("top")
 
     """
 
     def __init__(
@@ -362,23 +361,23 @@
         else:
             self._thickness = None
         if self._layer_type == "dielectric":
             obj_3d = self._app.modeler.create_box(
                 ["dielectric_x_position", "dielectric_y_position", layer_position],
                 ["dielectric_length", "dielectric_width", self._thickness_variable],
                 name=self._name,
-                matname=self.material_name,
+                material=self.material_name,
             )
         elif self._layer_type == "ground":
             if thickness:
                 obj_3d = self._app.modeler.create_box(
                     ["dielectric_x_position", "dielectric_y_position", layer_position],
                     ["dielectric_length", "dielectric_width", self._thickness_variable],
                     name=self._name,
-                    matname=self.material_name,
+                    material=self.material_name,
                 )
 
             else:
                 obj_3d = self._app.modeler.create_rectangle(
                     constants.PLANE.XY,
                     ["dielectric_x_position", "dielectric_y_position", layer_position],
                     ["dielectric_length", "dielectric_width"],
@@ -387,15 +386,15 @@
                 )
         elif self._layer_type == "signal":
             if thickness:
                 obj_3d = self._app.modeler.create_box(
                     ["dielectric_x_position", "dielectric_y_position", layer_position],
                     ["dielectric_length", "dielectric_width", self._thickness_variable],
                     name=self._name,
-                    matname=self._fill_material.name,
+                    material=self._fill_material.name,
                 )
             else:
                 obj_3d = self._app.modeler.create_rectangle(
                     constants.PLANE.XY,
                     ["dielectric_x_position", "dielectric_y_position", layer_position],
                     ["dielectric_length", "dielectric_width"],
                     name=self._name,
@@ -594,15 +593,15 @@
             cloned_material_name = cloned_material_name.name
         if not cloned_material_name:  # If a name has not been defined, create one.
             cloned_material_name = "cloned_" + material_name
         for duplicated_material in self._stackup.duplicated_material_list:  # If the new material exists, don't
             if duplicated_material.name == cloned_material_name:  # return that material.
                 return duplicated_material
         duplicated_material = self._app.materials.duplicate_material(
-            material_name, cloned_material_name, props=list_of_properties
+            material_name, cloned_material_name, properties=list_of_properties
         )
         #        duplicated_material = DuplicatedParametrizedMaterial(
         #            application, material_name, cloned_material_name, list_of_properties
         #        )
         self._stackup.duplicated_material_list.append(duplicated_material)
         return duplicated_material
 
@@ -1172,39 +1171,39 @@
                 if v._pad_radius > 0:
                     cyls.append(
                         self._app.modeler.create_cylinder(
                             "Z",
                             [position_x, position_y, v._layer_elevation.name],
                             v._pad_radius,
                             v._layer_thickness.name,
-                            matname=self._padstacks_material,
+                            num_sides=self._num_sides,
                             name=instance_name,
-                            numSides=self._num_sides,
+                            material=self._padstacks_material,
                         )
                     )
                     if self.plating_ratio < 1:
                         hole = self._app.modeler.create_cylinder(
                             "Z",
                             [position_x, position_y, v._layer_elevation.name],
                             "{}*{}".format(self._app.modeler._arg_with_dim(v._pad_radius), 1 - self.plating_ratio),
                             v._layer_thickness.name,
-                            matname=self._padstacks_material,
+                            num_sides=self._num_sides,
                             name=instance_name,
-                            numSides=self._num_sides,
+                            material=self._padstacks_material,
                         )
                         cyls[-1].subtract(hole, False)
                 if v._antipad_radius > 0:
                     anti = self._app.modeler.create_cylinder(
                         "Z",
                         [position_x, position_y, v._layer_elevation.name],
                         v._antipad_radius,
                         v._layer_thickness.name,
-                        matname="air",
+                        num_sides=self._num_sides,
                         name=instance_name + "_antipad",
-                        numSides=self._num_sides,
+                        material="air",
                     )
                     self._app.modeler.subtract(
                         self._stackup._signal_list + self._stackup._ground_list + self._stackup._dielectric_list,
                         anti,
                         False,
                     )
             if len(cyls) > 1:
@@ -1549,16 +1548,15 @@
         Examples
         --------
 
         >>> from pyaedt import Hfss
         >>> from pyaedt.modeler.stackup_3d import Stackup3D
         >>> hfss = Hfss()
         >>> my_stackup = Stackup3D(hfss, 2.5e9)
-        >>> my_layer = my_stackup.add_layer("my_layer", layer_type="D", material_name="air",
-        >>> thickness=3, fill_material=None)
+        >>> my_layer = my_stackup.add_layer("my_layer")
 
         """
         self._shifted_index += 1
         if not layer_type:
             raise ValueError("Layer type has to be an S, D, or G string.")
         self._layer_name.append(name)  # update the list of layer names.
 
@@ -1991,15 +1989,15 @@
     >>> stackup = Stackup3D(hfss)
     >>> gnd = stackup.add_ground_layer("ground", material="copper", thickness=0.035, fill_material="air")
     >>> dielectric = stackup.add_dielectric_layer("dielectric", thickness="0.5" + length_units, material="Duroid (tm)")
     >>> signal = stackup.add_signal_layer("signal", material="copper", thickness=0.035, fill_material="air")
     >>> patch = signal.add_patch(patch_length=9.57, patch_width=9.25, patch_name="Patch")
     >>> stackup.resize_around_element(patch)
     >>> pad_length = [3, 3, 3, 3, 3, 3]  # Air bounding box buffer in mm.
-    >>> region = hfss.modeler.create_region(pad_length, is_percentage=False)
+    >>> region = hfss.modeler.create_region(pad_length,is_percentage=False)
     >>> hfss.assign_radiation_boundary_to_objects(region)
     >>> patch.create_probe_port(gnd, rel_x_offset=0.485)
 
     """
 
     def __init__(
         self,
@@ -2091,29 +2089,29 @@
             else:
                 start_point = ["-{}_width/2".format(patch_name), 0, 0]
             application.modeler.set_working_coordinate_system(patch_name + "_CS")
 
             self._reference_system = patch_name + "_CS"
         if signal_layer.thickness:
             self._aedt_object = application.modeler.create_box(
-                position=start_point,
-                dimensions_list=[
+                origin=start_point,
+                sizes=[
                     "{}_length".format(patch_name),
                     "{}_width".format(patch_name),
                     signal_layer.thickness.name,
                 ],
                 name=patch_name,
-                matname=signal_layer.material_name,
+                material=signal_layer.material_name,
             )
         else:
             self._aedt_object = application.modeler.create_rectangle(
-                position=start_point,
-                dimension_list=[self.length.name, self.width.name],
+                origin=start_point,
+                sizes=[self.length.name, self.width.name],
                 name=patch_name,
-                matname=signal_layer.material_name,
+                material=signal_layer.material_name,
             )
             application.assign_coating(self._aedt_object.name, signal_layer.material)
         application.modeler.set_working_coordinate_system("Global")
         application.modeler.subtract(blank_list=[signal_layer.name], tool_list=[patch_name], keep_originals=True)
 
     @property
     def frequency(self):
@@ -2422,26 +2420,31 @@
             + reference_layer.elevation.name
             + " - "
             + reference_layer.thickness.name
         )
         z_ref = reference_layer.elevation.name + " + " + reference_layer.thickness.name
         probe_pos = [x_probe, y_probe, z_ref]  # Probe base position.
         probe_wire = self.application.modeler.create_cylinder(
-            cs_axis="Z", position=probe_pos, radius=r, height=probe_height, name=name, matname="copper"
+            orientation="Z", origin=probe_pos, radius=r, height=probe_height, name=name, material="copper"
         )
         probe_feed_wire = self.application.modeler.create_cylinder(
-            cs_axis="Z", position=probe_pos, radius=r, height=-feed_length, name=name + "_feed_wire", matname="copper"
+            orientation="Z",
+            origin=probe_pos,
+            radius=r,
+            height=-feed_length,
+            name=name + "_feed_wire",
+            material="copper",
         )
         probe_feed_outer = self.application.modeler.create_cylinder(
-            cs_axis="Z",
-            position=probe_pos,
+            orientation="Z",
+            origin=probe_pos,
             radius=probe_or,
             height=-feed_length,
             name=name + "_feed_outer",
-            matname="vacuum",
+            material="vacuum",
         )
 
         # Probe extends through the ground plane.
         self.application.modeler.subtract(reference_layer.name, probe_feed_outer.name)
 
         # Find face on probe with max area. This is the outer ground and will be assigned PEC.
         areas = [f.area for f in probe_feed_outer.faces]
@@ -2498,19 +2501,19 @@
             self._signal_layer.elevation.name
             + " + "
             + self._signal_layer.thickness.name
             + " - "
             + reference_layer.elevation.name
         )
         rect = self.application.modeler.create_rectangle(
-            csPlane=constants.PLANE.YZ,
-            position=[string_position_x, string_position_y, string_position_z],
-            dimension_list=[string_width, string_length],
+            orientation=constants.PLANE.YZ,
+            origin=[string_position_x, string_position_y, string_position_z],
+            sizes=[string_width, string_length],
             name=self.name + "_port",
-            matname=None,
+            material=None,
         )
         if self.application.solution_type == "Modal":
             if axisdir is None:
                 axisdir = self.application.AxisDir.ZPos
             port = self.application.lumped_port(rect.name, integration_line=axisdir, name=port_name)
         elif self.application.solution_type == "Terminal":
             port = self.application.lumped_port(rect.name, reference=[reference_layer.name], name=port_name)
@@ -2760,29 +2763,29 @@
             if axis == "X":
                 start_point = [0, "-" + self.width.name + "/2", 0]
             else:
                 start_point = ["-" + self.width.name + "/2", 0, 0]
             self._reference_system = line_name + "_CS"
         if signal_layer.thickness:
             self._aedt_object = application.modeler.create_box(
-                position=start_point,
-                dimensions_list=[
+                origin=start_point,
+                sizes=[
                     "{}_length".format(self._name),
                     self.width.name,
                     signal_layer.thickness.name,
                 ],
                 name=line_name,
-                matname=signal_layer.material_name,
+                material=signal_layer.material_name,
             )
         else:
             self._aedt_object = application.modeler.create_rectangle(
-                position=start_point,
-                dimension_list=["{}_length".format(self._name), self.width.name],
+                oring=start_point,
+                sizes=["{}_length".format(self._name), self.width.name],
                 name=line_name,
-                matname=signal_layer.material_name,
+                material=signal_layer.material_name,
             )
         application.modeler.set_working_coordinate_system("Global")
         application.modeler.subtract(blank_list=[signal_layer.name], tool_list=[line_name], keep_originals=True)
 
     @property
     def frequency(self):
         """Frequency.
@@ -3238,19 +3241,19 @@
             self._signal_layer.elevation.name
             + " + "
             + self._signal_layer.thickness.name
             + " - "
             + reference_layer.elevation.name
         )
         port = self.application.modeler.create_rectangle(
-            csPlane=constants.PLANE.YZ,
-            position=[string_position_x, string_position_y, string_position_z],
-            dimension_list=[string_width, string_length],
+            orientation=constants.PLANE.YZ,
+            origin=[string_position_x, string_position_y, string_position_z],
+            sizes=[string_width, string_length],
             name=self.name + "_port",
-            matname=None,
+            material=None,
         )
         if self.application.solution_type == "Modal":
             if axisdir is None:
                 axisdir = self.application.AxisDir.ZPos
             port = self.application.lumped_port(
                 signal=port.name, name=port_name, integration_line=axisdir, create_port_sheet=False
             )
@@ -3338,15 +3341,15 @@
             application.modeler.create_coordinate_system(
                 origin=[0, 0, 0], reference_cs="Global", name=poly_name + "_CS"
             )
             application.modeler.set_working_coordinate_system(poly_name + "_CS")
 
             self._reference_system = poly_name + "_CS"
         self._aedt_object = application.modeler.create_polyline(
-            position_list=pts, name=poly_name, matname=mat_name, cover_surface=True
+            points=pts, cover_surface=True, name=poly_name, material=mat_name
         )
         if self._thickness:
             application.modeler.sweep_along_vector(
                 self._aedt_object, [0, 0, self._thickness.name], draft_type="Natural"
             )
         application.modeler.set_working_coordinate_system("Global")
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/Modeler.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/Modeler.py`

 * *Files 1% similar despite different names*

```diff
@@ -334,31 +334,31 @@
         list
             List of changed properties of the coordinate system.
 
         """
         arguments = ["NAME:AllTabs", ["NAME:Geometry3DCSTab", ["NAME:PropServers", name], arg]]
         self._modeler.oeditor.ChangeProperty(arguments)
 
-    @pyaedt_function_handler()
-    def rename(self, newname):
+    @pyaedt_function_handler(newname="name")
+    def rename(self, name):
         """Rename the coordinate system.
 
         Parameters
         ----------
-        newname : str
+        name : str
             New name for the coordinate system.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        self._change_property(self.name, ["NAME:ChangedProps", ["NAME:Name", "Value:=", newname]])
-        self.name = newname
+        self._change_property(self.name, ["NAME:ChangedProps", ["NAME:Name", "Value:=", name]])
+        self.name = name
         return True
 
     @pyaedt_function_handler()
     def delete(self):
         """Delete the coordinate system.
 
         Returns
@@ -450,25 +450,25 @@
 
     @property
     def _attributes(self):
         """Internal named array for attributes of the face coordinate system."""
         coordinateSystemAttributes = ["NAME:Attributes", "Name:=", self.name, "PartName:=", self._part_name]
         return coordinateSystemAttributes
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(face="assignment")
     def create(
-        self, face, origin, axis_position, axis="X", name=None, offset=None, rotation=0, always_move_to_end=True
+        self, assignment, origin, axis_position, axis="X", name=None, offset=None, rotation=0, always_move_to_end=True
     ):
         """Create a face coordinate system.
         The face coordinate has always the Z axis parallel to face normal.
         The X and Y axis lie on the face plane.
 
         Parameters
         ----------
-        face : int, FacePrimitive
+        assignment : int, FacePrimitive
             Face where the coordinate system is defined.
         origin : int, FacePrimitive, EdgePrimitive, VertexPrimitive
             Specify the coordinate system origin. The origin must belong to the face where the
             coordinate system is defined.
             If a face is specified, the origin is placed on the face center. It must be the same as ``face``.
             If an edge is specified, the origin is placed on the edge midpoint.
             If a vertex is specified, the origin is placed on the vertex.
@@ -499,15 +499,15 @@
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
 
-        face_id = self._modeler.convert_to_selections(face, True)[0]
+        face_id = self._modeler.convert_to_selections(assignment, True)[0]
         if not isinstance(face_id, int):  # pragma: no cover
             raise ValueError("Unable to find reference face.")
         else:
             self.face_id = face_id
 
         if isinstance(origin, int):
             origin_id = origin
@@ -1290,30 +1290,30 @@
 
     @property
     def _attributes(self):
         """Internally named array for attributes of the object coordinate system."""
         coordinateSystemAttributes = ["NAME:Attributes", "Name:=", self.name, "PartName:=", self._part_name]
         return coordinateSystemAttributes
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(obj="assignment")
     def create(
         self,
-        obj,
+        assignment,
         origin,
         x_axis,
         y_axis,
         move_to_end=True,
         reverse_x_axis=False,
         reverse_y_axis=False,
     ):
         """Create an object coordinate system.
 
         Parameters
         ----------
-        obj : str, :class:`pyaedt.modeler.cad.object3d.Object3d`
+        assignment : str, :class:`pyaedt.modeler.cad.object3d.Object3d`
             Object to attach the object coordinate system to.
         origin : int, VertexPrimitive, EdgePrimitive, FacePrimitive, list
             Origin where the object coordinate system is anchored.
             The value can be:
 
              - An integer, in which case it refers to the entity ID.
              - A VertexPrimitive, EdgePrimitive, or FacePrimitive object, in which case it refers to the entity type.
@@ -1347,18 +1347,18 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        if isinstance(obj, str):
-            self.entity_id = self._modeler.objects_by_name[obj].id
-        elif isinstance(obj, Object3d):
-            self.entity_id = obj.id
+        if isinstance(assignment, str):
+            self.entity_id = self._modeler.objects_by_name[assignment].id
+        elif isinstance(assignment, Object3d):
+            self.entity_id = assignment.id
         else:
             raise ValueError("Object provided is invalid.")
 
         # Origin
         if (
             isinstance(origin, int)
             or isinstance(origin, VertexPrimitive)
@@ -1707,59 +1707,59 @@
         try:
             self._modeler.oeditor.EditEntityList(argument1, argument2)
         except Exception:  # pragma: no cover
             raise ValueError("Input List not correct for the type " + self.props["Type"])
 
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(object_list="assignment", type="entity_type")
     def create(
         self,
-        object_list,
+        assignment,
         name=None,
-        type="Object",
+        entity_type="Object",
     ):
         """Create a List.
 
         Parameters
         ----------
-        object_list : list
+        assignment : list
             List of ``["Obj1", "Obj2"]`` objects or face ID if type is "Face".
             The default is ``None``, in which case all objects are selected.
         name : list, str
             List of names. The default is ``None``.
-        type : str, optional
+        entity_type : str, optional
             List type. Options are ``"Object"``, ``"Face"``. The default is ``"Object"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
 
         if not name:
-            name = generate_unique_name(type + "List")
+            name = generate_unique_name(entity_type + "List")
 
-        object_list_new = self._list_verification(object_list, type)
+        object_list_new = self._list_verification(assignment, entity_type)
 
         if object_list_new:
             olist = object_list_new
-            if type == "Object":
+            if entity_type == "Object":
                 olist = ",".join(object_list_new)
 
             self.name = self._modeler.oeditor.CreateEntityList(
-                ["NAME:GeometryEntityListParameters", "EntityType:=", type, "EntityList:=", olist],
+                ["NAME:GeometryEntityListParameters", "EntityType:=", entity_type, "EntityList:=", olist],
                 ["NAME:Attributes", "Name:=", name],
             )
             props = {}
             props["List"] = object_list_new
 
             props["ID"] = self._modeler.get_entitylist_id(self.name)
-            props["Type"] = type
+            props["Type"] = entity_type
 
             self.props = ListsProps(self, props)
             self._modeler.user_lists.append(self)
             return True
         else:
             return False
 
@@ -1773,39 +1773,39 @@
             ``True`` when successful, ``False`` when failed.
 
         """
         self._modeler.oeditor.Delete(["NAME:Selections", "Selections:=", self.name])
         self._modeler.user_lists.remove(self)
         return True
 
-    @pyaedt_function_handler()
-    def rename(self, newname):
+    @pyaedt_function_handler(newname="name")
+    def rename(self, name):
         """Rename the List.
 
         Parameters
         ----------
-        newname : str
+        name : str
             New name for the List.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         argument = [
             "NAME:AllTabs",
             [
                 "NAME:Geometry3DListTab",
                 ["NAME:PropServers", self.name],
-                ["NAME:ChangedProps", ["NAME:Name", "Value:=", newname]],
+                ["NAME:ChangedProps", ["NAME:Name", "Value:=", name]],
             ],
         ]
         self._modeler.oeditor.ChangeProperty(argument)
-        self.name = newname
+        self.name = name
         return True
 
     def _list_verification(self, object_list, list_type):
         object_list = self._modeler.convert_to_selections(object_list, True)
         object_list_new = []
         if list_type == "Object":
             obj_names = [i for i in self._modeler.object_names]
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/Primitives.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/Primitives.py`

 * *Files 10% similar despite different names*

```diff
@@ -133,25 +133,25 @@
             if isinstance(item, int):
                 try:
                     id = item
                     name = self.__parent.oeditor.GetObjectNameByID(id)
                     o = self.__parent._create_object(name, id)
                     self.__setitem__(id, o)
                     return o
-                except:
+                except Exception:
                     raise KeyError(item)
 
             elif isinstance(item, str):
                 try:
                     name = item
                     id = self.__parent.oeditor.GetObjectIDByName(name)
                     o = self.__parent._create_object(name, id)
                     self.__setitem__(id, o)
                     return o
-                except:
+                except Exception:
                     raise KeyError(item)
 
             elif isinstance(item, (Object3d, Polyline)):
                 self.__setitem__(item.id, item)
                 return item
             else:
                 raise TypeError(item)
@@ -204,15 +204,15 @@
             Returns ``None`` if the part ID or the object name is not found.
 
         """
         if isinstance(partId, (Object3d, UserDefinedComponent, Point)):
             return partId
         try:
             return self.objects[partId]
-        except:
+        except Exception:
             if partId in self.user_defined_components.keys():
                 return self.user_defined_components[partId]
         self.logger.error("Object '{}' not found.".format(partId))
         return None
 
     def __init__(self, app, is3d=True):
         self._app = app
@@ -842,21 +842,21 @@
                 ]
             if attribs["Name"] in self._all_object_names:
                 pid = 0
 
                 if operations and isinstance(operations.get("Operation", None), (OrderedDict, dict)):
                     try:
                         pid = operations["Operation"]["ParentPartID"]
-                    except Exception:  # pragma: no cover
-                        pass
+                    except Exception as e:  # pragma: no cover
+                        self.logger.debug(e)
                 elif operations and isinstance(operations.get("Operation", None), list):
                     try:
                         pid = operations["Operation"][0]["ParentPartID"]
-                    except Exception:
-                        pass
+                    except Exception as e:
+                        self.logger.debug(e)
 
                 is_polyline = False
                 if operations and "PolylineParameters" in operations.get("Operation", {}):
                     is_polyline = True
 
                 o = self._create_object(name=attribs["Name"], pid=pid, use_cached=True, is_polyline=is_polyline)
                 o._part_coordinate_system = attribs["PartCoordinateSystem"]
@@ -1005,23 +1005,23 @@
 
         """
         added_objects = []
 
         for obj_name in self.object_names:
             if obj_name not in self._object_names_to_ids:
                 try:
-                    pid = self.oeditor.GetObjectIDByName(obj)
+                    pid = self.oeditor.GetObjectIDByName(obj_name)
                 except Exception:
                     pid = 0
                 self._create_object(obj_name, pid=pid, use_cached=True)
                 added_objects.append(obj_name)
         for obj_name in self.unclassified_names:
             if obj_name not in self._object_names_to_ids:
                 try:
-                    pid = self.oeditor.GetObjectIDByName(obj)
+                    pid = self.oeditor.GetObjectIDByName(obj_name)
                 except Exception:
                     pid = 0
                 self._create_object(obj_name, pid=pid, use_cached=True)
                 added_objects.append(obj_name)
 
         return added_objects
 
@@ -1070,21 +1070,21 @@
         self.add_new_solids()
         self.add_new_points()
         self.add_new_user_defined_component()
         self.cleanup_objects()
 
         return len(self.objects)
 
-    @pyaedt_function_handler()
-    def get_objects_by_material(self, materialname=None):
+    @pyaedt_function_handler(materialname="material")
+    def get_objects_by_material(self, material=None):
         """Get a list of objects either of a specified material or classified by material.
 
         Parameters
         ----------
-        materialname : str
+        material : str
             Name of the material. The default is ``None``.
 
         Returns
         -------
         list of class:`pyaedt.modeler.cad.object3d.Object3d`
             If a material name is not provided, the method returns
             a list of dictionaries where keys are material names
@@ -1096,26 +1096,26 @@
         References
         ----------
 
         >>> oEditor.GetObjectsByMaterial
 
         """
         obj_lst = []
-        if materialname is not None:
+        if material is not None:
             for obj in self.object_list:
                 if obj and ("[" in obj.material_name or "(" in obj.material_name) and obj.object_type == "Solid":
                     material = (
                         self._app.odesign.GetChildObject("3D Modeler")
                         .GetChildObject(obj.name)
                         .GetPropEvaluatedValue("Material")
                         .lower()
                     )
-                    if materialname.lower() == material:
+                    if material.lower() == material:
                         obj_lst.append(obj)
-                elif obj and (obj.material_name == materialname or obj.material_name == materialname.lower()):
+                elif obj and (obj.material_name == material or obj.material_name == material.lower()):
                     obj_lst.append(obj)
         else:
             obj_lst = [
                 self._get_object_dict_by_material(self.materials.conductors),
                 self._get_object_dict_by_material(self.materials.dielectrics),
                 self._get_object_dict_by_material(self.materials.gases),
                 self._get_object_dict_by_material(self.materials.liquids),
@@ -1226,22 +1226,22 @@
                                                 coord.append(FaceCoordinateSystem(self, props, name))
                                         elif isinstance(op, list):
                                             for iop in op:
                                                 if iop["ID"] == op_id:
                                                     props = iop["FaceCSParameters"]
                                                     coord.append(FaceCoordinateSystem(self, props, name))
                                                     break
-                except Exception:
-                    pass
+                except Exception as e:
+                    self.logger.debug(e)
             for cs in coord:
                 if isinstance(cs, CoordinateSystem):
                     try:
                         cs._ref_cs = id2name[name2refid[cs.name]]
-                    except Exception:
-                        pass
+                    except Exception as e:
+                        self.logger.debug(e)
         coord.reverse()
         return coord
 
     def _get_lists_data(self):
         """Retrieve user object list data.
 
         Returns
@@ -1341,56 +1341,56 @@
                 break
         if not a_end:
             a_end = vertices[1]
             b_end = vertices[2]
             return False, (origin, a_end, b_end)
         return True, (origin, a_end, b_end)
 
-    @pyaedt_function_handler()
-    def cover_lines(self, selection):
+    @pyaedt_function_handler(selection="assignment")
+    def cover_lines(self, assignment):
         """Cover closed lines and transform them to a sheet.
 
         Parameters
         ----------
-        selection : str, int
+        assignment : str, int
             Polyline object to cover.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CoverLines
         """
-        obj_to_cover = self.convert_to_selections(selection, False)
+        obj_to_cover = self.convert_to_selections(assignment, False)
         self.oeditor.CoverLines(["NAME:Selections", "Selections:=", obj_to_cover, "NewPartsModelFlag:=", "Model"])
         return True
 
-    @pyaedt_function_handler()
-    def cover_faces(self, selection):
+    @pyaedt_function_handler(selection="assignment")
+    def cover_faces(self, assignment):
         """Cover a face.
 
         Parameters
         ----------
-        selection : str, int
+        assignment : str, int
             Sheet object to cover.
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CoverLines
         """
-        obj_to_cover = self.convert_to_selections(selection, False)
+        obj_to_cover = self.convert_to_selections(assignment, False)
         self.oeditor.CoverSurfaces(["NAME:Selections", "Selections:=", obj_to_cover, "NewPartsModelFlag:=", "Model"])
         return True
 
     @pyaedt_function_handler()
     def create_coordinate_system(
         self,
         origin=None,
@@ -1557,37 +1557,45 @@
             cs_names = [i.name for i in self.coordinate_systems]
             if name in cs_names:  # pragma: no cover
                 raise AttributeError("A coordinate system with the specified name already exists!")
 
         cs = FaceCoordinateSystem(self)
         if cs:
             result = cs.create(
-                face=face,
+                assignment=face,
                 origin=origin,
                 axis_position=axis_position,
                 axis=axis,
                 name=name,
                 offset=offset,
                 rotation=rotation,
                 always_move_to_end=always_move_to_end,
             )
 
             if result:
                 return cs
         return False
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(obj="assignment")
     def create_object_coordinate_system(
-        self, obj, origin, x_axis, y_axis, move_to_end=True, reverse_x_axis=False, reverse_y_axis=False, name=None
+        self,
+        assignment,
+        origin,
+        x_axis,
+        y_axis,
+        move_to_end=True,
+        reverse_x_axis=False,
+        reverse_y_axis=False,
+        name=None,
     ):
         """Create an object coordinate system.
 
         Parameters
         ----------
-        obj : str, :class:`pyaedt.modeler.cad.object3d.Object3d`
+        assignment : str, :class:`pyaedt.modeler.cad.object3d.Object3d`
             Object to attach the object coordinate system to.
         origin : int, VertexPrimitive, EdgePrimitive, FacePrimitive, list
             Refer to the origin where the object coordinate system is anchored.
             It can be:
 
              - int in which case it refers to the entity Id.
              - VertexPrimitive, EdgePrimitive, FacePrimitive in which case it refers to the entity type.
@@ -1631,36 +1639,36 @@
             cs_names = [i.name for i in self.coordinate_systems]
             if name in cs_names:  # pragma: no cover
                 raise AttributeError("A coordinate system with the specified name already exists.")
 
         cs = ObjectCoordinateSystem(self, name=name)
         if cs:
             result = cs.create(
-                obj=obj,
+                assignment=assignment,
                 origin=origin,
                 x_axis=x_axis,
                 y_axis=y_axis,
                 move_to_end=move_to_end,
                 reverse_x_axis=reverse_x_axis,
                 reverse_y_axis=reverse_y_axis,
             )
 
             if result:
                 return cs
         return False
 
-    @pyaedt_function_handler()
-    def global_to_cs(self, point, ref_cs):
+    @pyaedt_function_handler(ref_cs="coordinate_system")
+    def global_to_cs(self, point, coordinate_system):
         """Transform a point from the global coordinate system to another coordinate system.
 
         Parameters
         ----------
         point : list
             List of the ``[x, y, z]`` coordinates to transform.
-        ref_cs : str, CoordinateSystem
+        coordinate_system : str, CoordinateSystem
             Name of the destination reference system. The ``CoordinateSystem`` object can also be
             used.
 
         Returns
         -------
         list
             List of the transformed ``[x, y, z]`` coordinates.
@@ -1668,18 +1676,18 @@
         """
         if type(point) is not list or len(point) != 3:
             raise AttributeError("Point must be in format [x, y, z].")
         try:
             point = [float(i) for i in point]
         except Exception:
             raise AttributeError("Point must be in format [x, y, z].")
-        if isinstance(ref_cs, BaseCoordinateSystem):
-            ref_cs_name = ref_cs.name
-        elif isinstance(ref_cs, str):
-            ref_cs_name = ref_cs
+        if isinstance(coordinate_system, BaseCoordinateSystem):
+            ref_cs_name = coordinate_system.name
+        elif isinstance(coordinate_system, str):
+            ref_cs_name = coordinate_system
         else:
             raise AttributeError("ref_cs must be either a string or a CoordinateSystem object.")
         if ref_cs_name == "Global":
             return point
         cs_names = [i.name for i in self.coordinate_systems]
         if ref_cs_name not in cs_names:
             raise AttributeError("Specified coordinate system does not exist in the design.")
@@ -1901,15 +1909,15 @@
                     for edge in face.edges
                     for vertex in edge.vertices
                     if vertex.id == face_cs.props["AxisPosn"]["EntityID"]
                 ][0]
                 axis_position = [v for v in edge.vertices if v.id == face_cs.props["AxisPosn"]["EntityID"]][0]
             if face_cs:
                 result = face_cs.create(
-                    face=face,
+                    assignment=face,
                     origin=origin,
                     axis_position=axis_position,
                     axis=face_cs.props["WhichAxis"],
                     name=name,
                     offset=[face_cs["XOffset"], face_cs["YOffset"]],
                     rotation=decompose_variable_value(face_cs["ZRotationAngle"])[0],
                     always_move_to_end=face_cs["MoveToEnd"],
@@ -1973,66 +1981,66 @@
                 y_axis = [
                     cs.props["yAxis"]["xDirection"],
                     cs.props["yAxis"]["yDirection"],
                     cs.props["yAxis"]["zDirection"],
                 ]
             if obj_cs:
                 result = obj_cs.create(
-                    obj=obj,
+                    assignment=obj,
                     origin=origin,
                     x_axis=x_axis,
                     y_axis=y_axis,
                     move_to_end=cs.props["MoveToEnd"],
                     reverse_x_axis=cs.props["ReverseXAxis"],
                     reverse_y_axis=cs.props["ReverseYAxis"],
                 )
                 if result:
                     return obj_cs
         return False
 
-    @pyaedt_function_handler()
-    def set_objects_deformation(self, objects):
+    @pyaedt_function_handler(objects="assignment")
+    def set_objects_deformation(self, assignment):
         """Assign deformation objects to a Workbench link.
 
         Parameters
         ----------
-        objects : list
+        assignment : list
             List of the deformation objects to assign to the Workbench link.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oDesign.SetObjectDeformation
         """
         self.logger.info("Enabling deformation feedback")
         try:
-            self._odesign.SetObjectDeformation(["EnabledObjects:=", objects])
+            self._odesign.SetObjectDeformation(["EnabledObjects:=", assignment])
         except Exception:
             self.logger.error("Failed to enable the deformation dependence")
             return False
         else:
             self.logger.info("Successfully enabled deformation feedback")
             return True
 
-    @pyaedt_function_handler()
-    def set_objects_temperature(self, objects, ambient_temp=22, create_project_var=False):
+    @pyaedt_function_handler(objects="assignment", ambient_temp="ambient_temperature")
+    def set_objects_temperature(self, assignment, ambient_temperature=22, create_project_var=False):
         """Assign temperatures to objects.
 
         The materials assigned to the objects must have a thermal modifier.
 
         Parameters
         ----------
-        objects : list
+        assignment : list
             List of objects.
-        ambient_temp : float, optional
+        ambient_temperature : float, optional
             Ambient temperature. The default is ``22``.
         create_project_var : bool, optional
             Whether to create a project variable for the ambient temperature.
             The default is ``False``. If ``True,`` ``$AmbientTemp`` is created.
 
         Returns
         -------
@@ -2042,28 +2050,28 @@
         References
         ----------
 
         >>> oDesign.SetObjectTemperature
         """
         self.logger.info("Set model temperature and enabling Thermal Feedback")
         if create_project_var:
-            self._app.variable_manager["$AmbientTemp"] = str(ambient_temp) + "cel"
+            self._app.variable_manager["$AmbientTemp"] = str(ambient_temperature) + "cel"
             var = "$AmbientTemp"
         else:
-            var = str(ambient_temp) + "cel"
+            var = str(ambient_temperature) + "cel"
         vargs1 = [
             "NAME:TemperatureSettings",
             "IncludeTemperatureDependence:=",
             True,
             "EnableFeedback:=",
             True,
             "Temperatures:=",
         ]
         vargs2 = []
-        for obj in objects:
+        for obj in assignment:
             mat = self[obj].material_name
             th = self._app.materials.check_thermal_modifier(mat)
             if th:
                 vargs2.append(obj)
                 vargs2.append(var)
         if not vargs2:
             return False
@@ -2117,23 +2125,26 @@
         edge_1 = port_edges[1].edges[0]
         sheet_name = port_edges[0].name
         point0 = edge_0.midpoint
         point1 = edge_1.midpoint
         self.connect(port_edges)
         return sheet_name, point0, point1
 
-    @pyaedt_function_handler()
-    def find_point_around(self, objectname, startposition, offset, plane):
+    @pyaedt_function_handler(
+        objectname="assignment",
+        startposition="origin",
+    )
+    def find_point_around(self, assignment, origin, offset, plane):
         """Find the point around an object.
 
         Parameters
         ----------
-        objectname : str
+        assignment : str
             Name of the object.
-        startposition : list
+        origin : list
             List of the ``[x, y, z]`` coordinates for the starting
             position of the object.
         offset :
             Offset to apply.
         plane : str
             Coordinate plane of the arc. Choices are ``"YZ"``,
             ``"ZX"``, and ``"XY"``.
@@ -2145,125 +2156,125 @@
             List of the ``[x, y, z]`` coordinates for the point.
 
         """
         position = [0, 0, 0]
         angle = 0
         if plane == 0:
             while angle <= 360:
-                position[0] = startposition[0] + offset * math.cos(math.pi * angle / 180)
-                position[1] = startposition[1] + offset * math.sin(math.pi * angle / 180)
-                if objectname in self.get_bodynames_from_position(startposition):
+                position[0] = origin[0] + offset * math.cos(math.pi * angle / 180)
+                position[1] = origin[1] + offset * math.sin(math.pi * angle / 180)
+                if assignment in self.get_bodynames_from_position(origin):
                     angle = 400
                 else:
                     angle += 90
         elif plane == 1:
             while angle <= 360:
-                position[1] = startposition[1] + offset * math.cos(math.pi * angle / 180)
-                position[2] = startposition[2] + offset * math.sin(math.pi * angle / 180)
-                if objectname in self.get_bodynames_from_position(startposition):
+                position[1] = origin[1] + offset * math.cos(math.pi * angle / 180)
+                position[2] = origin[2] + offset * math.sin(math.pi * angle / 180)
+                if assignment in self.get_bodynames_from_position(origin):
                     angle = 400
                 else:
                     angle += 90
         elif plane == 2:
             while angle <= 360:
-                position[0] = startposition[0] + offset * math.cos(math.pi * angle / 180)
-                position[2] = startposition[2] + offset * math.sin(math.pi * angle / 180)
-                if objectname in self.get_bodynames_from_position(startposition):
+                position[0] = origin[0] + offset * math.cos(math.pi * angle / 180)
+                position[2] = origin[2] + offset * math.sin(math.pi * angle / 180)
+                if assignment in self.get_bodynames_from_position(origin):
                     angle = 400
                 else:
                     angle += 90
         return position
 
-    @pyaedt_function_handler()
-    def create_sheet_to_ground(self, objectname, groundname=None, axisdir=0, sheet_dim=1):
+    @pyaedt_function_handler(objectname="assignment", groundname="ground_name", axisdir="orientation")
+    def create_sheet_to_ground(self, assignment, ground_name=None, orientation=0, sheet_dim=1):
         """Create a sheet between an object and a ground plane.
 
         The ground plane must be bigger than the object and perpendicular
         to one of the three axes.
 
         Parameters
         ----------
-        objectname : str
+        assignment : str
             Name of the object.
-        groundname : str, optional
+        ground_name : str, optional
             Name of the ground. The default is ``None``, in which case the
             bounding box is used.
-        axisdir : int, optional
+        orientation : int, optional
             Axis direction. Options are ``0`` through ``5``. The default is ``0``.
         sheet_dim : optional
             Sheet dimension in millimeters. The default is ``1``.
 
         Returns
         -------
         int
             ID of the sheet created.
 
         References
         ----------
 
         >>> oEditor.CreatePolyline
         """
-        if axisdir > 2:
+        if orientation > 2:
             obj_cent = [-1e6, -1e6, -1e6]
         else:
             obj_cent = [1e6, 1e6, 1e6]
         face_ob = None
-        for face in self[objectname].faces:
+        for face in self[assignment].faces:
             center = face.center
             if not center:
                 continue
-            if axisdir > 2 and center[axisdir - 3] > obj_cent[axisdir - 3]:
+            if orientation > 2 and center[orientation - 3] > obj_cent[orientation - 3]:
                 obj_cent = center
                 face_ob = face
-            elif axisdir <= 2 and center[axisdir] < obj_cent[axisdir]:
+            elif orientation <= 2 and center[orientation] < obj_cent[orientation]:
                 obj_cent = center
                 face_ob = face
         vertex = face_ob.vertices
         start = vertex[0].position
 
-        if not groundname:
+        if not ground_name:
             gnd_cent = []
             bounding = self.get_model_bounding_box()
-            if axisdir < 3:
+            if orientation < 3:
                 for i in bounding[0:3]:
                     gnd_cent.append(float(i))
             else:
                 for i in bounding[3:]:
                     gnd_cent.append(float(i))
         else:
-            ground_plate = self[groundname]
-            if axisdir > 2:
+            ground_plate = self[ground_name]
+            if orientation > 2:
                 gnd_cent = [1e6, 1e6, 1e6]
             else:
                 gnd_cent = [-1e6, -1e6, -1e6]
             face_gnd = ground_plate.faces
             for face in face_gnd:
                 center = face.center
                 if not center:
                     continue
-                if axisdir > 2 and center[axisdir - 3] < gnd_cent[axisdir - 3]:
+                if orientation > 2 and center[orientation - 3] < gnd_cent[orientation - 3]:
                     gnd_cent = center
-                elif axisdir <= 2 and center[axisdir] > gnd_cent[axisdir]:
+                elif orientation <= 2 and center[orientation] > gnd_cent[orientation]:
                     gnd_cent = center
 
-        axisdist = obj_cent[divmod(axisdir, 3)[1]] - gnd_cent[divmod(axisdir, 3)[1]]
-        if axisdir < 3:
+        axisdist = obj_cent[divmod(orientation, 3)[1]] - gnd_cent[divmod(orientation, 3)[1]]
+        if orientation < 3:
             axisdist = -axisdist
 
-        if divmod(axisdir, 3)[1] == 0:
+        if divmod(orientation, 3)[1] == 0:
             cs = self._app.PLANE.YZ
             vector = [axisdist, 0, 0]
-        elif divmod(axisdir, 3)[1] == 1:
+        elif divmod(orientation, 3)[1] == 1:
             cs = self._app.PLANE.ZX
             vector = [0, axisdist, 0]
-        elif divmod(axisdir, 3)[1] == 2:
+        elif divmod(orientation, 3)[1] == 2:
             cs = self._app.PLANE.XY
             vector = [0, 0, axisdist]
 
-        offset = self.find_point_around(objectname, start, sheet_dim, cs)
+        offset = self.find_point_around(assignment, start, sheet_dim, cs)
         p1 = self.create_polyline([start, offset])
         p2 = p1.clone().move(vector)
         self.connect([p1, p2])
 
         return p1
 
     @pyaedt_function_handler()
@@ -2366,21 +2377,21 @@
         >>> oModule.GetBoundaries
         """
         if self._app.design_type == "Icepak":
             return list(self._app.odesign.GetChildObject("Thermal").GetChildNames())
         else:
             return list(self._app.odesign.GetChildObject("Boundaries").GetChildNames())
 
-    @pyaedt_function_handler()
-    def set_object_model_state(self, obj_list, model=True):
+    @pyaedt_function_handler(obj_list="assignment")
+    def set_object_model_state(self, assignment, model=True):
         """Set a list of objects to either models or non-models.
 
         Parameters
         ----------
-        obj_list : list
+        assignment : list
             List of objects IDs or names.
         model : bool, optional
             Whether to set the objects as models. The default is ``True``.
             If ``False``, the objects are set as non-models.
 
         Returns
         -------
@@ -2388,15 +2399,15 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        selections = self.convert_to_selections(obj_list, True)
+        selections = self.convert_to_selections(assignment, True)
         arguments = [
             "NAME:AllTabs",
             [
                 "NAME:Geometry3DAttributeTab",
                 ["NAME:PropServers"] + selections,
                 ["NAME:ChangedProps", ["NAME:Model", "Value:=", model]],
             ],
@@ -2463,23 +2474,23 @@
             self._change_geometry_property(vArg1, objs_to_unmodel)
             bounding = self.get_model_bounding_box()
             self._odesign.Undo()
         else:
             bounding = self.get_model_bounding_box()
         return bounding
 
-    @pyaedt_function_handler()
-    def convert_to_selections(self, object_id, return_list=False):
+    @pyaedt_function_handler(object_id="assignment")
+    def convert_to_selections(self, assignment, return_list=False):
         """Convert modeler objects.
 
         This method converts modeler object or IDs to the corresponding
         output according to the following scheme:
 
         ====================  ===========================
-          ``object_id``          Return value
+          ``assignment``          Return value
         ====================  ===========================
 
          ``int``                 object name (str)
           ``Object3D``           object name (str)
           ``FacePrimitive``      int, face ID
           ``EdgePrimitive``      int, edge ID
           ``str``                return the same ``str``
@@ -2491,32 +2502,32 @@
 
         - If the second argument, ``return_list``, is set to `False` (default), a
         string is returned with elements separated by a comma (,)".
 
 
         Parameters
         ----------
-        object_id : str, int, list
+        assignment : str, int, list
             One or more object IDs whose name will be returned. A list can contain
             both strings (object names) and integers (object IDs).
         return_list : bool, option
             Whether to return a list of the selections. The default is
             ``False``, in which case a string of the selections is returned.
             If ``True``, a list of the selections is returned.
 
         Returns
         -------
         str or list
            Name of the objects corresponding to the one or more object IDs passed as arguments.
 
         """
-        if not isinstance(object_id, list):
-            object_id = [object_id]
+        if not isinstance(assignment, list):
+            assignment = [assignment]
         objnames = []
-        for el in object_id:
+        for el in assignment:
             if isinstance(el, int) and el in self.objects:
                 objnames.append(self.objects[el].name)
             elif isinstance(el, int):
                 objnames.append(el)
             elif isinstance(el, Object3d):
                 objnames.append(el.name)
             elif isinstance(el, FacePrimitive) or isinstance(el, EdgePrimitive) or isinstance(el, VertexPrimitive):
@@ -2524,23 +2535,25 @@
             elif isinstance(el, str):
                 objnames.append(el)
         if return_list:
             return objnames
         else:
             return ",".join([str(i) for i in objnames])
 
-    @pyaedt_function_handler()
-    def split(self, objects, plane=None, sides="Both", tool=None, split_crossing_objs=False, delete_invalid_objs=True):
+    @pyaedt_function_handler(objects="assignment")
+    def split(
+        self, assignment, plane=None, sides="Both", tool=None, split_crossing_objs=False, delete_invalid_objs=True
+    ):
         """Split a list of objects.
         In case of 3D design possible splitting options are plane, Face Primitive, Edge Primitive or Polyline.
         In case of 2D design possible splitting option is plane.
 
         Parameters
         ----------
-        objects : str, int, or list
+        assignment : str, int, or list
             One or more objects to split. A list can contain
             both strings (object names) and integers (object IDs).
         plane : str, optional
             Coordinate plane of the cut or the Application.PLANE object.
             The default value is ``None``.
             Choices for the coordinate plane are ``"XY"``, ``"YZ"``, and ``"ZX"``.
             If plane or tool parameter are not provided the method returns ``False``.
@@ -2570,28 +2583,28 @@
         ----------
 
         >>> oEditor.Split
         """
         if plane is None and not tool or plane and tool:
             self.logger.info("One method to split the objects has to be defined.")
             return False
-        objects = self.convert_to_selections(objects)
+        assignment = self.convert_to_selections(assignment)
         all_objs = [i for i in self.object_names]
         selections = []
         planes = "Dummy"
         tool_type = "PlaneTool"
         tool_entity_id = -1
         if self._is3d:
             obj_name = None
             obj = []
             if plane is not None and not tool:
                 tool_type = "PlaneTool"
                 tool_entity_id = -1
                 planes = GeometryOperators.cs_plane_to_plane_str(plane)
-                selections = ["NAME:Selections", "Selections:=", objects, "NewPartsModelFlag:=", "Model"]
+                selections = ["NAME:Selections", "Selections:=", assignment, "NewPartsModelFlag:=", "Model"]
             elif tool and plane is None:
                 if isinstance(tool, str):
                     obj = [f for f in self.object_list if f.name == tool][0]
                     obj_name = obj.name
                     if isinstance(obj, Object3d) and obj.object_type != "Line":
                         obj = obj.faces[0]
                         tool_type = "FaceTool"
@@ -2643,29 +2656,29 @@
                     return False
                 planes = "Dummy"
                 tool_type = tool_type
                 tool_entity_id = obj.id
                 selections = [
                     "NAME:Selections",
                     "Selections:=",
-                    objects,
+                    assignment,
                     "NewPartsModelFlag:=",
                     "Model",
                     "ToolPart:=",
                     obj_name,
                 ]
         else:
             if plane is None and tool or not plane:
                 self.logger.info("For 2D design types only planes can be defined.")
                 return False
             elif plane is not None:
                 tool_type = "PlaneTool"
                 tool_entity_id = -1
                 planes = GeometryOperators.cs_plane_to_plane_str(plane)
-                selections = ["NAME:Selections", "Selections:=", objects, "NewPartsModelFlag:=", "Model"]
+                selections = ["NAME:Selections", "Selections:=", assignment, "NewPartsModelFlag:=", "Model"]
         self.oeditor.Split(
             selections,
             [
                 "NAME:SplitToParameters",
                 "SplitPlane:=",
                 planes,
                 "WhichSide:=",
@@ -2677,35 +2690,35 @@
                 "SplitCrossingObjectsOnly:=",
                 split_crossing_objs,
                 "DeleteInvalidObjects:=",
                 delete_invalid_objs,
             ],
         )
         self.refresh_all_ids()
-        return [objects] + [i for i in self.object_names if i not in all_objs]
+        return [assignment] + [i for i in self.object_names if i not in all_objs]
 
-    @pyaedt_function_handler()  # TODO: Deprecate this and add duplicate as an option in the mirror method.
+    @pyaedt_function_handler(objid="assignment", position="origin")
     def duplicate_and_mirror(
         self,
-        objid,
-        position,
+        assignment,
+        origin,
         vector,
         is_3d_comp=False,
         duplicate_assignment=True,
     ):
         """Duplicate and mirror a selection.
 
         Parameters
         ----------
-        objid : str, int, or  Object3d
+        assignment : str, int, or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name or ID of the object.
-        position : float
+        origin : list
             List of the ``[x, y, z]`` coordinates or
             Application.Position object for the selection.
-        vector : float
+        vector : float, str
             List of the ``[x1, y1, z1]`` coordinates or
             Application.Position object for the vector.
         is_3d_comp : bool, optional
             If ``True``, the method will try to return the duplicated list of 3dcomponents. The default is ``False``.
         duplicate_assignment : bool, optional
             If True, the method duplicates selection assignments. The default value is ``True``.
 
@@ -2716,35 +2729,35 @@
 
         References
         ----------
 
         >>> oEditor.DuplicateMirror
         """
         return self.mirror(
-            objid, position, vector, duplicate=True, is_3d_comp=is_3d_comp, duplicate_assignment=duplicate_assignment
+            assignment, origin, vector, duplicate=True, is_3d_comp=is_3d_comp, duplicate_assignment=duplicate_assignment
         )
         # selections = self.convert_to_selections(objid)
 
-    @pyaedt_function_handler()
-    def mirror(self, objid, position, vector, duplicate=False, is_3d_comp=False, duplicate_assignment=True):
+    @pyaedt_function_handler(objid="assignment", position="origin")
+    def mirror(self, assignment, origin, vector, duplicate=False, is_3d_comp=False, duplicate_assignment=True):
         """Mirror a selection.
 
         Parameters
         ----------
-        objid : str, int, or Object3d
+        assignment : str, int, or Object3d
             Name or ID of the object.
-        position : int or float
+        origin : int or float
             List of the ``[x, y, z]`` coordinates or the
             ``Application.Position`` object for the selection.
         duplicate : bool, optional
             Whether if duplicate the object before mirror or not. Default is ``False``.
         is_3d_comp : bool, optional
             Whether the component is 3D. The default is ``False``. If ``True``, the method
             tries to return the duplicated list of 3D components.
-        vector : float
+        vector : list
             List of the ``[x1, y1, z1]`` coordinates or
             the ``Application.Position`` object for the vector.
         duplicate_assignment : bool, optional
             Whether to duplicate selection assignments. The default is ``True``.
 
         Returns
         -------
@@ -2753,16 +2766,16 @@
 
         References
         ----------
 
         >>> oEditor.Mirror
         >>> oEditor.DuplicateMirror
         """
-        selections = self.convert_to_selections(objid)
-        Xpos, Ypos, Zpos = self._pos_with_arg(position)
+        selections = self.convert_to_selections(assignment)
+        Xpos, Ypos, Zpos = self._pos_with_arg(origin)
         Xnorm, Ynorm, Znorm = self._pos_with_arg(vector)
         if duplicate:
             vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
             vArg2 = ["NAME:DuplicateToMirrorParameters"]
             vArg2.append("DuplicateMirrorBaseX:="), vArg2.append(Xpos)
             vArg2.append("DuplicateMirrorBaseY:="), vArg2.append(Ypos)
             vArg2.append("DuplicateMirrorBaseZ:="), vArg2.append(Zpos)
@@ -2789,21 +2802,21 @@
             vArg2.append("MirrorNormalX:="), vArg2.append(Xnorm)
             vArg2.append("MirrorNormalY:="), vArg2.append(Ynorm)
             vArg2.append("MirrorNormalZ:="), vArg2.append(Znorm)
 
             self.oeditor.Mirror(vArg1, vArg2)
             return True
 
-    @pyaedt_function_handler()
-    def move(self, objid, vector):
+    @pyaedt_function_handler(objid="assignment")
+    def move(self, assignment, vector):
         """Move objects from a list.
 
         Parameters
         ----------
-        objid : list, Position object
+        assignment : list, Position object
             List of object IDs.
         vector : list
             Vector of the direction move. It can be a list of the ``[x, y, z]``
             coordinates or a Position object.
 
         Returns
         -------
@@ -2812,48 +2825,48 @@
 
         References
         ----------
 
         >>> oEditor.Move
         """
         Xvec, Yvec, Zvec = self._pos_with_arg(vector)
-        szSelections = self.convert_to_selections(objid)
+        szSelections = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", szSelections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:TranslateParameters"]
         vArg2.append("TranslateVectorX:="), vArg2.append(Xvec)
         vArg2.append("TranslateVectorY:="), vArg2.append(Yvec)
         vArg2.append("TranslateVectorZ:="), vArg2.append(Zvec)
 
         if self.oeditor is not None:
             self.oeditor.Move(vArg1, vArg2)
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(objid="assignment", cs_axis="axis", nclones="clones")
     def duplicate_around_axis(
         self,
-        objid,
-        cs_axis,
+        assignment,
+        axis,
         angle=90,
-        nclones=2,
+        clones=2,
         create_new_objects=True,
         is_3d_comp=False,
         duplicate_assignment=True,
     ):
         """Duplicate a selection around an axis.
 
         Parameters
         ----------
-        objid : list, str, int, Object3d or UserDefinedComponent
+        assignment : list, str, int, Object3d or UserDefinedComponent
             Name or ID of the object.
-        cs_axis :
+        axis : str
             Coordinate system axis or the Application.AXIS object.
         angle : float, optional
             Angle rotation in degees. The default is ``90``.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
         create_new_objects :
             Whether to create the copies as new objects. The
             default is ``True``.
         is_3d_comp : bool, optional
             If ``True``, the method will try to return the duplicated list of 3dcomponents. The default is ``False``.
         duplicate_assignment : bool, optional
@@ -2864,27 +2877,27 @@
         tuple
 
         References
         ----------
 
         >>> oEditor.DuplicateAroundAxis
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = [
             "NAME:DuplicateAroundAxisParameters",
             "CreateNewObjects:=",
             create_new_objects,
             "WhichAxis:=",
-            GeometryOperators.cs_axis_str(cs_axis),
+            GeometryOperators.cs_axis_str(axis),
             "AngleStr:=",
             self._arg_with_dim(angle, "deg"),
             "Numclones:=",
-            str(nclones),
+            str(clones),
         ]
         vArg3 = ["NAME:Options", "DuplicateAssignments:=", duplicate_assignment]
         added_objs = self.oeditor.DuplicateAroundAxis(vArg1, vArg2, vArg3)
         self._duplicate_added_objects_tuple()
         if is_3d_comp:
             return self._duplicate_added_components_tuple()
         return True, list(added_objs)
@@ -2899,36 +2912,36 @@
     def _duplicate_added_components_tuple(self):
         added_component = self.add_new_user_defined_component()
         if added_component:
             return True, added_component
         else:
             return False, []
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(objid="assignment", nclones="clones", attachObject="attach")
     def duplicate_along_line(
         self,
-        objid,
+        assignment,
         vector,
-        nclones=2,
-        attachObject=False,
+        clones=2,
+        attach=False,
         is_3d_comp=False,
         duplicate_assignment=True,
     ):
         """Duplicate a selection along a line.
 
         Parameters
         ----------
-        objid : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
         vector : list
             List of ``[x1,y1,z1]`` coordinates or the Application.Position object for
             the vector.
-        attachObject : bool, optional
+        attach : bool, optional
             The default is ``False``.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
         is_3d_comp : bool, optional
             If True, the method will try to return the duplicated list of 3dcomponents. The default is ``False``.
         duplicate_assignment : bool, optional
             If True, the method duplicates selection assignments. The default value is ``True``.
 
         Returns
@@ -2936,102 +2949,102 @@
         tuple
 
         References
         ----------
 
         >>> oEditor.DuplicateAlongLine
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
         Xpos, Ypos, Zpos = self._pos_with_arg(vector)
 
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:DuplicateToAlongLineParameters"]
-        vArg2.append("CreateNewObjects:="), vArg2.append(not attachObject)
+        vArg2.append("CreateNewObjects:="), vArg2.append(not attach)
         vArg2.append("XComponent:="), vArg2.append(Xpos)
         vArg2.append("YComponent:="), vArg2.append(Ypos)
         vArg2.append("ZComponent:="), vArg2.append(Zpos)
-        vArg2.append("Numclones:="), vArg2.append(str(nclones))
+        vArg2.append("Numclones:="), vArg2.append(str(clones))
         vArg3 = ["NAME:Options", "DuplicateAssignments:=", duplicate_assignment]
         self.oeditor.DuplicateAlongLine(vArg1, vArg2, vArg3)
         if is_3d_comp:
             return self._duplicate_added_components_tuple()
-        if attachObject:
+        if attach:
             return True, []
         return self._duplicate_added_objects_tuple()
 
-    @pyaedt_function_handler()
-    def thicken_sheet(self, objid, thickness, bBothSides=False):
+    @pyaedt_function_handler(objid="assignment", bBothSides="both_sides")
+    def thicken_sheet(self, assignment, thickness, both_sides=False):
         """Thicken the sheet of the selection.
 
         Parameters
         ----------
-        objid : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
         thickness : float, str
             Amount to thicken the sheet by.
-        bBothSides : bool, optional
+        both_sides : bool, optional
             Whether to thicken the sheet on both side. The default is ``False``.
 
         Returns
         -------
         pyaedt.modeler.cad.object3d.Object3d
 
         References
         ----------
 
         >>> oEditor.ThickenSheet
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:SheetThickenParameters"]
         vArg2.append("Thickness:="), vArg2.append(self._arg_with_dim(thickness))
-        vArg2.append("BothSides:="), vArg2.append(bBothSides)
+        vArg2.append("BothSides:="), vArg2.append(both_sides)
 
         self.oeditor.ThickenSheet(vArg1, vArg2)
 
-        if isinstance(objid, list):
+        if isinstance(assignment, list):
             obj_list = []
-            for objl in objid:
+            for objl in assignment:
                 obj_list.append(self.update_object(objl))
             return obj_list
-        return self.update_object(objid)
+        return self.update_object(assignment)
 
-    @pyaedt_function_handler()
-    def sweep_along_normal(self, obj_name, face_id, sweep_value=0.1):
+    @pyaedt_function_handler(obj_name="assignment", face_id="faces")
+    def sweep_along_normal(self, assignment, faces, sweep_value=0.1):
         """Sweep the selection along the vector.
 
         Parameters
         ----------
-        obj_name : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
-        face_id : int or list
+        faces : int or list
             Face or list of faces to sweep.
         sweep_value : float, optional
             Sweep value. The default is ``0.1``.
 
         Returns
         -------
         pyaedt.modeler.cad.object3d.Object3d
 
         References
         ----------
 
         >>> oEditor.SweepFacesAlongNormal
         """
-        if not isinstance(face_id, list):
-            face_id = [face_id]
-        selections = self.convert_to_selections(obj_name)
+        if not isinstance(faces, list):
+            faces = [faces]
+        selections = self.convert_to_selections(assignment)
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:Parameters"]
         vArg2.append(
             [
                 "NAME:SweepFaceAlongNormalToParameters",
                 "FacesToDetach:=",
-                face_id,
+                faces,
                 "LengthOfSweep:=",
                 self._arg_with_dim(sweep_value),
             ]
         )
 
         objs = self._all_object_names
         self.oeditor.SweepFacesAlongNormal(vArg1, vArg2)
@@ -3043,21 +3056,21 @@
         if obj:
             if len(obj) > 1:
                 return [self.update_object(self[o]) for o in obj]
             else:
                 return self.update_object(self[obj[0]])
         return False
 
-    @pyaedt_function_handler()
-    def sweep_along_vector(self, objid, sweep_vector, draft_angle=0, draft_type="Round"):
+    @pyaedt_function_handler(objid="assignment")
+    def sweep_along_vector(self, assignment, sweep_vector, draft_angle=0, draft_type="Round"):
         """Sweep the selection along a vector.
 
         Parameters
         ----------
-        objid : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
         sweep_vector : float
             List of ``[x1, y1, z1]`` coordinates or Application.Position object for
             the vector.
         draft_angle : float, optional
             Draft angle in degrees. The default is ``0``.
         draft_type : str
@@ -3070,43 +3083,49 @@
             One or more objects created.
 
         References
         ----------
 
         >>> oEditor.SweepAlongVector
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
         vectorx, vectory, vectorz = self._pos_with_arg(sweep_vector)
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:VectorSweepParameters"]
         vArg2.append("DraftAngle:="), vArg2.append(self._arg_with_dim(draft_angle, "deg"))
         vArg2.append("DraftType:="), vArg2.append(GeometryOperators.draft_type_str(draft_type))
         vArg2.append("SweepVectorX:="), vArg2.append(vectorx)
         vArg2.append("SweepVectorY:="), vArg2.append(vectory)
         vArg2.append("SweepVectorZ:="), vArg2.append(vectorz)
 
         self.oeditor.SweepAlongVector(vArg1, vArg2)
 
-        if isinstance(objid, list):
+        if isinstance(assignment, list):
             updated_obj = []
-            for sel_obj in objid:
+            for sel_obj in assignment:
                 updated_obj.append(self.update_object(sel_obj))
             return updated_obj
         else:
-            return self.update_object(objid)
+            return self.update_object(assignment)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(objid="assignment")
     def sweep_along_path(
-        self, objid, sweep_object, draft_angle=0, draft_type="Round", is_check_face_intersection=False, twist_angle=0
+        self,
+        assignment,
+        sweep_object,
+        draft_angle=0,
+        draft_type="Round",
+        is_check_face_intersection=False,
+        twist_angle=0,
     ):
         """Sweep the selection along a path.
 
         Parameters
         ----------
-        objid : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
         sweep_object : str, int
             Name or ID of the sweep.
         draft_angle : float, optional
             Draft angle in degrees. The default is ``0``.
         draft_type : str
             Type of the draft. Options are ``"Round"``, ``"Natural"``,
@@ -3122,35 +3141,35 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.SweepAlongPath
         """
-        selections = self.convert_to_selections(objid) + "," + self.convert_to_selections(sweep_object)
+        selections = self.convert_to_selections(assignment) + "," + self.convert_to_selections(sweep_object)
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:PathSweepParameters"]
         vArg2.append("DraftAngle:="), vArg2.append(self._arg_with_dim(draft_angle, "deg"))
         vArg2.append("DraftType:="), vArg2.append(GeometryOperators.draft_type_str(draft_type))
         vArg2.append("CheckFaceFaceIntersection:="), vArg2.append(is_check_face_intersection)
         vArg2.append("TwistAngle:="), vArg2.append(str(twist_angle) + "deg")
 
         self.oeditor.SweepAlongPath(vArg1, vArg2)
 
-        return self.update_object(objid)
+        return self.update_object(assignment)
 
-    @pyaedt_function_handler()
-    def sweep_around_axis(self, objid, cs_axis, sweep_angle=360, draft_angle=0, number_of_segments=0):
+    @pyaedt_function_handler(objid="assignment", cs_axis="axis")
+    def sweep_around_axis(self, assignment, axis, sweep_angle=360, draft_angle=0, number_of_segments=0):
         """Sweep the selection around the axis.
 
         Parameters
         ----------
-        objid : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, :class:`pyaedt.modeler.Object3d.Object3d`
             Name or ID of the object.
-        cs_axis :
+        axis :
             Coordinate system axis or the Application.AXIS object.
         sweep_angle : float
             Sweep angle in degrees. The default is ``360``.
         draft_angle : float
             Draft angle in degrees. The default is ``0``.
         number_of_segments : int, optional
             Number of segments of the sweep operation. Default is ``0``.
@@ -3161,44 +3180,44 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.SweepAroundAxis
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = [
             "NAME:AxisSweepParameters",
             "DraftAngle:=",
             self._arg_with_dim(draft_angle, "deg"),
             "DraftType:=",
             "Round",
             "CheckFaceFaceIntersection:=",
             False,
             "SweepAxis:=",
-            GeometryOperators.cs_axis_str(cs_axis),
+            GeometryOperators.cs_axis_str(axis),
             "SweepAngle:=",
             self._arg_with_dim(sweep_angle, "deg"),
             "NumOfSegments:=",
             str(number_of_segments),
         ]
 
         self.oeditor.SweepAroundAxis(vArg1, vArg2)
 
-        return self.update_object(objid)
+        return self.update_object(assignment)
 
-    @pyaedt_function_handler()
-    def section(self, object_list, plane, create_new=True, section_cross_object=False):
+    @pyaedt_function_handler(object_list="assignment")
+    def section(self, assignment, plane, create_new=True, section_cross_object=False):
         """Section the selection.
 
         Parameters
         ----------
-        object_list : list, str, int, or  :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : list, str, int, or  :class:`pyaedt.modeler.Object3d.Object3d`
             One or more objects to section.
         plane : str
             Coordinate plane or Application.PLANE object.
             Choices for the coordinate plane are ``"XY"``, ``"YZ"``, and ``"ZX"``.'
         create_new : bool, optional
             The default is ``True``, but this parameter has no effect.
         section_cross_object : bool, optional
@@ -3212,15 +3231,15 @@
         References
         ----------
 
         >>> oEditor.Section
         """
         section_plane = GeometryOperators.cs_plane_to_plane_str(plane)
 
-        selections = self.convert_to_selections(object_list)
+        selections = self.convert_to_selections(assignment)
 
         self.oeditor.Section(
             ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"],
             [
                 "NAME:SectionToParameters",
                 "CreateNewObjects:=",
                 create_new,
@@ -3229,21 +3248,21 @@
                 "SectionCrossObject:=",
                 section_cross_object,
             ],
         )
         self.refresh_all_ids()
         return True
 
-    @pyaedt_function_handler()
-    def separate_bodies(self, object_list, create_group=False):
+    @pyaedt_function_handler(object_list="assignment")
+    def separate_bodies(self, assignment, create_group=False):
         """Separate bodies of the selection.
 
         Parameters
         ----------
-        object_list : list, str
+        assignment : list, str
             List of objects to separate.
         create_group : bool, optional
             Whether to create a group. The default is ``False``.
 
         Returns
         -------
         pyaedt.modeler.Object3d.Object3d, bool
@@ -3252,15 +3271,15 @@
 
         References
         ----------
 
         >>> oEditor.SeparateBody
         """
         try:
-            selections = self.convert_to_selections(object_list)
+            selections = self.convert_to_selections(assignment)
             all_objs = [i for i in self.object_names]
             self.oeditor.SeparateBody(
                 ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"],
                 ["CreateGroupsForNewObjects:=", create_group],
             )
             self.refresh_all_ids()
             new_objects_list_names = [selections] + [i for i in self.object_names if i not in all_objs]
@@ -3269,46 +3288,50 @@
                 for new_obj in new_objects_list_names:
                     if obj.name == new_obj:
                         new_objects_list.append(obj)
             return new_objects_list
         except Exception:
             return False
 
-    @pyaedt_function_handler()
-    def rotate(self, objid, cs_axis, angle=90.0, unit="deg"):
+    @pyaedt_function_handler(
+        objid="assignment",
+        cs_axis="axis",
+        unit="units",
+    )
+    def rotate(self, assignment, axis, angle=90.0, units="deg"):
         """Rotate the selection.
 
         Parameters
         ----------
-        objid :  list, str, int, or  :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment :  list, str, int, or  :class:`pyaedt.modeler.Object3d.Object3d`
              ID of the object.
-        cs_axis
+        axis : str
             Coordinate system axis or the Application.AXIS object.
-        angle : float
+        angle : float, str
             Angle of rotation. The units, defined by ``unit``, can be either
             degrees or radians. The default is ``90.0``.
-        unit : text, optional
+        units : text, optional
              Units for the angle. Options are ``"deg"`` or ``"rad"``.
              The default is ``"deg"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Rotate
         """
-        selections = self.convert_to_selections(objid)
+        selections = self.convert_to_selections(assignment)
         vArg1 = ["NAME:Selections", "Selections:=", selections, "NewPartsModelFlag:=", "Model"]
         vArg2 = ["NAME:RotateParameters"]
-        vArg2.append("RotateAxis:="), vArg2.append(GeometryOperators.cs_axis_str(cs_axis))
-        vArg2.append("RotateAngle:="), vArg2.append(self._arg_with_dim(angle, unit))
+        vArg2.append("RotateAxis:="), vArg2.append(GeometryOperators.cs_axis_str(axis))
+        vArg2.append("RotateAngle:="), vArg2.append(self._arg_with_dim(angle, units))
 
         if self.oeditor is not None:
             self.oeditor.Rotate(vArg1, vArg2)
 
         return True
 
     @pyaedt_function_handler()
@@ -3410,25 +3433,25 @@
             varg2.append(self._app.value_with_units(vector_direction[2]))
 
         self.oeditor.ImprintProjection(varg1, varg2)
         if not keep_originals:
             self.cleanup_objects()
         return True
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler(tool_list="assignment")
     def imprint_normal_projection(
         self,
-        tool_list,
+        assignment,
         keep_originals=True,
     ):
         """Imprint the normal projection of objects over a sheet.
 
         Parameters
         ----------
-        tool_list : list
+        assignment : list
             List of objects to imprint. The list can be of
             either Object3d objects or object IDs.
         keep_originals : bool, optional
             Whether to keep the original objects. The default is ``True``.
 
         Returns
         -------
@@ -3436,29 +3459,29 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ImprintProjection
         """
-        return self._imprint_projection(tool_list, keep_originals, True)
+        return self._imprint_projection(assignment, keep_originals, True)
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler(tool_list="assignment")
     def imprint_vector_projection(
         self,
-        tool_list,
+        assignment,
         vector_points,
         distance,
         keep_originals=True,
     ):
         """Imprint the projection of objects over a sheet with a specified vector and distance.
 
         Parameters
         ----------
-        tool_list : list
+        assignment : list
             List of objects to imprint. The list can be of
             either Object3d objects or object IDs.
         vector_points : list
             List of [x,y,z] vector projection.
         distance : str, int
             Distance of Projection.
         keep_originals : bool, optional
@@ -3470,36 +3493,36 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ImprintProjection
         """
-        return self._imprint_projection(tool_list, keep_originals, False, vector_points, distance)
+        return self._imprint_projection(assignment, keep_originals, False, vector_points, distance)
 
-    @pyaedt_function_handler()
-    def purge_history(self, theList):
+    @pyaedt_function_handler(theList="assignment")
+    def purge_history(self, assignment):
         """Purge history objects from object names.
 
         Parameters
         ----------
-        theList : list
+        assignment : list
             List of object names to purge.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.PurgeHistory
         """
-        szList = self.convert_to_selections(theList)
+        szList = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", szList, "NewPartsModelFlag:=", "Model"]
 
         self.oeditor.PurgeHistory(vArg1)
         return True
 
     @pyaedt_function_handler()
@@ -3518,21 +3541,21 @@
 
         >>> oEditor.GetModelBoundingBox
         """
         bb = list(self.oeditor.GetModelBoundingBox())
         bound = [float(b) for b in bb]
         return bound
 
-    @pyaedt_function_handler()
-    def unite(self, unite_list, purge=False, keep_originals=False):
+    @pyaedt_function_handler(unite_list="assignment")
+    def unite(self, assignment, purge=False, keep_originals=False):
         """Unite objects from a list.
 
         Parameters
         ----------
-        unite_list : list, str
+        assignment : list, str
             List of objects to unite.
         purge : bool, optional
             Purge history after unite. Default is False.
         keep_originals : bool, optional
             Keep original objects used for the operation. Default is False.
 
         Returns
@@ -3541,20 +3564,20 @@
             The united object that is the first in the list.
 
         References
         ----------
 
         >>> oEditor.Unite
         """
-        slice = min(100, len(unite_list))
-        num_objects = len(unite_list)
+        slice = min(100, len(assignment))
+        num_objects = len(assignment)
         remaining = num_objects
         objs_groups = []
         while remaining > 1:
-            objs = unite_list[:slice]
+            objs = assignment[:slice]
             szSelections = self.convert_to_selections(objs)
             vArg1 = ["NAME:Selections", "Selections:=", szSelections]
             vArg2 = ["NAME:UniteParameters", "KeepOriginals:=", keep_originals]
             if settings.aedt_version > "2022.2":
                 vArg2.append("TurnOnNBodyBoolean:=")
                 vArg2.append(True)
             self.oeditor.Unite(vArg1, vArg2)
@@ -3564,30 +3587,30 @@
                 self.cleanup_objects()
                 return False
             elif purge:
                 self.purge_history(objs[0])
             objs_groups.append(objs[0])
             remaining -= slice
             if remaining > 0:
-                unite_list = unite_list[slice:]
+                assignment = assignment[slice:]
         if remaining > 0:
-            objs_groups.extend(unite_list)
+            objs_groups.extend(assignment)
         self.cleanup_objects()
         if len(objs_groups) > 1:
             return self.unite(objs_groups, purge=purge)
         self.logger.info("Union of {} objects has been executed.".format(num_objects))
-        return self.convert_to_selections(unite_list[0], False)
+        return self.convert_to_selections(assignment[0], False)
 
-    @pyaedt_function_handler()
-    def clone(self, objid):
+    @pyaedt_function_handler(objid="assignment")
+    def clone(self, assignment):
         """Clone objects from a list of object IDs.
 
         Parameters
         ----------
-        objid : list
+        assignment : list
             List of object IDs.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         List
@@ -3595,25 +3618,25 @@
 
         References
         ----------
 
         >>> oEditor.Copy
         >>> oEditor.Paste
         """
-        self.copy(objid)
+        self.copy(assignment)
         new_objects = self.paste()
         return True, new_objects
 
-    @pyaedt_function_handler()
-    def copy(self, object_list):
+    @pyaedt_function_handler(object_list="assignment")
+    def copy(self, assignment):
         """Copy objects to the clipboard.
 
             Parameters
             ----------
-            object_list : list
+            assignment : list
                 List of objects (IDs or names).
 
             Returns
             -------
             list
                 List of names of the objects copied when successful.
 
@@ -3621,15 +3644,15 @@
         ----------
 
         >>> oEditor.Copy
         """
         # convert to string
 
         try:
-            selections = self.convert_to_selections(object_list)
+            selections = self.convert_to_selections(assignment)
             vArg1 = ["NAME:Selections", "Selections:=", selections]
             self.oeditor.Copy(vArg1)
             return selections
         except AttributeError:
             self.logger.error("Unable to copy selections to clipboard.")
             return None
 
@@ -3647,21 +3670,21 @@
 
         >>> oEditor.Paste
         """
         self.oeditor.Paste()
         new_objects = self.add_new_objects()
         return new_objects
 
-    @pyaedt_function_handler()
-    def intersect(self, theList, keep_originals=False, **kwargs):
+    @pyaedt_function_handler(theList="assignment")
+    def intersect(self, assignment, keep_originals=False, **kwargs):
         """Intersect objects from a list.
 
         Parameters
         ----------
-        theList : list
+        assignment : list
             List of objects.
         keep_originals : bool, optional
             Whether to keep the original object. The default is ``False``.
 
         Returns
         -------
         str
@@ -3672,36 +3695,70 @@
 
         >>> oEditor.Intersect
         """
         if "keeporiginal" in kwargs:
             warnings.warn("keeporiginal has been deprecated. use keep_originals.", DeprecationWarning)
             keep_originals = kwargs["keeporiginal"]
         unclassified = list(self.oeditor.GetObjectsInGroup("Unclassified"))
-        szSelections = self.convert_to_selections(theList)
+        szSelections = self.convert_to_selections(assignment)
 
         vArg1 = ["NAME:Selections", "Selections:=", szSelections]
         vArg2 = ["NAME:IntersectParameters", "KeepOriginals:=", keep_originals]
 
         self.oeditor.Intersect(vArg1, vArg2)
         unclassified1 = list(self.oeditor.GetObjectsInGroup("Unclassified"))
         if unclassified != unclassified1:
             self._odesign.Undo()
             self.logger.error("Error in intersection. Reverting Operation")
             return
         self.cleanup_objects()
         self.logger.info("Intersection Succeeded")
-        return self.convert_to_selections(theList[0], False)
+        return self.convert_to_selections(assignment[0], False)
 
     @pyaedt_function_handler()
-    def connect(self, theList):
+    def detach_faces(self, assignment, faces):
+        """Section the object.
+
+        Parameters
+        ----------
+        assignment : Object3d or str
+            Object from which to detach faces.
+        faces : List[FacePrimitive] or List[int] or int or FacePrimitive
+            Face or faces to detach from the object.
+
+        Returns
+        -------
+        List[:class:`pyaedt.modeler.cad.object3d.Object3d`]
+            List of objects resulting from the operation (including the original one).
+
+        References
+        ----------
+
+        >>> oEditor.DetachFaces
+
+        """
+        if isinstance(assignment, str):
+            assignment = self._modeler[assignment]
+        if isinstance(faces, FacePrimitive) or isinstance(faces, int):
+            faces = [faces]
+        if isinstance(faces[0], FacePrimitive):
+            faces = [f.id for f in faces]
+        result = self.oeditor.DetachFaces(
+            ["NAME:Selections", "Selections:=", assignment.name, "NewPartsModelFlag:=", "Model"],
+            ["NAME:Parameters", ["NAME:DetachFacesToParameters", "FacesToDetach:=", faces]],
+        )
+        return [assignment] + [self._modeler[o] for o in result]
+
+    @pyaedt_function_handler(theList="assignment")
+    def connect(self, assignment):
         """Connect objects from a list.
 
         Parameters
         ----------
-        theList : list
+        assignment : list
             List of objects.
 
         Returns
         -------
         pyaedt.modeler.Object3d.Object3d, bool
             3D object.
             ``False`` when failed.
@@ -3709,15 +3766,15 @@
         References
         ----------
 
         >>> oEditor.Connect
         """
         try:
             unclassified_before = list(self.unclassified_names)
-            szSelections = self.convert_to_selections(theList)
+            szSelections = self.convert_to_selections(assignment)
             szSelections_list = szSelections.split(",")
             vArg1 = ["NAME:Selections", "Selections:=", szSelections]
 
             self.oeditor.Connect(vArg1)
             if unclassified_before != self.unclassified_names:
                 self._odesign.Undo()
                 self.logger.error("Error in connection. Reverting Operation")
@@ -3807,45 +3864,45 @@
             off3 = 0
         elif i != 4 and i != 7 and i != 8 and i != 11:
             off3 = -offset
         else:
             off3 = +offset
         return off1, off2, off3
 
-    @pyaedt_function_handler()
-    def check_plane(self, obj, faceposition, offset=1):
+    @pyaedt_function_handler(obj="assignment", face_position="face_location")
+    def check_plane(self, assignment, face_location, offset=1):
         """Check for the plane that is defined as the face for an object.
 
         Parameters
         ----------
-        obj : str
+        assignment : str
             Name of the object.
-        faceposition : list
+        face_location : list
             List of the ``[x, y, z]`` coordinates for the position of the face.
         offset : optional
             Offset to apply. The default is ``1``.
 
         Returns
         -------
         str
             Name of the plane. It can be "XY", "XZ" or "YZ".
 
         """
 
-        Xvec, Yvec, Zvec = self._pos_with_arg(faceposition)
+        Xvec, Yvec, Zvec = self._pos_with_arg(face_location)
 
-        if isinstance(obj, int):
-            obj = self.objects[obj].name
+        if isinstance(assignment, int):
+            assignment = self.objects[assignment].name
         plane = None
         found = False
         i = 0
         while not found:
             off1, off2, off3 = self._offset_on_plane(i, offset)
             vArg1 = ["NAME:FaceParameters"]
-            vArg1.append("BodyName:="), vArg1.append(obj)
+            vArg1.append("BodyName:="), vArg1.append(assignment)
             vArg1.append("XPosition:="), vArg1.append(Xvec + "+" + self._arg_with_dim(off1))
             vArg1.append("YPosition:="), vArg1.append(Yvec + "+" + self._arg_with_dim(off2))
             vArg1.append("ZPosition:="), vArg1.append(Zvec + "+" + self._arg_with_dim(off3))
             try:
                 face_id = self.oeditor.GetFaceByPosition(vArg1)
                 if i < 4:
                     plane = "XY"
@@ -3911,28 +3968,28 @@
             RenameArgs = {}
             RenameArgs["NAME"] = "Rename Data"
             RenameArgs["Old Name"] = name
             RenameArgs["New Name"] = name.replace(CADSuffix, "")
             self.oeditor.RenamePart(RenameArgs)
         return True
 
-    @pyaedt_function_handler()
-    def create_airbox(self, offset=0, offset_type="Absolute", defname="AirBox_Auto"):
+    @pyaedt_function_handler(defname="name")
+    def create_airbox(self, offset=0, offset_type="Absolute", name="AirBox_Auto"):
         """Create an airbox that is as big as the bounding extension of the project.
 
         Parameters
         ----------
         offset :
             Double offset value to apply on the airbox faces versus the bounding box.
             The default is ``0``.
         offset_type : str
             Type of the offset. Options are ``"Absolute"`` and ``"Relative"``.
             The default is ``"Absolute"``. If ``"Relative"``, the offset input
             is between 0 and 100.
-        defname : str, optional
+        name : str, optional
             Name of the airbox. The default is ``"AirBox_Auto"``.
 
         Returns
         -------
         int
             ID of the airbox created.
 
@@ -3952,15 +4009,15 @@
             offset3 = (bound[5] - bound[2]) * offset / 100
         startpos = self.Position(bound[0] - offset1, bound[1] - offset2, bound[2] - offset3)
 
         dim = []
         dim.append(bound[3] - bound[0] + 2 * offset1)
         dim.append(bound[4] - bound[1] + 2 * offset2)
         dim.append(bound[5] - bound[2] + 2 * offset3)
-        airid = self.create_box(startpos, dim, defname)
+        airid = self.create_box(startpos, dim, name)
         return airid
 
     @pyaedt_function_handler()
     def create_air_region(self, x_pos=0, y_pos=0, z_pos=0, x_neg=0, y_neg=0, z_neg=0, is_percentage=True):
         """Create an air region.
 
         Parameters
@@ -4000,21 +4057,21 @@
         References
         ----------
 
         >>> oEditor.CreateRegion
         """
         return self.create_region(pad_percent=[x_pos, y_pos, z_pos, x_neg, y_neg, z_neg], is_percentage=is_percentage)
 
-    @pyaedt_function_handler()
-    def edit_region_dimensions(self, listvalues):
+    @pyaedt_function_handler(listvalues="values")
+    def edit_region_dimensions(self, values):
         """Modify the dimensions of the region.
 
         Parameters
         ----------
-        listvalues : list
+        values : list
             List of the padding percentages along all six directions in
             the form ``[+X, -X, +Y, -Y, +Z, -Z]``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
@@ -4024,32 +4081,32 @@
 
         >>> oEditor.ChangeProperty
         """
         arg = ["NAME:AllTabs"]
         arg2 = ["NAME:Geometry3DCmdTab", ["NAME:PropServers", "Region:CreateRegion:1"]]
         arg3 = ["NAME:ChangedProps"]
         p = ["+X", "-X", "+Y", "-Y", "+Z", "-Z"]
-        for label, value in zip(p, listvalues):
+        for label, value in zip(p, values):
             padding = []
             padding.append("NAME:" + label + " Padding Data")
             padding.append("Value:=")
             padding.append(str(value))
             arg3.append(padding)
         arg2.append(arg3)
         arg.append(arg2)
         self.oeditor.ChangeProperty(arg)
         return True
 
-    @pyaedt_function_handler()
-    def create_face_list(self, face_list, name=None):
+    @pyaedt_function_handler(face_list="assignment")
+    def create_face_list(self, assignment, name=None):
         """Create a list of faces given a list of face ID or a list of objects.
 
         Parameters
         ----------
-        face_list : list
+        assignment : list
             List of face ID or list of objects
 
         name : str, optional
            Name of the new list.
 
         Returns
         -------
@@ -4062,39 +4119,35 @@
         >>> oEditor.CreateEntityList
         """
         if name:
             for i in self.user_lists:
                 if i.name == name:
                     self.logger.warning("A List with the specified name already exists!")
                     return i
-        face_list = self.convert_to_selections(face_list, True)
+        assignment = self.convert_to_selections(assignment, True)
         user_list = Lists(self)
         list_type = "Face"
         if user_list:
-            result = user_list.create(
-                object_list=face_list,
-                name=name,
-                type=list_type,
-            )
+            result = user_list.create(assignment=assignment, name=name, entity_type=list_type)
             if result:
                 return user_list
             else:
                 self._app.logger.error("Wrong object definition. Review object list and type")
                 return False
         else:
             self._app.logger.error("User list object could not be created")
             return False
 
-    @pyaedt_function_handler()
-    def create_object_list(self, object_list, name=None):
+    @pyaedt_function_handler(object_list="assignment")
+    def create_object_list(self, assignment, name=None):
         """Create an object list given a list of object names.
 
         Parameters
         ----------
-        object_list : list
+        assignment : list
             List of object names.
         name : str, optional
             Name of the new object list.
 
         Returns
         -------
         :class:`pyaedt.modeler.Modeler.Lists`
@@ -4106,80 +4159,76 @@
         >>> oEditor.CreateEntityList
         """
         if name:
             for i in self.user_lists:
                 if i.name == name:
                     self.logger.warning("A List with the specified name already exists!")
                     return i
-        object_list = self.convert_to_selections(object_list, True)
+        assignment = self.convert_to_selections(assignment, True)
         user_list = Lists(self)
         list_type = "Object"
         if user_list:
-            result = user_list.create(
-                object_list=object_list,
-                name=name,
-                type=list_type,
-            )
+            result = user_list.create(assignment=assignment, name=name, entity_type=list_type)
             if result:
                 return user_list
             else:
                 self._app.logger.error("Wrong object definition. Review object list and type")
                 return False
         else:
             self._app.logger.error("User list object could not be created")
             return False
 
-    @pyaedt_function_handler()
-    def generate_object_history(self, objectname):
+    @pyaedt_function_handler(objectname="assignment")
+    def generate_object_history(self, assignment):
         """Generate history for the object.
 
         Parameters
         ----------
-        objectname : str
+        assignment : str
             Name of the history object.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.GenerateHistory
         """
-        objectname = self.convert_to_selections(objectname)
+        assignment = self.convert_to_selections(assignment)
         self.oeditor.GenerateHistory(
-            ["NAME:Selections", "Selections:=", objectname, "NewPartsModelFlag:=", "Model", "UseCurrentCS:=", True]
+            ["NAME:Selections", "Selections:=", assignment, "NewPartsModelFlag:=", "Model", "UseCurrentCS:=", True]
         )
         self.cleanup_objects()
         return True
 
-    @pyaedt_function_handler()
-    def create_faceted_bondwire_from_true_surface(self, bondname, bond_direction, min_size=0.2, numberofsegments=8):
+    @pyaedt_function_handler(bondname="assignment", bond_direction="direction", numberofsegments="number_of_segments")
+    def create_faceted_bondwire_from_true_surface(self, assignment, direction, min_size=0.2, number_of_segments=8):
         """Create a faceted bondwire from an existing true surface bondwire.
 
         Parameters
         ----------
-        bondname : str
+        assignment : str
             Name of the bondwire to replace.
-        bond_direction : list
+        direction : list
             List of the ``[x, y, z]`` coordinates for the axis direction
             of the bondwire. For example, ``[0, 1, 2]``.
         min_size : float
             Minimum size of the subsegment of the new polyline. The default is ``0.2``.
-        numberofsegments : int, optional
+        number_of_segments : int, optional
             Number of segments. The default is ``8``.
 
         Returns
         -------
         str
             Name of the bondwire created.
         """
-        old_bondwire = self.get_object_from_name(bondname)
+        old_bondwire = self.get_object_from_name(assignment)
         if not old_bondwire:
             return False
         edges = old_bondwire.edges
         faces = old_bondwire.faces
         centers = []
         for el in faces:
             center = el.center
@@ -4192,15 +4241,15 @@
             if len(ver) < 2:
                 continue
             p1 = ver[0].position
             p2 = ver[1].position
             p3 = [abs(i - j) for i, j in zip(p1, p2)]
 
             dir = p3.index(max(p3))
-            if dir == bond_direction:
+            if dir == direction:
                 edgelist.append(el)
                 verlist.append([p1, p2])
         if not edgelist:
             self.logger.error("No edges found specified direction. Check again")
             return False
         connected = [edgelist[0]]
         tol = 1e-6
@@ -4256,23 +4305,23 @@
         move_vector = None
         for fc in centers:
             dist = GeometryOperators.points_distance(fc, first_vert)
             if dist < rad:
                 rad = dist
                 move_vector = GeometryOperators.v_sub(fc, first_vert)
 
-        P = self.get_existing_polyline(object=new_edges[0])
+        P = self.get_existing_polyline(assignment=new_edges[0])
 
         if edge_to_delete:
             P.remove_edges(edge_to_delete)
 
-        angle = math.pi * (180 - 360 / numberofsegments) / 360
+        angle = math.pi * (180 - 360 / number_of_segments) / 360
 
         status = P.set_crosssection_properties(
-            type="Circle", num_seg=numberofsegments, width=(rad * (2 - math.sin(angle))) * 2
+            type="Circle", num_seg=number_of_segments, width=(rad * (2 - math.sin(angle))) * 2
         )
         if status:
             self.move(new_edges[0], move_vector)
             old_bondwire.model = False
             return new_edges[0]
         else:
             return False
@@ -4295,109 +4344,109 @@
         ----------
 
         >>> oEditor.GetEntityListIDByName
         """
         id = self.oeditor.GetEntityListIDByName(name)
         return id
 
-    @pyaedt_function_handler()
-    def create_outer_facelist(self, externalobjects, name="outer_faces"):
+    @pyaedt_function_handler(externalobjects="assignment")
+    def create_outer_facelist(self, assignment, name="outer_faces"):
         """Create a face list from a list of outer objects.
 
         Parameters
         ----------
-        externalobjects : list
+        assignment : list
             List of outer objects.
         name : str, optional
             Name of the new list. The default is ``"outer_faces"``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        list2 = self.select_allfaces_fromobjects(externalobjects)  # find ALL faces of outer objects
+        list2 = self.select_allfaces_fromobjects(assignment)  # find ALL faces of outer objects
         self.create_face_list(list2, name)
         self.logger.info("Extfaces of thermal model = " + str(len(list2)))
         return True
 
-    @pyaedt_function_handler()
-    def explicitly_subtract(self, diellist, metallist):
+    @pyaedt_function_handler(diellist="tool_parts", metallist="blank_parts")
+    def explicitly_subtract(self, tool_parts, blank_parts):
         """Explicitly subtract all elements in a SolveInside list and a SolveSurface list.
 
         Parameters
         ----------
-        diellist : list
+        tool_parts : list
             List of dielectrics.
-        metallist : list
+        blank_parts : list
             List of metals.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Subtract
         >>> oEditor.PurgeHistory
         """
         self.logger.info("Creating explicit subtraction between objects.")
-        for el in diellist:
+        for el in tool_parts:
             list1 = el
             list2 = ""
-            for el1 in metallist:
+            for el1 in blank_parts:
                 list2 = list2 + el1 + ","
-            for el1 in diellist:
+            for el1 in tool_parts:
                 if el1 is not el:
                     list2 = list2 + el1 + ","
             if list2:
                 list2 = list2[:-1]
                 self.subtract(list1, list2, True)
                 self.purge_history(list1)
                 self.purge_history(list2)
-        for el in metallist:
+        for el in blank_parts:
             list1 = el
             list2 = ""
-            for el1 in metallist:
+            for el1 in blank_parts:
                 if el1 is not el:
                     list2 = list2 + el1 + ","
             if list2:
                 list2 = list2[:-1]
                 self.subtract(list1, list2, True)
                 self.purge_history(list1)
                 self.purge_history(list2)
         self.logger.info("Explicit subtraction is completed.")
         return True
 
-    @pyaedt_function_handler()
-    def find_port_faces(self, port_sheets):
+    @pyaedt_function_handler(port_sheets="assignment")
+    def find_port_faces(self, assignment):
         """Find the vacuums given a list of input sheets.
 
         Starting from a list of input sheets, this method creates a list of output sheets
         that represent the blank parts (vacuums) and the tool parts of all the intersections
         of solids on the sheets. After a vacuum on a sheet is found, a port can be
         created on it.
 
         Parameters
         ----------
-        port_sheets : list
+        assignment : list
             List of input sheets names.
 
         Returns
         -------
         List
             List of output sheets (`2x len(port_sheets)`).
 
         """
         faces = []
         solids = [s for s in self.solid_objects if s.material_name not in ["vacuum", "air"] and s.model]
-        for sheet_name in port_sheets:
+        for sheet_name in assignment:
             sheet = self[sheet_name]  # get the sheet object
             _, cloned = self.clone(sheet)
             cloned = self[cloned[0]]
             cloned.subtract(solids)
             sheet.subtract(cloned)
             cloned.name = sheet.name + "_Face1Vacuum"
             faces.append(sheet.name)
@@ -4435,21 +4484,21 @@
         oBoundingBox = list(self.oeditor.GetModelBoundingBox())
         dimensions = []
         dimensions.append(abs(float(oBoundingBox[0]) - float(oBoundingBox[3])))
         dimensions.append(abs(float(oBoundingBox[1]) - float(oBoundingBox[4])))
         dimensions.append(abs(float(oBoundingBox[2]) - float(oBoundingBox[5])))
         return dimensions
 
-    @pyaedt_function_handler()
-    def get_object_name_from_edge_id(self, edge_id):
+    @pyaedt_function_handler(edge_id="assignment")
+    def get_object_name_from_edge_id(self, assignment):
         """Retrieve the object name for a predefined edge ID.
 
         Parameters
         ----------
-        edge_id : int
+        assignment : int
             ID of the edge.
 
         Returns
         -------
         str
             Name of the edge if it exists, ``False`` otherwise.
 
@@ -4457,15 +4506,15 @@
         ----------
 
         >>> oEditor.GetEdgeIDsFromObject
         """
         for object in self.solid_names + self.sheet_names + self.line_names:
             try:
                 oEdgeIDs = self.oeditor.GetEdgeIDsFromObject(object)
-                if str(edge_id) in oEdgeIDs:
+                if str(assignment) in oEdgeIDs:
                     return object
             except Exception:
                 return False
         return False
 
     @pyaedt_function_handler()
     def get_solving_volume(self):
@@ -4482,46 +4531,46 @@
         >>> oEditor.GetModelBoundingBox
         """
         bound = self.get_model_bounding_box()
         volume = abs(bound[3] - bound[0]) * abs(bound[4] - bound[1]) * abs(bound[5] - bound[2])
         volume = str(round(volume, 0))
         return volume
 
-    @pyaedt_function_handler()
-    def vertex_data_of_lines(self, txtfilter=None):
+    @pyaedt_function_handler(txtfilter="text_filter")
+    def vertex_data_of_lines(self, text_filter=None):
         """Generate a dictionary of line vertex data for all lines contained within the design.
 
         Parameters
         ----------
-        txtfilter : str, optional
+        text_filter : str, optional
             Text string for filtering. The default is ``None``. When a text string is specified,
             line data is generated only if this text string is contained within the line name.
 
         Returns
         -------
         dict
             Dictionary of the line name with a list of vertex positions in either 2D or 3D.
 
         """
         line_data = {}
         lines = self.get_line_ids()
-        if txtfilter is not None:
-            lines = [n for n in lines if txtfilter in n]
+        if text_filter is not None:
+            lines = [n for n in lines if text_filter in n]
         for x in lines:
             line_data[x] = self.get_vertices_of_line(x)
 
         return line_data
 
-    @pyaedt_function_handler()
-    def get_vertices_of_line(self, sLineName):
+    @pyaedt_function_handler(sLineName="assignment")
+    def get_vertices_of_line(self, assignment):
         """Generate a list of vertex positions for a line object from AEDT in model units.
 
         Parameters
         ----------
-        sLineName : str
+        assignment : str
             Name of the line object in AEDT.
 
         Returns
         -------
         list
             List of the ``[x, y, (z)]`` coordinates for the 2D or 3D line object.
 
@@ -4529,15 +4578,15 @@
         ----------
 
         >>> oEditor.GetVertexIDsFromObject
         """
         position_list = []
 
         # Get all vertices in the line
-        vertices_on_line = self.oeditor.GetVertexIDsFromObject(sLineName)
+        vertices_on_line = self.oeditor.GetVertexIDsFromObject(assignment)
 
         if settings.aedt_version > "2022.2":
             vertices_on_line = vertices_on_line[::-1]
 
         for x in vertices_on_line:
             pos = self.oeditor.GetVertexPosition(x)
             if self.design_type == "Maxwell 2D":
@@ -4546,33 +4595,33 @@
                 else:
                     position_list.append([float(pos[0]), float(pos[2])])
             else:
                 position_list.append([float(pos[0]), float(pos[1]), float(pos[2])])
 
         return position_list
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(filename="input_file")
     def import_3d_cad(
         self,
-        filename,
+        input_file,
         healing=False,
         refresh_all_ids=True,
         import_materials=False,
         create_lightweigth_part=False,
         group_by_assembly=False,
         create_group=True,
         separate_disjoints_lumped_object=False,
         import_free_surfaces=False,
         point_coicidence_tolerance=1e-6,
     ):
         """Import a CAD model.
 
         Parameters
         ----------
-        filename : str
+        input_file : str
             Full path and name of the CAD file.
         healing : bool, optional
             Whether to perform healing. The default is ``False``, in which
             case healing is not performed.
         healing : int, optional
             Whether to perform healing. The default is ``0``, in which
             case healing is not performed.
@@ -4620,28 +4669,28 @@
         vArg1.append("CreateGroup:="), vArg1.append(create_group)
         vArg1.append("STLFileUnit:="), vArg1.append("Auto")
         vArg1.append("MergeFacesAngle:="), vArg1.append(-1)
         vArg1.append("PointCoincidenceTol:="), vArg1.append(point_coicidence_tolerance)
         vArg1.append("CreateLightweightPart:="), vArg1.append(create_lightweigth_part)
         vArg1.append("ImportMaterialNames:="), vArg1.append(import_materials)
         vArg1.append("SeparateDisjointLumps:="), vArg1.append(separate_disjoints_lumped_object)
-        vArg1.append("SourceFile:="), vArg1.append(filename)
+        vArg1.append("SourceFile:="), vArg1.append(input_file)
         self.oeditor.Import(vArg1)
         if refresh_all_ids:
             self.refresh_all_ids()
-        self.logger.info("Step file {} imported".format(filename))
+        self.logger.info("Step file {} imported".format(input_file))
         return True
 
-    @pyaedt_function_handler()
-    def import_spaceclaim_document(self, SCFile):
+    @pyaedt_function_handler(SCFile="input_file")
+    def import_spaceclaim_document(self, input_file):
         """Import a SpaceClaim document.
 
         Parameters
         ----------
-        SCFile :
+        input_file :
             Full path and name of the SpaceClaim file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -4667,15 +4716,15 @@
                 [
                     "NAME:Definition",
                     [
                         "NAME:UDMParam",
                         "Name:=",
                         "GeometryFilePath",
                         "Value:=",
-                        '"' + SCFile + '"',
+                        '"' + input_file + '"',
                         "DataType:=",
                         "String",
                         "PropType2:=",
                         0,
                         "PropFlag2:=",
                         1,
                     ],
@@ -4849,37 +4898,37 @@
                 "ConnectionID:=",
                 "",
             ]
         )
         self.refresh_all_ids()
         return True
 
-    @pyaedt_function_handler()
-    def import_primitives_from_file(self, input_file=None, input_dict=None):
+    @pyaedt_function_handler(input_dict="primitives")
+    def import_primitives_from_file(self, input_file=None, primitives=None):
         """Import and create primitives from a JSON file or dictionary of properties.
 
         Parameters
         ----------
         input_file : str, optional
-            Path to a JSON file containing report settings.
-        input_dict : dict, optional
-            Dictionary containing report settings.
+            Path to a JSON file containing all primitives to import. It can be used in alternative to ``parameters``.
+        primitives : dict, optional
+            Dictionary containing all primitives to import. It can be used in alternative to ``input_file``.
 
         Returns
         -------
         list
             List of created primitives.
 
         Examples
         --------
         >>> from pyaedt import Icepak
         >>> aedtapp = Icepak()
         >>> aedtapp.modeler.import_primitives_from_file(r'C:\\temp\\primitives.json')
         """
-        primitives_builder = PrimitivesBuilder(self._app, input_file, input_dict)
+        primitives_builder = PrimitivesBuilder(self._app, input_file, primitives)
         primitive_names = primitives_builder.create()
         return primitive_names
 
     @pyaedt_function_handler()
     def modeler_variable(self, value):
         """Modeler variable.
 
@@ -4911,46 +4960,46 @@
 
         >>> oEditor.BreakUDMConnection
         """
         args = ["NAME:Selections", "Selections:=", "SpaceClaim1"]
         self.oeditor.BreakUDMConnection(args)
         return True
 
-    @pyaedt_function_handler()
-    def load_scdm_in_hfss(self, SpaceClaimFile):
+    @pyaedt_function_handler(SpaceClaimFile="input_file")
+    def load_scdm_in_hfss(self, input_file):
         """Load a SpaceClaim file in HFSS.
 
         Parameters
         ----------
-        SpaceClaimFile : str
+        input_file : str
             Full path and name of the SpaceClaim file.
 
 
         Returns
         -------
          bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.CreateUserDefinedModel
         >>> oEditor.BreakUDMConnection
         """
-        self.import_spaceclaim_document(SpaceClaimFile)
+        self.import_spaceclaim_document(input_file)
         self.break_spaceclaim_connection()
         return True
 
-    @pyaedt_function_handler()
-    def get_faces_from_materials(self, mats):
+    @pyaedt_function_handler(mats="filter_materials")
+    def get_faces_from_materials(self, filter_materials):
         """Select all outer faces given a list of materials.
 
         Parameters
         ----------
-        mats : list
+        filter_materials : list
             List of materials to include in the search for outer
             faces.
 
         Returns
         -------
         list
             List of all outer faces of the specified materials.
@@ -4961,33 +5010,33 @@
         >>> oEditor.GetObjectsByMaterial
         >>> oEditor.GetFaceIDs
         """
         self.logger.info("Selecting outer faces.")
 
         sel = []
         objs = []
-        if isinstance(mats, str):
-            mats = [mats]
-        for mat in mats:
+        if isinstance(filter_materials, str):
+            filter_materials = [filter_materials]
+        for mat in filter_materials:
             objs.extend(list(self.oeditor.GetObjectsByMaterial(mat.lower())))
 
             for i in objs:
                 oFaceIDs = self.oeditor.GetFaceIDs(i)
 
                 for face in oFaceIDs:
                     sel.append(int(face))
         return sel
 
-    @pyaedt_function_handler()
-    def scale(self, obj_list, x=2.0, y=2.0, z=2.0):
+    @pyaedt_function_handler(obj_list="assignment")
+    def scale(self, assignment, x=2.0, y=2.0, z=2.0):
         """Scale a list of objects.
 
         Parameters
         ----------
-        obj_list : list
+        assignment : list
             List of objects IDs or names.
         x : float, optional
             Scale factor for X.
         y : float, optional
             Scale factor for Y.
         z : float, optional
             Scale factor for Z.
@@ -4998,27 +5047,27 @@
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Scale
         """
-        selections = self.convert_to_selections(obj_list, True)
+        selections = self.convert_to_selections(assignment, True)
         arg1 = ["NAME:Selections", "Selections:=", ", ".join(selections), "NewPartsModelFlag:=", "Model"]
         arg2 = ["NAME:ScaleParameters", "ScaleX:=", str(x), "ScaleY:=", str(y), "ScaleZ:=", str(z)]
         self.oeditor.Scale(arg1, arg2)
         return True
 
-    @pyaedt_function_handler()
-    def select_allfaces_fromobjects(self, elements):
+    @pyaedt_function_handler(elements="assignment")
+    def select_allfaces_fromobjects(self, assignment):
         """Select all outer faces given a list of objects.
 
         Parameters
         ----------
-        elements : list
+        assignment : list
             List of objects to include in the search for outer faces.
 
         Returns
         -------
         List
             List of outer faces in the given list of objects.
 
@@ -5027,15 +5076,15 @@
 
         >>> oEditor.GetFaceIDs
         """
         self.logger.info("Selecting outer faces.")
 
         sel = []
 
-        for i in elements:
+        for i in assignment:
             oFaceIDs = self.oeditor.GetFaceIDs(i)
 
             for face in oFaceIDs:
                 sel.append(int(face))
         return sel
 
     @pyaedt_function_handler()
@@ -5055,29 +5104,31 @@
         oObjects = list(self.oeditor.GetObjectsInGroup("Solids"))
         for obj in oObjects:
             pro = self.oeditor.GetPropertyValue("Geometry3DAttributeTab", obj, "Material")
             if pro == '""':
                 self.oeditor.SetPropertyValue("Geometry3DAttributeTab", obj, "Model", False)
         return True
 
-    @pyaedt_function_handler()
-    def automatic_thicken_sheets(self, inputlist, value, internalExtr=True, internalvalue=1):
+    @pyaedt_function_handler(
+        inputlist="assignment", internalExtr="extrude_internally", internalvalue="internal_extrusion"
+    )
+    def automatic_thicken_sheets(self, assignment, value, extrude_internally=True, internal_extrusion=1):
         """Create thickened sheets for a list of input faces.
 
         This method automatically checks the direction in which to thicken the sheets.
 
         Parameters
         ----------
-        inputlist : list
+        assignment : list
             List of faces.
         value : float
             Value in millimeters to thicken the sheets.
-        internalExtr : bool, optional
+        extrude_internally : bool, optional
             Whether to extrude sheets internally. The default is ``True``.
-        internalvalue : float, optional
+        internal_extrusion : float, optional
             Value in millimeters to thicken the sheets internally (vgoing into the model).
             The default is ``1``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
@@ -5085,16 +5136,16 @@
         References
         ----------
 
         >>> oEditor.ThickenSheet
         """
         aedt_bounding_box = self.get_model_bounding_box()
         directions = {}
-        inputlist = self.convert_to_selections(inputlist, True)
-        for el in inputlist:
+        assignment = self.convert_to_selections(assignment, True)
+        for el in assignment:
             objID = self.oeditor.GetFaceIDs(el)
             faceCenter = self.oeditor.GetFaceCenter(int(objID[0]))
             directionfound = False
             thickness = 10
             while not directionfound:
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
@@ -5114,43 +5165,43 @@
                 self._odesign.Undo()
 
                 if aedt_bounding_box != aedt_bounding_box2:
                     directions[el] = "Internal"
                     directionfound = True
                 else:
                     thickness = thickness + 10
-        for el in inputlist:
+        for el in assignment:
             objID = self.oeditor.GetFaceIDs(el)
             faceCenter = self.oeditor.GetFaceCenter(int(objID[0]))
             if directions[el] == "Internal":
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                     ["NAME:SheetThickenParameters", "Thickness:=", "-" + str(value) + "mm", "BothSides:=", False],
                 )
             else:
                 self.oeditor.ThickenSheet(
                     ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                     ["NAME:SheetThickenParameters", "Thickness:=", str(value) + "mm", "BothSides:=", False],
                 )
-            if internalExtr:
+            if extrude_internally:
                 objID2 = self.oeditor.GetFaceIDs(el)
                 for fid in objID2:
                     try:
                         faceCenter2 = self.oeditor.GetFaceCenter(int(fid))
                         if faceCenter2 == faceCenter:
                             self.oeditor.MoveFaces(
                                 ["NAME:Selections", "Selections:=", el, "NewPartsModelFlag:=", "Model"],
                                 [
                                     "NAME:Parameters",
                                     [
                                         "NAME:MoveFacesParameters",
                                         "MoveAlongNormalFlag:=",
                                         True,
                                         "OffsetDistance:=",
-                                        str(internalvalue) + "mm",
+                                        str(internal_extrusion) + "mm",
                                         "MoveVectorX:=",
                                         "0mm",
                                         "MoveVectorY:=",
                                         "0mm",
                                         "MoveVectorZ:=",
                                         "0mm",
                                         "FacesToMove:=",
@@ -5159,23 +5210,23 @@
                                 ],
                             )
                     except Exception:
                         self.logger.info("done")
                         # self.modeler_oproject.ClearMessages()
         return True
 
-    @pyaedt_function_handler()
-    def move_face(self, faces, offset=1.0):
+    @pyaedt_function_handler(faces="assignment")
+    def move_face(self, assignment, offset=1.0):
         """Move an input face or a list of input faces of a specific object.
 
         This method moves a face or a list of faces which belong to the same solid.
 
         Parameters
         ----------
-        faces : list
+        assignment : list
             List of Face ID or List of :class:`pyaedt.modeler.Object3d.FacePrimitive` object or mixed.
         offset : float, optional
              Offset to apply in model units. The default is ``1.0``.
 
         Returns
         -------
         bool
@@ -5183,15 +5234,15 @@
 
         References
         ----------
 
         >>> oEditor.MoveFaces
 
         """
-        face_selection = self.convert_to_selections(faces, True)
+        face_selection = self.convert_to_selections(assignment, True)
         selection = {}
         for f in face_selection:
             if self.oeditor.GetObjectNameByFaceID(f) in selection:
                 selection[self.oeditor.GetObjectNameByFaceID(f)].append(f)
             else:
                 selection[self.oeditor.GetObjectNameByFaceID(f)] = [f]
 
@@ -5220,23 +5271,23 @@
                     "FacesToMove:=",
                     selection[el],
                 ]
             )
         self.oeditor.MoveFaces(arg1, arg2)
         return True
 
-    @pyaedt_function_handler()
-    def move_edge(self, edges, offset=1.0):
+    @pyaedt_function_handler(edges="assignment")
+    def move_edge(self, assignment, offset=1.0):
         """Move an input edge or a list of input edges of a specific object.
 
         This method moves an edge or a list of edges which belong to the same solid.
 
         Parameters
         ----------
-        edges : list
+        assignment : list
             List of Edge ID or List of :class:`pyaedt.modeler.Object3d.EdgePrimitive` object or mixed.
         offset : float, optional
              Offset to apply in model units. The default is ``1.0``.
 
         Returns
         -------
         bool
@@ -5244,15 +5295,15 @@
 
         References
         ----------
 
         >>> oEditor.MoveEdges
 
         """
-        edge_selection = self.convert_to_selections(edges, True)
+        edge_selection = self.convert_to_selections(assignment, True)
         selection = {}
         for f in edge_selection:
             if self.oeditor.GetObjectNameByEdgeID(f) in selection:
                 selection[self.oeditor.GetObjectNameByEdgeID(f)].append(f)
             else:
                 selection[self.oeditor.GetObjectNameByEdgeID(f)] = [f]
 
@@ -5396,60 +5447,60 @@
         ----------
 
         >>> oEditor.FlattenGroup
         """
         self.oeditor.FlattenGroup(["Groups:=", ["Model"]])
         return True
 
-    @pyaedt_function_handler()
-    def wrap_sheet(self, sheet_name, object_name, imprinted=False):
+    @pyaedt_function_handler(sheet_name="sheet", object_name="object")
+    def wrap_sheet(self, sheet, object, imprinted=False):
         """Execute the sheet wrapping around an object.
         If wrapping produces an unclassified operation it will be reverted.
 
         Parameters
         ----------
-        sheet_name : str, :class:`pyaedt.modeler.Object3d.Object3d`
+        sheet : str, :class:`pyaedt.modeler.Object3d.Object3d`
             Sheet name or sheet object.
-        object_name : str, :class:`pyaedt.modeler.Object3d.Object3d`
+        object : str, :class:`pyaedt.modeler.Object3d.Object3d`
             Object name or solid object.
         imprinted : bool, optional
             Either if imprint or not over the sheet. Default is ``False``.
 
         Returns
         -------
         bool
             Command execution status.
         """
-        sheet_name = self.convert_to_selections(sheet_name, False)
-        object_name = self.convert_to_selections(object_name, False)
+        sheet = self.convert_to_selections(sheet, False)
+        object = self.convert_to_selections(object, False)
 
-        if sheet_name not in self.sheet_names:
-            self.logger.error("{} is not a valid sheet.".format(sheet_name))
+        if sheet not in self.sheet_names:
+            self.logger.error("{} is not a valid sheet.".format(sheet))
             return False
-        if object_name not in self.solid_names:
-            self.logger.error("{} is not a valid solid body.".format(object_name))
+        if object not in self.solid_names:
+            self.logger.error("{} is not a valid solid body.".format(object))
             return False
         unclassified = [i for i in self.unclassified_objects]
         self.oeditor.WrapSheet(
-            ["NAME:Selections", "Selections:=", "{},{}".format(sheet_name, object_name)],
+            ["NAME:Selections", "Selections:=", "{},{}".format(sheet, object)],
             ["NAME:WrapSheetParameters", "Imprinted:=", imprinted],
         )
         is_unclassified = [i for i in self.unclassified_objects if i not in unclassified]
         if is_unclassified:
             self.logger.error("Failed to Wrap sheet. Reverting to original objects.")
             self._odesign.Undo()
             return False
         if imprinted:
             self.cleanup_objects()
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(input_objects_list="assignment")
     def heal_objects(
         self,
-        input_objects_list,
+        assignment,
         auto_heal=True,
         tolerant_stitch=True,
         simplify_geometry=True,
         tighten_gaps=True,
         heal_to_solid=False,
         stop_after_first_stitch_error=False,
         max_stitch_tolerance=0.001,
@@ -5474,15 +5525,15 @@
         allowable_surface_area_change=5,
         allowable_volume_change=5,
     ):
         """Repair invalid geometry entities for the selected objects within the specified tolerance settings.
 
         Parameters
         ----------
-        input_objects_list : str
+        assignment : str
             List of object names to analyze.
         auto_heal : bool, optional
             Auto heal option. Default value is ``True``.
         tolerant_stitch : bool, optional
             Tolerant stitch for manual healing. The default is ``True``.
         simplify_geometry : bool, optional
             Simplify geometry for manual healing. The default is ``True``.
@@ -5537,33 +5588,33 @@
             Allowable volume change for manual healing in mm. The default is ``1``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
-        if not input_objects_list:
+        if not assignment:
             self.logger.error("Provide an object name or a list of object names as a string.")
             return False
-        elif not isinstance(input_objects_list, str):
+        elif not isinstance(assignment, str):
             self.logger.error("Provide an object name or a list of object names as a string.")
             return False
-        elif "," in input_objects_list:
-            input_objects_list = input_objects_list.strip()
-            if ", " in input_objects_list:
-                input_objects_list_split = input_objects_list.split(", ")
+        elif "," in assignment:
+            assignment = assignment.strip()
+            if ", " in assignment:
+                input_objects_list_split = assignment.split(", ")
             else:
-                input_objects_list_split = input_objects_list.split(",")
+                input_objects_list_split = assignment.split(",")
             for obj in input_objects_list_split:
                 if obj not in self.object_names:
                     self.logger.error("Provide an object name or a list of object names that exists in current design.")
                     return False
             objects_selection = ",".join(input_objects_list_split)
         else:
-            objects_selection = input_objects_list
+            objects_selection = assignment
 
         if simplify_type not in [0, 1, 2]:
             self.logger.error("Invalid simplify type.")
             return False
 
         selections_args = ["NAME:Selections", "Selections:=", objects_selection, "NewPartsModelFlag:=", "Model"]
         healing_parameters = [
@@ -5630,18 +5681,18 @@
             allowable_surface_area_change,
             "AllowableVolumeChange:=",
             allowable_volume_change,
         ]
         self.oeditor.HealObject(selections_args, healing_parameters)
         return True
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(input_objects_list="assignment")
     def simplify_objects(
         self,
-        input_objects_list,
+        assignment,
         simplify_type="Polygon Fit",
         extrusion_axis="Auto",
         clean_up=True,
         allow_splitting=True,
         separate_bodies=True,
         clone_body=True,
         generate_primitive_history=False,
@@ -5649,15 +5700,15 @@
         length_threshold_percentage=25,
         create_group_for_new_objects=False,
     ):
         """Simplify command to converts complex objects into simpler primitives which are easy to mesh and solve.
 
         Parameters
         ----------
-        input_objects_list : str
+        assignment : str
             List of object names to simplify.
         simplify_type : str, optional
             Simplify type. The default is ``"Polygon Fit"``. Options are
             ``"Bounding Box"``, ``"Polygon Fit"``, and ``"Primitive Fit"`.
         extrusion_axis : str, optional
             Extrusion axis. The default is ``"Auto"``.
             Options are ``"Auto"``, ``"X"``, ``"Y"``, and ``"Z"``.
@@ -5681,33 +5732,33 @@
             Create group for new objects. The default is ``False``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
-        if not input_objects_list:
+        if not assignment:
             self.logger.error("Provide an object name or a list of object names as a string.")
             return False
-        elif not isinstance(input_objects_list, str):
+        elif not isinstance(assignment, str):
             self.logger.error("Provide an object name or a list of object names as a string.")
             return False
-        elif "," in input_objects_list:
-            input_objects_list = input_objects_list.strip()
-            if ", " in input_objects_list:
-                input_objects_list_split = input_objects_list.split(", ")
+        elif "," in assignment:
+            assignment = assignment.strip()
+            if ", " in assignment:
+                input_objects_list_split = assignment.split(", ")
             else:
-                input_objects_list_split = input_objects_list.split(",")
+                input_objects_list_split = assignment.split(",")
             for obj in input_objects_list_split:
                 if obj not in self.object_names:
                     self.logger.error("Provide an object name or a list of object names that exists in current design.")
                     return False
             objects_selection = ",".join(input_objects_list_split)
         else:
-            objects_selection = input_objects_list
+            objects_selection = assignment
 
         if simplify_type not in ["Polygon Fit", "Primitive Fit", "Bounding Box"]:
             self.logger.error("Invalid simplify type.")
             return False
 
         if extrusion_axis not in ["Auto", "X", "Y", "Z"]:
             self.logger.error("Invalid extrusion axis.")
@@ -5740,32 +5791,32 @@
         try:
             self.oeditor.Simplify(selections_args, simplify_parameters, groups_for_new_object)
             return True
         except Exception:
             self.logger.error("Simplify objects failed.")
             return False
 
-    @pyaedt_function_handler
-    def get_face_by_id(self, id):
+    @pyaedt_function_handler(id="assignment")
+    def get_face_by_id(self, assignment):
         """Get the face object given its ID.
 
         Parameters
         ----------
-        id : int
+        assignment : int
             ID of the face to retrieve.
 
         Returns
         -------
         modeler.cad.elements3d.FacePrimitive
             Face object.
 
         """
-        obj = [o for o in self.object_list for face in o.faces if face.id == id]
+        obj = [o for o in self.object_list for face in o.faces if face.id == assignment]
         if obj:
-            face_obj = [face for face in obj[0].faces if face.id == id][0]
+            face_obj = [face for face in obj[0].faces if face.id == assignment][0]
             return face_obj
         else:
             return False
 
     @pyaedt_function_handler()
     def create_point(self, position, name=None, color="(143 175 143)"):
         """Create a point.
@@ -5945,31 +5996,31 @@
         vGeo3d = ["NAME:Geometry3DPlaneTab", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3d]
         self.oeditor.ChangeProperty(vOut)
         if "NAME:Name" in vPropChange:
             self.cleanup_objects()
         return True
 
-    @pyaedt_function_handler()
-    def update_object(self, obj):
+    @pyaedt_function_handler(obj="assignment")
+    def update_object(self, assignment):
         """Update any :class:`pyaedt.modeler.Object3d.Object3d` derivatives
         that have potentially been modified by a modeler operation.
 
         Parameters
         ----------
-        obj : int, str, or :class:`pyaedt.modeler.Object3d.Object3d`
+        assignment : int, str, or :class:`pyaedt.modeler.Object3d.Object3d`
             Object to be updated after a modeler operation.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
            Updated 3D object.
 
         """
-        o = self._resolve_object(obj)
+        o = self._resolve_object(assignment)
         name = o.name
 
         del self.objects[self.objects_by_name[name].id]
         del self._object_names_to_ids[name]
         o = self._create_object(name)
         return o
 
@@ -6013,38 +6064,38 @@
             numeric_list.append(num_val)
 
         if scalar:
             return numeric_list[0]
         else:
             return numeric_list
 
-    @pyaedt_function_handler()
-    def does_object_exists(self, obj_to_check):
+    @pyaedt_function_handler(obj_to_check="assignment")
+    def does_object_exists(self, assignment):
         """Check to see if an object exists.
 
         Parameters
         ----------
-        obj_to_check : str, int
+        assignment : str, int
             Object name or object ID.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        if isinstance(obj_to_check, int) and obj_to_check in self.objects:
+        if isinstance(assignment, int) and assignment in self.objects:
             return True
-        elif obj_to_check in self.objects_by_name:
+        elif assignment in self.objects_by_name:
             return True
         else:
             return False
 
-    @pyaedt_function_handler
-    def create_subregion(self, padding_values, padding_types, parts, region_name=None):
+    @pyaedt_function_handler(parts="assignment", region_name="name")
+    def create_subregion(self, padding_values, padding_types, assignment, name=None):
         """Create a subregion.
 
         Parameters
         ----------
         padding_values : float, str, list of floats or list of str
             Padding values to apply. If a list is not provided, the same
             value is applied to all padding directions. If a list of floats
@@ -6053,38 +6104,36 @@
         padding_types : str or list of str, optional
             Padding definition. The default is ``"Percentage Offset"``.
             Options are ``"Absolute Offset"``,
             ``"Absolute Position"``, ``"Percentage Offset"``, and
             ``"Transverse Percentage Offset"``. When using a list,
             different padding types can be provided for different
            directions.
-        parts : list of str
+        assignment : list of str
             One or more names of the parts to include in the subregion.
-        region_name : str, optional
+        name : str, optional
             Region name. The default is ``None``, in which case the name
             is generated automatically.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             Subregion object.
 
         References
         ----------
 
         >>> oEditor.CreateRegion
         """
-        if region_name is None:
-            region_name = generate_unique_name("SubRegion")
+        if name is None:
+            name = generate_unique_name("SubRegion")
         is_percentage = padding_types in ["Percentage Offset", "Transverse Percentage Offset"]
-        arg, arg2 = self._parse_region_args(
-            padding_values, padding_types, region_name, parts, "SubRegion", is_percentage
-        )
+        arg, arg2 = self._parse_region_args(padding_values, padding_types, name, assignment, "SubRegion", is_percentage)
         self.oeditor.CreateSubregion(arg, arg2)
-        return self._create_object(region_name)
+        return self._create_object(name)
 
     def reassign_subregion(self, region, parts):
         """Modify parts in the subregion.
 
         Parameters
         ----------
         region : :class:`pyaedt.modules.MeshIcepak.SubRegion`
@@ -6171,33 +6220,33 @@
             "UseMaterialAppearance:=",
             False,
             "IsLightweight:=",
             False,
         ]
         return arg, arg2
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(region_name="name")
     def _create_region(
-        self, pad_value=300, pad_type="Percentage Offset", region_name="Region", parts=None, region_type="Region"
+        self, pad_value=300, pad_type="Percentage Offset", name="Region", parts=None, region_type="Region"
     ):
-        if region_name in self._app.modeler.objects_by_name:
-            self._app.logger.error("{} object already exists".format(region_name))
+        if name in self._app.modeler.objects_by_name:
+            self._app.logger.error("{} object already exists".format(name))
             return False
         if not isinstance(pad_value, list):
             pad_value = [pad_value] * 6
         is_percentage = pad_type in ["Percentage Offset", "Transverse Percentage Offset"]
-        arg, arg2 = self._parse_region_args(pad_value, pad_type, region_name, parts, region_type, is_percentage)
+        arg, arg2 = self._parse_region_args(pad_value, pad_type, name, parts, region_type, is_percentage)
         if arg and arg2:
             self.oeditor.CreateRegion(arg, arg2)
-            return self._create_object(region_name)
+            return self._create_object(name)
         else:
             return False
 
-    @pyaedt_function_handler()
-    def create_region(self, pad_value=300, pad_type="Percentage Offset", region_name="Region", **kwarg):
+    @pyaedt_function_handler(region_name="name")
+    def create_region(self, pad_value=300, pad_type="Percentage Offset", name="Region", **kwarg):
         """Create an air region.
 
         Parameters
         ----------
         pad_value : float, str, list of floats or list of str, optional
             Padding values to apply. If a list is not provided, the same
             value is applied to all padding directions. If a list of floats
@@ -6206,15 +6255,15 @@
         pad_type : str, optional
             Padding definition. The default is ``"Percentage Offset"``.
             Options are ``"Absolute Offset"``,
             ``"Absolute Position"``, ``"Percentage Offset"``, and
             ``"Transverse Percentage Offset"``. When using a list,
             different padding types can be provided for different
            directions.
-        region_name : str, optional
+        name : str, optional
             Region name. The default is ``None``, in which case the name
             is generated automatically.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             Region object.
@@ -6238,38 +6287,38 @@
             pad_type = ["Absolute Offset", "Percentage Offset"][int(is_percentage)]
 
         if isinstance(pad_type, bool):
             pad_type = ["Absolute Offset", "Percentage Offset"][int(pad_type)]
             if isinstance(pad_value, list):
                 pad_value = [pad_value[i // 2 + 3 * (i % 2)] for i in range(6)]
 
-        return self._create_region(pad_value, pad_type, region_name, region_type="Region")
+        return self._create_region(pad_value, pad_type, name, region_type="Region")
 
-    @pyaedt_function_handler()
-    def create_object_from_edge(self, edge, non_model=False):
+    @pyaedt_function_handler(edge="assignment")
+    def create_object_from_edge(self, assignment, non_model=False):
         """Create an object from one or multiple edges.
 
         Parameters
         ----------
-        edge : list, int or :class:`pyaedt.modeler.Object3d.FacePrimitive`
+        assignment : list, int or :class:`pyaedt.modeler.Object3d.FacePrimitive`
             Face ID or :class:`pyaedt.modeler.Object3d.FacePrimitive` object or Face List.
         non_model : bool, optional
             Either if create the new object as model or non-model. The default is `False`.
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.Object3d` or list of :class:`pyaedt.modeler.Object3d.Object3d`
             3D objects.
 
         References
         ----------
 
         >>> oEditor.CreateObjectFromFaces
         """
-        edge_ids = self.convert_to_selections(edge, True)
+        edge_ids = self.convert_to_selections(assignment, True)
         objs = OrderedDict()
         for edge_id in edge_ids:
             obj_name = self._find_object_from_edge_id(edge_id)
             if obj_name not in objs:
                 objs[obj_name] = [edge_id]
             else:
                 objs[obj_name].append(edge_id)
@@ -6290,36 +6339,36 @@
             if len(new_objects) > 1:
                 return new_objects
             else:
                 return new_objects[0]
         self.logger.error("Error creating object from edges.")
         return
 
-    @pyaedt_function_handler()
-    def create_object_from_face(self, face, non_model=False):
+    @pyaedt_function_handler(face="assignment")
+    def create_object_from_face(self, assignment, non_model=False):
         """Create an object from one or multiple face.
 
         Parameters
         ----------
-        face : list, int or :class:`pyaedt.modeler.Object3d.FacePrimitive`
+        assignment : list, int or :class:`pyaedt.modeler.Object3d.FacePrimitive`
             Face ID or :class:`pyaedt.modeler.Object3d.FacePrimitive` object or Face List.
         non_model : bool, optional
             Either if create the new object as model or non-model. Default is `False`.
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.Object3d` or list of :class:`pyaedt.modeler.Object3d.Object3d`
             3D objects.
 
         References
         ----------
 
         >>> oEditor.CreateObjectFromFaces
         """
-        face_ids = self.convert_to_selections(face, True)
+        face_ids = self.convert_to_selections(assignment, True)
         objs = OrderedDict()
         for face_id in face_ids:
             obj_name = self._find_object_from_face_id(face_id)
             if obj_name not in objs:
                 objs[obj_name] = [face_id]
             else:
                 objs[obj_name].append(face_id)
@@ -6385,23 +6434,23 @@
             num_seg=num_seg,
             num_points=num_points,
             arc_angle=arc_angle,
             arc_center=arc_center,
             arc_plane=arc_plane,
         )
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(position_list="points", matname="material")
     def create_polyline(
         self,
-        position_list,
+        points,
         segment_type=None,
         cover_surface=False,
         close_surface=False,
         name=None,
-        matname=None,
+        material=None,
         xsection_type=None,
         xsection_orient=None,
         xsection_width=1,
         xsection_topwidth=1,
         xsection_height=1,
         xsection_num_seg=0,
         xsection_bend_type=None,
@@ -6416,15 +6465,15 @@
         :func:`pyaedt.modeler.Primitives.Polyline.insert_segment` to
         insert a segment or
         :attr:`pyaedt.modeler.Primitives.Polyline.id` to retrieve the
         ID of the polyline object.
 
         Parameters
         ----------
-        position_list : list
+        points : list
             Array of positions of each point of the polyline.  A
             position is a list of 2D or 3D coordinates. Position
             coordinate values can be numbers or valid AEDT string
             expressions. For example, ``[0, 1, 2]``, ``["0mm", "5mm",
             "1mm"]``, or ``["x1", "y1", "z1"]``.
         segment_type : str or PolylineSegment or list, optional
             The default behavior is to connect all points as
@@ -6436,15 +6485,15 @@
         cover_surface : bool, optional
             The default is ``False``.
         close_surface : bool, optional
             The default is ``False``, which automatically joins the
             starting and ending points.
         name : str, optional
             Name of the polyline. The default is ``None``.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
         xsection_type : str, optional
             Type of the cross-section. Options are ``"Line"``, ``"Circle"``,
             ``"Rectangle"``, and ``"Isosceles Trapezoid"``. The default is ``None``.
         xsection_orient : str, optional
             Direction of the normal vector to the width of the cross-section.
@@ -6497,107 +6546,109 @@
 
         >>> test_points = [["0mm", "0mm", "0mm"], ["100mm", "20mm", "0mm"],
         ...                ["71mm", "71mm", "0mm"], ["0mm", "100mm", "0mm"]]
 
         The default behavior assumes that all points are to be
         connected by line segments.  Optionally specify the name.
 
-        >>> P1 = modeler.create_polyline(test_points, name="PL_line_segments")
+        >>> P1 = modeler.create_polyline(test_points,name="PL_line_segments")
 
         Specify that the first segment is a line and the last three
         points define a three-point arc.
 
-        >>> P2 = modeler.create_polyline(test_points, segment_type=["Line", "Arc"], name="PL_line_plus_arc")
+        >>> P2 = modeler.create_polyline(test_points,segment_type=["Line", "Arc"],name="PL_line_plus_arc")
 
         Redraw the 3-point arc alone from the last three points and
         additionally specify five segments using ``PolylineSegment``.
 
-        >>> P3 = modeler.create_polyline(test_points[1:],
-        ...                               segment_type=PolylineSegment(segment_type="Arc", num_seg=7),
-        ...                               name="PL_segmented_arc")
+        >>> P3 = modeler.create_polyline(test_points[1:],segment_type=PolylineSegment(segment_type="Arc", num_seg=7),
+        ...                              name="PL_segmented_arc")
 
         Specify that the four points form a spline and add a circular
         cross-section with a diameter of 1 mm.
 
-        >>> P4 = modeler.create_polyline(test_points, segment_type="Spline", name="PL_spline",
-        ...                               xsection_type="Circle", xsection_width="1mm")
+        >>> P4 = modeler.create_polyline(test_points,segment_type="Spline",name="PL_spline",
+        ...                              xsection_type="Circle",xsection_width="1mm")
 
         Use the `PolylineSegment` object to specify more detail about
         the individual segments.  Create a center point arc starting
         from the position ``test_points[1]``, rotating about the
         center point position ``test_points[0]`` in the XY plane.
 
         >>> start_point = test_points[1]
         >>> center_point = test_points[0]
         >>> segment_def = PolylineSegment(segment_type="AngularArc", arc_center=center_point,
         ...                                arc_angle="90deg", arc_plane="XY")
-        >>> modeler.create_polyline(start_point, segment_type=segment_def, name="PL_center_point_arc")
+        >>> modeler.create_polyline(start_point,segment_type=segment_def,name="PL_center_point_arc")
 
         Create a spline using a list of variables for the coordinates of the points.
 
         >>> x0, y0, z0 = "0", "0", "1"
         >>> x1, y1, z1 = "1", "3", "1"
         >>> x2, y2, z2 = "2", "2", "1"
-        >>> P5 = modeler.create_polyline(position_list = [[x0, y0, z0], [x1, y1, z1], [x2, y2, z2]],
-        ...                                 segment_type="Spline", name="polyline_with_variables")
+        >>> P5 = modeler.create_polyline(points=[[x0, y0, z0], [x1, y1, z1], [x2, y2, z2]],
+        ...                              segment_type="Spline",name="polyline_with_variables")
 
         """
         new_polyline = Polyline(
             primitives=self,
-            position_list=position_list,
+            position_list=points,
             segment_type=segment_type,
             cover_surface=cover_surface,
             close_surface=close_surface,
             name=name,
-            matname=matname,
+            matname=material,
             xsection_type=xsection_type,
             xsection_orient=xsection_orient,
             xsection_width=xsection_width,
             xsection_topwidth=xsection_topwidth,
             xsection_height=xsection_height,
             xsection_num_seg=xsection_num_seg,
             xsection_bend_type=xsection_bend_type,
             non_model=non_model,
         )
         return new_polyline
 
-    @pyaedt_function_handler()
-    def create_spiral_on_face(self, face, poly_width, filling_factor=1.5):
+    @pyaedt_function_handler(
+        face="assignment",
+        poly_width="width",
+    )
+    def create_spiral_on_face(self, assignment, width, filling_factor=1.5):
         """Create a Spiral Polyline inside a face.
 
         Parameters
         ----------
-        face : int or str or :class:`pyaedt.modeler.elements3d.FacePrimitive`
-        poly_width : float
+        assignment : int or str or :class:`pyaedt.modeler.elements3d.FacePrimitive`
+        width : float
         filling_factor : float
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.Polyline`
         """
         # fmt: off
-        if isinstance(face, FacePrimitive):
-            face_id = face.id
-        elif isinstance(face, int):
-            face_id = face
+        if isinstance(assignment, FacePrimitive):
+            face_id = assignment.id
+        elif isinstance(assignment, int):
+            face_id = assignment
         else:
-            face_id = self.get_object_faces(face)[0]
+            face_id = self.get_object_faces(assignment)[0]
 
         vertices = self.get_face_vertices(face_id)
         vertex_coordinates = []
         for v in vertices:
             vertex_coordinates.append(self.get_vertex_position(v))
 
         centroid = self.get_face_center(face_id)
 
         segments_lengths = []
         for vc in vertex_coordinates:
             segments_lengths.append(GeometryOperators.points_distance(vc, centroid))
 
-        n = math.floor(min(segments_lengths) / (poly_width * filling_factor))
+        n = math.floor(min(segments_lengths) / (width * filling_factor))
 
         if n % 2 == 0:
             n_points = int(n / 2 - 1)
         else:
             n_points = int((n - 1) / 2)
 
         if n_points < 1:
@@ -6616,43 +6667,47 @@
         for p in range(n_points):
             for v in inner_points:
                 poly_points_list.append(v[p])
 
         del poly_points_list[-1]
 
         # fmt: on
-        return self.create_polyline(poly_points_list, xsection_type="Line", xsection_width=poly_width)
+        return self.create_polyline(poly_points_list, xsection_type="Line", xsection_width=width)
 
-    @pyaedt_function_handler()
-    def get_existing_polyline(self, object):
+    @pyaedt_function_handler(object="assignment")
+    def get_existing_polyline(self, assignment):
         """Retrieve a polyline object to manipulate it.
 
         Parameters
         ----------
         src_object : :class:`pyaedt.modeler.cad.object3d.Object3d`
             An existing polyline object in the 3D Modeler.
 
         Returns
         -------
         Polyline
         """
-        return Polyline(self, src_object=object)
+        return Polyline(self, src_object=assignment)
 
-    @pyaedt_function_handler()
-    def create_udp(self, udp_dll_name, udp_parameters_list, upd_library="syslib", name=None):
+    @pyaedt_function_handler(
+        udp_dll_name="dll",
+        udp_parameters_list="parameters",
+        upd_library="library",
+    )
+    def create_udp(self, dll, parameters, library="syslib", name=None):
         """Create a user-defined primitive (UDP).
 
         Parameters
         ----------
-        udp_dll_name : str
+        dll : str
             Name of the UDP DLL or Python file. The default for the file format
             is ``".dll"``.
-        udp_parameters_list :
+        parameters :
             List of the UDP parameters.
-        upd_library : str, optional
+        library : str, optional
             Name of the UDP library. The default is ``"syslib"``.
         name : str, optional
             Name of the component. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
@@ -6661,154 +6716,151 @@
         References
         ----------
 
         >>> oEditor.CreateUserDefinedPart
 
         Examples
         --------
-        >>> my_udp = self.aedtapp.modeler.create_udp(udp_dll_name="RMxprt/ClawPoleCore",
-        ...                                          udp_parameters_list=my_udpPairs,
-        ...                                          upd_library="syslib")
+        >>> my_udp = self.aedtapp.modeler.create_udp(dll="RMxprt/ClawPoleCore",parameters=my_udpPairs,library="syslib")
         <class 'pyaedt.modeler.Object3d.Object3d'>
 
         """
-        if ".dll" not in udp_dll_name and ".py" not in udp_dll_name:
+        if ".dll" not in dll and ".py" not in dll:
             vArg1 = [
                 "NAME:UserDefinedPrimitiveParameters",
                 "DllName:=",
-                udp_dll_name + ".dll",
+                dll + ".dll",
                 "Library:=",
-                upd_library,
+                library,
             ]
         else:
-            vArg1 = ["NAME:UserDefinedPrimitiveParameters", "DllName:=", udp_dll_name, "Library:=", upd_library]
+            vArg1 = ["NAME:UserDefinedPrimitiveParameters", "DllName:=", dll, "Library:=", library]
 
         vArgParamVector = ["NAME:ParamVector"]
 
-        for pair in udp_parameters_list:
+        for pair in parameters:
             if isinstance(pair, list):
                 vArgParamVector.append(["NAME:Pair", "Name:=", pair[0], "Value:=", pair[1]])
 
             else:
                 vArgParamVector.append(["NAME:Pair", "Name:=", pair.Name, "Value:=", pair.Value])
 
         vArg1.append(vArgParamVector)
         if name:
             obj_name = name
         else:
-            obj_name, ext = os.path.splitext(os.path.basename(udp_dll_name))
+            obj_name, ext = os.path.splitext(os.path.basename(dll))
         vArg2 = self._default_object_attributes(name=obj_name)
         obj_name = self.oeditor.CreateUserDefinedPart(vArg1, vArg2)
         return self._create_object(obj_name)
 
-    @pyaedt_function_handler()
-    def update_udp(self, object_name, operation_name, udp_parameters_list):
+    @pyaedt_function_handler(object_name="assignment", operation_name="operation", udp_parameters_list="parameters")
+    def update_udp(self, assignment, operation, parameters):
         """Update an existing geometrical object that was originally created using a user-defined primitive (UDP).
 
         Parameters
         ----------
-        object_name : str
+        assignment : str
             Name of the object to update.
-        operation_name : str
+        operation : str
             Name of the operation used to create the object.
-        udp_parameters_list : list
+        parameters : list
             List of the UDP parameters to update and their value.
 
         Returns
         -------
         bool
             ``True`` when successful.
 
         References
         ----------
 
         >>> oEditor.CreateUserDefinedPart
 
         Examples
         --------
-        >>> self.aedtapp.modeler.update_udp(object_name="ClawPoleCore",
-        ...                                 operation_name="CreateUserDefinedPart",
-        ...                                 udp_parameters_list=[["Length","110mm"], ["DiaGap","125mm"]])
+        >>> self.aedtapp.modeler.update_udp(assignment="ClawPoleCore",operation="CreateUserDefinedPart",
+        ...                                 parameters=[["Length","110mm"], ["DiaGap","125mm"]])
         True
 
         """
 
         vArg1 = ["NAME:AllTabs"]
 
         prop_servers = ["NAME:PropServers"]
-        prop_servers.append("{0}:{1}:1".format(object_name, operation_name))
+        prop_servers.append("{0}:{1}:1".format(assignment, operation))
 
         cmd_tab = ["NAME:Geometry3DCmdTab"]
         cmd_tab.append(prop_servers)
 
         changed_props = ["NAME:ChangedProps"]
 
-        for pair in udp_parameters_list:
+        for pair in parameters:
             if isinstance(pair, list):
                 changed_props.append(["NAME:{0}".format(pair[0]), "Value:=", pair[1]])
             else:
                 changed_props.append(["NAME:", pair.Name, "Value:=", pair.Value])
 
         cmd_tab.append(changed_props)
         vArg1.append(cmd_tab)
         self.oeditor.ChangeProperty(vArg1)
         return True
 
-    @pyaedt_function_handler()
-    def delete(self, objects=None):
+    @pyaedt_function_handler(objects="assignment")
+    def delete(self, assignment=None):
         """Delete objects or groups.
 
         Parameters
         ----------
-        objects : list, optional
+        assignment : list, optional
             List of objects or group names. The default is ``None``,
             in which case all objects are deleted.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Delete
 
         """
-        if objects is None:
-            objects = self.object_names
-        objects = self._modeler.convert_to_selections(objects, return_list=True)
-        for el in objects:
+        if assignment is None:
+            assignment = self.object_names
+        assignment = self._modeler.convert_to_selections(assignment, return_list=True)
+        for el in assignment:
             if (
                 el not in self.object_names
                 and not list(self.oeditor.GetObjectsInGroup(el))
                 and not self.oeditor.GetObjectsInGroup("Unclassified")
             ):
-                objects.remove(el)
-        if not objects:
+                assignment.remove(el)
+        if not assignment:
             self.logger.warning("No objects to delete")
             return False
-        slice = min(100, len(objects))
-        num_objects = len(objects)
+        slice = min(100, len(assignment))
+        num_objects = len(assignment)
         remaining = num_objects
         while remaining > 0:
-            objs = objects[:slice]
+            objs = assignment[:slice]
             objects_str = self._modeler.convert_to_selections(objs, return_list=False)
             arg = ["NAME:Selections", "Selections:=", objects_str]
             try:
                 self.oeditor.Delete(arg)
             except Exception:
                 self.logger.warning("Failed to delete {}.".format(objects_str))
             remaining -= slice
             if remaining > 0:
-                objects = objects[slice:]
+                assignment = assignment[slice:]
 
         self._refresh_object_types()
 
-        if len(objects) > 0:
+        if len(assignment) > 0:
             self.cleanup_objects()
             self.logger.info("Deleted {} Objects: {}.".format(num_objects, objects_str))
         return True
 
     @pyaedt_function_handler()
     def delete_objects_containing(self, contained_string, case_sensitive=True):
         """Delete all objects with a given prefix.
@@ -6841,150 +6893,150 @@
             else:
                 if contained_string.lower() in el.lower():
                     self.delete(el)
                     num_del += 1
         self.logger.info("Deleted %s objects", num_del)
         return True
 
-    @pyaedt_function_handler()
-    def get_obj_id(self, objname):
+    @pyaedt_function_handler(objname="assignment")
+    def get_obj_id(self, assignment):
         """Return the object ID from an object name.
 
         Parameters
         ----------
-        objname : str
+        assignment : str
             Name of the object.
 
         Returns
         -------
         int
             Object ID.
 
         """
-        if objname in self.objects_by_name:
-            return self.objects_by_name[objname].id
+        if assignment in self.objects_by_name:
+            return self.objects_by_name[assignment].id
         return None
 
-    @pyaedt_function_handler()
-    def get_object_from_name(self, objname):
+    @pyaedt_function_handler(objname="assignment")
+    def get_object_from_name(self, assignment):
         """Return the object from an object name.
 
         Parameters
         ----------
-        objname : str
+        assignment : str
             Name of the object.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object returned.
 
         """
-        if objname in self.object_names:
+        if assignment in self.object_names:
             # object_id = self.get_obj_id(objname)
-            return self.objects[objname]
+            return self.objects[assignment]
 
-    @pyaedt_function_handler()
-    def get_objects_w_string(self, stringname, case_sensitive=True):
+    @pyaedt_function_handler(stringname="string_name")
+    def get_objects_w_string(self, string_name, case_sensitive=True):
         """Retrieve all objects with a given string in their names.
 
         Parameters
         ----------
-        stringname : str
+        string_name : str
             String to search object names for.
         case_sensitive : bool, optional
             Whether the string is case-sensitive. The default is ``True``.
 
         Returns
         -------
         list
             List of object names with the given string.
 
         """
         list_objs = []
         for name in list(self.objects_by_name.keys()):
             if case_sensitive:
-                if stringname in name:
+                if string_name in name:
                     list_objs.append(name)
             else:
-                if stringname.lower() in name.lower():
+                if string_name.lower() in name.lower():
                     list_objs.append(name)
         return list_objs
 
-    @pyaedt_function_handler()
-    def find_closest_edges(self, start_obj, end_obj, port_direction=0):
+    @pyaedt_function_handler(start_obj="start_object", end_obj="end_object", port_direction="direction")
+    def find_closest_edges(self, start_object, end_object, direction=0):
         """Retrieve the two closest edges that are not perpendicular for two objects.
 
         Parameters
         ----------
-        start_obj : str
+        start_object : str
             Name of the starting object.
-        end_obj : str
+        end_object : str
             Name of the ending object.
-        port_direction : str, optional
+        direction : str, optional
             Direction of the port to which to give edges precedence when more than two couples
             are at the same distance. For example, for a coax or microstrip, precedence is given
             to the edges that are on the given axis direction, such as ``"XNeg"``. Options are
             ``"XNeg"``, ``"XPos"``, ``"YNeg"``, ``"YPos`"``, ``"ZNeg"``, and ``"ZPos"``.
             The default is ``0``.
 
         Returns
         -------
         list
             List with two edges if present.
 
         """
-        start_obj = self._resolve_object(start_obj)
-        end_obj = self._resolve_object(end_obj)
+        start_object = self._resolve_object(start_object)
+        end_object = self._resolve_object(end_object)
         edge_start_list = None
         edge_stop_list = None
-        if port_direction == 0:
-            if start_obj.bottom_face_x:
-                edge_start_list = start_obj.bottom_face_x.edges
-            if end_obj.bottom_face_x:
-                edge_stop_list = end_obj.bottom_face_x.edges
-        elif port_direction == 3:
-            if start_obj.top_face_x:
-                edge_start_list = start_obj.top_face_x.edges
-            if end_obj.top_face_x:
-                edge_stop_list = end_obj.top_face_x.edges
-        elif port_direction == 1:
-            if start_obj.bottom_face_y:
-                edge_start_list = start_obj.bottom_face_y.edges
-            if end_obj.bottom_face_y:
-                edge_stop_list = end_obj.bottom_face_y.edges
-        elif port_direction == 4:
-            if start_obj.top_face_y:
-                edge_start_list = start_obj.top_face_y.edges
-            if end_obj.top_face_y:
-                edge_stop_list = end_obj.top_face_y.edges
-        elif port_direction == 2:
-            if start_obj.bottom_face_z:
-                edge_start_list = start_obj.bottom_face_z.edges
-            if end_obj.bottom_face_z:
-                edge_stop_list = end_obj.bottom_face_z.edges
-        elif port_direction == 5:
-            if start_obj.top_face_z:
-                edge_start_list = start_obj.top_face_z.edges
-            if end_obj.top_face_z:
-                edge_stop_list = end_obj.top_face_z.edges
+        if direction == 0:
+            if start_object.bottom_face_x:
+                edge_start_list = start_object.bottom_face_x.edges
+            if end_object.bottom_face_x:
+                edge_stop_list = end_object.bottom_face_x.edges
+        elif direction == 3:
+            if start_object.top_face_x:
+                edge_start_list = start_object.top_face_x.edges
+            if end_object.top_face_x:
+                edge_stop_list = end_object.top_face_x.edges
+        elif direction == 1:
+            if start_object.bottom_face_y:
+                edge_start_list = start_object.bottom_face_y.edges
+            if end_object.bottom_face_y:
+                edge_stop_list = end_object.bottom_face_y.edges
+        elif direction == 4:
+            if start_object.top_face_y:
+                edge_start_list = start_object.top_face_y.edges
+            if end_object.top_face_y:
+                edge_stop_list = end_object.top_face_y.edges
+        elif direction == 2:
+            if start_object.bottom_face_z:
+                edge_start_list = start_object.bottom_face_z.edges
+            if end_object.bottom_face_z:
+                edge_stop_list = end_object.bottom_face_z.edges
+        elif direction == 5:
+            if start_object.top_face_z:
+                edge_start_list = start_object.top_face_z.edges
+            if end_object.top_face_z:
+                edge_stop_list = end_object.top_face_z.edges
         if not edge_start_list:
-            edge_start_list = start_obj.edges
+            edge_start_list = start_object.edges
         if not edge_stop_list:
-            edge_stop_list = end_obj.edges
+            edge_stop_list = end_object.edges
         mindist = 1e6
         tol = 1e-12
         pos_tol = 1e-6
         edge_list = []
         actual_point = None
         is_parallel = False
         for el in edge_start_list:
             vertices_i = el.vertices
             if not vertices_i:
-                for f in start_obj.faces:
+                for f in start_object.faces:
                     if len(f.edges) == 1:
                         edges_ids = [i.id for i in f.edges]
                         if el.id in edges_ids:
                             vertices_i.append(f.center)
                             break
             vertex1_i = None
             vertex2_i = None
@@ -6998,15 +7050,15 @@
                 else:
                     start_midpoint = vertices_i[0].position
             else:
                 continue
             for el1 in edge_stop_list:
                 vertices_j = el1.vertices
                 if not vertices_j:
-                    for f in end_obj.faces:
+                    for f in end_object.faces:
                         if len(f.edges) == 1:
                             edges_ids = [i.id for i in f.edges]
                             if el1.id in edges_ids:
                                 vertices_j.append(f.center)
                                 break
                 vertex1_j = None
                 vertex2_j = None
@@ -7058,86 +7110,92 @@
                         vertex1_j, vertex2_j, vertex1_i, vertex2_i
                     ):
                         continue
 
                 if actual_point is None:
                     edge_list = [el, el1]
                     is_parallel = parallel_edges
-                    actual_point = GeometryOperators.find_point_on_plane([start_midpoint, end_midpoint], port_direction)
+                    actual_point = GeometryOperators.find_point_on_plane([start_midpoint, end_midpoint], direction)
                     mindist = vert_dist_sum
                 else:
-                    new_point = GeometryOperators.find_point_on_plane([start_midpoint, end_midpoint], port_direction)
-                    if (port_direction <= 2 and new_point - actual_point < 0) or (
-                        port_direction > 2 and actual_point - new_point < 0
+                    new_point = GeometryOperators.find_point_on_plane([start_midpoint, end_midpoint], direction)
+                    if (direction <= 2 and new_point - actual_point < 0) or (
+                        direction > 2 and actual_point - new_point < 0
                     ):
                         edge_list = [el, el1]
                         is_parallel = parallel_edges
                         actual_point = new_point
                         mindist = vert_dist_sum
-                    elif port_direction <= 2 and new_point - actual_point < tol and vert_dist_sum - mindist < pos_tol:
+                    elif direction <= 2 and new_point - actual_point < tol and vert_dist_sum - mindist < pos_tol:
                         edge_list = [el, el1]
                         is_parallel = parallel_edges
                         actual_point = new_point
                         mindist = vert_dist_sum
-                    elif port_direction > 2 and actual_point - new_point < tol and vert_dist_sum - mindist < pos_tol:
+                    elif direction > 2 and actual_point - new_point < tol and vert_dist_sum - mindist < pos_tol:
                         edge_list = [el, el1]
                         is_parallel = parallel_edges
                         actual_point = new_point
                         mindist = vert_dist_sum
         return edge_list, is_parallel
 
-    @pyaedt_function_handler()
-    def get_equivalent_parallel_edges(self, edgelist, portonplane=True, axisdir=0, startobj="", endobject=""):
+    @pyaedt_function_handler(
+        edgelist="assignment",
+        portonplane="port_on_plane",
+        axisdir="axis",
+        startobj="start_object",
+        endobject="end_object",
+    )
+    def get_equivalent_parallel_edges(self, assignment, port_on_plane=True, axis=0, start_object="", end_object=""):
         """Create two new edges that are parallel and equal to the smallest edge given a parallel couple of edges.
 
         Parameters
         ----------
-        edgelist : list
+        assignment : list
             List of two parallel edges.
-        portonplane : bool, optional
+        port_on_plane : bool, optional
             Whether edges are to be on the plane orthogonal to the axis direction.
             The default is ``True``.
-        axisdir : int, optional
+        axis : int, optional
             Axis direction. Choices are ``0`` through ``5``. The default is ``0``.
-        startobj : str, optional
+        start_object : str, optional
              Name of the starting object. The default is ``""``.
-        endobject : str, optional
+        end_object : str, optional
              Name of the ending object. The default is ``""``.
 
         Returns
         -------
         list
             List of two created edges.
 
         """
-        if isinstance(edgelist[0], str):
-            edgelist[0] = self.get_object_from_name(edgelist[0])
-        if isinstance(edgelist[1], str):
-            edgelist[1] = self.get_object_from_name(edgelist[1])
+        if isinstance(assignment[0], str):
+            assignment[0] = self.get_object_from_name(assignment[0])
+        if isinstance(assignment[1], str):
+            assignment[1] = self.get_object_from_name(assignment[1])
 
-        l1 = edgelist[0].length
-        l2 = edgelist[1].length
+        l1 = assignment[0].length
+        l2 = assignment[1].length
         if l1 < l2:
-            orig_edge = edgelist[0]
-            dest_edge = edgelist[1]
+            orig_edge = assignment[0]
+            dest_edge = assignment[1]
         else:
-            orig_edge = edgelist[1]
-            dest_edge = edgelist[0]
+            orig_edge = assignment[1]
+            dest_edge = assignment[0]
 
         first_edge = self.create_object_from_edge(orig_edge)
         second_edge = self.create_object_from_edge(orig_edge)
         ver1 = orig_edge.vertices
         ver2 = dest_edge.vertices
         if len(ver2) == 2:
             p = ver1[0].position
             a1 = ver2[0].position
             a2 = ver2[1].position
             vect = GeometryOperators.distance_vector(p, a1, a2)
-            if portonplane:
-                vect[divmod(axisdir, 3)[1]] = 0
+            if port_on_plane:
+                vect[divmod(axis, 3)[1]] = 0
             # TODO: can we avoid this translate operation - is there another way to check ?
             self.move(second_edge, vect)
             p_check = second_edge.vertices[0].position
             p_check2 = second_edge.vertices[1].position
         # elif len(ver2) == 1:  # for circular edges with one vertex
         #     p_check = first_edge.vertices[0].position
         #     p_check2 = second_edge.vertices[0].position
@@ -7145,147 +7203,149 @@
             self.delete(first_edge)
             self.delete(second_edge)
             return False
 
         obj_check = self.get_bodynames_from_position(p_check)
         obj_check2 = self.get_bodynames_from_position(p_check2)
         # if (startobj in obj_check and endobject in obj_check2) or (startobj in obj_check2 and endobject in obj_check):
-        if (startobj in obj_check or endobject in obj_check) and (startobj in obj_check2 or endobject in obj_check2):
+        if (start_object in obj_check or end_object in obj_check) and (
+            start_object in obj_check2 or end_object in obj_check2
+        ):
             if l1 < l2:
                 return_edges = [first_edge, second_edge]
             else:
                 return_edges = [second_edge, first_edge]
             return return_edges
         else:
             self.delete(second_edge)
             self.delete(first_edge)
             return None
 
-    @pyaedt_function_handler()
-    def get_object_faces(self, partId):
+    @pyaedt_function_handler(partId="assignment")
+    def get_object_faces(self, assignment):
         """Retrieve the face IDs of a given object ID or object name.
 
         Parameters
         ----------
-        partId : int or str
+        assignment : int or str
             Object ID or object name.
 
         Returns
         -------
         List
             List of faces IDs.
 
         References
         ----------
 
         >>> oEditor.GetFaceIDs
 
         """
         oFaceIDs = []
-        if isinstance(partId, str) and partId in self.objects_by_name:
-            oFaceIDs = self.oeditor.GetFaceIDs(partId)
+        if isinstance(assignment, str) and assignment in self.objects_by_name:
+            oFaceIDs = self.oeditor.GetFaceIDs(assignment)
             oFaceIDs = [int(i) for i in oFaceIDs]
-        elif partId in self.objects:
-            o = self.objects[partId]
+        elif assignment in self.objects:
+            o = self.objects[assignment]
             name = o.name
             oFaceIDs = self.oeditor.GetFaceIDs(name)
             oFaceIDs = [int(i) for i in oFaceIDs]
         return oFaceIDs
 
-    @pyaedt_function_handler()
-    def get_object_edges(self, partId):
+    @pyaedt_function_handler(partId="assignment")
+    def get_object_edges(self, assignment):
         """Retrieve the edge IDs of a given object ID or object name.
 
         Parameters
         ----------
-        partId : int or str
+        assignment : int or str
             Object ID or object name.
 
         Returns
         -------
         List
             List of edge IDs.
 
         References
         ----------
 
         >>> oEditor.GetEdgeIDsFromObject
 
         """
         oEdgeIDs = []
-        if isinstance(partId, str) and partId in self._object_names_to_ids:
-            oEdgeIDs = self.oeditor.GetEdgeIDsFromObject(partId)
+        if isinstance(assignment, str) and assignment in self._object_names_to_ids:
+            oEdgeIDs = self.oeditor.GetEdgeIDsFromObject(assignment)
             oEdgeIDs = [int(i) for i in oEdgeIDs]
-        elif partId in self.objects:
-            o = self.objects[partId]
+        elif assignment in self.objects:
+            o = self.objects[assignment]
             oEdgeIDs = self.oeditor.GetEdgeIDsFromObject(o.name)
             oEdgeIDs = [int(i) for i in oEdgeIDs]
         return oEdgeIDs
 
-    @pyaedt_function_handler()
-    def get_face_edges(self, partId):
+    @pyaedt_function_handler(partID="assignment")
+    def get_face_edges(self, assignment):
         """Retrieve the edge IDs of a given face name or face ID.
 
         Parameters
         ----------
-        partId : int or str
+        assignment : int or str
             Object ID or object name.
 
         Returns
         -------
         List
             List of edge IDs.
 
         References
         ----------
 
         >>> oEditor.GetEdgeIDsFromFace
 
         """
-        oEdgeIDs = self.oeditor.GetEdgeIDsFromFace(partId)
+        oEdgeIDs = self.oeditor.GetEdgeIDsFromFace(assignment)
         oEdgeIDs = [int(i) for i in oEdgeIDs]
         return oEdgeIDs
 
-    @pyaedt_function_handler()
-    def get_object_vertices(self, partID):
+    @pyaedt_function_handler(partID="assignment")
+    def get_object_vertices(self, assignment):
         """Retrieve the vertex IDs of a given object name or object ID.
 
         Parameters
         ----------
-        partID : int or str
+        assignment : int or str
             Object ID or object name.
 
         Returns
         -------
         List
             List of vertex IDs.
 
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromObject
 
         """
         oVertexIDs = []
-        if isinstance(partID, str) and partID in self._object_names_to_ids:
-            oVertexIDs = self.oeditor.GetVertexIDsFromObject(partID)
+        if isinstance(assignment, str) and assignment in self._object_names_to_ids:
+            oVertexIDs = self.oeditor.GetVertexIDsFromObject(assignment)
             oVertexIDs = [int(i) for i in oVertexIDs]
-        elif partID in self.objects:
-            o = self.objects[partID]
+        elif assignment in self.objects:
+            o = self.objects[assignment]
             oVertexIDs = self.oeditor.GetVertexIDsFromObject(o.name)
             oVertexIDs = [int(i) for i in oVertexIDs]
         return oVertexIDs
 
-    @pyaedt_function_handler()
-    def get_face_vertices(self, face_id):
+    @pyaedt_function_handler(face_id="assignment")
+    def get_face_vertices(self, assignment):
         """Retrieve the vertex IDs of a given face ID or face name.
 
         Parameters
         ----------
-        face_id : int or str
+        assignment : int or str
             Object ID or object name, which is available
             using the methods :func:`pyaedt.modeler.Primitives3D.Primitives3D.get_object_vertices`
             or :func:`pyaedt.modeler.Primitives2D.Primitives2D.get_object_vertices`.
 
         Returns
         -------
         List
@@ -7294,51 +7354,51 @@
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromFace
 
         """
         try:
-            oVertexIDs = self.oeditor.GetVertexIDsFromFace(face_id)
+            oVertexIDs = self.oeditor.GetVertexIDsFromFace(assignment)
         except Exception:
             oVertexIDs = []
         else:
             oVertexIDs = [int(i) for i in oVertexIDs]
         return oVertexIDs
 
-    @pyaedt_function_handler()
-    def get_edge_length(self, edgeID):
+    @pyaedt_function_handler(edgeID="assignment")
+    def get_edge_length(self, assignment):
         """Get the length of an edge.
 
         Parameters
         ----------
-        edgeID : int
+        assignment : int
             ID of the edge.
 
         Returns
         -------
         type
             Edge length.
 
         """
-        vertexID = self.get_edge_vertices(edgeID)
+        vertexID = self.get_edge_vertices(assignment)
         pos1 = self.get_vertex_position(vertexID[0])
         if len(vertexID) < 2:
             return 0
         pos2 = self.get_vertex_position(vertexID[1])
         length = GeometryOperators.points_distance(pos1, pos2)
         return length
 
-    @pyaedt_function_handler()
-    def get_edge_vertices(self, edgeID):
+    @pyaedt_function_handler(edgeID="assignment")
+    def get_edge_vertices(self, assignment):
         """Retrieve the vertex IDs of a given edge ID or edge name.
 
         Parameters
         ----------
-        edgeID : int, str
+        assignment : int, str
             Object ID or object name, which is available using the
             methods :func:`pyaedt.modeler.Primitives3D.Primitives3D.get_object_vertices`
             or :func:`pyaedt.modeler.Primitives2D.Primitives2D.get_object_vertices`.
 
         Returns
         -------
         List
@@ -7347,80 +7407,80 @@
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromEdge
 
         """
         try:
-            oVertexIDs = self.oeditor.GetVertexIDsFromEdge(edgeID)
+            oVertexIDs = self.oeditor.GetVertexIDsFromEdge(assignment)
         except Exception:
             oVertexIDs = []
         else:
             oVertexIDs = [int(i) for i in oVertexIDs]
         return oVertexIDs
 
-    @pyaedt_function_handler()
-    def get_vertex_position(self, vertex_id):
+    @pyaedt_function_handler(vertex_id="assignment")
+    def get_vertex_position(self, assignment):
         """Retrieve a vector of vertex coordinates.
 
         Parameters
         ----------
-        vertex_id : int or str
+        assignment : int or str
             ID or name of the vertex.
 
         Returns
         -------
         List
             List of ``[x, y, z]`` coordinates indicating the position.
 
         References
         ----------
 
         >>> oEditor.GetVertexPosition
 
         """
         try:
-            pos = self.oeditor.GetVertexPosition(vertex_id)
+            pos = self.oeditor.GetVertexPosition(assignment)
         except Exception:
             position = []
         else:
             position = [float(i) for i in pos]
         return position
 
-    @pyaedt_function_handler()
-    def get_face_area(self, face_id):
+    @pyaedt_function_handler(face_id="assignment")
+    def get_face_area(self, assignment):
         """Retrieve the area of a given face ID.
 
         Parameters
         ----------
-        face_id : int
+        assignment : int
             ID of the face.
 
         Returns
         -------
         float
             Value for the face area.
 
         References
         ----------
 
         >>> oEditor.GetFaceArea
 
         """
 
-        area = self.oeditor.GetFaceArea(face_id)
+        area = self.oeditor.GetFaceArea(assignment)
         return area
 
-    @pyaedt_function_handler()
-    def get_face_center(self, face_id):
+    @pyaedt_function_handler(face_id="assignment")
+    def get_face_center(self, assignment):
         """Retrieve the center position for a given planar face ID.
 
         Parameters
         ----------
-        face_id : int
+        assignment : int
             ID of the face.
 
         Returns
         -------
         List
             A list of ``[x, y, z]`` coordinates for the
             planar face center position.
@@ -7428,78 +7488,78 @@
         References
         ----------
 
         >>> oEditor.GetFaceCenter
 
         """
         try:
-            c = self.oeditor.GetFaceCenter(face_id)
+            c = self.oeditor.GetFaceCenter(assignment)
         except Exception:
             self.logger.warning("Non Planar Faces doesn't provide any Face Center")
             return False
         center = [float(i) for i in c]
         return center
 
-    @pyaedt_function_handler()
-    def get_mid_points_on_dir(self, sheet, axisdir):
+    @pyaedt_function_handler(sheet="assignment", axisdir="axis")
+    def get_mid_points_on_dir(self, assignment, axis):
         """Retrieve midpoints on a given axis direction.
 
         Parameters
         ----------
-        sheet :
+        assignment :
 
-        axisdir : int
+        axis : int
             Axis direction. Choices are ``0`` through ``5``.
 
         Returns
         -------
         type
 
         """
-        edgesid = self.get_object_edges(sheet)
-        id_ = divmod(axisdir, 3)[1]
+        edgesid = self.get_object_edges(assignment)
+        id_ = divmod(axis, 3)[1]
         midpoint_array = []
         for ed in edgesid:
             midpoint_array.append(self.get_edge_midpoint(ed))
         point0 = []
         point1 = []
         for el in midpoint_array:
             if not point0:
                 point0 = el
                 point1 = el
-            elif axisdir < 3 and el[id_] < point0[id_] or axisdir > 2 and el[id_] > point0[id_]:
+            elif axis < 3 and el[id_] < point0[id_] or axis > 2 and el[id_] > point0[id_]:
                 point0 = el
-            elif axisdir < 3 and el[id_] > point1[id_] or axisdir > 2 and el[id_] < point1[id_]:
+            elif axis < 3 and el[id_] > point1[id_] or axis > 2 and el[id_] < point1[id_]:
                 point1 = el
         return point0, point1
 
-    @pyaedt_function_handler()
-    def get_edge_midpoint(self, partID):
+    @pyaedt_function_handler(partID="assignment")
+    def get_edge_midpoint(self, assignment):
         """Retrieve the midpoint coordinates of a given edge ID or edge name.
 
         Parameters
         ----------
-        partID : int or str
+        assignment : int or str
             Object ID  or object name.
 
         Returns
         -------
         list
             List of midpoint coordinates. If the edge is not a segment with
             two vertices, an empty list is returned.
         """
 
-        if isinstance(partID, str) and partID in self._object_names_to_ids:
-            partID = self._object_names_to_ids[partID]
+        if isinstance(assignment, str) and assignment in self._object_names_to_ids:
+            assignment = self._object_names_to_ids[assignment]
 
-        if partID in self.objects and self.objects[partID].object_type == "Line":
-            vertices = self.get_object_vertices(partID)
+        if assignment in self.objects and self.objects[assignment].object_type == "Line":
+            vertices = self.get_object_vertices(assignment)
         else:
             try:
-                vertices = self.get_edge_vertices(partID)
+                vertices = self.get_edge_vertices(assignment)
             except Exception:
                 vertices = []
         if len(vertices) == 2:
             vertex1 = self.get_vertex_position(vertices[0])
             vertex2 = self.get_vertex_position(vertices[1])
             midpoint = GeometryOperators.get_mid_point(vertex1, vertex2)
             return list(midpoint)
@@ -7543,36 +7603,36 @@
         vArg1.append("ZPosition:="), vArg1.append(ZCenter)
         list_of_bodies = list(self.oeditor.GetBodyNamesByPosition(vArg1))
         if not include_non_model:
             non_models = [i for i in self.non_model_objects]
             list_of_bodies = [i for i in list_of_bodies if i not in non_models]
         return list_of_bodies
 
-    @pyaedt_function_handler()
-    def get_edgeid_from_position(self, position, obj_name=None, units=None):
+    @pyaedt_function_handler(obj_name="assignment")
+    def get_edgeid_from_position(self, position, assignment=None, units=None):
         """Get an edge ID from a position.
 
         Parameters
         ----------
         position : list
             List of ``[x, y, z]`` coordinates for the position.
-        obj_name : str, optional
+        assignment : str, optional
             Name of the object. The default is ``None``, in which case all
             objects are searched.
         units : str, optional
             Units for the position, such as ``"m"``. The default is ``None``,
             in which case the model units are used.
 
         Returns
         -------
         type
             Edge ID of the first object touching this position.
         """
-        if isinstance(obj_name, str):
-            object_list = [obj_name]
+        if isinstance(assignment, str):
+            object_list = [assignment]
         else:
             object_list = self.object_names
 
         edgeID = -1
         XCenter, YCenter, ZCenter = self._pos_with_arg(position, units)
 
         vArg1 = ["NAME:EdgeParameters"]
@@ -7584,23 +7644,23 @@
             vArg1[2] = obj
             try:
                 edgeID = int(self.oeditor.GetEdgeByPosition(vArg1))
                 return edgeID
             except Exception:
                 pass
 
-    @pyaedt_function_handler()
-    def get_edgeids_from_vertexid(self, vertexid, obj_name):
+    @pyaedt_function_handler(vertexid="vertex", obj_name="assignment")
+    def get_edgeids_from_vertexid(self, vertex, assignment):
         """Retrieve edge IDs for a vertex ID.
 
         Parameters
         ----------
-        vertexid : int
+        vertex : int
             Vertex ID.
-        obj_name :
+        assignment : str
             Name of the object.
 
         Returns
         -------
         List
             List of edge IDs for the vertex ID.
 
@@ -7608,31 +7668,31 @@
         ----------
 
         >>> oEditor.GetEdgeIDsFromObject
         >>> oEditor.GetVertexIDsFromEdge
 
         """
         edgeID = []
-        edges = self.get_object_edges(obj_name)
+        edges = self.get_object_edges(assignment)
         for edge in edges:
             vertices = self.get_edge_vertices(edge)
-            if vertexid in vertices:
+            if vertex in vertices:
                 edgeID.append(edge)
 
         return edgeID
 
-    @pyaedt_function_handler()
-    def get_faceid_from_position(self, position, obj_name=None, units=None):
+    @pyaedt_function_handler(obj_name="assignment")
+    def get_faceid_from_position(self, position, assignment=None, units=None):
         """Retrieve a face ID from a position.
 
         Parameters
         ----------
         position : list
             List of ``[x, y, z]`` coordinates for the position.
-        obj_name : str, optional
+        assignment : str, optional
             Name of the object. The default is ``None``, in which case all
             objects are searched.
         units : str, optional
             Units, such as ``"m"``. The default is ``None``, in which case the
             model units are used.
 
         Returns
@@ -7642,16 +7702,16 @@
 
         References
         ----------
 
         >>> oEditor.GetFaceByPosition
 
         """
-        if isinstance(obj_name, str):
-            object_list = [obj_name]
+        if isinstance(assignment, str):
+            object_list = [assignment]
         else:
             object_list = self.object_names
 
         XCenter, YCenter, ZCenter = self._pos_with_arg(position, units)
         vArg1 = ["NAME:FaceParameters"]
         vArg1.append("BodyName:="), vArg1.append("")
         vArg1.append("XPosition:="), vArg1.append(XCenter)
@@ -7662,54 +7722,54 @@
             try:
                 face_id = self.oeditor.GetFaceByPosition(vArg1)
                 return face_id
             except Exception:
                 # Not Found, keep looking
                 pass
 
-    @pyaedt_function_handler()
-    def get_edges_on_bounding_box(self, sheets, return_colinear=True, tol=1e-6):
+    @pyaedt_function_handler(sheets="assignment", tol="tolerance")
+    def get_edges_on_bounding_box(self, assignment, return_colinear=True, tolerance=1e-6):
         """Retrieve the edges of the sheets passed in the input that are lying on the bounding box.
 
         This method creates new lines for the detected edges and returns the IDs of these lines.
         If required, only colinear edges are returned.
 
         Parameters
         ----------
-        sheets : int, str, or list
+        assignment : int, str, or list
             ID or name for one or more sheets.
         return_colinear : bool, optional
             Whether to return only colinear edges. The default is ``True``.
             If ``False``, all edges on the bounding box are returned.
-        tol : float, optional
+        tolerance : float, optional
             Geometric tolerance. The default is ``1e-6``.
 
         Returns
         -------
         list
             List of edge IDs lying on the bounding box.
 
         """
-        port_sheets = self._modeler.convert_to_selections(sheets, return_list=True)
+        port_sheets = self._modeler.convert_to_selections(assignment, return_list=True)
         bb = self._modeler.get_model_bounding_box()
 
         candidate_edges = []
         for p in port_sheets:
             edges = self[p].edges
             for edge in edges:
                 vertices = edge.vertices
                 v_flag = False
                 for vertex in vertices:
                     v = vertex.position
                     xyz_flag = 0
-                    if abs(v[0] - bb[0]) < tol or abs(v[0] - bb[3]) < tol:
+                    if abs(v[0] - bb[0]) < tolerance or abs(v[0] - bb[3]) < tolerance:
                         xyz_flag += 1
-                    if abs(v[1] - bb[1]) < tol or abs(v[1] - bb[4]) < tol:
+                    if abs(v[1] - bb[1]) < tolerance or abs(v[1] - bb[4]) < tolerance:
                         xyz_flag += 1
-                    if abs(v[2] - bb[2]) < tol or abs(v[2] - bb[5]) < tol:
+                    if abs(v[2] - bb[2]) < tolerance or abs(v[2] - bb[5]) < tolerance:
                         xyz_flag += 1
                     if xyz_flag >= 2:
                         v_flag = True
                     else:
                         v_flag = False
                         break
                 if v_flag:
@@ -7721,67 +7781,69 @@
         selected_edges = []
         for i, edge_i in enumerate(candidate_edges[:-1]):
             vertex1_i = edge_i.vertices[0].position
             midpoint_i = edge_i.midpoint
             for j, edge_j in enumerate(candidate_edges[i + 1 :]):
                 midpoint_j = edge_j.midpoint
                 area = GeometryOperators.get_triangle_area(midpoint_i, midpoint_j, vertex1_i)
-                if area < tol**2:
+                if area < tolerance**2:
                     selected_edges.extend([edge_i, edge_j])
                     break
         selected_edges = list(set(selected_edges))
 
         for edge in selected_edges:
             self.create_object_from_edge(edge)
             time.sleep(aedt_wait_time)
 
         return selected_edges
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        sheet="assignment", XY_plane="xy_plane", YZ_plane="yz_plane", XZ_plane="xz_plane", tol="tolerance"
+    )
     def get_edges_for_circuit_port_from_sheet(
-        self, sheet, XY_plane=True, YZ_plane=True, XZ_plane=True, allow_perpendicular=False, tol=1e-6
+        self, assignment, xy_plane=True, yz_plane=True, xz_plane=True, allow_perpendicular=False, tolerance=1e-6
     ):
         """Retrieve two edge IDs that are suitable for a circuit port from a sheet.
 
         One edge belongs to the sheet passed in the input, and the second edge
         is the closest edge's coplanar to the first edge (aligned to the XY, YZ,
         or XZ plane). This method creates new lines for the detected edges and returns
         the IDs of these lines.
 
         This method accepts one or more sheet objects as input,
         while the method :func:`Primitives.get_edges_for_circuit_port`
         accepts a face ID.
 
         Parameters
         ----------
-        sheet : int, str, or list
+        assignment : int, str, or list
             ID or name for one or more sheets.
-        XY_plane : bool, optional
+        xy_plane : bool, optional
             Whether the edge's pair are to be on the XY plane.
             The default is ``True``.
-        YZ_plane : bool, optional
+        yz_plane : bool, optional
             Whether the edge's pair are to be on the YZ plane.
             The default is ``True``.
-        XZ_plane : bool, optional
+        xz_plane : bool, optional
             Whether the edge's pair are to be on the XZ plane.
             The default is ``True``.
         allow_perpendicular : bool, optional
             Whether the edge's pair are to be perpendicular.
             The default is ``False``.
-        tol : float, optional
+        tolerance : float, optional
             Geometric tolerance. The default is ``1e-6``.
 
         Returns
         -------
         list
             List of edge IDs.
 
         """
-        tol2 = tol**2
-        port_sheet = self._modeler.convert_to_selections(sheet, return_list=True)
+        tol2 = tolerance**2
+        port_sheet = self._modeler.convert_to_selections(assignment, return_list=True)
         if len(port_sheet) > 1:
             return []
         else:
             port_sheet = port_sheet[0]
         port_edges = self.get_object_edges(port_sheet)
 
         # find the bodies to exclude
@@ -7840,36 +7902,36 @@
                     not allow_perpendicular
                     and abs(
                         GeometryOperators._v_dot(
                             GeometryOperators.v_points(vertex1_i, vertex2_i),
                             GeometryOperators.v_points(vertex1_j, vertex2_j),
                         )
                     )
-                    < tol
+                    < tolerance
                 ):
                     continue
 
                 normal1 = GeometryOperators.v_cross(
                     GeometryOperators.v_points(vertex1_i, vertex2_i), GeometryOperators.v_points(vertex1_i, vertex1_j)
                 )
                 normal1_norm = GeometryOperators.v_norm(normal1)
-                if YZ_plane and abs(abs(GeometryOperators._v_dot(normal1, ux)) - normal1_norm) < tol:
+                if yz_plane and abs(abs(GeometryOperators._v_dot(normal1, ux)) - normal1_norm) < tolerance:
                     pass
-                elif XZ_plane and abs(abs(GeometryOperators._v_dot(normal1, uy)) - normal1_norm) < tol:
+                elif xz_plane and abs(abs(GeometryOperators._v_dot(normal1, uy)) - normal1_norm) < tolerance:
                     pass
-                elif XY_plane and abs(abs(GeometryOperators._v_dot(normal1, uz)) - normal1_norm) < tol:
+                elif xy_plane and abs(abs(GeometryOperators._v_dot(normal1, uz)) - normal1_norm) < tolerance:
                     pass
                 else:
                     continue
 
                 vec1 = GeometryOperators.v_points(vertex1_i, vertex2_j)
                 if abs(GeometryOperators._v_dot(normal1, vec1)) < tol2:  # the 4th point is coplanar
                     candidate_edges.append(ej)
 
-        minimum_distance = tol**-1
+        minimum_distance = tolerance**-1
         selected_edges = []
         for ei in midpoints:
             midpoint_i = midpoints[ei]
             for ej in candidate_edges:
                 midpoint_j = self.get_edge_midpoint(ej)
                 d = GeometryOperators.points_distance(midpoint_i, midpoint_j)
                 if d < minimum_distance:
@@ -7880,59 +7942,61 @@
             new_edge1 = self.create_object_from_edge(selected_edges[0])
             time.sleep(aedt_wait_time)
             new_edge2 = self.create_object_from_edge(selected_edges[1])
             return selected_edges
         else:
             return []
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        face_id="assignment", XY_plane="xy_plane", YZ_plane="yz_plane", XZ_plane="xz_plane", tol="tolerance"
+    )
     def get_edges_for_circuit_port(
-        self, face_id, XY_plane=True, YZ_plane=True, XZ_plane=True, allow_perpendicular=False, tol=1e-6
+        self, assignment, xy_plane=True, yz_plane=True, xz_plane=True, allow_perpendicular=False, tolerance=1e-6
     ):
         """Retrieve two edge IDs suitable for the circuit port.
 
         One edge belongs to the face ID passed in the input, and the second edge
         is the closest edge's coplanar to the first edge (aligned to the XY, YZ,
         or XZ plane). This method creates new lines for the detected edges and returns
         the IDs of these lines.
 
         This method accepts a face ID in the input, while the `get_edges_for_circuit_port_from_port`
         method accepts one or more sheet objects.
 
         Parameters
         ----------
-        face_id :
+        assignment :
             ID of the face.
-        XY_plane : bool, optional
+        xy_plane : bool, optional
             Whether the edge's pair are to be on the XY plane.
             The default is ``True``.
-        YZ_plane : bool, optional
+        yz_plane : bool, optional
             Whether the edge's pair are to be on the YZ plane.
             The default is ``True``.
-        XZ_plane : bool, optional
+        xz_plane : bool, optional
             Whether the edge's pair are to be on the XZ plane.
             The default is ``True``.
         allow_perpendicular : bool, optional
             Whether the edge's pair are to be perpendicular.
             The default is ``False``.
-        tol : float, optional
+        tolerance : float, optional
             Geometric tolerance. The default is ``1e-6``.
 
         Returns
         -------
         list
             List of edge IDs.
 
         """
-        tol2 = tol**2
+        tol2 = tolerance**2
 
-        port_edges = self.get_face_edges(face_id)
+        port_edges = self.get_face_edges(assignment)
 
         # find the bodies to exclude
-        port_sheet_midpoint = self.get_face_center(face_id)
+        port_sheet_midpoint = self.get_face_center(assignment)
         point = self._modeler.Position(port_sheet_midpoint)
         list_of_bodies = self.get_bodynames_from_position(point)
 
         # select all edges
         all_edges = []
         solids = [s for s in self.solid_names if s not in list_of_bodies]
         for solid in solids:
@@ -7946,18 +8010,18 @@
         uz = [0.0, 0.0, 1.0]
         midpoints = {}
         candidate_edges = []
         for ei in port_edges:
             vertices_i = self.get_edge_vertices(ei)
             if len(vertices_i) == 1:  # maybe a circle
                 vertex1_i = self.get_vertex_position(vertices_i[0])
-                area_i = self.get_face_area(face_id)
+                area_i = self.get_face_area(assignment)
                 if area_i is None or area_i < tol2:  # degenerated face
                     continue
-                center_i = self.get_face_center(face_id)
+                center_i = self.get_face_center(assignment)
                 if not center_i:  # non planar face
                     continue
                 radius_i = GeometryOperators.points_distance(vertex1_i, center_i)
                 area_i_eval = math.pi * radius_i**2
                 if abs(area_i - area_i_eval) < tol2:  # it is a circle
                     vertex2_i = center_i
                     midpoints[ei] = center_i
@@ -7983,36 +8047,36 @@
                     not allow_perpendicular
                     and abs(
                         GeometryOperators._v_dot(
                             GeometryOperators.v_points(vertex1_i, vertex2_i),
                             GeometryOperators.v_points(vertex1_j, vertex2_j),
                         )
                     )
-                    < tol
+                    < tolerance
                 ):
                     continue
 
                 normal1 = GeometryOperators.v_cross(
                     GeometryOperators.v_points(vertex1_i, vertex2_i), GeometryOperators.v_points(vertex1_i, vertex1_j)
                 )
                 normal1_norm = GeometryOperators.v_norm(normal1)
-                if YZ_plane and abs(abs(GeometryOperators._v_dot(normal1, ux)) - normal1_norm) < tol:
+                if yz_plane and abs(abs(GeometryOperators._v_dot(normal1, ux)) - normal1_norm) < tolerance:
                     pass
-                elif XZ_plane and abs(abs(GeometryOperators._v_dot(normal1, uy)) - normal1_norm) < tol:
+                elif xz_plane and abs(abs(GeometryOperators._v_dot(normal1, uy)) - normal1_norm) < tolerance:
                     pass
-                elif XY_plane and abs(abs(GeometryOperators._v_dot(normal1, uz)) - normal1_norm) < tol:
+                elif xy_plane and abs(abs(GeometryOperators._v_dot(normal1, uz)) - normal1_norm) < tolerance:
                     pass
                 else:
                     continue
 
                 vec1 = GeometryOperators.v_points(vertex1_i, vertex2_j)
                 if abs(GeometryOperators._v_dot(normal1, vec1)) < tol2:  # the 4th point is coplanar
                     candidate_edges.append(ej)
 
-        minimum_distance = tol**-1
+        minimum_distance = tolerance**-1
         selected_edges = []
         for ei in midpoints:
             midpoint_i = midpoints[ei]
             for ej in candidate_edges:
                 midpoint_j = self.get_edge_midpoint(ej)
                 d = GeometryOperators.points_distance(midpoint_i, midpoint_j)
                 if d < minimum_distance:
@@ -8045,15 +8109,15 @@
 
         """
         if isinstance(position, list):
             position = self.Position(position)
 
         bodies = self.get_bodynames_from_position(position, units)
         # the function searches in all bodies, not efficient
-        face_id = self.get_faceid_from_position(position, obj_name=bodies[0], units=units)
+        face_id = self.get_faceid_from_position(position, assignment=bodies[0], units=units)
         edges = self.get_face_edges(face_id)
         distance = 1e6
         selected_edge = None
         for edge in edges:
             midpoint = self.get_edge_midpoint(edge)
             if self.model_units == "mm" and units == "meter":
                 midpoint = [i / 1000 for i in midpoint]
@@ -8271,15 +8335,15 @@
             for k, val in kwargs.items():
                 if k in props:  # Only try to set valid properties.
                     try:
                         setattr(o, k, val)
                     except Exception:
                         self.logger.warning("Unable to assign " + str(k) + " to object " + o.name + ".")
                 else:
-                    self.logger.error("'" + str(k) + "' is not a valid property of the primitive ")
+                    self.logger.debug("'" + str(k) + "' is not a valid property of the primitive.")
         return o
 
     @pyaedt_function_handler()
     def _default_object_attributes(self, name=None, matname=None, flags=""):
         if not matname:
             matname = self.defaultmaterial
 
@@ -8478,15 +8542,15 @@
                             native_comp_properties = data
                             break
             except Exception:
                 return native_comp_properties
 
         return native_comp_properties
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _get_object_dict_by_material(self, material):
         obj_dict = {}
         for mat in material:
             objs = []
             for obj in self.object_list:
                 if obj and ("[" in obj.material_name or "(" in obj.material_name):
                     if (
@@ -8498,23 +8562,23 @@
                     ):
                         objs.append(obj)
                 elif obj and (obj.material_name == mat or obj.material_name == mat.lower()):
                     objs.append(obj)
             obj_dict[mat] = objs
         return obj_dict
 
-    @pyaedt_function_handler()
-    def convert_segments_to_line(self, object_name):
+    @pyaedt_function_handler(object_name="assignment")
+    def convert_segments_to_line(self, assignment):
         """Convert a CreatePolyline list of segments to lines.
 
         This method applies to splines and 3-point arguments.
 
         Parameters
         ----------
-        object_name : int, str, or :class:`pyaedt.modeler.cad.object3d.Object3d`
+        assignment : int, str, or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Specified for the object.
 
         Returns
         -------
         bool
             ``True`` if successful, ``False`` if it fails.
 
@@ -8529,15 +8593,15 @@
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
         >>> edge_object = aedtapp.modeler.create_object_from_edge("my_edge")
         >>> aedtapp.modeler.generate_object_history(edge_object)
         >>> aedtapp.modeler.convert_segments_to_line(edge_object.name)
 
         """
-        this_object = self._resolve_object(object_name)
+        this_object = self._resolve_object(assignment)
         edges = this_object.edges
         for i in reversed(range(len(edges))):
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:Geometry3DPolylineTab",
@@ -8569,15 +8633,15 @@
     Examples
     --------
     >>> from pyaedt import Hfss
     >>> from pyaedt.modeler.cad.Primitives import PrimitivesBuilder
     >>> aedtapp = Hfss()
     >>> primitive_file = "primitives_file.json"
     >>> primitives_builder = PrimitivesBuilder(aedtapp, input_file=primitive_file)
-    >>> primitives_builder.create()
+    >>> primitives_builder.create(),,
     >>> aedtapp.release_desktop()
     """
 
     def __init__(self, app, input_file=None, input_dict=None):
         self._app = app
         props = {}
         if not input_dict and not input_file:  # pragma: no cover
@@ -8748,35 +8812,35 @@
             data["Height"] = 50
         if not data.get("Number of Segments"):
             data["Number of Segments"] = 0
 
         self._app.modeler.set_working_coordinate_system(cs)
 
         cyl1 = self._app.modeler.create_cylinder(
-            cs_axis=data.get("Plane"),
-            position=origin,
+            orientation=data.get("Plane"),
+            origin=origin,
             radius=data.get("Radius"),
             height=data.get("Height"),
-            numSides=int(data.get("Number of Segments")),
+            num_sides=int(data.get("Number of Segments")),
             name=name,
         )
 
         internal_radius = data.get("Internal Radius")
         if internal_radius:
             internal_radius = self.convert_units([internal_radius])[0]
             radius = self.convert_units([data.get("Radius")])[0]
             if internal_radius > radius:
                 self.logger.warning("Internal radius is larger than external radius.")
             elif internal_radius != 0:
                 cyl2 = self._app.modeler.create_cylinder(
-                    cs_axis=data.get("Plane"),
-                    position=origin,
+                    orientation=data.get("Plane"),
+                    origin=origin,
                     radius=internal_radius,
                     height=data.get("Height"),
-                    numSides=data.get("Number of Segments"),
+                    num_sides=data.get("Number of Segments"),
                     name=name,
                 )
                 self._app.modeler.subtract(blank_list=cyl1, tool_list=cyl2, keep_originals=False)
 
         return cyl1
 
     def _create_box_instance(self, name, cs, origin, data):
@@ -8804,17 +8868,15 @@
             data["Y Length"] = 10
         if not data.get("Z Length"):
             data["Z Length"] = 10
 
         self._app.modeler.set_working_coordinate_system(cs)
 
         box1 = self._app.modeler.create_box(
-            position=origin,
-            dimensions_list=[data["X Length"], data["Y Length"], data["Z Length"]],
-            name=name,
+            origin=origin, sizes=[data["X Length"], data["Y Length"], data["Z Length"]], name=name
         )
         return box1
 
     @pyaedt_function_handler()
     def _read_csv_cylinder_props(self, csv_data):
         """Convert CSV data to ``PrimitivesBuilder`` properties.
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/Primitives2D.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/Primitives2D.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,34 +26,34 @@
             if self._app._odesign.GetGeometryMode() == "about Z":
                 plane = "Y"
         return plane
 
     def __init__(self, application):
         GeometryModeler.__init__(self, application, is3d=False)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(position="origin", matname="material")
     def create_circle(
-        self, position, radius, num_sides=0, is_covered=True, name=None, matname=None, non_model=False, **kwargs
+        self, origin, radius, num_sides=0, is_covered=True, name=None, material=None, non_model=False, **kwargs
     ):
         """Create a circle.
 
         Parameters
         ----------
-        position : list
+        origin : list
             ApplicationName.modeler.Position(x,y,z) object
         radius : float
             Radius of the object.
         num_sides : int, optional
             Number of sides. The default is ``0``, which is correct for a circle.
         is_covered : bool
             Specify whether the ellipse is a sheet (covered) or a line object
         name : str, optional
             Name of the object. The default is ``None``. If ``None`` ,
             a unique name ``"NewObject_xxxxxx"`` will be assigned)
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``. If ``None``,
             the default material is assigned.
         non_model : bool, optional
              Either to create the new object as model or non-model. The default is ``False``.
          **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
@@ -67,58 +67,58 @@
         References
         ----------
 
         >>> oEditor.CreateCircle
 
         Examples
         --------
-        >>> circle1 = aedtapp.modeler.create_circle([0, -2, -2], 3)
-        >>> circle2 = aedtapp.modeler.create_circle(position=[0, -2, -2], radius=3, num_sides=6,
-        ...                                         name="MyCircle", matname="Copper")
+        >>> circle1 = aedtapp.modeler.create_circle([0, -2, -2],3)
+        >>> circle2 = aedtapp.modeler.create_circle(origin=[0, -2, -2],radius=3,
+        ...                                         num_sides=6,name="MyCircle",material="Copper")
 
 
         """
         # TODO: kwargs such as 'matname' and 'nonmodel' should be deprecated.
         szAxis = self.plane2d
-        XCenter, YCenter, ZCenter = self._pos_with_arg(position)
+        XCenter, YCenter, ZCenter = self._pos_with_arg(origin)
         Radius = self._arg_with_dim(radius)
 
         vArg1 = ["NAME:CircleParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XCenter:="), vArg1.append(XCenter)
         vArg1.append("YCenter:="), vArg1.append(YCenter)
         vArg1.append("ZCenter:="), vArg1.append(ZCenter)
         vArg1.append("Radius:="), vArg1.append(Radius)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
         vArg1.append("NumSegments:="), vArg1.append("{}".format(num_sides))
 
-        vArg2 = self._default_object_attributes(name=name, matname=matname, flags="NonModel#" if non_model else "")
+        vArg2 = self._default_object_attributes(name=name, matname=material, flags="NonModel#" if non_model else "")
         new_object_name = self.oeditor.CreateCircle(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(position="origin", matname="material")
     def create_ellipse(
-        self, position, major_radius, ratio, is_covered=True, name=None, matname=None, non_model=False, **kwargs
+        self, origin, major_radius, ratio, is_covered=True, name=None, material=None, non_model=False, **kwargs
     ):
         """Create an ellipse.
 
         Parameters
         ----------
-        position : list of float
+        origin : list of float
             Center Position of the ellipse
         major_radius : flost
             Length of the major axis of the ellipse
         ratio : float
             Ratio of the major axis to the minor axis of the ellipse
         is_covered : bool
             Specify whether the ellipse is a sheet (covered) or a line object
         name : str, default=None
             Name of the object. The default is ``None``. If ``None`` ,
             a unique name NewObject_xxxxxx will be assigned)
-        matname : str, default=None
+        material : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
         non_model : bool, optional
              Either if create the new object as model or non-model. The default is ``False``.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
@@ -133,51 +133,49 @@
         ----------
 
         >>> oEditor.CreateEllipse
 
         Examples
         --------
         >>> ellipse1 = aedtapp.modeler.create_ellipse([0, -2, -2], 4.0, 0.2)
-        >>> ellipse2 = aedtapp.modeler.create_ellipse(position=[0, -2, -2], major_radius=4.0, ratio=0.2,
-        ...                                           name="MyEllipse", matname="Copper")
+        >>> ellipse2 = aedtapp.modeler.create_ellipse(origin=[0, -2, -2], major_radius=4.0, ratio=0.2,
+        ...                                           name="MyEllipse", material="Copper")
         """
         szAxis = self.plane2d
-        XStart, YStart, ZStart = self._pos_with_arg(position)
+        XStart, YStart, ZStart = self._pos_with_arg(origin)
 
         vArg1 = ["NAME:EllipseParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XCenter:="), vArg1.append(XStart)
         vArg1.append("YCenter:="), vArg1.append(YStart)
         vArg1.append("ZCenter:="), vArg1.append(ZStart)
         vArg1.append("MajRadius:="), vArg1.append(self._arg_with_dim(major_radius))
         vArg1.append("Ratio:="), vArg1.append(ratio)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
 
-        vArg2 = self._default_object_attributes(name=name, matname=matname, flags="NonModel#" if non_model else "")
+        vArg2 = self._default_object_attributes(name=name, matname=material, flags="NonModel#" if non_model else "")
         new_object_name = self.oeditor.CreateEllipse(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_rectangle(
-        self, position, dimension_list, is_covered=True, name=None, matname=None, non_model=False, **kwargs
-    ):
+    @pyaedt_function_handler(position="origin", dimension_list="sizes", matname="material")
+    def create_rectangle(self, origin, sizes, is_covered=True, name=None, material=None, non_model=False, **kwargs):
         """Create a rectangle.
 
         Parameters
         ----------
-        position : list of float
+        origin : list
             Position of the lower-left corner of the rectangle
-        dimension_list : list of float
+        sizes : list
             List of rectangle sizes: [X size, Y size] for XY planes or [Z size, R size] for RZ planes
         is_covered : bool
             Specify whether the ellipse is a sheet (covered) or a line object
         name : str, default=None
             Name of the object. The default is ``None``. If ``None`` ,
             a unique name NewObject_xxxxxx will be assigned)
-        matname : str, default=None
+        material : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
         non_model : bool, optional
              Either if create the new object as model or non-model. The default is ``False``.
 
         Returns
         -------
@@ -187,56 +185,55 @@
         ----------
 
         >>> oEditor.CreateRectangle
 
         Examples
         --------
 
-        >>> rect1 = aedtapp.modeler.create_rectangle([0, -2, -2], [3, 4])
-        >>> rect2 = aedtapp.modeler.create_rectangle(position=[0, -2, -2], dimension_list=[3, 4],
-        ...                                          name="MyCircle", matname="Copper")
+        >>> rect1 = aedtapp.modeler.create_rectangle([0, -2, -2],[3, 4])
+        >>> rect2 = aedtapp.modeler.create_rectangle(origin=[0, -2, -2],sizes=[3, 4],name="MyCircle",material="Copper")
 
         """
         # TODO: Primitives in Maxwell 2D must have Z=0, otherwise the transparency cannot be changed. (issue 4071)
         axis = self.plane2d
-        x_start, y_start, z_start = self._pos_with_arg(position)
-        width = self._arg_with_dim(dimension_list[0])
-        height = self._arg_with_dim(dimension_list[1])
+        x_start, y_start, z_start = self._pos_with_arg(origin)
+        width = self._arg_with_dim(sizes[0])
+        height = self._arg_with_dim(sizes[1])
 
         vArg1 = ["NAME:RectangleParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XStart:="), vArg1.append(x_start)
         vArg1.append("YStart:="), vArg1.append(y_start)
         vArg1.append("ZStart:="), vArg1.append(z_start)
         vArg1.append("Width:="), vArg1.append(width)
         vArg1.append("Height:="), vArg1.append(height)
         vArg1.append("WhichAxis:="), vArg1.append(axis)
 
-        vArg2 = self._default_object_attributes(name=name, matname=matname, flags="NonModel#" if non_model else "")
+        vArg2 = self._default_object_attributes(name=name, matname=material, flags="NonModel#" if non_model else "")
         new_object_name = self.oeditor.CreateRectangle(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(position="origin", matname="material")
     def create_regular_polygon(
-        self, position, start_point, num_sides=6, name=None, matname=None, non_model=False, **kwargs
+        self, origin, start_point, num_sides=6, name=None, material=None, non_model=False, **kwargs
     ):
         """Create a rectangle.
 
         Parameters
         ----------
-        position : list of float
+        origin : list of float
             Position of the center of the polygon in ``[x, y, z]``.
         start_point : list of float
             Start point for the outer path of the polygon in ``[x, y, z]``.
         num_sides : int
             Number of sides of the polygon. Must be an integer >= 3.
         name : str, default=None
             Name of the object. The default is ``None``. If ``None`` ,
             a unique name NewObject_xxxxxx will be assigned)
-        matname : str, default=None
+        material : str, default=None
              Name of the material. The default is ``None``. If ``None``,
              the default material is assigned.
         non_model : bool, optional
              Either if create the new object as model or non-model. The default is ``False``.
          **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
@@ -251,19 +248,19 @@
 
         >>> oEditor.CreateRegularPolygon
 
         Examples
         --------
 
         >>> pg1 = aedtapp.modeler.create_regular_polygon([0, 0, 0], [0, 2, 0])
-        >>> pg2 = aedtapp.modeler.create_regular_polygon(position=[0, 0, 0], start_point=[0, 2, 0],
-        ...                                              name="MyPolygon", matname="Copper")
+        >>> pg2 = aedtapp.modeler.create_regular_polygon(origin=[0, 0, 0], start_point=[0, 2, 0],
+        ...                                              name="MyPolygon", material="Copper")
 
         """
-        x_center, y_center, z_center = self._pos_with_arg(position)
+        x_center, y_center, z_center = self._pos_with_arg(origin)
         x_start, y_start, z_start = self._pos_with_arg(start_point)
 
         n_sides = int(num_sides)
         assert n_sides > 2  # TODO: Replace assert with an exception.
 
         vArg1 = ["NAME:RegularPolygonParameters"]
         vArg1.append("XCenter:="), vArg1.append(x_center)
@@ -272,20 +269,20 @@
         vArg1.append("XStart:="), vArg1.append(x_start)
         vArg1.append("YStart:="), vArg1.append(y_start)
         vArg1.append("ZStart:="), vArg1.append(z_start)
 
         vArg1.append("NumSides:="), vArg1.append(n_sides)
         vArg1.append("WhichAxis:="), vArg1.append(self.plane2d)
 
-        vArg2 = self._default_object_attributes(name=name, matname=matname, flags="NonModel#" if non_model else "")
+        vArg2 = self._default_object_attributes(name=name, matname=material, flags="NonModel#" if non_model else "")
         new_object_name = self.oeditor.CreateRegularPolygon(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_region(self, pad_value=300, pad_type="Percentage Offset", region_name="Region", **kwarg):
+    @pyaedt_function_handler(region_name="name")
+    def create_region(self, pad_value=300, pad_type="Percentage Offset", name="Region", **kwarg):
         """Create an air region.
 
         Parameters
         ----------
         pad_value : float, str, list of floats or list of str, optional
             Padding values to apply. If a list is not provided, the same
             value is applied to all padding directions. If a list of floats
@@ -294,15 +291,15 @@
         pad_type : str, optional
             Padding definition. The default is ``"Percentage Offset"``.
             Options are ``"Absolute Offset"``,
             ``"Absolute Position"``, ``"Percentage Offset"``, and
             ``"Transverse Percentage Offset"``. When using a list,
             different padding types can be provided for different
            directions.
-        region_name : str, optional
+        name : str, optional
             Region name. The default is ``None``, in which case the name
             is generated automatically.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             Region object.
@@ -339,8 +336,8 @@
             pad_value = [pad_value[0], pad_value[2], pad_value[1], pad_value[3], 0, 0]
         else:
             if len(pad_value) < 3:
                 self.logger.error("Wrong padding list provided. Three values have to be provided for RZ geometry.")
                 return False
             pad_value = [pad_value[0], 0, 0, 0, pad_value[1], pad_value[2]]
 
-        return self._create_region(pad_value, pad_type, region_name, region_type="Region")
+        return self._create_region(pad_value, pad_type, name, region_type="Region")
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/Primitives3D.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/Primitives3D.py`

 * *Files 4% similar despite different names*

```diff
@@ -69,40 +69,39 @@
 
     Examples
     --------
     Basic usage demonstrated with an HFSS, Maxwell 3D, Icepak, Q3D, or Mechanical design:
 
     >>> from pyaedt import Hfss
     >>> app = Hfss()
-    >>> box = app.modeler.create_box(position=[0,0,0], dimensions_list=[10,5,3], name="my_box",
-    ...                              matname="copper", color=(240, 120, 0),
-    ...                              transparency=0.5)
+    >>> box = app.modeler.create_box(origin=[0,0,0],sizes=[10,5,3],
+    ...                              name="my_box",material="copper",color=(240, 120, 0),transparency=0.5)
 
     In this example, ``color`` and ``transparency`` are the variable named arguments that
     can be passed to any method that creates a primitive.
     """
 
     def __init__(self, application):
         GeometryModeler.__init__(self, application, is3d=True)
         self.multiparts = []
 
-    @pyaedt_function_handler()
-    def create_box(self, position, dimensions_list, name=None, matname=None, **kwargs):
+    @pyaedt_function_handler(position="origin", dimensions_list="sizes", matname="material")
+    def create_box(self, origin, sizes, name=None, material=None, **kwargs):
         """Create a box.
 
         Parameters
         ----------
-        position : list
+        origin : list
             Anchor point for the box in Cartesian``[x, y, z]`` coordinates.
-        dimensions_list : list
+        sizes : list
            Length of the box edges in Cartesian``[x, y, z]`` coordinates.
         name : str, optional
             Name of the box. The default is ``None``, in which case the
             default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material.  The default is ``None``, in which case the
             default material is assigned. If the material name supplied is
             invalid, the default material is assigned.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.cad.object3d.Object3d`
@@ -124,62 +123,59 @@
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, and
         Mechanical.
 
         >>> from pyaedt import hfss
         >>> hfss = Hfss()
         >>> origin = [0,0,0]
         >>> dimensions = [10,5,20]
-        >>> box_object = hfss.modeler.create_box(position=origin,
-        ...                                      dimensions_list=dimensions,
-        ...                                      name="mybox",
-        ...                                      matname="copper")
+        >>> box_object = hfss.modeler.create_box(origin=origin,sizes=dimensions,name="mybox",material="copper")
 
         """
-        if len(position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``position`` argument must be a valid three-element list.")
             return False
-        if len(dimensions_list) != 3:
+        if len(sizes) != 3:
             self.logger.error("The ``dimension_list`` argument must be a valid three-element list.")
             return False
 
-        XPosition, YPosition, ZPosition = self._pos_with_arg(position)
-        XSize, YSize, ZSize = self._pos_with_arg(dimensions_list)
+        XPosition, YPosition, ZPosition = self._pos_with_arg(origin)
+        XSize, YSize, ZSize = self._pos_with_arg(sizes)
         vArg1 = ["NAME:BoxParameters"]
         vArg1.append("XPosition:="), vArg1.append(XPosition)
         vArg1.append("YPosition:="), vArg1.append(YPosition)
         vArg1.append("ZPosition:="), vArg1.append(ZPosition)
         vArg1.append("XSize:="), vArg1.append(XSize)
         vArg1.append("YSize:="), vArg1.append(YSize)
         vArg1.append("ZSize:="), vArg1.append(ZSize)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateBox(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_cylinder(self, cs_axis, position, radius, height, numSides=0, name=None, matname=None, **kwargs):
+    @pyaedt_function_handler(cs_axis="orientation", position="origin", numSides="num_sides", matname="material")
+    def create_cylinder(self, orientation, origin, radius, height, num_sides=0, name=None, material=None, **kwargs):
         """Create a cylinder.
 
         Parameters
         ----------
-        cs_axis : int or str
+        orientation : int or str
             Axis of rotation of the starting point around the center point.
             :class:`pyaedt.constants.AXIS` Enumerator can be used as input.
-        position : list
+        origin : list
             Center point of the cylinder in a list of ``(x, y, z)`` coordinates.
         radius : float
             Radius of the cylinder.
         height : float
             Height of the cylinder.
-        numSides : int, optional
+        num_sides : int, optional
             Number of sides. The default is ``0``, which is correct for
             a cylinder.
         name : str, optional
             Name of the cylinder. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object or ``False`` if it fails.
@@ -201,69 +197,70 @@
         The optional parameter ``name`` allows to assign a name to the cylinder.
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, and
         Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> cylinder_object = aedtapp.modeler.create_cylinder(cs_axis='Z', position=[0,0,0],
-        ...                                                   radius=2, height=3, name="mycyl",
-        ...                                                   matname="vacuum")
+        >>> cylinder_object = aedtapp.modeler.create_cylinder(orientation='Z',
+        ...                                                   origin=[0,0,0],radius=2,
+        ...                                                   height=3,name="mycyl",material="vacuum")
 
         """
         if isinstance(radius, (int, float)) and radius < 0:
             self.logger.error("The ``radius`` argument must be greater than 0.")
             return False
-        if len(position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``position`` argument must be a valid three-element list.")
             return False
 
-        szAxis = GeometryOperators.cs_axis_str(cs_axis)
-        XCenter, YCenter, ZCenter = self._pos_with_arg(position)
+        szAxis = GeometryOperators.cs_axis_str(orientation)
+        XCenter, YCenter, ZCenter = self._pos_with_arg(origin)
 
         Radius = self._arg_with_dim(radius)
         Height = self._arg_with_dim(height)
 
         vArg1 = ["NAME:CylinderParameters"]
         vArg1.append("XCenter:="), vArg1.append(XCenter)
         vArg1.append("YCenter:="), vArg1.append(YCenter)
         vArg1.append("ZCenter:="), vArg1.append(ZCenter)
         vArg1.append("Radius:="), vArg1.append(Radius)
         vArg1.append("Height:="), vArg1.append(Height)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
-        vArg1.append("NumSides:="), vArg1.append("{}".format(numSides))
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg1.append("NumSides:="), vArg1.append("{}".format(num_sides))
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateCylinder(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
     # fmt: off
-    @pyaedt_function_handler()
-    def create_polyhedron(self, cs_axis=None, center_position=(0.0, 0.0, 0.0), start_position=(0.0, 1.0, 0.0),
-                          height=1.0, num_sides=12, name=None, matname=None, **kwargs):  # fmt: on
+    @pyaedt_function_handler(cs_axis="orientation", center_position="center",
+                             start_position="origin", matname="material")
+    def create_polyhedron(self, orientation=None, center=(0.0, 0.0, 0.0), origin=(0.0, 1.0, 0.0),
+                          height=1.0, num_sides=12, name=None, material=None, **kwargs):  # fmt: on
         """Create a regular polyhedron.
 
         Parameters
         ----------
-        cs_axis : optional
+        orientation : optional
             Axis of rotation of the starting point around the center point.
             The default is ``None``, in which case the Z axis is used.
-        center_position : list, optional
+        center : list, optional
             List of ``[x, y, z]`` coordinates for the center position.
             The default is ``(0.0, 0.0, 0.0)``.
-        start_position : list, optional
+        origin : list, optional
             List of ``[x, y, z]`` coordinates for the starting position.
             The default is ``(0.0, 0.0, 0.0)``.
         height : float, optional
             Height of the polyhedron. The default is ``1.0``.
         num_sides : int, optional
             Number of sides of the polyhedron. The default is ``12``.
         name : str, optional
             Name of the polyhedron. The default is ``None``, in which the
             default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which the
             default material is assigned.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object or ``False`` if it fails.
@@ -281,70 +278,70 @@
         height of the polyhedron and num_sides to determine the number of sides.
         The parameter matname is optional and allows to set the material name of the polyhedron.
         The parameter name is optional and allows to give a name to the polyhedron.
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> ret_obj = aedtapp.modeler.create_polyhedron(cs_axis='X', center_position=[0, 0, 0],
-        ...                                             start_position=[0,5,0], height=0.5,
-        ...                                              num_sides=8, name="mybox", matname="copper")
+        >>> ret_obj = aedtapp.modeler.create_polyhedron(orientation='X',center=[0, 0, 0],
+        ...                                             origin=[0,5,0],height=0.5,num_sides=8,
+        ...                                             name="mybox",material="copper")
         """
-        cs_axis = GeometryOperators.cs_axis_str(cs_axis)
-        if len(center_position) != 3:
+        orientation = GeometryOperators.cs_axis_str(orientation)
+        if len(center) != 3:
             self.logger.error("The ``center_position`` argument must be a valid three-element list.")
             return False
-        if len(start_position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``start_position`` argument must be a valid three-element list.")
             return False
-        if center_position == start_position:
+        if center == origin:
             self.logger.error("The ``center_position`` and ``start_position`` arguments must be different.")
             return False
 
-        x_center, y_center, z_center = self._pos_with_arg(center_position)
-        x_start, y_start, z_start = self._pos_with_arg(start_position)
+        x_center, y_center, z_center = self._pos_with_arg(center)
+        x_start, y_start, z_start = self._pos_with_arg(origin)
 
         height = self._arg_with_dim(height)
 
         vArg1 = ["NAME:PolyhedronParameters"]
         vArg1.append("XCenter:="), vArg1.append(x_center)
         vArg1.append("YCenter:="), vArg1.append(y_center)
         vArg1.append("ZCenter:="), vArg1.append(z_center)
         vArg1.append("XStart:="), vArg1.append(x_start)
         vArg1.append("YStart:="), vArg1.append(y_start)
         vArg1.append("ZStart:="), vArg1.append(z_start)
         vArg1.append("Height:="), vArg1.append(height)
         vArg1.append("NumSides:="), vArg1.append(int(num_sides))
-        vArg1.append("WhichAxis:="), vArg1.append(cs_axis)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg1.append("WhichAxis:="), vArg1.append(orientation)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateRegularPolyhedron(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_cone(self, cs_axis, position, bottom_radius, top_radius, height, name=None, matname=None, **kwargs):
+    @pyaedt_function_handler(cs_axis="orientation", position="origin", matname="material")
+    def create_cone(self, orientation, origin, bottom_radius, top_radius, height, name=None, material=None, **kwargs):
         """Create a cone.
 
         Parameters
         ----------
-        cs_axis : str
+        orientation : str
             Axis of rotation of the starting point around the center point.
             The default is ``None``, in which case the Z axis is used.
-        position : list, optional
+        origin : list, optional
             List of ``[x, y, z]`` coordinates for the center position
             of the bottom of the cone.
         bottom_radius : float
             Bottom radius of the cone.
         top_radius : float
             Top radius of the cone.
         height : float
             Height of the cone.
         name : str, optional
             Name of the cone. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object or ``False`` if it fails.
@@ -367,68 +364,68 @@
         The optional parameter ``name`` allows you to assign a name to the cone.
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, and
         Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> cone_object = aedtapp.modeler.create_cone(cs_axis='Z', position=[0, 0, 0],
-        ...                                           bottom_radius=2, top_radius=3, height=4,
-        ...                                           name="mybox", matname="copper")
+        >>> cone_object = aedtapp.modeler.create_cone(orientation='Z',origin=[0, 0, 0],
+        ...                                           bottom_radius=2,top_radius=3,height=4,
+        ...                                           name="mybox",material="copper")
 
         """
         if bottom_radius == top_radius:
             self.logger.error("the ``bottom_radius`` and ``top_radius`` arguments must have different values.")
             return False
         if isinstance(bottom_radius, (int, float)) and bottom_radius < 0:
             self.logger.error("The ``bottom_radius`` argument must be greater than 0.")
             return False
         if isinstance(top_radius, (int, float)) and top_radius < 0:
             self.logger.error("The ``top_radius`` argument must be greater than 0.")
             return False
         if isinstance(height, (int, float)) and height <= 0:
             self.logger.error("The ``height`` argument must be greater than 0.")
             return False
-        if len(position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``position`` argument must be a valid three-element list.")
             return False
 
-        XCenter, YCenter, ZCenter = self._pos_with_arg(position)
-        szAxis = GeometryOperators.cs_axis_str(cs_axis)
+        XCenter, YCenter, ZCenter = self._pos_with_arg(origin)
+        szAxis = GeometryOperators.cs_axis_str(orientation)
         Height = self._arg_with_dim(height)
         RadiusBt = self._arg_with_dim(bottom_radius)
         RadiusUp = self._arg_with_dim(top_radius)
 
         vArg1 = ["NAME:ConeParameters"]
         vArg1.append("XCenter:="), vArg1.append(XCenter)
         vArg1.append("YCenter:="), vArg1.append(YCenter)
         vArg1.append("ZCenter:="), vArg1.append(ZCenter)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
         vArg1.append("Height:="), vArg1.append(Height)
         vArg1.append("BottomRadius:="), vArg1.append(RadiusBt)
         vArg1.append("TopRadius:="), vArg1.append(RadiusUp)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateCone(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_sphere(self, position, radius, name=None, matname=None, **kwargs):
+    @pyaedt_function_handler(position="origin", matname="material")
+    def create_sphere(self, origin, radius, name=None, material=None, **kwargs):
         """Create a sphere.
 
         Parameters
         ----------
-        position : list
+        origin : list
             List of ``[x, y, z]`` coordinates for the center position
             of the sphere.
         radius : float
             Radius of the sphere.
         name : str, optional
             Name of the sphere. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object or ``False`` if it fails.
@@ -447,56 +444,55 @@
         ``name``  allows to assign a name to the sphere.
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, and
         Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> ret_object = aedtapp.modeler.create_sphere(position=[0,0,0], radius=2,
-        ...                                            name="mysphere", matname="copper")
+        >>> ret_object = aedtapp.modeler.create_sphere(origin=[0,0,0],radius=2,name="mysphere",material="copper")
         """
-        if len(position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``position`` argument must be a valid three-element list.")
             return False
         if isinstance(radius, (int, float)) and radius < 0:
             self.logger.error("The ``radius`` argument must be greater than 0.")
             return False
 
-        XCenter, YCenter, ZCenter = self._pos_with_arg(position)
+        XCenter, YCenter, ZCenter = self._pos_with_arg(origin)
 
         Radius = self._arg_with_dim(radius)
 
         vArg1 = ["NAME:SphereParameters"]
         vArg1.append("XCenter:="), vArg1.append(XCenter)
         vArg1.append("YCenter:="), vArg1.append(YCenter)
         vArg1.append("ZCenter:="), vArg1.append(ZCenter)
         vArg1.append("Radius:="), vArg1.append(Radius)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateSphere(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_torus(self, center, major_radius, minor_radius, axis=None, name=None, material_name=None, **kwargs):
+    @pyaedt_function_handler(center="origin", material_name="material")
+    def create_torus(self, origin, major_radius, minor_radius, axis=None, name=None, material=None, **kwargs):
         """Create a torus.
 
         Parameters
         ----------
-        center : list
+        origin : list
             Center point for the torus in a list of ``[x, y, z]`` coordinates.
         major_radius : float
            Major radius of the torus.
         minor_radius : float
            Minor radius of the torus.
         axis : str, optional
             Axis of revolution.
             The default is ``None``, in which case the Z axis is used.
         name : str, optional
             Name of the torus. The default is ``None``, in which case the
             default name is assigned.
-        material_name : str, optional
+        material : str, optional
             Name of the material.  The default is ``None``, in which case the
             default material is assigned. If the material name supplied is
             invalid, the default material is assigned.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
 
@@ -519,56 +515,56 @@
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D, and
         Mechanical.
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> origin = [0, 0, 0]
-        >>> torus = hfss.modeler.create_torus(center=origin, major_radius=1,
-        ...                                   minor_radius=0.5, axis="Z",
-        ...                                    name="mytorus", material_name="copper")
+        >>> torus = hfss.modeler.create_torus(origin=origin,major_radius=1,minor_radius=0.5,
+        ...                                   axis="Z",name="mytorus",material="copper")
+
         """
-        if len(center) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``center`` argument must be a valid three-element list.")
             return False
         # if major_radius <= 0 or minor_radius <= 0:
         #     raise ValueError("Both major and minor radius must be greater than 0.")
         # if minor_radius >= major_radius:
         #     raise ValueError("Major radius must be greater than minor radius.")
 
-        x_center, y_center, z_center = self._pos_with_arg(center)
+        x_center, y_center, z_center = self._pos_with_arg(origin)
         axis = GeometryOperators.cs_axis_str(axis)
         major_radius = self._arg_with_dim(major_radius)
         minor_radius = self._arg_with_dim(minor_radius)
 
         first_argument = ["NAME:TorusParameters"]
         first_argument.append("XCenter:="), first_argument.append(x_center)
         first_argument.append("YCenter:="), first_argument.append(y_center)
         first_argument.append("ZCenter:="), first_argument.append(z_center)
         first_argument.append("MajorRadius:="), first_argument.append(major_radius)
         first_argument.append("MinorRadius:="), first_argument.append(minor_radius)
         first_argument.append("WhichAxis:="), first_argument.append(axis)
-        second_argument = self._default_object_attributes(name=name, matname=material_name)
+        second_argument = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateTorus(first_argument, second_argument)
         return self._create_object(new_object_name, **kwargs)
 
     # fmt: off
-    @pyaedt_function_handler()
-    def create_bondwire(self, start_position, end_position, h1=0.2, h2=0, alpha=80, beta=5, bond_type=0,
-                        diameter=0.025, facets=6, name=None, matname=None, cs_axis="Z", **kwargs):  # fmt: on
+    @pyaedt_function_handler(start_position="start", end_position="end", matname="material", cs_axis="orientation")
+    def create_bondwire(self, start, end, h1=0.2, h2=0, alpha=80, beta=5, bond_type=0,
+                        diameter=0.025, facets=6, name=None, material=None, orientation="Z", **kwargs):  # fmt: on
         # type : (list, list, float|str=0.2, float|str=0, float=80, float=5, int=0, float|str=0.025, int=6, str=None,
         # str=None) -> Object3d
         """Create a bondwire.
 
         Parameters
         ----------
-        start_position : list
+        start : list
             List of ``[x, y, z]`` coordinates for the starting
             position of the bond pad.
-        end_position :  list
+        end :  list
             List of ``[x, y, z]`` coordinates for the ending position
             of the bond pad.
         h1 : float|str optional
             Height between the IC die I/O pad and the top of the bondwire.
             If the height is provided as a parameter, its value has to be provided as value + unit.
             The default is ``0.2``.
         h2 : float|str optional
@@ -593,18 +589,18 @@
         diameter : float|str optional
             Diameter of the wire. The default is ``0.025``.
         facets : int, optional
             Number of wire facets. The default is ``6``.
         name : str, optional
             Name of the bondwire. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
-        cs_axis : str, optional
+        orientation : str, optional
             Coordinate system axis. The default is ``"Z"``.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
 
         Returns
         -------
@@ -619,32 +615,32 @@
         Examples
         --------
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> origin = [0,0,0]
         >>> endpos = [10,5,20]
         >>> #Material and name are not mandatory fields
-        >>> object_id = hfss.modeler.create_bondwire(origin, endpos,h1=0.5, h2=0.1, alpha=75, beta=4,
-        ...                                          bond_type=0, name="mybox", matname="copper")
+        >>> object_id = hfss.modeler.create_bondwire(origin,endpos,h1=0.5,h2=0.1,alpha=75,
+        ...                                          beta=4,bond_type=0,name="mybox",material="copper")
         """
-        if len(start_position) != 3:
+        if len(start) != 3:
             self.logger.error("The ``start_position`` argument must be a valid three-Element List")
             return False
-        x_position, y_position, z_position = self._pos_with_arg(start_position)
-        if len(end_position) != 3:
+        x_position, y_position, z_position = self._pos_with_arg(start)
+        if len(end) != 3:
             self.logger.error("The ``end_position`` argument must be a valid three-Element List")
             return False
-        x_position_end, y_position_end, z_position_end = self._pos_with_arg(end_position)
+        x_position_end, y_position_end, z_position_end = self._pos_with_arg(end)
 
         cont = 0
         x_length = None
         y_length = None
         z_length = None
 
-        for m, n in zip(start_position, end_position):
+        for m, n in zip(start, end):
             if not isinstance(m, str):
                 m = self._arg_with_dim(m)
             if not isinstance(n, str):
                 n = self._arg_with_dim(n)
             if cont == 0:
                 x_length = "(" + str(n) + ") - (" + str(m) + ")"
             elif cont == 1:
@@ -690,38 +686,38 @@
 
         first_argument.append("Distance:="), first_argument.append(distance)
 
         first_argument.append("h1:="), first_argument.append(self._arg_with_dim(h1))
         first_argument.append("h2:="), first_argument.append(self._arg_with_dim(h2))
         first_argument.append("alpha:="), first_argument.append(self._arg_with_dim(alpha, "deg"))
         first_argument.append("beta:="), first_argument.append(self._arg_with_dim(beta, "deg"))
-        first_argument.append("WhichAxis:="), first_argument.append(GeometryOperators.cs_axis_str(cs_axis))
+        first_argument.append("WhichAxis:="), first_argument.append(GeometryOperators.cs_axis_str(orientation))
         first_argument.append("ReverseDirection:="), first_argument.append(False)
-        second_argument = self._default_object_attributes(name=name, matname=matname)
+        second_argument = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateBondwire(first_argument, second_argument)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_rectangle(self, csPlane, position, dimension_list, name=None, matname=None, is_covered=True, **kwargs):
+    @pyaedt_function_handler(csPlane="orientation", position="origin", dimension_list="sizes", matname="material")
+    def create_rectangle(self, orientation, origin, sizes, name=None, material=None, is_covered=True, **kwargs):
         """Create a rectangle.
 
         Parameters
         ----------
-        csPlane : str or int
+        orientation : str or int
             Coordinate system plane for orienting the rectangle.
             :class:`pyaedt.constants.PLANE` Enumerator can be used as input.
-        position : list or Position
+        origin : list or Position
             List of ``[x, y, z]`` coordinates of the lower-left corner of the rectangle or
             the position ApplicationName.modeler.Position(x,y,z) object.
-        dimension_list : list
+        sizes : list
             List of ``[width, height]`` dimensions.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is assigned.
         is_covered : bool, optional
             Whether the rectangle is covered. The default is ``True``.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
@@ -732,56 +728,56 @@
             3D object or ``False`` if it fails.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
         """
-        if len(dimension_list) != 2:
-            self.logger.error("The ``dimension_list`` argument must be a valid two-element list.")
+        if len(sizes) != 2:
+            self.logger.error("The ``sizes`` argument must be a valid two-element list.")
             return False
-        szAxis = GeometryOperators.cs_plane_to_axis_str(csPlane)
-        XStart, YStart, ZStart = self._pos_with_arg(position)
+        szAxis = GeometryOperators.cs_plane_to_axis_str(orientation)
+        XStart, YStart, ZStart = self._pos_with_arg(origin)
 
-        Width = self._arg_with_dim(dimension_list[0])
-        Height = self._arg_with_dim(dimension_list[1])
+        Width = self._arg_with_dim(sizes[0])
+        Height = self._arg_with_dim(sizes[1])
 
         vArg1 = ["NAME:RectangleParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XStart:="), vArg1.append(XStart)
         vArg1.append("YStart:="), vArg1.append(YStart)
         vArg1.append("ZStart:="), vArg1.append(ZStart)
         vArg1.append("Width:="), vArg1.append(Width)
         vArg1.append("Height:="), vArg1.append(Height)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateRectangle(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
     # fmt: off
-    @pyaedt_function_handler()
-    def create_circle(self, cs_plane, position, radius, numSides=0, is_covered=True, name=None,
-                      matname=None, non_model=False, **kwargs):  # fmt: on
+    @pyaedt_function_handler(cs_plane="orientation", position="origin", numSides="num_sides", matname="material")
+    def create_circle(self, orientation, origin, radius, num_sides=0, is_covered=True, name=None,
+                      material=None, non_model=False, **kwargs):  # fmt: on
         """Create a circle.
 
         Parameters
         ----------
-        cs_plane : str or int
+        orientation : str or int
             Coordinate system plane for orienting the circle.
             :class:`pyaedt.constants.PLANE` Enumerator can be used as input.
-        position : list
+        origin : list
             List of ``[x, y, z]`` coordinates for the center point of the circle.
         radius : float
             Radius of the circle.
-        numSides : int, optional
+        num_sides : int, optional
             Number of sides. The default is ``0``, which is correct for a circle.
         name : str, optional
             Name of the circle. The default is ``None``, in which case the
             default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
         non_model : bool, optional
              Either if create the new object as model or non-model. The default is ``False``.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
@@ -810,61 +806,61 @@
         to the circle.
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D,
         and Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> circle_object = aedtapp.modeler.create_circle(cs_plane='Z', position=[0,0,0],
+        >>> circle_object = aedtapp.modeler.create_circle(orientation='Z', origin=[0,0,0],
         ...                                                   radius=2, num_sides=8, name="mycyl",
-        ...                                                   matname="vacuum")
+        ...                                                   material="vacuum")
         """
         non_model_flag = ""
         if non_model:
             non_model_flag = "NonModel#"
-        szAxis = GeometryOperators.cs_plane_to_axis_str(cs_plane)
-        XCenter, YCenter, ZCenter = self._pos_with_arg(position)
+        szAxis = GeometryOperators.cs_plane_to_axis_str(orientation)
+        XCenter, YCenter, ZCenter = self._pos_with_arg(origin)
         Radius = self._arg_with_dim(radius)
         vArg1 = ["NAME:CircleParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XCenter:="), vArg1.append(XCenter)
         vArg1.append("YCenter:="), vArg1.append(YCenter)
         vArg1.append("ZCenter:="), vArg1.append(ZCenter)
         vArg1.append("Radius:="), vArg1.append(Radius)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
-        vArg1.append("NumSegments:="), vArg1.append("{}".format(numSides))
-        vArg2 = self._default_object_attributes(name=name, matname=matname, flags=non_model_flag)
+        vArg1.append("NumSegments:="), vArg1.append("{}".format(num_sides))
+        vArg2 = self._default_object_attributes(name=name, matname=material, flags=non_model_flag)
         new_object_name = self.oeditor.CreateCircle(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(cs_plane="orientation", position="origin", matname="material")
     def create_ellipse(
-            self, cs_plane, position, major_radius, ratio, is_covered=True, name=None, matname=None, **kwargs
+            self, orientation, origin, major_radius, ratio, is_covered=True, name=None, material=None, **kwargs
     ):
         """Create an ellipse.
 
         Parameters
         ----------
-        cs_plane : str or int
+        orientation : str or int
             Coordinate system plane for orienting the ellipse.
             :class:`pyaedt.constants.PLANE` Enumerator can be used as input.
-        position : list
+        origin : list
             List of ``[x, y, z]`` coordinates for the center point of the ellipse.
         major_radius : float
             Base radius of the ellipse.
         ratio : float
             Aspect ratio of the secondary radius to the base radius.
         is_covered : bool, optional
             Whether the ellipse is covered. The default is ``True``,
             in which case the result is a 2D sheet object. If ``False,``
             the result is a closed 1D polyline object.
         name : str, optional
             Name of the ellipse. The default is ``None``, in which case the
             default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case the
             default material is assigned.
         **kwargs : optional
             Additional keyword arguments may be passed when creating the primitive to set properties. See
             ``pyaedt.modeler.cad.object3d.Object3d`` for more details.
 
         Returns
@@ -893,34 +889,34 @@
         to the ellipse.
 
         This method applies to all 3D applications: HFSS, Q3D, Icepak, Maxwell 3D,
         and Mechanical.
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
-        >>> ellipse = aedtapp.modeler.create_ellipse(cs_plane='Z', position=[0,0,0],
+        >>> ellipse = aedtapp.modeler.create_ellipse(orientation='Z', origin=[0,0,0],
         ...                                          major_radius=2, ratio=2, is_covered=True, name="myell",
-        ...                                          matname="vacuum")
+        ...                                          material="vacuum")
 
 
         """
-        szAxis = GeometryOperators.cs_plane_to_axis_str(cs_plane)
-        XStart, YStart, ZStart = self._pos_with_arg(position)
+        szAxis = GeometryOperators.cs_plane_to_axis_str(orientation)
+        XStart, YStart, ZStart = self._pos_with_arg(origin)
 
         MajorRadius = self._arg_with_dim(major_radius)
 
         vArg1 = ["NAME:EllipseParameters"]
         vArg1.append("IsCovered:="), vArg1.append(is_covered)
         vArg1.append("XCenter:="), vArg1.append(XStart)
         vArg1.append("YCenter:="), vArg1.append(YStart)
         vArg1.append("ZCenter:="), vArg1.append(ZStart)
         vArg1.append("MajRadius:="), vArg1.append(MajorRadius)
         vArg1.append("Ratio:="), vArg1.append(ratio)
         vArg1.append("WhichAxis:="), vArg1.append(szAxis)
-        vArg2 = self._default_object_attributes(name=name, matname=matname)
+        vArg2 = self._default_object_attributes(name=name, matname=material)
         new_object_name = self.oeditor.CreateEllipse(vArg1, vArg2)
         return self._create_object(new_object_name, **kwargs)
 
     # fmt: off
     @pyaedt_function_handler()
     def create_equationbased_curve(self, x_t=0, y_t=0, z_t=0, t_start=0, t_end=1, num_points=0, name=None,
                                    xsection_type=None, xsection_orient=None, xsection_width=1, xsection_topwidth=1,
@@ -1043,32 +1039,32 @@
 
         vArg2 = self._default_object_attributes(name)
 
         new_name = self.oeditor.CreateEquationCurve(vArg1, vArg2)
         return self._create_object(new_name, **kwargs)
 
     # fmt: off
-    @pyaedt_function_handler()
-    def create_helix(self, polyline_name, position, x_start_dir, y_start_dir, z_start_dir, num_thread=1,
+    @pyaedt_function_handler(polyline_name="assignment", position="origin", num_thread="turns")
+    def create_helix(self, assignment, origin, x_start_dir, y_start_dir, z_start_dir, turns=1,
                      right_hand=True, radius_increment=0.0, thread=1, **kwargs):  # fmt: on
         """Create an helix from a polyline.
 
         Parameters
         ----------
-        polyline_name : str
+        assignment : str
             Name of the polyline used as the base for the helix.
-        position : list
+        origin : list
             List of ``[x, y, z]`` coordinates for the center point of the circle.
         x_start_dir : float
             Distance along x axis from the polyline.
         y_start_dir : float
             Distance along y axis from the polyline.
         z_start_dir : float
             Distance along z axis from the polyline.
-        num_thread : int, optional
+        turns : int, optional
             Number of turns. The default value is ``1``.
         right_hand : bool, optional
             Whether the helix turning direction is right hand. The default value is ``True``.
         radius_increment : float, optional
             Radius change per turn. The default value is ``0.0``.
         thread : float
         **kwargs : optional
@@ -1093,41 +1089,31 @@
 
         >>> from pyaedt import Hfss
         >>> aedtapp = Hfss()
         >>> udp1 = [0, 0, 0]
         >>> udp2 = [5, 0, 0]
         >>> udp3 = [10, 5, 0]
         >>> udp4 = [15, 3, 0]
-        >>> polyline = aedtapp.modeler.create_polyline(
-        ...     [udp1, udp2, udp3, udp4], cover_surface=False, name="helix_polyline"
-        ... )
-
-        >>> helix_right_turn = aedtapp.modeler.create_helix(
-        ...     polyline_name=polyline.name,
-        ...     position=[0, 0, 0],
-        ...     x_start_dir=0,
-        ...     y_start_dir=1.0,
-        ...     z_start_dir=1.0,
-        ...     num_thread=1,
-        ...     right_hand=True,
-        ...     radius_increment=0.0,
-        ...     thread=1.0,
-        ... )
+        >>> polyline = aedtapp.modeler.create_polyline([udp1, udp2, udp3, udp4],cover_surface=False,
+        ...                                            name="helix_polyline")
+        >>> helix_right_turn = aedtapp.modeler.create_helix(assignment=polyline.name,origin=[0, 0, 0],
+        ...                                                 x_start_dir=0,y_start_dir=1.0,z_start_dir=1.0,
+        ...                                                 turns=1,right_hand=True,radius_increment=0.0,thread=1.0)
         """
-        if not polyline_name or polyline_name == "":
+        if not assignment or assignment == "":
             self.logger.error("The name of the polyline cannot be an empty string.")
             return False
 
-        if len(position) != 3:
+        if len(origin) != 3:
             self.logger.error("The ``position`` argument must be a valid three-element list.")
             return False
-        x_center, y_center, z_center = self._pos_with_arg(position)
+        x_center, y_center, z_center = self._pos_with_arg(origin)
 
         vArg1 = ["NAME:Selections"]
-        vArg1.append("Selections:="), vArg1.append(polyline_name)
+        vArg1.append("Selections:="), vArg1.append(assignment)
         vArg1.append("NewPartsModelFlag:="), vArg1.append("Model")
 
         vArg2 = ["NAME:HelixParameters"]
         vArg2.append("XCenter:=")
         vArg2.append(x_center)
         vArg2.append("YCenter:=")
         vArg2.append(y_center)
@@ -1136,44 +1122,44 @@
         vArg2.append("XStartDir:=")
         vArg2.append(self._arg_with_dim(x_start_dir))
         vArg2.append("YStartDir:=")
         vArg2.append(self._arg_with_dim(y_start_dir))
         vArg2.append("ZStartDir:=")
         vArg2.append(self._arg_with_dim(z_start_dir))
         vArg2.append("NumThread:=")
-        vArg2.append(num_thread)
+        vArg2.append(turns)
         vArg2.append("RightHand:=")
         vArg2.append(right_hand)
         vArg2.append("RadiusIncrement:=")
         vArg2.append(self._arg_with_dim(radius_increment))
         vArg2.append("Thread:=")
         vArg2.append(self._arg_with_dim(thread))
 
         self.oeditor.CreateHelix(vArg1, vArg2)
-        if polyline_name in self.objects_by_name:
-            del self.objects[self.objects_by_name[polyline_name].id]
-        return self._create_object(polyline_name, **kwargs)
+        if assignment in self.objects_by_name:
+            del self.objects[self.objects_by_name[assignment].id]
+        return self._create_object(assignment, **kwargs)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(udmfullname="udm_full_name", udm_params_list="parameters", udm_library="library")
     def create_udm(
             self,
-            udmfullname,
-            udm_params_list,
-            udm_library="syslib",
+            udm_full_name,
+            parameters,
+            library="syslib",
             name=None,
     ):
         """Create a user-defined model.
 
         Parameters
         ----------
-        udmfullname : str
+        udm_full_name : str
             Full name for the user-defined model, including the folder name.
-        udm_params_list :
+        parameters :
             List of user-defined object pairs for the model.
-        udm_library : str, optional
+        library : str, optional
             Name of the library for the user-defined model. The default is ``"syslib"``.
         name : str, optional
             Name of the user-defined model. The default is ``None```.
 
         Returns
         -------
         bool, :class:`pyaedt.modeler.components_3d.UserDefinedComponent`
@@ -1184,15 +1170,15 @@
 
         >>> oEditor.CreateUserDefinedModel
 
         """
         vArg1 = ["NAME:UserDefinedModelParameters", ["NAME:Definition"], ["NAME:Options"]]
         vArgParamVector = ["NAME:GeometryParams"]
 
-        for pair in udm_params_list:
+        for pair in parameters:
             if isinstance(pair, list):
                 name_param = pair[0]
                 val = pair[1]
             else:
                 name_param = pair.Name
                 val = pair.Value
             if isinstance(val, int):
@@ -1222,17 +1208,17 @@
                         "PropFlag2:=",
                         0,
                     ]
                 )
 
         vArg1.append(vArgParamVector)
         vArg1.append("DllName:=")
-        vArg1.append(udmfullname)
+        vArg1.append(udm_full_name)
         vArg1.append("Library:=")
-        vArg1.append(udm_library)
+        vArg1.append(library)
         vArg1.append("Version:=")
         vArg1.append("2.0")
         vArg1.append("ConnectionID:=")
         vArg1.append("")
         oname = self.oeditor.CreateUserDefinedModel(vArg1)
         if oname:
             obj_list = list(self.oeditor.GetPartsForUserDefinedModel(oname))
@@ -1302,33 +1288,32 @@
             rin += dr
             theta += dtheta
             x0, y0 = pts[-1][:2]
             x1, y1 = x0 + rin * cos(theta), y0 + rin * sin(theta)
             pts.append((x1, y1, elevation))
 
         pts.append((x1, 0, elevation))
-        p1 = self.create_polyline(
-            pts, xsection_type="Rectangle", xsection_width=width, xsection_height=thickness, matname=material
-        )
+        p1 = self.create_polyline(pts, material=material, xsection_type="Rectangle", xsection_width=width,
+                                  xsection_height=thickness)
         if name:
             p1.name = name
             self._create_object(name, **kwargs)
         return p1
 
-    @pyaedt_function_handler()
-    def _create_reference_cs_from_3dcomp(self, udm_obj, password):
+    @pyaedt_function_handler(udm_obj="assignment")
+    def _create_reference_cs_from_3dcomp(self, assignment, password):
         """Create a new coordinate system from the 3d component reference one.
 
         Returns
         -------
         str
             Name of the created coordinate system that mirrors the reference one of the
             3d component.
         """
-        app = udm_obj.edit_definition(password=password)
+        app = assignment.edit_definition(password=password)
         wcs = app.modeler.oeditor.GetActiveCoordinateSystem()
         if wcs != "Global":
             temp_folder = os.path.join(
                 self._app.toolkit_directory, self._app.design_name, generate_unique_name("temp_folder")
             )
             os.makedirs(os.path.join(temp_folder))
             if not os.path.exists(os.path.join(self._app.toolkit_directory, self._app.design_name)):  # pragma: no cover
@@ -1340,75 +1325,78 @@
             for root, dirs, files in os.walk(temp_folder, topdown=False):
                 for name in files:
                     os.remove(os.path.join(root, name))
                 for name in dirs:
                     os.rmdir(os.path.join(root, name))
             os.rmdir(temp_folder)
             phi, theta, psi = GeometryOperators.quaternion_to_euler_zxz(q)
-            cs_name = udm_obj.name + "_" + wcs + "_ref"
+            cs_name = assignment.name + "_" + wcs + "_ref"
             if cs_name not in [i.name for i in self.coordinate_systems]:
                 self.create_coordinate_system(
                     mode="zxz",
                     origin=o,
                     name=cs_name,
-                    reference_cs=udm_obj.target_coordinate_system,
+                    reference_cs=assignment.target_coordinate_system,
                     psi=psi,
                     theta=theta,
                     phi=phi,
                 )
             return cs_name
         else:
             app.oproject.Close()
-            return udm_obj.target_coordinate_system
+            return assignment.target_coordinate_system
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(comp_file="input_file", geo_params="geometry_parameters",
+                             sz_mat_params="material_parameters",
+                             sz_design_params="design_parameters",
+                             targetCS="coordinate_system", auxiliary_dict="auxiliary_parameters")
     def insert_3d_component(
             self,
-            comp_file,
-            geo_params=None,
-            sz_mat_params="",
-            sz_design_params="",
-            targetCS="Global",
+            input_file,
+            geometry_parameters=None,
+            material_parameters="",
+            design_parameters="",
+            coordinate_system="Global",
             name=None,
             password="",
-            auxiliary_dict=False,
+            auxiliary_parameters=False,
     ):
         """Insert a new 3D component.
 
         Parameters
         ----------
-        comp_file : str
+        input_file : str
             Name of the component file.
-        geo_params : dict, optional
+        geometry_parameters : dict, optional
             Geometrical parameters.
-        sz_mat_params : str, optional
+        material_parameters : str, optional
             Material parameters. The default is ``""``.
-        sz_design_params : str, optional
+        design_parameters : str, optional
             Design parameters. The default is ``""``.
-        targetCS : str, optional
+        coordinate_system : str, optional
             Target coordinate system. The default is ``"Global"``.
         name : str, optional
             3D component name. The default is ``None``.
         password : str, optional
             Password for encrypted components. The default is an empty string.
-        auxiliary_dict : bool or str, optional
+        auxiliary_parameters : bool or str, optional
             Enable the advanced 3d component import. It is possible to set explicitly the json file.
             The default is ``False``.
 
         Returns
         -------
         :class:`pyaedt.modeler.components_3d.UserDefinedComponent`
             User defined component object.
 
         References
         ----------
 
         >>> oEditor.Insert3DComponent
         """
-        aedt_fh = open_file(comp_file, "rb")
+        aedt_fh = open_file(input_file, "rb")
         if aedt_fh:
             temp = aedt_fh.read().splitlines()
             _all_lines = []
             for line in temp:
                 try:
                     _all_lines.append(line.decode("utf-8").lstrip("\t"))
                 except UnicodeDecodeError:
@@ -1417,51 +1405,51 @@
                 if "IsEncrypted" in line:
                     line_list = line.split("=")
                     if line_list[1] in ["true", "True", True] and password == "":
                         self.logger.warning("Encrypted model.")
             aedt_fh.close()
         vArg1 = ["NAME:InsertComponentData"]
         sz_geo_params = ""
-        if not geo_params:
-            geometryparams = self._app.get_components3d_vars(comp_file)
+        if not geometry_parameters:
+            geometryparams = self._app.get_components3d_vars(input_file)
             if geometryparams:
-                geo_params = geometryparams
+                geometry_parameters = geometryparams
 
-        if geo_params:
-            sz_geo_params = "".join(["{0}='{1}' ".format(par, val) for par, val in geo_params.items()])
+        if geometry_parameters:
+            sz_geo_params = "".join(["{0}='{1}' ".format(par, val) for par, val in geometry_parameters.items()])
         vArg1.append("TargetCS:=")
-        vArg1.append(targetCS)
+        vArg1.append(coordinate_system)
         vArg1.append("ComponentFile:=")
-        vArg1.append(comp_file)
+        vArg1.append(input_file)
         vArg1.append("IsLocal:=")
         vArg1.append(False)
         vArg1.append("UniqueIdentifier:=")
         vArg1.append("")
         varg2 = [
             "NAME:InstanceParameters",
             "GeometryParameters:=",
             sz_geo_params,
             "MaterialParameters:=",
-            sz_mat_params,
+            material_parameters,
             "DesignParameters:=",
-            sz_design_params,
+            design_parameters,
         ]
         vArg1.append(varg2)
         vArg1.append("Password:=")
         vArg1.append(password)
         try:
             new_object_name = self.oeditor.Insert3DComponent(vArg1)
             if new_object_name:
                 obj_list = list(self.oeditor.Get3DComponentPartNames(new_object_name))
                 for new_name in obj_list:
                     self._create_object(new_name)
-                if auxiliary_dict:
-                    if isinstance(auxiliary_dict, bool):
-                        auxiliary_dict = comp_file + ".json"
-                    aux_dict = json.load(open(auxiliary_dict, "r"))
+                if auxiliary_parameters:
+                    if isinstance(auxiliary_parameters, bool):
+                        auxiliary_parameters = input_file + ".json"
+                    aux_dict = json.load(open(auxiliary_parameters, "r"))
                     if aux_dict.get("datasets", None):
                         for dat in aux_dict["datasets"]:
                             key = dat["Name"]
                             if key.startswith("$"):
                                 is_project_dataset = True
                                 dsname = key[1:]
                             else:
@@ -1476,19 +1464,19 @@
                                 is_project_dataset,
                                 dat["xunit"],
                                 dat["yunit"],
                                 dat["zunit"],
                                 dat["vunit"],
                             )
                 udm_obj = self._create_user_defined_component(new_object_name)
-                if name and not auxiliary_dict:
+                if name and not auxiliary_parameters:
                     udm_obj.name = name
         except Exception:  # pragma: no cover
             udm_obj = False
-        if auxiliary_dict and udm_obj:
+        if auxiliary_parameters and udm_obj:
             mapping_dict = {}
             if aux_dict.get("native components", None):
                 if aux_dict.get("coordinatesystems", None):
                     for cs in list(aux_dict["coordinatesystems"].keys()):
                         aux_dict["coordinatesystems"][udm_obj.name + "_" + cs] = aux_dict["coordinatesystems"][cs]
                         aux_dict["coordinatesystems"].pop(cs)
                         if aux_dict["coordinatesystems"][udm_obj.name + "_" + cs]["Reference CS"] != "Global":
@@ -1519,23 +1507,23 @@
                 temp_dict_file = os.path.join(self._app.toolkit_directory, generate_unique_name("tempdict_"))
                 with open_file(temp_dict_file, "w") as f:
                     json.dump(temp_dict, f)
                 exclude_set = set([obj.name for _, obj in self._app.modeler.objects.items()])
                 old_udm = set(list(self._app.modeler.user_defined_components))
                 old_cs = set(self._app.modeler.coordinate_systems)
                 self._app.configurations.import_config(temp_dict_file, exclude_set)
-                targetCS = self._create_reference_cs_from_3dcomp(udm_obj, password)
-                if targetCS != "Global":
+                coordinate_system = self._create_reference_cs_from_3dcomp(udm_obj, password)
+                if coordinate_system != "Global":
                     self._app.modeler.refresh_all_ids()
                     for udm in set(list(self._app.modeler.user_defined_components)) - old_udm:
                         if self._app.modeler.user_defined_components[udm].target_coordinate_system == "Global":
-                            self._app.modeler.user_defined_components[udm].target_coordinate_system = targetCS
+                            self._app.modeler.user_defined_components[udm].target_coordinate_system = coordinate_system
                 for cs in set(self._app.modeler.coordinate_systems) - old_cs:
                     if cs.ref_cs == "Global":
-                        cs.ref_cs = targetCS
+                        cs.ref_cs = coordinate_system
             if aux_dict.get("monitors", None):
                 temp_proj_name = generate_unique_project_name()
                 ipkapp_temp = Icepak(projectname=os.path.join(self._app.toolkit_directory, temp_proj_name))
                 ipkapp_temp.delete_design(ipkapp_temp.design_name)
                 self._app.oproject.CopyDesign(self._app.design_name)
                 ipkapp_temp.oproject.Paste()
                 temp_proj = ipkapp_temp.project_file
@@ -1596,15 +1584,15 @@
                 else:
                     mapping_dict["ReferenceCoordSystemName"] = "Global"
                 for mon in aux_dict["monitors"]:
                     key = udm_obj.name + "_" + mon["Name"]
                     m_case = mon["Type"]
                     if m_case == "Point":
                         cs_old = self._app.odesign.SetActiveEditor("3D Modeler").GetActiveCoordinateSystem()
-                        self._app.modeler.set_working_coordinate_system(targetCS)
+                        self._app.modeler.set_working_coordinate_system(coordinate_system)
                         self._app.monitor.assign_point_monitor(
                             mon["Location"], monitor_quantity=mon["Quantity"], monitor_name=key
                         )
                         self._app.modeler.set_working_coordinate_system(cs_old)
                     elif m_case == "Face":
                         self._app.monitor.assign_face_monitor(
                             mapping_dict["FaceKeyIDMap"][str(mon["ID"])],
@@ -1632,29 +1620,29 @@
             if name:
                 udm_obj.name = name
             os.remove(temp_proj)
             return udm_obj, mapping_dict, aux_dict
         else:
             return udm_obj
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(comp_file="input_file")
     def insert_layout_component(
             self,
-            comp_file,
+            input_file,
             coordinate_system="Global",
             name=None,
             parameter_mapping=False,
             layout_coordinate_systems=None,
             reference_coordinate_system="Global"
     ):
         """Insert a new layout component.
 
         Parameters
         ----------
-        comp_file : str
+        input_file : str
             Path of the component file. Either ``".aedb"`` and ``".aedbcomp"`` are allowed.
         coordinate_system : str, optional
             Target coordinate system. The default is ``"Global"``.
         name : str, optional
             3D component name. The default is ``None``.
         parameter_mapping : bool, optional
             Whether to map the layout parameters in the target HFSS design. The default is ``False``.
@@ -1683,15 +1671,15 @@
         """
         if layout_coordinate_systems is None:
             layout_coordinate_systems = []
         if self._app.solution_type != "Terminal" and self._app.solution_type != "TransientAPhiFormulation":
             self.logger.warning("Solution type must be terminal in HFSS or APhi in Maxwell")
             return False
 
-        component_name = os.path.splitext(os.path.basename(comp_file))[0]
+        component_name = os.path.splitext(os.path.basename(input_file))[0]
         aedt_component_name = component_name
         if component_name not in self._app.o_component_manager.GetNames():
             compInfo = ["NAME:" + str(component_name), "Info:=", []]
 
             compInfo.extend(
                 [
                     "CircuitEnv:=",
@@ -1703,28 +1691,28 @@
                     "ModSinceLib:=",
                     True,
                     "Terminal:=",
                     [],
                     "CompExtID:=",
                     9,
                     "ModelEDBFilePath:=",
-                    comp_file,
+                    input_file,
                     "EDBCompPassword:=",
                     "",
                 ]
             )
 
             aedt_component_name = self._app.o_component_manager.Add(compInfo)
 
         if not name or name in self.user_defined_component_names:
             name = generate_unique_name("LC")
 
         # Open Layout component and get information
-        aedb_component_path = comp_file
-        if os.path.splitext(os.path.basename(comp_file))[1] == ".aedbcomp":
+        aedb_component_path = input_file
+        if os.path.splitext(os.path.basename(input_file))[1] == ".aedbcomp":
             aedb_project_path = os.path.join(self._app.project_path, self._app.project_name + ".aedb")
             aedb_component_path = os.path.join(
                 aedb_project_path, "LayoutComponents", aedt_component_name, aedt_component_name + ".aedb"
             )
             aedb_component_path = normalize_path(aedb_component_path)
 
         is_edb_open = False
@@ -1901,35 +1889,35 @@
                     udm_obj.name = name
                     udm_obj.layout_component._name = name
 
         except Exception:  # pragma: no cover
             udm_obj = False
         return udm_obj
 
-    @pyaedt_function_handler()
-    def get_3d_component_object_list(self, componentname):
+    @pyaedt_function_handler(componentname="name")
+    def get_3d_component_object_list(self, name):
         """Retrieve all objects belonging to a 3D component.
 
         Parameters
         ----------
-        componentname : str
+        name : str
             Name of the 3D component.
 
         Returns
         -------
         List
             List of objects belonging to the 3D component.
 
         References
         ----------
 
         >>> oeditor.GetChildObject
         """
         if self._app._is_object_oriented_enabled():
-            compobj = self.oeditor.GetChildObject(componentname)
+            compobj = self.oeditor.GetChildObject(name)
             if compobj:
                 return list(compobj.GetChildNames())
         else:
             self.logger.warning("Object Oriented Beta Option is not enabled in this Desktop.")
         return []
 
     @pyaedt_function_handler()
@@ -1947,25 +1935,25 @@
     @pyaedt_function_handler()
     def _initialize_multipart(self):
         if MultiPartComponent._t in self._app._variable_manager.independent_variable_names:
             return True
         else:
             return MultiPartComponent.start(self._app)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(actor_folder="input_dir", relative_cs_name="coordinate_system", actor_name="name")
     def add_person(
             self,
-            actor_folder,
+            input_dir,
             speed=0.0,
             global_offset=[0, 0, 0],
             yaw=0,
             pitch=0,
             roll=0,
-            relative_cs_name=None,
-            actor_name=None,
+            coordinate_system=None,
+            name=None,
     ):
         """Add a Walking Person Multipart from 3D Components.
 
         It requires a json file in the folder containing person
         infos. An example json file follows:
 
          .. code-block:: json
@@ -2014,66 +2002,66 @@
                         "rotation_axis":null
                         }
                 }
             }
 
         Parameters
         ----------
-        actor_folder : str
+        input_dir : str
             Path to the actor folder. It must contain a json settings
             file and a 3dcomponent (.a3dcomp).
         speed :  float, optional
             Object movement speed with time (m_per_sec).
         global_offset : list, optional
             Offset from Global Coordinate System [x,y,z] in meters.
         yaw : float, optional
             Yaw Rotation from Global Coordinate System in deg.
         pitch : float, optional
             Pitch Rotation from Global Coordinate System in deg.
         roll : float, optional
             Roll Rotation from Global Coordinate System in deg.
-        relative_cs_name : str
+        coordinate_system : str
             Relative CS Name of the actor. ``None`` for Global CS.
-        actor_name : str
+        name : str
             If provided, it overrides the actor name in the JSON.
 
         Returns
         -------
         :class:`pyaedt.modeler.actors.Person`
 
         References
         ----------
 
         >>> oEditor.Insert3DComponent
         """
         self._initialize_multipart()
-        if not self._check_actor_folder(actor_folder):
+        if not self._check_actor_folder(input_dir):
             return False
-        person1 = Person(actor_folder, speed=speed, relative_cs_name=relative_cs_name)
-        if actor_name:
-            person1._name = actor_name
+        person1 = Person(input_dir, speed=speed, relative_cs_name=coordinate_system)
+        if name:
+            person1._name = name
         person1.offset = global_offset
         person1.yaw = self._arg_with_dim(yaw, "deg")
         person1.pitch = self._arg_with_dim(pitch, "deg")
         person1.roll = self._arg_with_dim(roll, "deg")
         person1.insert(self._app)
         self.multiparts.append(person1)
         return person1
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(actor_folder="input_dir", relative_cs_name="coordinate_system", actor_name="name")
     def add_vehicle(
             self,
-            actor_folder,
+            input_dir,
             speed=0,
             global_offset=[0, 0, 0],
             yaw=0,
             pitch=0,
             roll=0,
-            relative_cs_name=None,
-            actor_name=None,
+            coordinate_system=None,
+            name=None,
     ):
         """Add a Moving Vehicle Multipart from 3D Components.
 
         It requires a json file in the folder containing vehicle
         infos. An example json file follows:
 
          .. code-block:: json
@@ -2105,66 +2093,66 @@
                         "rotation_axis":null
                         }
                 }
             }
 
         Parameters
         ----------
-        actor_folder : str
+        input_dir : str
             Path to the actor directory. It must contain a json settings file
             and a 3dcomponent (``.a3dcomp`` file).
         speed :  float, optional
             Object movement speed with time (m_per_sec).
         global_offset : list, optional
             Offset from Global Coordinate System [x,y,z] in meters.
         yaw : float, optional
             Yaw Rotation from Global Coordinate System in deg.
         pitch : float, optional
             Pitch Rotation from Global Coordinate System in deg.
         roll : float, optional
             Roll Rotation from Global Coordinate System in deg.
-        relative_cs_name : str
+        coordinate_system : str
             Relative CS Name of the actor. ``None`` for Global CS.
 
         Returns
         -------
         :class:`pyaedt.modeler.actors.Vehicle`
 
         References
         ----------
 
         >>> oEditor.Insert3DComponent
         """
         self._initialize_multipart()
 
-        if not self._check_actor_folder(actor_folder):
+        if not self._check_actor_folder(input_dir):
             return False
-        vehicle = Vehicle(actor_folder, speed=speed, relative_cs_name=relative_cs_name)
-        if actor_name:
-            vehicle._name = actor_name
+        vehicle = Vehicle(input_dir, speed=speed, relative_cs_name=coordinate_system)
+        if name:
+            vehicle._name = name
         vehicle.offset = global_offset
         vehicle.yaw = self._arg_with_dim(yaw, "deg")
         vehicle.pitch = self._arg_with_dim(pitch, "deg")
         vehicle.roll = self._arg_with_dim(roll, "deg")
         vehicle.insert(self._app)
         self.multiparts.append(vehicle)
         return vehicle
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(actor_folder="input_dir", relative_cs_name="coordinate_system", actor_name="name")
     def add_bird(
             self,
-            actor_folder,
+            input_dir,
             speed=0,
             global_offset=[0, 0, 0],
             yaw=0,
             pitch=0,
             roll=0,
             flapping_rate=50,
-            relative_cs_name=None,
-            actor_name=None,
+            coordinate_system=None,
+            name=None,
     ):
         """Add a Bird Multipart from 3D Components.
 
         It requires a json file in the folder containing bird infos. An example json file is showed here.
 
          .. code-block:: json
 
@@ -2206,30 +2194,30 @@
                         "rotation_axis":null
                     }
                 }
             }
 
         Parameters
         ----------
-        actor_folder : str
+        input_dir : str
             Path to the actor directory. It must contain a json settings file and a
             3dcomponent (``.a3dcomp`` file)
         speed :  float, optional
             Object movement speed with time (m_per_sec).
         global_offset : list, optional
             Offset from Global Coordinate System [x,y,z] in meters.
         yaw : float, optional
             Yaw Rotation from Global Coordinate System in deg.
         pitch : float, optional
             Pitch Rotation from Global Coordinate System in deg.
         roll : float, optional
             Roll Rotation from Global Coordinate System in deg.
         flapping_rate : float, optional
             Motion flapping rate in Hz.
-        relative_cs_name : str
+        coordinate_system : str
             Relative CS Name of the actor. ``None`` for Global CS.
 
         Returns
         -------
         :class:`pyaedt.modeler.actors.Bird`
 
         References
@@ -2238,41 +2226,41 @@
         >>> oEditor.Insert3DComponent
 
         Examples
         --------
         >>> from pyaedt import Hfss
         >>> app = Hfss()
         >>> bird_dir = "path/to/bird/directory"
-        >>> bird1 = app.modeler.add_bird(bird_dir, 1.0, [19, 4, 3], 120, -5, flapping_rate=30)
+        >>> bird1 = app.modeler.add_bird(bird_dir,1.0,[19, 4, 3],120,-5,flapping_rate=30)
 
         """
         self._initialize_multipart()
 
-        if not self._check_actor_folder(actor_folder):
+        if not self._check_actor_folder(input_dir):
             return False
         bird = Bird(
-            actor_folder,
+            input_dir,
             speed=speed,
             flapping_rate=self._arg_with_dim(flapping_rate, "Hz"),
-            relative_cs_name=relative_cs_name,
+            relative_cs_name=coordinate_system,
         )
-        if actor_name:
-            bird._name = actor_name
+        if name:
+            bird._name = name
         bird.offset = global_offset
         bird.yaw = self._arg_with_dim(yaw, "deg")
         bird.pitch = self._arg_with_dim(pitch, "deg")
         bird.roll = self._arg_with_dim(roll, "deg")
         bird.insert(self._app)
         self.multiparts.append(bird)
         return bird
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(env_folder="input_dir", relative_cs_name="coordinate_system", environment_name="name")
     def add_environment(
-            self, env_folder, global_offset=[0, 0, 0], yaw=0, pitch=0, roll=0, relative_cs_name=None,
-            environment_name=None
+            self, input_dir, global_offset=[0, 0, 0], yaw=0, pitch=0, roll=0, coordinate_system=None,
+            name=None
     ):
         """Add an Environment Multipart Component from JSON file.
 
          .. code-block:: json
 
             {
                 "name": "open1",
@@ -2291,59 +2279,59 @@
                         "duplicate_vector":null
                         }
                 }
             }
 
         Parameters
         ----------
-        env_folder : str
+        input_dir : str
             Path to the actor directory. It must contain a json
             settings file and a 3dcomponent (``.a3dcomp`` file).
         global_offset : list, optional
             Offset from Global Coordinate System [x,y,z] in meters.
         yaw : float, optional
             Yaw Rotation from Global Coordinate System in deg.
         pitch : float, optional
             Pitch Rotation from Global Coordinate System in deg.
         roll : float, optional
             Roll Rotation from Global Coordinate System in deg.
-        relative_cs_name : str
+        coordinate_system : str
             Relative CS Name of the actor. ``None`` for Global CS.
 
         Returns
         -------
         :class:`pyaedt.modeler.multiparts.Environment`
 
         References
         ----------
 
         >>> oEditor.Insert3DComponent
 
         """
         self._initialize_multipart()
-        if not self._check_actor_folder(env_folder):
+        if not self._check_actor_folder(input_dir):
             return False
-        environment = Environment(env_folder, relative_cs_name=relative_cs_name)
-        if environment_name:
-            environment._name = environment_name
+        environment = Environment(input_dir, relative_cs_name=coordinate_system)
+        if name:
+            environment._name = name
         environment.offset = global_offset
         environment.yaw = self._arg_with_dim(yaw, "deg")
         environment.pitch = self._arg_with_dim(pitch, "deg")
         environment.roll = self._arg_with_dim(roll, "deg")
         environment.insert(self._app)
         self.multiparts.append(environment)
         return environment
 
-    @pyaedt_function_handler()
-    def create_choke(self, json_file):
+    @pyaedt_function_handler(json_file="input_file")
+    def create_choke(self, input_file):
         """Create a choke from a JSON setting file.
 
         Parameters
         ----------
-        json_file : str
+        input_file : str
             Full path of the JSON file with the choke settings.
 
         Returns
         -------
         List of
             bool
                 ``True`` when successful, ``False`` when failed.
@@ -2364,15 +2352,15 @@
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> dictionary_values = hfss.modeler.check_choke_values("C:/Example/Of/Path/myJsonFile.json")
         >>> mychoke = hfss.modeler.create_choke("C:/Example/Of/Path/myJsonFile_Corrected.json")
         """
 
-        with open_file(json_file, "r") as read_file:
+        with open_file(input_file, "r") as read_file:
             values = json.load(read_file)
         self.logger.info("CHOKE INFO: " + str(values))
 
         sr = 1.1  # security factor
         segment_number = 0
         if values["Wire Section"]["Hexagon"]:
             segment_number = 6
@@ -2507,50 +2495,45 @@
         for key in values["Number of Windings"].keys():
             if values["Number of Windings"][key]:
                 number_duplication = int(key)
         if number_duplication >= 2:
             if values["Mode"]["Common"] and number_duplication == 2:
                 if isinstance(list_object[0], list):
                     for i in range(len(list_object)):
-                        duplication = self.create_polyline(
-                            position_list=list_object[i][1], name=name_wind, matname=material_wind
-                        )
+                        duplication = self.create_polyline(points=list_object[i][1], name=name_wind,
+                                                           material=material_wind)
                         duplication.mirror([0, 0, 0], [-1, 0, 0])
                         duplication_points = self.get_vertices_of_line(duplication.name)
                         success = duplication.set_crosssection_properties(
                             type=section, width=w_dia, num_seg=segment_number
                         )
                         list_duplicated_object.append([duplication, duplication_points])
 
                 else:
-                    duplication = self.create_polyline(
-                        position_list=list_object[1], name=name_wind, matname=material_wind
-                    )
+                    duplication = self.create_polyline(points=list_object[1], name=name_wind, material=material_wind)
                     duplication.mirror([0, 0, 0], [-1, 0, 0])
                     duplication_points = self.get_vertices_of_line(duplication.name)
                     success = duplication.set_crosssection_properties(type=section, width=w_dia, num_seg=segment_number)
                     list_duplicated_object.append([duplication, duplication_points])
             else:
                 if isinstance(list_object[0], list):
                     for j in range(number_duplication - 1):
                         for i in range(len(list_object)):
-                            duplication = self.create_polyline(
-                                position_list=list_object[i][1], name=name_wind, matname=material_wind
-                            )
+                            duplication = self.create_polyline(points=list_object[i][1], name=name_wind,
+                                                               material=material_wind)
                             duplication.rotate("Z", (j + 1) * 360 / number_duplication)
                             duplication_points = self.get_vertices_of_line(duplication.name)
                             success = duplication.set_crosssection_properties(
                                 type=section, width=w_dia, num_seg=segment_number
                             )
                             list_duplicated_object.append([duplication, duplication_points])
                 else:
                     for j in range(number_duplication - 1):
-                        duplication = self.create_polyline(
-                            position_list=list_object[1], name=name_wind, matname=material_wind
-                        )
+                        duplication = self.create_polyline(points=list_object[1], name=name_wind,
+                                                           material=material_wind)
                         duplication.rotate("Z", (j + 1) * 360 / number_duplication)
                         duplication_points = self.get_vertices_of_line(duplication.name)
                         success = duplication.set_crosssection_properties(
                             type=section, width=w_dia, num_seg=segment_number
                         )
                         list_duplicated_object.append([duplication, duplication_points])
             returned_list = returned_list + list_duplicated_object
@@ -2587,20 +2570,19 @@
                     [
                         point[0] * math.cos(i * angle) + point[1] * math.sin(i * angle),
                         -point[0] * math.sin(i * angle) + point[1] * math.cos(i * angle),
                         point[2],
                     ]
                 )
 
-        polyline = self.create_polyline(position_list=points, name=name, matname=material)
+        polyline = self.create_polyline(points=points, name=name, material=material)
         union_polyline1 = [polyline.name]
         if turns > 1:
-            union_polyline2 = polyline.duplicate_around_axis(
-                cs_axis="Z", angle=2 * teta, nclones=turns, create_new_objects=True
-            )
+            union_polyline2 = polyline.duplicate_around_axis(axis="Z", angle=2 * teta, clones=turns,
+                                                             create_new_objects=True)
         else:
             union_polyline2 = []
         union_polyline = union_polyline1 + union_polyline2
         list_positions2 = []
         for i, p in enumerate(union_polyline):
             if i == 0:
                 list_positions2.extend(self.get_vertices_of_line(p))
@@ -2610,15 +2592,15 @@
         # del list_positions[0]
 
         if sep_layer:
             for i in range(4):
                 positions.pop()
             positions.insert(0, [positions[0][0], positions[0][1], -height])
             positions.append([positions[-1][0], positions[-1][1], -height])
-            true_polyline = self.create_polyline(position_list=positions, name=name, matname=material)
+            true_polyline = self.create_polyline(points=positions, name=name, material=material)
             true_polyline.rotate("Z", 180 - (turns - 1) * teta)
             positions = self.get_vertices_of_line(true_polyline.name)
             return [true_polyline, positions]
 
         return positions
 
     @pyaedt_function_handler()
@@ -2661,27 +2643,27 @@
             points_out_wind.pop()
         points_out_wind.pop()
         points_out_wind[-1] = [points_out_wind[-2][0], points_out_wind[-2][1], -height]
         points_in_wind.insert(0, [points_in_wind[0][0], points_in_wind[0][1], -height])
         points_in_wind[-1] = [points_in_wind[-2][0], points_in_wind[-2][1], points_out_wind[1][2]]
         points_in_wind.append([points_in_wind[-3][0], points_in_wind[-3][1], points_out_wind[0][2]])
 
-        outer_polyline = self.create_polyline(position_list=points_out_wind, name=name, matname=material)
+        outer_polyline = self.create_polyline(points=points_out_wind, name=name, material=material)
         outer_polyline.rotate("Z", 180 - (turns - 1) * teta)
-        inner_polyline = self.create_polyline(position_list=points_in_wind, name=name, matname=material)
+        inner_polyline = self.create_polyline(points=points_in_wind, name=name, material=material)
         inner_polyline.rotate("Z", 180 - (turns_in_wind - 1) * teta_in_wind)
         outer_polyline.mirror([0, 0, 0], [0, -1, 0])
         outer_polyline.rotate("Z", turns_in_wind * teta_in_wind - turns * teta)
 
         list_polyline = [inner_polyline.name, outer_polyline.name]
         list_positions = []
         for i in range(len(list_polyline)):
             list_positions = list_positions + self.get_vertices_of_line(list_polyline[i])
         self.delete(list_polyline)
-        true_polyline = self.create_polyline(position_list=list_positions, name=name, matname=material)
+        true_polyline = self.create_polyline(points=list_positions, name=name, material=material)
         return [true_polyline, list_positions]
 
     @pyaedt_function_handler()
     def _make_triple_linked_winding(
             self,
             name,
             material,
@@ -2731,32 +2713,32 @@
         points_mid_wind.pop()
         points_mid_wind[-1] = [points_mid_wind[-2][0], points_mid_wind[-2][1], points_out_wind[1][2]]
         points_mid_wind.append([points_mid_wind[-4][0], points_mid_wind[-4][1], points_out_wind[0][2]])
         points_in_wind.insert(0, [points_in_wind[0][0], points_in_wind[0][1], -height])
         points_in_wind[-1] = [points_in_wind[-2][0], points_in_wind[-2][1], points_mid_wind[1][2]]
         points_in_wind.append([points_in_wind[-3][0], points_in_wind[-3][1], points_mid_wind[0][2]])
 
-        outer_polyline = self.create_polyline(position_list=points_out_wind, name=name, matname=material)
+        outer_polyline = self.create_polyline(points=points_out_wind, name=name, material=material)
         outer_polyline.rotate("Z", 180 - (turns - 1) * teta)
-        mid_polyline = self.create_polyline(position_list=points_mid_wind, name=name, matname=material)
+        mid_polyline = self.create_polyline(points=points_mid_wind, name=name, material=material)
         mid_polyline.rotate("Z", 180 - (turns_mid_wind - 1) * teta_mid_wind)
-        inner_polyline = self.create_polyline(position_list=points_in_wind, name=name, matname=material)
+        inner_polyline = self.create_polyline(points=points_in_wind, name=name, material=material)
 
         inner_polyline.rotate("Z", 180 - (turns_in_wind - 1) * teta_in_wind)
         mid_polyline.mirror([0, 0, 0], [0, -1, 0])
         outer_polyline.rotate("Z", turns * teta - turns_mid_wind * teta_mid_wind)
         mid_polyline.rotate("Z", turns_in_wind * teta_in_wind - turns_mid_wind * teta_mid_wind)
         outer_polyline.rotate("Z", turns_in_wind * teta_in_wind - turns_mid_wind * teta_mid_wind)
 
         list_polyline = [inner_polyline.name, mid_polyline.name, outer_polyline.name]
         list_positions = []
         for i in range(len(list_polyline)):
             list_positions = list_positions + self.get_vertices_of_line(list_polyline[i])
         self.delete(list_polyline)
-        true_polyline = self.create_polyline(position_list=list_positions, name=name, matname=material)
+        true_polyline = self.create_polyline(points=list_positions, name=name, material=material)
         return [true_polyline, list_positions]
 
     @pyaedt_function_handler()
     def _make_double_winding(
             self,
             name,
             material,
@@ -2846,28 +2828,28 @@
                 sep_layer,
             ),
         ]
         return list_object
 
     @pyaedt_function_handler()
     def _make_core(self, name, material, in_rad, out_rad, height, chamfer):
-        tool = self.create_cylinder("Z", [0, 0, -height / 2], in_rad, height, 0, "Tool", matname=material)
-        core = self.create_cylinder("Z", [0, 0, -height / 2], out_rad, height, 0, name=name, matname=material)
+        tool = self.create_cylinder("Z", [0, 0, -height / 2], in_rad, height, 0, "Tool", material=material)
+        core = self.create_cylinder("Z", [0, 0, -height / 2], out_rad, height, 0, name=name, material=material)
         core.subtract(tool, False)
         for n in core.edges:
             n.chamfer(chamfer)
         return core
 
-    @pyaedt_function_handler()
-    def check_choke_values(self, json_file, create_another_file=True):
+    @pyaedt_function_handler(json_file="input_dir", )
+    def check_choke_values(self, input_dir, create_another_file=True):
         """Verify the values in the json file and create another one with corrected values next to the first one.
 
         Parameters
         ----------
-        json_file : str
+        input_dir : str
             Full path to json file;
             Specific json file containing all the parameters to design your on choke.
         create_another_file : bool
             Create another file next to the first one in adding _Corrected to the file name if it is True
             else truncate the existing file
 
         Returns
@@ -2929,15 +2911,15 @@
                 "Occupation(%)": 0,
             },
             "Mid Winding": {"Turns": 8, "Coil Pit(deg)": 0.1, "Occupation(%)": 0},
             "Inner Winding": {"Turns": 12, "Coil Pit(deg)": 0.1, "Occupation(%)": 0},
         }
         are_inequations_checkable = True
         sr = 1.1  # Security factor
-        with open_file(json_file, "r") as read_file:
+        with open_file(input_dir, "r") as read_file:
             values = json.load(read_file)
 
         for key, value in dictionary_model.items():
             if key not in values:
                 self.logger.error("Missing or incorrect key {}.".format(key))
                 return [False, values]
             if isinstance(value, dict):
@@ -3293,20 +3275,20 @@
                 values["Inner Winding"]["Coil Pit(deg)"] = teta
                 values["Mid Winding"]["Turns"] = turns
                 values["Inner Winding"]["Turns"] = turns
                 values["Mid Winding"]["Occupation(%)"] = occ
                 values["Inner Winding"]["Occupation(%)"] = occ
 
             if create_another_file:
-                root_path, extension_path = os.path.splitext(json_file)
+                root_path, extension_path = os.path.splitext(input_dir)
                 new_path = root_path + "_Corrected" + extension_path
                 with open_file(new_path, "w") as outfile:
                     json.dump(values, outfile)
             else:
-                with open_file(json_file, "w") as outfile:
+                with open_file(input_dir, "w") as outfile:
                     json.dump(values, outfile)
 
         return [are_inequations_checkable, values]
 
     @pyaedt_function_handler()
     def _make_winding_follow_chamfer(self, chamfer, sr, wire_diameter, layer_number):
         w_rad_inc = layer_number * sr * wire_diameter / 2
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/component_array.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/component_array.py`

 * *Files 1% similar despite different names*

```diff
@@ -39,15 +39,15 @@
         self.__app = app
         if name is None:
             name = _uname("Array_")
         self.__name = name
 
         # Leverage csv file if possible (aedt version > 2023.2)
         if self.__app.settings.aedt_version > "2023.2":  # pragma: no cover
-            self.export_array_info(array_path=None)
+            self.export_array_info(output_file=None)
             self.__array_info_path = os.path.join(self.__app.toolkit_directory, "array_info.csv")
         else:
             self.__app.save_project()
             self.__array_info_path = None
 
         # Data that cannot be obtained from CSV
         try:
@@ -92,15 +92,15 @@
     @property
     def cells(self):
         """List of :class:`pyaedt.modeler.cad.component_array.CellArray` objects."""
         if not self.update_cells:
             return self.__cells
 
         if self.__app.settings.aedt_version > "2023.2":  # pragma: no cover
-            self.export_array_info(array_path=None)
+            self.export_array_info(output_file=None)
         else:
             self.__app.save_project()
 
         self.__cells = [[None for _ in range(self.b_size)] for _ in range(self.a_size)]
         array_props = self.properties
         component_names = self.component_names
         for row_cell in range(0, self.a_size):
@@ -316,15 +316,15 @@
         Returns
         -------
         dict
            Ordered dictionary of the properties of the component array.
         """
         # From 2024R1, array information can be loaded from a CSV, and this method is not needed.
         if self.__app.settings.aedt_version > "2023.2":  # pragma: no cover
-            self.export_array_info(array_path=None)
+            self.export_array_info(output_file=None)
         else:
             self.__app.save_project()
         new_properties = self.properties
         # TODO : post_processing_cells property can not be retrieved, so if the length of the components and the
         #  property is different, the method will reset the property.
         if len(new_properties["component"]) != len(self.post_processing_cells):
             self.__post_processing_cells = {}
@@ -341,16 +341,16 @@
         >>> oModule.DeleteArray
 
         """
         self.__app.omodelsetup.DeleteArray()
         del self.__app.component_array[self.name]
         self.__app.component_array_names = list(self.__app.get_oo_name(self.__app.odesign, "Model"))
 
-    @pyaedt_function_handler()
-    def export_array_info(self, array_path=None):  # pragma: no cover
+    @pyaedt_function_handler(array_path="output_file")
+    def export_array_info(self, output_file=None):  # pragma: no cover
         """Export array information to a CSV file.
 
         Returns
         -------
         str
            Path of the CSV file.
 
@@ -360,26 +360,26 @@
         >>> oModule.ExportArray
 
         """
         if self.__app.settings.aedt_version < "2024.1":  # pragma: no cover
             self.logger.warning("This feature is not available in {}.".format(str(self.__app.settings.aedt_version)))
             return False
 
-        if not array_path:  # pragma: no cover
-            array_path = os.path.join(self.__app.toolkit_directory, "array_info.csv")
-        self.__app.omodelsetup.ExportArray(self.name, array_path)
-        return array_path
+        if not output_file:  # pragma: no cover
+            output_file = os.path.join(self.__app.toolkit_directory, "array_info.csv")
+        self.__app.omodelsetup.ExportArray(self.name, output_file)
+        return output_file
 
-    @pyaedt_function_handler()
-    def parse_array_info_from_csv(self, csv_file):  # pragma: no cover
+    @pyaedt_function_handler(csv_file="input_file")
+    def parse_array_info_from_csv(self, input_file):  # pragma: no cover
         """Parse component array information from the CSV file.
 
         Parameters
         ----------
-        csv_file : str
+        input_file : str
              Name of the CSV file.
 
         Returns
         -------
         dict
            Ordered dictionary of the properties of the component array.
 
@@ -389,15 +389,15 @@
         >>> aedtapp = Hfss(projectname="Array.aedt")
         >>> array_names = aedtapp.component_array_names[0]
         >>> array = aedtapp.component_array[array_names[0]]
         >>> array_csv = array.export_array_info()
         >>> array_info = array.array_info_parser(array_csv)
         """
 
-        info = read_csv(csv_file)
+        info = read_csv(input_file)
         if not info:
             self.logger.error("Data from CSV file is not loaded.")
             return False
 
         components = {}
         array_matrix = []
         array_matrix_rotation = []
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/components_3d.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/components_3d.py`

 * *Files 0% similar despite different names*

```diff
@@ -481,21 +481,21 @@
         """
         arg = ["NAME:Selections", "Selections:=", self._m_name]
         self._m_Editor.Delete(arg)
         del self._primitives.user_defined_components[self.name]
         self._primitives.cleanup_objects()
         self.__dict__ = {}
 
-    @pyaedt_function_handler()
-    def duplicate_and_mirror(self, position, vector):
+    @pyaedt_function_handler(position="origin")
+    def duplicate_and_mirror(self, origin, vector):
         """Duplicate and mirror a selection.
 
         Parameters
         ----------
-        position : float
+        origin : float
             List of the ``[x, y, z]`` coordinates or
             Application.Position object for the selection.
         vector : float
             List of the ``[x1, y1, z1]`` coordinates or
             Application.Position object for the vector.
 
         Returns
@@ -504,17 +504,15 @@
             List of objects created or an empty list.
 
         References
         ----------
 
         >>> oEditor.DuplicateMirror
         """
-        return self._primitives.duplicate_and_mirror(
-            self.name, position, vector, is_3d_comp=True, duplicate_assignment=True
-        )
+        return self._primitives.duplicate_and_mirror(self.name, origin=origin, vector=vector, is_3d_comp=True)
 
     @pyaedt_function_handler()
     def mirror(self, position, vector):
         """Mirror a selection.
 
         Parameters
         ----------
@@ -540,45 +538,45 @@
                 return self
         else:
             for part in self.parts:
                 self._primitives.mirror(part, position=position, vector=vector)
             return self
         return False
 
-    @pyaedt_function_handler()
-    def rotate(self, cs_axis, angle=90.0, unit="deg"):
+    @pyaedt_function_handler(cs_axis="axis", unit="units")
+    def rotate(self, axis, angle=90.0, units="deg"):
         """Rotate the selection.
 
         Parameters
         ----------
-        cs_axis
+        axis
             Coordinate system axis or the Application.AXIS object.
         angle : float, optional
             Angle of rotation. The units, defined by ``unit``, can be either
             degrees or radians. The default is ``90.0``.
-        unit : text, optional
+        units : text, optional
              Units for the angle. Options are ``"deg"`` or ``"rad"``.
              The default is ``"deg"``.
 
         Returns
         -------
         pyaedt.modeler.cad.components_3d.UserDefinedComponent, bool
             3D object when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Rotate
         """
         if self.is3dcomponent:
-            if self._primitives.rotate(self.name, cs_axis=cs_axis, angle=angle, unit=unit):
+            if self._primitives.rotate(self.name, axis=axis, angle=angle, units=units):
                 return self
         else:
             for part in self.parts:
-                self._primitives.rotate(part, cs_axis=cs_axis, angle=angle, unit=unit)
+                self._primitives.rotate(part, axis=axis, angle=angle, units=units)
             return self
         return False
 
     @pyaedt_function_handler()
     def move(self, vector):
         """Move component from a list.
 
@@ -594,34 +592,34 @@
             3D object when successful, ``False`` when failed.
 
         References
         ----------
         >>> oEditor.Move
         """
         if self.is3dcomponent:
-            if self._primitives.move(self.name, vector=vector):
+            if self._primitives.move(self.name, vector):
                 return self
         else:
             for part in self.parts:
-                self._primitives.move(part, vector=vector)
+                self._primitives.move(part, vector)
             return self
 
         return False
 
-    @pyaedt_function_handler()
-    def duplicate_around_axis(self, cs_axis, angle=90, nclones=2, create_new_objects=True):
+    @pyaedt_function_handler(cs_axis="axis", nclones="clones")
+    def duplicate_around_axis(self, axis, angle=90, clones=2, create_new_objects=True):
         """Duplicate the component around the axis.
 
         Parameters
         ----------
-        cs_axis : Application.AXIS object
+        axis : Application.AXIS object
             Coordinate system axis of the object.
         angle : float, optional
             Angle of rotation in degrees. The default is ``90``.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
         create_new_objects : bool, optional
             Whether to create copies as new objects. The default is ``True``.
 
         Returns
         -------
         list
@@ -631,31 +629,31 @@
         ----------
 
         >>> oEditor.DuplicateAroundAxis
 
         """
         if self.is3dcomponent:
             ret, added_objects = self._primitives.duplicate_around_axis(
-                self.name, cs_axis, angle, nclones, create_new_objects, True
+                self.name, axis, angle, clones, create_new_objects=create_new_objects, is_3d_comp=True
             )
             return added_objects
         self._logger.warning("User-defined models do not support this operation.")
         return False
 
-    @pyaedt_function_handler()
-    def duplicate_along_line(self, vector, nclones=2, attach_object=False, **kwargs):
+    @pyaedt_function_handler(nclones="clones", attach_object="attach")
+    def duplicate_along_line(self, vector, clones=2, attach=False, **kwargs):
         """Duplicate the object along a line.
 
         Parameters
         ----------
         vector : list
             List of ``[x1 ,y1, z1]`` coordinates for the vector or the Application.Position object.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
-        attach_object : bool, optional
+        attach : bool, optional
             Whether to attach the object. The default is ``False``.
 
         Returns
         -------
         list
             List of names of the newly added objects.
 
@@ -670,15 +668,17 @@
                 "``attachObject`` is deprecated. Use ``attach_object`` instead.",
                 DeprecationWarning,
             )
             attach_object = kwargs["attachObject"]
 
         if self.is3dcomponent:
             old_component_list = self._primitives.user_defined_component_names
-            _, added_objects = self._primitives.duplicate_along_line(self.name, vector, nclones, attach_object, True)
+            _, added_objects = self._primitives.duplicate_along_line(
+                self.name, vector, clones, attach=attach, is_3d_comp=True
+            )
             return list(set(added_objects) - set(old_component_list))
         self._logger.warning("User-defined models do not support this operation.")
         return False
 
     @pyaedt_function_handler()
     def update_native(self):
         """Update the Native Component in AEDT.
@@ -815,23 +815,23 @@
             Path of the 3d component file.
         """
 
         return self._primitives._app.get_oo_object(self._primitives._app.oeditor, self.definition_name).GetPropValue(
             "3D Component File Path"
         )
 
-    @pyaedt_function_handler()
-    def update_definition(self, password="", new_filepath=""):
+    @pyaedt_function_handler(new_filepath="output_file")
+    def update_definition(self, password="", output_file=""):
         """Update 3d component definition.
 
         Parameters
         ----------
         password : str, optional
             Password for encrypted models. The default value is ``""``.
-        new_filepath : str, optional
+        output_file : str, optional
             New path containing the 3d component file. The default value is ``""``, which means
             that the 3d component file has not changed.
 
         Returns
         -------
         bool
             True if successful.
@@ -843,15 +843,15 @@
                 "ForLocalEdit:=",
                 False,
                 "DefinitionNames:=",
                 self.definition_name,
                 "Passwords:=",
                 [password],
                 "NewFilePath:=",
-                new_filepath,
+                output_file,
             ]
         )
         self._primitives._app.modeler.refresh_all_ids()
         return True
 
     @pyaedt_function_handler()
     def edit_definition(self, password=""):
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/elements3d.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/elements3d.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,16 +741,16 @@
         try:
             result = [(float(edge.midpoint[1]), edge) for edge in self.edges]
             result = sorted(result, key=lambda tup: tup[0])
             return result[0][1]
         except Exception:
             return None
 
-    @pyaedt_function_handler()
-    def is_on_bounding(self, tol=1e-9):
+    @pyaedt_function_handler(tol="tolerance")
+    def is_on_bounding(self, tolerance=1e-9):
         """Check if the face is on bounding box or Not.
 
         Parameters
         ----------
         tolerance : float, optional
             Tolerance of check between face center and bounding box.
 
@@ -758,20 +758,20 @@
         -------
         bool
             `True` if the face is on bounding box. `False` otherwise.
         """
         b = [float(i) for i in list(self.oeditor.GetModelBoundingBox())]
         c = self.center
         if c and (
-            abs(c[0] - b[0]) < tol
-            or abs(c[1] - b[1]) < tol
-            or abs(c[2] - b[2]) < tol
-            or abs(c[0] - b[3]) < tol
-            or abs(c[1] - b[4]) < tol
-            or abs(c[2] - b[5]) < tol
+            abs(c[0] - b[0]) < tolerance
+            or abs(c[1] - b[1]) < tolerance
+            or abs(c[2] - b[2]) < tolerance
+            or abs(c[0] - b[3]) < tolerance
+            or abs(c[1] - b[4]) < tolerance
+            or abs(c[2] - b[5]) < tolerance
         ):
             return True
         return False
 
     @pyaedt_function_handler()
     def move_with_offset(self, offset=1.0):
         """Move the face along the normal.
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/object3d.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/object3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,15 +44,15 @@
 
     >>> from pyaedt import Hfss
     >>> aedtapp = Hfss()
     >>> prim = aedtapp.modeler
 
     Create a part, such as box, to return an :class:`pyaedt.modeler.Object3d.Object3d`.
 
-    >>> id = prim.create_box([0, 0, 0], [10, 10, 5], "Mybox", "Copper")
+    >>> id = prim.create_box([0, 0, 0],[10, 10, 5],"Mybox","Copper")
     >>> part = prim[id]
     """
 
     def __init__(self, primitives, name=None):
         """
         Parameters
         ----------
@@ -254,41 +254,41 @@
             return self._primitives._app.post.plot_model_obj(
                 objects=[self.name],
                 plot_as_separate_objects=True,
                 plot_air_objects=True,
                 show=show,
             )
 
-    @pyaedt_function_handler()
-    def export_image(self, file_path=None):
+    @pyaedt_function_handler(file_path="output_file")
+    def export_image(self, output_file=None):
         """Export the current object to a specified file path.
 
 
         .. note::
            Works from AEDT 2021.2 in CPython only. PyVista has to be installed.
 
         Parameters
         ----------
-        file_path : str, optional
+        output_file : str, optional
             File name with full path. If `None` the exported image will be a ``png`` file that
             will be saved in ``working_directory``.
             To access the ``working_directory`` the use ``app.working_directory`` property.
 
         Returns
         -------
         str
             File path.
         """
         if not is_ironpython and self._primitives._app._aedt_version >= "2021.2":
-            if not file_path:
-                file_path = os.path.join(self._primitives._app.working_directory, self.name + ".png")
+            if not output_file:
+                output_file = os.path.join(self._primitives._app.working_directory, self.name + ".png")
             model_obj = self._primitives._app.post.plot_model_obj(
                 objects=[self.name],
                 show=False,
-                export_path=file_path,
+                export_path=output_file,
                 plot_as_separate_objects=True,
                 clean_files=True,
             )
             if model_obj:
                 return model_obj.image_file
         return False
 
@@ -323,33 +323,33 @@
         for face in self.faces:
             body_names = self._primitives.get_bodynames_from_position(face.center)
             a = [i for i in body_names if i != self.name and i not in list_names]
             if a:
                 list_names.extend(a)
         return list_names
 
-    @pyaedt_function_handler()
-    def get_touching_faces(self, object_name):
+    @pyaedt_function_handler(object_name="assignment")
+    def get_touching_faces(self, assignment):
         """Get the objects that touch one of the face center of each face of the object.
 
         Parameters
         ----------
-        object_name : str, :class:`Object3d`
+        assignment : str, :class:`Object3d`
             Object to check.
         Returns
         -------
         list
             list of objects and faces touching."""
 
         _names = []
-        if isinstance(object_name, Object3d):
-            object_name = object_name.name
+        if isinstance(assignment, Object3d):
+            assignment = assignment.name
         for face in self.faces:
             body_names = self._primitives.get_bodynames_from_position(face.center)
-            if object_name in body_names:
+            if assignment in body_names:
                 _names.append(face)
         return _names
 
     @property
     def faces(self):
         """Information for each face in the given part.
 
@@ -1371,61 +1371,61 @@
     @model.setter
     def model(self, fModel):
         vArg1 = ["NAME:Model", "Value:=", fModel]
         fModel = _to_boolean(fModel)
         self._change_property(vArg1)
         self._model = fModel
 
-    @pyaedt_function_handler()
-    def unite(self, object_list):
+    @pyaedt_function_handler(object_list="assignment")
+    def unite(self, assignment):
         """Unite a list of objects with this object.
 
         Parameters
         ----------
-        object_list : list of str or list of pyaedt.modeler.cad.object3d.Object3d
+        assignment : list of str or list of pyaedt.modeler.cad.object3d.Object3d
             List of objects.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
            Object 3D object.
 
         References
         ----------
 
         >>> oEditor.Unite
 
         """
-        unite_list = [self.name] + self._primitives.convert_to_selections(object_list, return_list=True)
+        unite_list = [self.name] + self._primitives.convert_to_selections(assignment, return_list=True)
         self._primitives.unite(unite_list)
         return self
 
-    @pyaedt_function_handler()
-    def intersect(self, theList, keep_originals=False):
+    @pyaedt_function_handler(theList="assignment")
+    def intersect(self, assignment, keep_originals=False):
         """Intersect the active object with a given list.
 
         Parameters
         ----------
-        theList : list
+        assignment : list
             List of objects.
         keep_originals : bool, optional
             Whether to keep the original object. The default is ``False``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             Retrieve the resulting 3D Object when succeeded.
 
         References
         ----------
 
         >>> oEditor.Intersect
         """
-        theList = [self.name] + self._primitives.convert_to_selections(theList, return_list=True)
-        self._primitives.intersect(theList, keep_originals)
+        assignment = [self.name] + self._primitives.convert_to_selections(assignment, return_list=True)
+        self._primitives.intersect(assignment)
         return self
 
     @pyaedt_function_handler()
     def split(self, plane, sides="Both"):
         """Split the active object.
 
         Parameters
@@ -1458,14 +1458,17 @@
         ----------
         position : list of int or float
             Cartesian ``[x, y, z]`` coordinates or
             the ``Application.Position`` object of a point in the plane used for the mirror operation.
         vector : list of float
             Vector in Cartesian coordinates ``[x1, y1, z1]``  or
             the ``Application.Position`` object for the vector normal to the plane used for the mirror operation.
+        duplicate : bool, optional
+             Whether to duplicate the object after mirroring it .n. The default
+             is ``False``, in which case AEDT is not duplicating the object.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
             ``False`` when failed.
 
@@ -1474,79 +1477,78 @@
 
         >>> oEditor.Mirror
         """
         if self._primitives.mirror(self.id, position=position, vector=vector, duplicate=duplicate):
             return self
         return False
 
-    @pyaedt_function_handler()
-    def rotate(self, cs_axis, angle=90.0, unit="deg"):
+    @pyaedt_function_handler(cs_axis="axis", unit="units")
+    def rotate(self, axis, angle=90.0, units="deg"):
         """Rotate the selection.
 
         Parameters
         ----------
-        cs_axis : int
+        axis : int
             Coordinate system axis or the Application.AXIS object.
         angle : float, optional
             Angle of rotation. The units, defined by ``unit``, can be either
             degrees or radians. The default is ``90.0``.
-        unit : text, optional
+        units : text, optional
              Units for the angle. Options are ``"deg"`` or ``"rad"``.
              The default is ``"deg"``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object. ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Rotate
         """
-        if self._primitives.rotate(self.id, cs_axis=cs_axis, angle=angle, unit=unit):
+        if self._primitives.rotate(self.id, axis=axis, angle=angle, units=units):
             return self
         return False
 
     @pyaedt_function_handler()
     def move(self, vector):
         """Move objects from a list.
 
         Parameters
         ----------
-        objid : list, Position object
-            List of object IDs.
         vector : list
             Vector of the direction move. It can be a list of the ``[x, y, z]``
             coordinates or a Position object.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
             ``False`` when failed.
 
         References
         ----------
         >>> oEditor.Move
         """
-        if self._primitives.move(self.id, vector=vector):
+        if self._primitives.move(self.id, vector):
             return self
         return False
 
-    def duplicate_around_axis(self, cs_axis, angle=90, nclones=2, create_new_objects=True):
+    @pyaedt_function_handler(cs_axis="axis", nclones="clones")
+    def duplicate_around_axis(self, axis, angle=90, clones=2, create_new_objects=True):
         """Duplicate the object around the axis.
 
         Parameters
         ----------
-        cs_axis : Application.AXIS object
+        axis : Application.AXIS object
             Coordinate system axis of the object.
         angle : float
             Angle of rotation in degrees. The default is ``90``.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
         create_new_objects : bool, optional
             Whether to create copies as new objects. The default is ``True``.
 
         Returns
         -------
         list of :class:`pyaedt.modeler.cad.object3d.Object3d`
@@ -1554,42 +1556,44 @@
 
         References
         ----------
 
         >>> oEditor.DuplicateAroundAxis
 
         """
-        _, added_objects = self._primitives.duplicate_around_axis(self, cs_axis, angle, nclones, create_new_objects)
+        _, added_objects = self._primitives.duplicate_around_axis(
+            self, axis, angle, clones, create_new_objects=create_new_objects
+        )
         return added_objects
 
-    @pyaedt_function_handler()
-    def duplicate_along_line(self, vector, nclones=2, attachObject=False):
+    @pyaedt_function_handler(nclones="clones", attachObject="attach")
+    def duplicate_along_line(self, vector, clones=2, attach=False):
         """Duplicate the object along a line.
 
         Parameters
         ----------
         vector : list
             List of ``[x1 ,y1, z1]`` coordinates for the vector or the Application.Position object.
-        nclones : int, optional
+        clones : int, optional
             Number of clones. The default is ``2``.
-        attachObject : bool, optional
+        attach : bool, optional
             Whether to attach the object. The default is ``False``.
 
         Returns
         -------
         list of str
             List of names of the newly added objects.
 
         References
         ----------
 
         >>> oEditor.DuplicateAlongLine
 
         """
-        _, added_objects = self._primitives.duplicate_along_line(self, vector, nclones, attachObject)
+        _, added_objects = self._primitives.duplicate_along_line(self, vector, clones, attach=attach)
         return added_objects
 
     @pyaedt_function_handler()
     def sweep_along_vector(self, sweep_vector, draft_angle=0, draft_type="Round"):
         """Sweep the selection along a vector.
 
         Parameters
@@ -1648,21 +1652,21 @@
 
         """
         self._primitives.sweep_along_path(
             self, sweep_object, draft_angle, draft_type, is_check_face_intersection, twist_angle
         )
         return self
 
-    @pyaedt_function_handler()
-    def sweep_around_axis(self, cs_axis, sweep_angle=360, draft_angle=0):
+    @pyaedt_function_handler(cs_axis="axis")
+    def sweep_around_axis(self, axis, sweep_angle=360, draft_angle=0):
         """Sweep around an axis.
 
         Parameters
         ----------
-        cs_axis : :class:`pyaedt.generic.constants.AXIS`
+        axis : :class:`pyaedt.generic.constants.AXIS`
             Coordinate system of the axis.
         sweep_angle : float, optional
              Sweep angle in degrees. The default is ``360``.
         draft_angle : float, optional
             Angle of the draft. The default is ``0``.
 
         Returns
@@ -1672,15 +1676,15 @@
 
         References
         ----------
 
         >>> oEditor.SweepAroundAxis
 
         """
-        self._primitives.sweep_around_axis(self, cs_axis, sweep_angle, draft_angle)
+        self._primitives.sweep_around_axis(self, axis, sweep_angle, draft_angle)
         return self
 
     @pyaedt_function_handler()
     def section(self, plane, create_new=True, section_cross_object=False):
         """Section the object.
 
         Parameters
@@ -1703,14 +1707,36 @@
         >>> oEditor.Section
 
         """
         self._primitives.section(self, plane, create_new, section_cross_object)
         return self
 
     @pyaedt_function_handler()
+    def detach_faces(self, faces):
+        """Section the object.
+
+        Parameters
+        ----------
+        faces : List[FacePrimitive] or List[int] or int or FacePrimitive
+            Face or faces to detach from the object.
+
+        Returns
+        -------
+        List[:class:`pyaedt.modeler.cad.object3d.Object3d`]
+            List of object resulting from the operation.
+
+        References
+        ----------
+
+        >>> oEditor.DetachFaces
+
+        """
+        return self._primitives.detach_faces(self, faces)
+
+    @pyaedt_function_handler()
     def clone(self):
         """Clone the object and return the new 3D object.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object that was added.
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/cad/polylines.py` & `pyaedt-0.8.9/pyaedt/modeler/cad/polylines.py`

 * *Files 2% similar despite different names*

```diff
@@ -472,15 +472,15 @@
         References
         ----------
 
         >>> oEditor.GetVertexIDsFromObject
         >>> oEditor.GetVertexPosition
 
         """
-        id_list = self._primitives.get_object_vertices(partID=self.id)
+        id_list = self._primitives.get_object_vertices(assignment=self.id)
         position_list = [self._primitives.get_vertex_position(id) for id in id_list]
         return position_list
 
     @pyaedt_function_handler()
     def _pl_point(self, pt):
         pt_data = ["NAME:PLPoint"]
         pt_data.append("X:=")
@@ -719,37 +719,26 @@
         new_objects = self._primitives.find_new_objects()
         assert len(new_objects) == 1
         new_name = new_objects[0]
         new_polyline = Polyline(self._primitives, src_object=self, name=new_name)
         new_polyline._id = None
         return self._primitives._create_object(new_name)
 
-    @pyaedt_function_handler()
-    def remove_vertex(self, position, abstol=1e-9):
-        """Remove a vertex from an existing polyline by position.
-
-        .. deprecated:: 0.6.55
-           Use :func:``remove_point`` method instead.
-
-        """
-        warnings.warn("`remove_vertex` is deprecated. Use `remove_point` method instead.", DeprecationWarning)
-        return self.remove_point(position, abstol)
-
-    @pyaedt_function_handler()
-    def remove_point(self, position, abstol=1e-9):
+    @pyaedt_function_handler(abstol="tolerance")
+    def remove_point(self, position, tolerance=1e-9):
         """Remove a point from an existing polyline by position.
 
         You must enter the exact position of the vertex as a list
         of ``[x, y, z]`` coordinates in the object's coordinate system.
 
         Parameters
         ----------
         position : list
             List of ``[x, y, z]`` coordinates specifying the vertex to remove.
-        abstol : float, optional
+        tolerance : float, optional
             Absolute tolerance of the comparison of a specified position to the
             vertex positions. The default is ``1e-9``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
@@ -771,24 +760,24 @@
         >>> P = modeler.create_polyline([[0, 1, 2], [0, 2, 3], [2, 1, 4]])
         >>> P.remove_point(["0mm", "1mm", "2mm"])
 
         Use string expressions for the vertex position and include an absolute
         tolerance when searching for the vertex to be removed.
 
         >>> P = modeler.create_polyline([[0, 1, 2], [0, 2, 3], [2, 1, 4]])
-        >>> P.remove_point(["0mm", "1mm", "2mm"], abstol=1e-6)
+        >>> P.remove_point(["0mm", "1mm", "2mm"],tolerance=1e-6)
         """
         found_vertex = False
         seg_id = None
         at_start = None
         pos_xyz = self._primitives.value_in_object_units(position)
         for ind, point_pos in enumerate(self.points):
             # compare the specified point with the vertex data using an absolute tolerance
             # (default of math.isclose is 1e-9 which should be ok in almost all cases)
-            found_vertex = GeometryOperators.points_distance(point_pos, pos_xyz) <= abstol
+            found_vertex = GeometryOperators.points_distance(point_pos, pos_xyz) <= tolerance
             if found_vertex:
                 if ind == len(self.points) - 1:
                     at_start = False
                     seg_id = self._get_segment_id_from_point_n(ind, at_start, allow_inner_points=True)
                 else:
                     at_start = True
                     seg_id = self._get_segment_id_from_point_n(ind, at_start, allow_inner_points=True)
@@ -814,34 +803,34 @@
         else:
             i_start, i_end = self._get_point_slice_from_segment_id(seg_id, at_start)
             del self._positions[i_start:i_end]
             del self._segment_types[seg_id]
 
         return True
 
-    @pyaedt_function_handler()
-    def remove_edges(self, edge_id):
+    @pyaedt_function_handler(edge_id="assignment")
+    def remove_edges(self, assignment):
         """Remove a segment from an existing polyline by segment id.
 
         .. deprecated:: 0.6.55
            Use :func:``remove_segments`` method instead.
 
         """
         warnings.warn("`remove_edges` is deprecated. Use `remove_segments` method instead.", DeprecationWarning)
-        return self.remove_segments(segment_id=edge_id)
+        return self.remove_segments(assignment=assignment)
 
-    @pyaedt_function_handler()
-    def remove_segments(self, segment_id):
+    @pyaedt_function_handler(segment_id="assignment")
+    def remove_segments(self, assignment):
         """Remove a segment from an existing polyline by segment id.
 
         You must enter the segment id or the list of the segment ids you want to remove.
 
         Parameters
         ----------
-        segment_id : int or List of int
+        assignment : int or List of int
             One or more edge IDs within the total number of edges of the polyline.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -849,39 +838,39 @@
         ----------
 
         >>> oEditor.DeletePolylinePoint
 
         Examples
         --------
         >>> P = modeler.create_polyline([[0, 1, 2], [0, 2, 3], [2, 1, 4]])
-        >>> P.remove_segments(segment_id=0)
+        >>> P.remove_segments(assignment=0)
         """
-        if isinstance(segment_id, int):
-            segment_id = [segment_id]
-        elif isinstance(segment_id, list):
-            segment_id.sort()
+        if isinstance(assignment, int):
+            assignment = [assignment]
+        elif isinstance(assignment, list):
+            assignment.sort()
         else:
             raise TypeError("segment_id must be int or list of int.")
         try:
             self._primitives.oeditor.DeletePolylinePoint(
                 [
                     "NAME:Delete Point",
                     "Selections:=",
                     self.name + ":CreatePolyline:1",
                     "Segment Indices:=",
-                    segment_id,
+                    assignment,
                     "At Start:=",
                     True,
                 ]
             )
         except Exception:  # pragma: no cover
-            raise ValueError("Invalid segment ID {} is specified on polyline {}.".format(segment_id, self.name))
+            raise ValueError("Invalid segment ID {} is specified on polyline {}.".format(assignment, self.name))
         else:
-            segment_id.reverse()
-            for sid in segment_id:
+            assignment.reverse()
+            for sid in assignment:
                 if sid == len(self._segment_types) - 1:
                     # removing the last segment, AEDT removes ALWAYS the last polyline point
                     at_start = False
                 else:
                     at_start = True
                 i_start, i_end = self._get_point_slice_from_segment_id(sid, at_start)
                 del self._positions[i_start:i_end]
@@ -1051,21 +1040,21 @@
                 n_points += s.num_points - 1
             if n_points == pn and not at_start:
                 return i
             if n_points_imu < pn < n_points and allow_inner_points:
                 return i
         return False
 
-    @pyaedt_function_handler()
-    def insert_segment(self, position_list, segment=None):
+    @pyaedt_function_handler(position_list="points")
+    def insert_segment(self, points, segment=None):
         """Add a segment to an existing polyline.
 
         Parameters
         ----------
-        position_list : List
+        points : List
             List of positions of the points that define the segment to insert.
             Either the starting point or ending point of the segment list must
             match one of the vertices of the existing polyline.
         segment : str or :class:`pyaedt.modeler.Primitives.PolylineSegment`, optional
             Definition of the segment to insert. For the types ``"Line"`` and ``"Arc"``,
             use their string values ``"Line"`` and ``"Arc"``. For the types ``"AngularArc"``
             and ``"Spline"``, use the :class:`pyaedt.modeler.Primitives.PolylineSegment`
@@ -1079,15 +1068,15 @@
         References
         ----------
 
         >>> oEditor.InsertPolylineSegment
 
         """
         # Check for a valid number of points
-        num_points = len(position_list)
+        num_points = len(points)
 
         # define the segment type from the number of points given
         if not segment:
             if num_points < 2:
                 raise ValueError("num_points must contain at least 2 points to auto-define a segment.")
             if num_points == 2:
                 segment = PolylineSegment("Line")
@@ -1098,28 +1087,28 @@
         else:
             if isinstance(segment, str) and segment in ["Line", "Arc"]:
                 segment = PolylineSegment(segment)
                 num_points = segment.num_points
             elif isinstance(segment, PolylineSegment):
                 num_points = segment.num_points
                 if segment.type == "AngularArc":
-                    self._evaluate_arc_angle_extra_points(segment, start_point=position_list[0])
+                    self._evaluate_arc_angle_extra_points(segment, start_point=points[0])
             else:
                 raise TypeError('segment must be either "Line", "Arc" or PolylineSegment object.')
-            if segment.type != "AngularArc" and len(position_list) < num_points:
+            if segment.type != "AngularArc" and len(points) < num_points:
                 raise ValueError("position_list must contain enough points for the specified segment type.")
-            elif segment.type == "AngularArc" and len(position_list) < 1:
+            elif segment.type == "AngularArc" and len(points) < 1:
                 raise ValueError("position_list must contain the start point for AngularArc segment.")
 
         # Check whether start-point and end-point of the segment is in the existing polylines points
-        start_point = position_list[0]
+        start_point = points[0]
 
         # End point does not exist for an AngularArc
         if segment.type != "AngularArc":
-            end_point = position_list[-1]
+            end_point = points[-1]
         else:
             end_point = []
 
         at_start = None
         p_insert_position = None
         insert_points = None
         num_polyline_points = len(self.points)
@@ -1129,43 +1118,43 @@
                 GeometryOperators.points_distance(
                     self._primitives.value_in_object_units(point), self._primitives.value_in_object_units(end_point)
                 )
                 < 1e-8
             ):
                 at_start = True
                 p_insert_position = i
-                insert_points = position_list[: num_points - 1]  # All points but last one.
+                insert_points = points[: num_points - 1]  # All points but last one.
                 if i == num_polyline_points - 1:
                     if segment.type != "Line":
                         # Inserting a segment in this position is not allowed in AEDT.
                         # We can make it work only for "Line" segments.
                         return False
                     at_start = False
-                    position_list = [self.points[-2], start_point]
+                    points = [self.points[-2], start_point]
                 break
             elif (
                 GeometryOperators.points_distance(
                     self._primitives.value_in_object_units(point), self._primitives.value_in_object_units(start_point)
                 )
                 < 1e-8
             ):
                 # note that AngularArc can only be here
                 at_start = False
                 p_insert_position = i + 1
                 if segment.type != "AngularArc":
-                    insert_points = position_list[1:num_points]  # Insert all points but first one
+                    insert_points = points[1:num_points]  # Insert all points but first one
                 else:
                     insert_points = segment.extra_points[:]  # For AngularArc insert the extra points
                 if i == 0:
                     if segment.type != "Line":
                         # Inserting a segment in this position is not allowed in AEDT.
                         # PyAEDT can make it work only for "Line" segments.
                         return False
                     at_start = True
-                    position_list = [end_point, self.points[1]]
+                    points = [end_point, self.points[1]]
                 break
 
         assert p_insert_position is not None, "Point for the insert is not found."
         assert insert_points is not None, "Point for the insert is not found."
 
         if i is None:
             raise ValueError("The polyline contains no points. It is impossible to insert a segment.")
@@ -1189,15 +1178,15 @@
         varg1.append("SegmentType:=")
         varg1.append(type)
 
         # Points and segment data
         varg2 = ["NAME:PolylinePoints"]
 
         if segment.type == "Line" or segment.type == "Spline" or segment.type == "Arc":
-            for pt in position_list[0:num_points]:
+            for pt in points[0:num_points]:
                 varg2.append(self._pl_point(pt))
             varg1.append(varg2)
         elif segment.type == "AngularArc":
             seg_str = self._segment_array(segment, start_point=start_point)
             varg2.append(self._pl_point(start_point))
             varg2.append(self._pl_point(segment.extra_points[0]))
             varg2.append(self._pl_point(segment.extra_points[1]))
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/calculators.py` & `pyaedt-0.8.9/pyaedt/modeler/calculators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesCircuit.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesCircuit.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 import math
 import os
 import random
-import warnings
 
 from pyaedt.application.Variables import decompose_variable_value
 from pyaedt.generic.LoadAEDTFile import load_keyword_in_aedt_file
 from pyaedt.generic.constants import AEDT_UNITS
 from pyaedt.generic.general_methods import filter_string
 from pyaedt.generic.general_methods import generate_unique_name
 from pyaedt.generic.general_methods import open_file
@@ -344,21 +343,21 @@
         id = int(name.split(";")[1])
         self.add_id_to_component(id)
         # return id, self.components[id].composed_name
         for el in self.components:
             if name in self.components[el].composed_name:
                 return self.components[el]
 
-    @pyaedt_function_handler()
-    def create_model_from_touchstone(self, touchstone_full_path, model_name=None, show_bitmap=True):
+    @pyaedt_function_handler(touchstone_full_path="input_file")
+    def create_model_from_touchstone(self, input_file, model_name=None, show_bitmap=True):
         """Create a model from a Touchstone file.
 
         Parameters
         ----------
-        touchstone_full_path : str
+        input_file : str
             Full path to the Touchstone file.
         model_name : str, optional
             Name of the model. The default is ``None``.
         show_bitmap : bool, optional
             Show bitmap image of schematic component.
             The default value is ``True``.
 
@@ -399,23 +398,23 @@
                     portnames.append(line.split(" = ")[1].strip())
                     line = file.readline()
             else:  # pragma: no cover
                 portnames = ["Port" + str(n) for n in range(1, num_terminal + 1)]
             return portnames
 
         if not model_name:
-            model_name = os.path.splitext(os.path.basename(touchstone_full_path))[0]
+            model_name = os.path.splitext(os.path.basename(input_file))[0]
         if model_name in list(self.o_model_manager.GetNames()):
             model_name = generate_unique_name(model_name, n=2)
-        num_terminal = int(os.path.splitext(touchstone_full_path)[1].lower().strip(".sp"))
+        num_terminal = int(os.path.splitext(input_file)[1].lower().strip(".sp"))
         # with open_file(touchstone_full_path, "r") as f:
         # port_names = _parse_ports_name(f, num_terminal)
 
         port_names = []
-        with open_file(touchstone_full_path, "r") as f:
+        with open_file(input_file, "r") as f:
             for line in f:
                 line = line.strip()
                 if line.startswith(("!", "#", "")):
                     if "Port" in line and "=" in line and "Impedance" not in line:
                         port_names.append(line.split("=")[-1].strip().replace(" ", "_").strip("[]"))
                 else:
                     break
@@ -446,15 +445,15 @@
             "ImageFile:=",
             image_subcircuit_path,
             "SymbolPinConfiguration:=",
             0,
             ["NAME:PortInfoBlk"],
             ["NAME:PortOrderBlk"],
             "filename:=",
-            touchstone_full_path,
+            input_file,
             "numberofports:=",
             num_terminal,
             "sssfilename:=",
             "",
             "sssmodel:=",
             False,
             "PortNames:=",
@@ -685,30 +684,30 @@
         arg1 = ["NAME:ComponentProps", "Name:=", model_name, "Id:=", str(id)]
         arg2 = ["NAME:Attributes", "Page:=", 1, "X:=", xpos, "Y:=", ypos, "Angle:=", angle, "Flip:=", False]
         id = self.oeditor.CreateComponent(arg1, arg2)
         id = int(id.split(";")[1])
         self.add_id_to_component(id)
         return self.components[id]
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(inst_name="name")
     def create_component(
         self,
-        inst_name=None,
+        name=None,
         component_library="Resistors",
         component_name="RES_",
         location=None,
         angle=0,
         use_instance_id_netlist=False,
         global_netlist_list=None,
     ):
         """Create a component from a library.
 
         Parameters
         ----------
-        inst_name : str, optional
+        name : str, optional
             Name of the instance. The default is ``None.``
         component_library : str, optional
             Name of the component library. The default is ``"Resistors"``.
         component_name : str, optional
             Name of component in the library. The default is ``"RES"``.
         location : list of float, optional
             Position on the X axis and Y axis.
@@ -732,81 +731,81 @@
         >>> oEditor.CreateComponent
 
         Examples
         --------
 
         >>> from pyaedt import TwinBuilder
         >>> aedtapp = TwinBuilder()
-        >>> cmp = aedtapp.modeler.schematic.create_component(component_library="", component_name="ExcitationComponent")
-        >>> cmp.set_property("ShowPin", True)
+        >>> cmp = aedtapp.modeler.schematic.create_component(component_library="",component_name="ExcitationComponent")
+        >>> cmp.set_property("ShowPin",True)
         >>> aedtapp.release_desktop(True, True)
         """
         id = self.create_unique_id()
         if component_library:
-            name = self.design_libray + "\\" + component_library + ":" + component_name
+            inst_name = self.design_libray + "\\" + component_library + ":" + component_name
         else:
-            name = component_name
-        arg1 = ["NAME:ComponentProps", "Name:=", name, "Id:=", str(id)]
+            inst_name = component_name
+        arg1 = ["NAME:ComponentProps", "Name:=", inst_name, "Id:=", str(id)]
         xpos, ypos = self._get_location(location)
         angle = math.pi * angle / 180
         arg2 = ["NAME:Attributes", "Page:=", 1, "X:=", xpos, "Y:=", ypos, "Angle:=", angle, "Flip:=", False]
         id = self.oeditor.CreateComponent(arg1, arg2)
         id = int(id.split(";")[1])
         # self.refresh_all_ids()
         self.add_id_to_component(id)
-        if inst_name:
-            self.components[id].set_property("InstanceName", inst_name)
+        if name:
+            self.components[id].set_property("InstanceName", name)
         if use_instance_id_netlist:
             self.enable_use_instance_name(component_library, component_name)
         elif global_netlist_list:
             self.enable_global_netlist(component_name, global_netlist_list)
         return self.components[id]
 
-    @pyaedt_function_handler()
-    def disable_data_netlist(self, component_name):
+    @pyaedt_function_handler(component_name="assignment")
+    def disable_data_netlist(self, assignment):
         """Disable the Nexxim global net list.
 
         Parameters
         ----------
-        component_name : str
+        assignment : str
             Name of the component.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oComponentManager.GetData
         >>> oComponentManager.Edit
         """
-        name = component_name
+        name = assignment
 
         properties = self.o_component_manager.GetData(name)
         if len(properties) > 0:
             nexxim = list(properties[len(properties) - 1][1])
             for el in nexxim:
                 if el == "Data:=":
                     nexxim_data = list(nexxim[nexxim.index(el) + 1])
                     nexxim_data[1] = ""
                     nexxim[nexxim.index(el) + 1] = nexxim_data
         self.o_component_manager.Edit(
-            name, ["Name:" + component_name, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]]
+            name, ["Name:" + assignment, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]]
         )
         return True
 
-    @pyaedt_function_handler()
-    def enable_global_netlist(self, component_name, global_netlist_list=None):
+    @pyaedt_function_handler(component_name="assignment")
+    def enable_global_netlist(self, assignment, global_netlist_list=None):
         """Enable Nexxim global net list.
 
         Parameters
         ----------
-        component_name : str
+        assignment : str
             Name of the component.
         global_netlist_list : list
             A list of lines to include. The default is ``None``.
 
         Returns
         -------
         bool
@@ -817,62 +816,62 @@
 
         >>> oComponentManager.GetData
         >>> oComponentManager.Edit
         """
         if global_netlist_list is None:
             global_netlist_list = []
 
-        name = component_name
+        name = assignment
 
         properties = self.o_component_manager.GetData(name)
         if len(properties) > 0:
             nexxim = list(properties[len(properties) - 1][1])
             for el in nexxim:
                 if el == "GRef:=":
                     nexxim_data = list(nexxim[nexxim.index(el) + 1])
                     nexxim_data[1] = "\n".join(global_netlist_list).replace("\\", "/")
                     nexxim[nexxim.index(el) + 1] = nexxim_data
         self.o_component_manager.Edit(
             name,
-            ["Name:" + component_name, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]],
+            ["Name:" + assignment, ["NAME:CosimDefinitions", nexxim, "DefaultCosim:=", "DefaultNetlist"]],
         )
         return True
 
-    @pyaedt_function_handler()
-    def create_symbol(self, symbol_name, pin_lists):
+    @pyaedt_function_handler(symbol_name="name", pin_lists="pins")
+    def create_symbol(self, name, pins):
         """Create a symbol.
 
         Parameters
         ----------
-        symbol_name : str
+        name : str
             Name of the symbol.
-        pin_lists : list
+        pins : list
             List of the pins.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oSymbolManager.Add
         """
-        numpins = len(pin_lists)
+        numpins = len(pins)
         h = int(numpins / 2)
         x1 = 0
         y2 = 0
         x2 = 0.00508
         y1 = 0.00254 * (h + 3)
         xp = -0.00254
         yp = 0.00254 * (h + 2)
         angle = 0
         arg = [
-            "NAME:" + symbol_name,
+            "NAME:" + name,
             "ModTime:=",
             1591858230,
             "Library:=",
             "",
             "ModSinceLib:=",
             False,
             "LibLocation:=",
@@ -887,15 +886,15 @@
         ]
         self.o_symbol_manager.Add(arg)
 
         id = 2
         i = 1
         id += 2
         r = numpins - (h * 2)
-        for pin in pin_lists:
+        for pin in pins:
             arg.append(
                 [
                     "NAME:PinDef",
                     "Pin:=",
                     [pin, xp, yp, angle, "N", 0, 0.00254, False, 0, True, "", False, False, pin, True],
                 ]
             )
@@ -910,15 +909,15 @@
 
         arg.append(
             [
                 "NAME:Graphics",
                 ["NAME:1", "Rect:=", [0, 0, 0, 0, (x1 + x2) / 2, (y1 + y2) / 2, x2 - x1, y1 - y2, 0, 0, 8192]],
             ]
         )
-        self.o_symbol_manager.EditWithComps(symbol_name, arg, [])
+        self.o_symbol_manager.EditWithComps(name, arg, [])
         return True
 
     @pyaedt_function_handler()
     def enable_use_instance_name(self, component_library="Resistors", component_name="RES_"):
         """Enable the use of the instance name.
 
         Parameters
@@ -1021,116 +1020,94 @@
                 else:
                     o.schematic_id = int(name[1])
                     objID = o.schematic_id
                 self.components[objID] = o
 
         return len(self.components)
 
-    @pyaedt_function_handler()
-    def get_obj_id(self, objname):
+    @pyaedt_function_handler(objname="assignment")
+    def get_obj_id(self, assignment):
         """Retrieve the ID of an object.
 
         Parameters
         ----------
-        objname : str
+        assignment : str
             Name of the object.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         for el in self.components:
-            if self.components[el].name == objname:
+            if self.components[el].name == assignment:
                 return el
         return None
 
-    @pyaedt_function_handler()
-    def get_pins(self, partid):
+    @pyaedt_function_handler(partid="assignment")
+    def get_pins(self, assignment):
         """Retrieve one or more pins.
 
         Parameters
         ----------
-        partid : int or str
+        assignment : int or str
             One or more IDs or names for the pins to retrieve.
 
         Returns
         -------
         type
             Pin with properties.
 
         References
         ----------
 
         >>> oEditor.GetComponentPins
         """
-        if isinstance(partid, CircuitComponent):
-            pins = self.oeditor.GetComponentPins(partid.composed_name)
-        elif isinstance(partid, str):
-            pins = self.oeditor.GetComponentPins(partid)
+        if isinstance(assignment, CircuitComponent):
+            pins = self.oeditor.GetComponentPins(assignment.composed_name)
+        elif isinstance(assignment, str):
+            pins = self.oeditor.GetComponentPins(assignment)
             # pins = self.oeditor.GetComponentPins(partid)
         else:
-            pins = self.oeditor.GetComponentPins(self.components[partid].composed_name)
+            pins = self.oeditor.GetComponentPins(self.components[assignment].composed_name)
             # pins = self.oeditor.GetComponentPins(self.components[partid].composed_name)
         return list(pins)
 
-    @pyaedt_function_handler()
-    def get_pin_location(self, partid, pinname):
+    @pyaedt_function_handler(partid="assignment", pinname="pin")
+    def get_pin_location(self, assignment, pin):
         """Retrieve the location of a pin.
 
         Parameters
         ----------
-        partid : int
+        assignment : int
             ID of the part.
-        pinname :
+        pin :
             Name of the pin.
 
         Returns
         -------
         List
             List of axis values ``[x, y]``.
 
         References
         ----------
 
         >>> oEditor.GetComponentPinLocation
 
         """
-        if isinstance(partid, str):
-            x = self.oeditor.GetComponentPinLocation(partid, pinname, True)
-            y = self.oeditor.GetComponentPinLocation(partid, pinname, False)
+        if isinstance(assignment, str):
+            x = self.oeditor.GetComponentPinLocation(assignment, pin, True)
+            y = self.oeditor.GetComponentPinLocation(assignment, pin, False)
         else:
-            x = self.oeditor.GetComponentPinLocation(self.components[partid].composed_name, pinname, True)
-            y = self.oeditor.GetComponentPinLocation(self.components[partid].composed_name, pinname, False)
+            x = self.oeditor.GetComponentPinLocation(self.components[assignment].composed_name, pin, True)
+            y = self.oeditor.GetComponentPinLocation(self.components[assignment].composed_name, pin, False)
         return self._convert_point_to_units([x, y])
 
     @pyaedt_function_handler()
-    def arg_with_dim(self, Value, sUnits=None):
-        """Format an argument with dimensions.
-
-        .. deprecated:: 0.6.56
-           Use :func:`number_with_units` instead.
-
-        Parameters
-        ----------
-        Value : str
-            Value of the quantity.
-        sUnits :
-            The default is ``None``.
-
-        Returns
-        -------
-        type
-
-        """
-        warnings.warn("Use :func:`number_with_units` instead.", DeprecationWarning)
-        return self._app.number_with_units(Value, sUnits)
-
-    @pyaedt_function_handler()
     def number_with_units(self, value, units=None):
         """Convert a number to a string with units. If value is a string, it's returned as is.
 
         Parameters
         ----------
         value : float, int, str
             Input  number or string.
@@ -1141,83 +1118,83 @@
         -------
         str
            String concatenating the value and unit.
 
         """
         return self._app.number_with_units(value, units)
 
-    @pyaedt_function_handler()
-    def create_line(self, points_array, color=0, line_width=0):
+    @pyaedt_function_handler(points_array="points", line_width="width")
+    def create_line(self, points, color=0, width=0):
         """Draw a graphical line.
 
         Parameters
         ----------
-        points_array : list
+        points : list
             A nested list of point coordinates. For example,
             ``[[x1, y1], [x2, y2], ...]``.
         color : string or 3 item list, optional
             Color or the line. The default is ``"0"``.
-        line_width : float, optional
+        width : float, optional
             Width of the line. The default is ``0``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.Line`
             Line Object.
 
         >>> oEditor.CreateLine
         """
-        points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
+        points = [str(tuple(self._convert_point_to_meter(i))) for i in points]
         id = self.create_unique_id()
         return self.oeditor.CreateLine(
-            ["NAME:LineData", "Points:=", points, "LineWidth:=", line_width, "Color:=", color, "Id:=", id],
+            ["NAME:LineData", "Points:=", points, "LineWidth:=", width, "Color:=", color, "Id:=", id],
             ["NAME:Attributes", "Page:=", 1],
         )
 
-    @pyaedt_function_handler()
-    def create_wire(self, points_array, wire_name=""):
+    @pyaedt_function_handler(points_array="points", wire_name="name")
+    def create_wire(self, points, name=""):
         """Create a wire.
 
         Parameters
         ----------
-        points_array : list
+        points : list
             A nested list of point coordinates. For example,
             ``[[x1, y1], [x2, y2], ...]``.
-        wire_name : str, optional
+        name : str, optional
             Name of the wire. Default value is ``""``.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.Wire`
             Wire Object.
 
         References
         ----------
 
         >>> oEditor.CreateWire
         """
-        points = [str(tuple(self._convert_point_to_meter(i))) for i in points_array]
+        points = [str(tuple(self._convert_point_to_meter(i))) for i in points]
         wire_id = self.create_unique_id()
-        arg1 = ["NAME:WireData", "Name:=", wire_name, "Id:=", wire_id, "Points:=", points]
+        arg1 = ["NAME:WireData", "Name:=", name, "Id:=", wire_id, "Points:=", points]
         arg2 = ["NAME:Attributes", "Page:=", 1]
         try:
             wire_id = self.oeditor.CreateWire(arg1, arg2)
             w = Wire(self._modeler)
             for segment in self._app.oeditor.GetWireSegments(wire_id):
                 key = "SegmentID_{}".format(segment.split(" ")[3])
                 point1 = [float(x) for x in segment.split(" ")[1].split(",")]
                 point2 = [float(x) for x in segment.split(" ")[2].split(",")]
                 w.points_in_segment[key] = [point1, point2]
             if ":" in wire_id.split(";")[1]:
                 wire_id = int(wire_id.split(";")[1].split(":")[0])
             else:
                 wire_id = int(wire_id.split(";")[1])
-            if not wire_name:
-                wire_name = generate_unique_name("Wire")
-            w.name = wire_name
+            if not name:
+                name = generate_unique_name("Wire")
+            w.name = name
             w.id = int(wire_id)
             self.wires[w.id] = w
             return w
         except Exception:
             return False
 
 
@@ -1234,21 +1211,21 @@
     @property
     def props(self):
         """Retrieve the component properties."""
         if not self._props:
             self._props = load_keyword_in_aedt_file(self.file_name, self.name)
         return self._props
 
-    @pyaedt_function_handler()
-    def place(self, inst_name, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(inst_name="assignment")
+    def place(self, assignment, location=None, angle=0, use_instance_id_netlist=False):
         """Create a component from a library.
 
         Parameters
         ----------
-        inst_name : str, optional
+        assignment : str, optional
             Name of the instance. The default is ``None.``
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to enable the instance ID in the net list.
@@ -1263,15 +1240,15 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         return self._component_manager.create_component(
-            inst_name=inst_name,
+            name=assignment,
             component_library=self.component_library,
             component_name=self.name,
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesEmit.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesEmit.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesMaxwellCircuit.py`

 * *Files 6% similar despite different names*

```diff
@@ -51,21 +51,21 @@
 
     def __init__(self, modeler):
         CircuitComponents.__init__(self, modeler)
         self._app = modeler._app
         self._modeler = modeler
         self._currentId = 0
 
-    @pyaedt_function_handler()
-    def create_resistor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_resistor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a resistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the resistor. The default is ``None``.
         value : float, optional
             Value for the resistor. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
@@ -82,33 +82,33 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Passive Elements",
             component_name="Res",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("R", value)
-        id.set_property("Name", compname)
+        id.set_property("Name", name)
         return id
 
-    @pyaedt_function_handler()
-    def create_inductor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_inductor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create an inductor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the inductor. The default is ``None``.
         value : float, optional
             Value for the inductor. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -125,33 +125,33 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Passive Elements",
             component_name="Ind",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("L", value)
-        id.set_property("Name", compname)
+        id.set_property("Name", name)
         return id
 
-    @pyaedt_function_handler()
-    def create_capacitor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_capacitor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a capacitor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the capacitor. The default is ``None``.
         value : float, optional
             Value for the capacitor. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
@@ -167,33 +167,33 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         id = self.create_component(
-            compname,
+            name,
             component_library="Passive Elements",
             component_name="Cap",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("C", value)
-        id.set_property("Name", compname)
+        id.set_property("Name", name)
         return id
 
-    @pyaedt_function_handler()
-    def create_diode(self, compname=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_diode(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a diode.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the diode. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle of rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
@@ -208,32 +208,32 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Passive Elements",
             component_name="DIODE",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
-        id.set_property("Name", compname)
+        id.set_property("Name", name)
         return id
 
-    @pyaedt_function_handler()
-    def create_winding(self, compname=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_winding(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create an NPN transistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the NPN transistor. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
@@ -247,16 +247,16 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         id = self.create_component(
-            compname,
+            name,
             component_library="Dedicated Elements",
             component_name="Winding",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
-        id.set_property("Name", compname)
+        id.set_property("Name", name)
         return id
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesNexxim.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesNexxim.py`

 * *Files 3% similar despite different names*

```diff
@@ -192,61 +192,61 @@
                         i / AEDT_UNITS["Length"][self.schematic_units] for i in self._get_location(location)
                     ]
                 if angle is not None:
                     self.components[el].angle = angle
                 return self.components[el]
         return False
 
-    @pyaedt_function_handler()
-    def duplicate(self, component, location=None, angle=0, flip=False):  # pragma: no cover
+    @pyaedt_function_handler(component="assignment")
+    def duplicate(self, assignment, location=None, angle=0, flip=False):  # pragma: no cover
         """Add a new subcircuit to the design.
 
         .. note::
             This works only in graphical mode.
 
         Parameters
         ----------
-        component : class:`pyaedt.modeler.Object3d.CircuitComponent` Circuit Component Object
+        assignment : class:`pyaedt.modeler.Object3d.CircuitComponent` Circuit Component Object
             Component to duplicate.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         flip : bool, optional
             Whether the component should be flipped. The default value is ``False``.
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.CircuitComponent` Circuit Component Object
         when successful or ``False`` when failed.
         """
         comp_names = []
-        if isinstance(component, CircuitComponent):
-            comp_names.append(component.composed_name)
+        if isinstance(assignment, CircuitComponent):
+            comp_names.append(assignment.composed_name)
         else:
-            comp_names.append(component)
+            comp_names.append(assignment)
         self._modeler.oeditor.Copy(["NAME:Selections", "Selections:=", comp_names])
         location = self._get_location(location)
         self._modeler.oeditor.Paste(
             ["NAME:Attributes", "Page:=", 1, "X:=", location[0], "Y:=", location[1], "Angle:=", angle, "Flip:=", flip]
         )
         ids = [id for id in list(self.components.keys())]
         self.refresh_all_ids()
         new_ids = [id for id in list(self.components.keys()) if id not in ids]
         if new_ids:
             return self.components[new_ids[0]]
         return False
 
-    @pyaedt_function_handler()
-    def connect_components_in_series(self, components_to_connect, use_wire=True):
+    @pyaedt_function_handler(components_to_connect="assignment")
+    def connect_components_in_series(self, assignment, use_wire=True):
         """Connect schematic components in series.
 
         Parameters
         ----------
-        components_to_connect : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+        assignment : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
            List of Components to connect. It can be a list of objects or component names.
         use_wire : bool, optional
             Whether to use wires or a page port to connect the pins.
             The default is ``True``, in which case wires are used. Note
             that if wires are not well placed, shorts can result.
 
         Returns
@@ -255,100 +255,100 @@
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
         >>> from pyaedt import Circuit
         >>> circuit = Circuit()
         >>> circuit.modeler.schematic_units = "mil"
-        >>> myind = circuit.modeler.schematic.create_inductor(compname="L100", value=1e-9, location=[0,0])
-        >>> myres = circuit.modeler.schematic.create_resistor(compname="R100", value=50, location=[100, 2000])
+        >>> myind = circuit.modeler.schematic.create_inductor(value=1e-9,location=[0,0])
+        >>> myres = circuit.modeler.schematic.create_resistor(value=50,location=[100, 2000])
         >>> circuit.modeler.schematic.connect_components_in_series([myind, myres])
         """
         comps = []
-        for component in components_to_connect:
+        for component in assignment:
             if isinstance(component, (CircuitComponent, Excitations)):
                 comps.append(component)
             else:
                 for id, cmp in self.components.items():
                     if component in [cmp.id, cmp.name, cmp.composed_name]:
                         comps.append(cmp)
                         break
         i = 0
         assert len(comps) > 1, "At least two components have to be passed."
         while i < (len(comps) - 1):
             comps[i].pins[-1].connect_to_component(comps[i + 1].pins[0], use_wire=use_wire)
             i += 1
         return True
 
-    @pyaedt_function_handler()
-    def connect_components_in_parallel(self, components_to_connect):
+    @pyaedt_function_handler(components_to_connect="assignment")
+    def connect_components_in_parallel(self, assignment):
         """Connect schematic components in parallel.
 
         Parameters
         ----------
-        components_to_connect : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
+        assignment : list of :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
            List of Components to connect. It can be a list of objects or component names.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
         >>> from pyaedt import Circuit
         >>> circuit = Circuit()
-        >>> myind = circuit.modeler.schematic.create_inductor("L100", 1e-9)
-        >>> myres = circuit.modeler.schematic.create_resistor("R100", 50)
+        >>> myind = circuit.modeler.schematic.create_inductor("L100",1e-9)
+        >>> myres = circuit.modeler.schematic.create_resistor("R100",50)
         >>> circuit.modeler.schematic.connect_components_in_parallel([myind, myres.composed_name])
         """
         comps = []
-        for component in components_to_connect:
+        for component in assignment:
             if isinstance(component, CircuitComponent):
                 comps.append(component)
             else:
                 for id, cmp in self.components.items():
                     if component in [cmp.id, cmp.name, cmp.composed_name]:
                         comps.append(cmp)
                         break
         assert len(comps) > 1, "At least two components have to be passed."
         comps[0].pins[0].connect_to_component([i.pins[0] for i in comps[1:]])
         terminal_to_connect = [cmp for cmp in comps if len(cmp.pins) >= 2]
         if len(terminal_to_connect) > 1:
             terminal_to_connect[0].pins[1].connect_to_component([i.pins[1] for i in terminal_to_connect[1:]])
         return True
 
-    @pyaedt_function_handler()
-    def add_subcircuit_3dlayout(self, sourcename):
+    @pyaedt_function_handler(sourcename="name")
+    def add_subcircuit_3dlayout(self, name):
         """Add a subcircuit from a HFSS 3DLayout.
 
         Parameters
         ----------
-        sourcename : str
+        name : str
             Name of the source design.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         References
         ----------
 
         >>> oProject.CopyDesign
         >>> oEditor.PasteDesign
         """
-        self._app._oproject.CopyDesign(sourcename)
+        self._app._oproject.CopyDesign(name)
         self.oeditor.PasteDesign(
             0,
             ["NAME:Attributes", "Page:=", 1, "X:=", 0, "Y:=", 0, "Angle:=", 0, "Flip:=", False],
         )
         self.refresh_all_ids()
         for el in self.components:
-            if sourcename in self.components[el].composed_name:
+            if name in self.components[el].composed_name:
                 return self.components[el]
         return False
 
     @pyaedt_function_handler()
     def create_field_model(self, design_name, solution_name, pin_names, model_type="hfss"):
         """Create a field model.
 
@@ -596,21 +596,21 @@
         self._app._odesign.AddCompInstance(component_name)
         self.refresh_all_ids()
         for el in self.components:
             if component_name in self.components[el].composed_name:
                 return el, self.components[el].composed_name
         return False
 
-    @pyaedt_function_handler()
-    def create_resistor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_resistor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a resistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the resistor. The default is ``None``.
         value : float, optional
             Resistance in ohms. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -627,27 +627,27 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname, location=location, angle=angle, use_instance_id_netlist=use_instance_id_netlist
+            name, location=location, angle=angle, use_instance_id_netlist=use_instance_id_netlist
         )
 
         cmpid.set_property("R", value)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_inductor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_inductor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create an inductor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the inductor. The default is ``None``.
         value : float, optional
             Inductance value. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -664,33 +664,33 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Inductors",
             component_name="IND_",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         cmpid.set_property("L", value)
 
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_capacitor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_capacitor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a capacitor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the capacitor. The default is ``None``.
         value : float, optional
             Capacitor value. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -704,37 +704,36 @@
             Circuit Component Object.
 
         References
         ----------
 
         >>> oEditor.CreateComponent
         """
-
         if location == None:
             location = []
 
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Capacitors",
             component_name="CAP_",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         cmpid.set_property("C", value)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_voltage_dc(self, compname=None, value=1, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_voltage_dc(self, name=None, value=1, location=None, angle=0, use_instance_id_netlist=False):
         """Create a voltage DC source.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the voltage DC source. The default is ``None``.
         value : float, optional
             Voltage value. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -752,32 +751,32 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Independent Sources",
             component_name="V_DC",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         cmpid.set_property("DC", value)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_voltage_probe(self, probe_name=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(probe_name="name")
+    def create_voltage_probe(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a voltage probe.
 
         Parameters
         ----------
-        probe_name :
+        name :
             Name of the voltage probe. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list.
@@ -803,26 +802,24 @@
             component_library="Probes",
             component_name="VPROBE",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
-        cmpid.set_property("Name", probe_name)
+        cmpid.set_property("Name", name)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_current_pulse(
-        self, compname=None, value_lists=None, location=None, angle=0, use_instance_id_netlist=False
-    ):
+    @pyaedt_function_handler(compname="name")
+    def create_current_pulse(self, name=None, value_lists=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a current pulse.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the current pulse. The default is ``None``.
         value_lists : list, optional
             List of values for the current pulse. The default is ``[]``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -841,15 +838,15 @@
         >>> oEditor.CreateComponent
         """
         if value_lists is None:
             value_lists = []
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Independent Sources",
             component_name="I_PULSE",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
@@ -866,23 +863,21 @@
         if len(value_lists) > 5:
             cmpid.set_property("PW", value_lists[5])
         if len(value_lists) > 6:
             cmpid.set_property("PER", value_lists[6])
 
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_voltage_pulse(
-        self, compname=None, value_lists=None, location=None, angle=0, use_instance_id_netlist=False
-    ):
+    @pyaedt_function_handler(compname="name")
+    def create_voltage_pulse(self, name=None, value_lists=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a voltage pulse.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the voltage pulse. The default is ``None``.
         value_lists : list, optional
             List of values for the voltage pulse. The default is ``[]``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -901,15 +896,15 @@
         >>> oEditor.CreateComponent
         """
         if value_lists is None:
             value_lists = []
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Independent Sources",
             component_name="V_PULSE",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
@@ -926,23 +921,23 @@
         if len(value_lists) > 5:
             cmpid.set_property("PW", value_lists[5])
         if len(value_lists) > 6:
             cmpid.set_property("PER", value_lists[6])
 
         return cmpid
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(compname="name")
     def create_voltage_pwl(
-        self, compname=None, time_list=None, voltage_list=None, location=None, angle=0, use_instance_id_netlist=False
+        self, name=None, time_list=None, voltage_list=None, location=None, angle=0, use_instance_id_netlist=False
     ):
         """Create a pwl voltage source.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the voltage pulse. The default is ``None``.
         time_list : list, optional
             List of time points for the pwl voltage source. The default is ``[0]``.
         voltage_list : list, optional
             List of voltages for the pwl voltage source. The default is ``[0]``.
         location : list of float, optional
             Position on the x-axis and y-xis.
@@ -961,41 +956,41 @@
         ----------
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
 
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Independent Sources",
             component_name="V_PWL",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         if (time_list is not None) and (voltage_list is not None):
 
             if len(time_list) != len(voltage_list):
                 self.logger.error("The number of time points is different than the number of voltages.")
                 return False
             else:
                 for nr, pair in enumerate(zip(time_list, voltage_list)):
-                    cmpid.set_property(property_name="time" + str(nr + 1), property_value=pair[0])
-                    cmpid.set_property(property_name="val" + str(nr + 1), property_value=pair[1])
+                    cmpid.set_property(name="time" + str(nr + 1), value=pair[0])
+                    cmpid.set_property(name="val" + str(nr + 1), value=pair[1])
 
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_current_dc(self, compname=None, value=1, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_current_dc(self, name=None, value=1, location=None, angle=0, use_instance_id_netlist=False):
         """Create a current DC source.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the current DC source. The default is ``None``.
         value : float, optional
             Current value. The default is ``1``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -1012,15 +1007,15 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Independent Sources",
             component_name="I_DC",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
@@ -1073,21 +1068,21 @@
         )
 
         cmpid.set_property("Inductor1", l1)
         cmpid.set_property("Inductor2", l2)
         cmpid.set_property("CouplingFactor", value)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_diode(self, compname=None, model_name="required", location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_diode(self, name=None, model_name="required", location=None, angle=0, use_instance_id_netlist=False):
         """Create a diode.
 
         Parameters
         ----------
-        compname : str
+        name : str
             Name of the diode. The default is ``None``.
         model_name : str, optional
             Name of the model. The default is ``"required"``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -1104,32 +1099,32 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         cmpid = self.create_component(
-            compname,
+            name,
             component_library="Diodes",
             component_name="DIODE_Level1",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         cmpid.set_property("MOD", model_name)
         return cmpid
 
-    @pyaedt_function_handler()
-    def create_npn(self, compname=None, value=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_npn(self, name=None, value=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create an NPN transistor.
 
         Parameters
         ----------
-        compname : str
+        name : str
             Name of the NPN transistor. The default is ``None``.
         value : float, optional
             Value for the NPN transistor. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -1146,32 +1141,32 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         id = self.create_component(
-            compname,
+            name,
             component_library="BJTs",
             component_name="Level01_NPN",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
         if value:
             id.set_property("MOD", value)
         return id
 
-    @pyaedt_function_handler()
-    def create_pnp(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_pnp(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a PNP transistor.
 
         Parameters
         ----------
-        compname : str
+        name : str
             Name of the PNP transistor. The default is ``None``.
         value : float, optional
             Value for the PNP transistor. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -1188,55 +1183,57 @@
         ----------
 
         >>> oEditor.CreateComponent
         """
         if location is None:
             location = []
         id = self.create_component(
-            compname,
+            name,
             component_library="BJTs",
             component_name="Level01_PNP",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
         if value:
             id.set_property("MOD", value)
 
         return id
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        symbol_name="name", pin_lists="pins", parameter_list="parameters", parameter_value="values"
+    )
     def create_new_component_from_symbol(
         self,
-        symbol_name,
-        pin_lists,
+        name,
+        pins,
         time_stamp=1591858313,
         description="",
         refbase="x",
-        parameter_list=[],
-        parameter_value=[],
+        parameters=[],
+        values=[],
         gref="",
     ):
         """Create a component from a symbol.
 
         Parameters
         ----------
-        symbol_name : str
+        name : str
             Name of the symbol.
-        pin_lists : list
+        pins : list
             List of pin names.
         time_stamp : int, optional
             UTC time stamp.
         description : str, optional
             Component description.
         refbase : str, optional
             Reference base. The default is ``"U"``.
-        parameter_list : list
+        parameters : list
             List of parameters. The default is ``[]``.
-        parameter_value : list
+        values : list
             List of parameter values. The default is ``[]``.
         gref : str, optional
             Global Reference
 
         Returns
         -------
         bool
@@ -1245,29 +1242,29 @@
         References
         ----------
 
         >>> oModelManager.Add
         >>> oComponentManager.Add
         """
         arg = [
-            "NAME:" + symbol_name,
+            "NAME:" + name,
             "Info:=",
             [
                 "Type:=",
                 0,
                 "NumTerminals:=",
-                len(pin_lists),
+                len(pins),
                 "DataSource:=",
                 "",
                 "ModifiedOn:=",
                 time_stamp,
                 "Manufacturer:=",
                 "",
                 "Symbol:=",
-                symbol_name,
+                name,
                 "ModelNames:=",
                 "",
                 "Footprint:=",
                 "",
                 "Description:=",
                 description,
                 "InfoTopic:=",
@@ -1303,22 +1300,22 @@
             refbase,
             "NumParts:=",
             1,
             "ModSinceLib:=",
             True,
         ]
 
-        for pin in pin_lists:
+        for pin in pins:
             arg.append("Terminal:=")
             arg.append([pin, pin, "A", False, 0, 1, "", "Electrical", "0"])
         arg.append("CompExtID:=")
         arg.append(1)
         arg2 = ["NAME:Parameters"]
 
-        for el, val in zip(parameter_list, parameter_value):
+        for el, val in zip(parameters, values):
             if "MOD" in el:
                 arg2.append("TextValueProp:=")
                 arg2.append([el, "D", "", val])
             else:
                 arg2.append("ValuePropNU:=")
                 arg2.append([el, "D", "", str(val), 0, ""])
 
@@ -1326,19 +1323,19 @@
         arg2.append(["CosimDefinition", "D", "", "Edit", "Edit", 40501, "ButtonPropClientData:=", []])
         arg2.append("MenuProp:=")
         arg2.append(["CoSimulator", "D", "", "DefaultNetlist", 0])
 
         arg.append(arg2)
         spicesintax = refbase + "@ID "
         id = 0
-        while id < len(pin_lists):
+        while id < len(pins):
             spicesintax += "%" + str(id) + " "
             id += 1
-            spicesintax += symbol_name + " "
-        for el, val in zip(parameter_list, parameter_value):
+            spicesintax += name + " "
+        for el, val in zip(parameters, values):
             if "MOD" in el:
                 spicesintax += "@{} ".format(el)
             else:
                 spicesintax += "{}=@{} ".format(el, el)
 
         arg3 = [
             "NAME:CosimDefinitions",
@@ -1361,23 +1358,24 @@
             "DefaultNetlist",
         ]
         arg.append(arg3)
         print(arg)
         self.o_component_manager.Add(arg)
         return True
 
-    @pyaedt_function_handler()
-    def get_comp_custom_settings(
-        self, toolNum, dc=0, interp=0, extrap=1, conv=0, passivity=0, reciprocal="False", opt="", data_type=1
+    @pyaedt_function_handler(toolNum="tool_index")
+    def _get_comp_custom_settings(
+        self, tool_index, dc=0, interp=0, extrap=1, conv=0, passivity=0, reciprocal="False", opt="", data_type=1
     ):
         """Retrieve custom settings for a resistor.
 
         Parameters
         ----------
-        toolNum :
+        tool_index : int
+            Tool index.
 
         dc :
             The default is ``0``.
         interp :
             The default is ``0``.
         extrap :
             The default is ``1``.
@@ -1394,17 +1392,17 @@
 
         Returns
         -------
         list
             List of the custom settings for the resistor.
 
         """
-        if toolNum == 1:
+        if tool_index == 1:
             custom = "NAME:DesignerCustomization"
-        elif toolNum == 2:
+        elif tool_index == 2:
             custom = "NAME:NexximCustomization"
         else:
             custom = "NAME:HSpiceCustomization"
 
         res = [
             custom,
             "DCOption:=",
@@ -1423,24 +1421,24 @@
             opt,
             "DataType:=",
             data_type,
         ]
 
         return res
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(comp_name="name")
     def add_subcircuit_dynamic_link(
         self,
         pyaedt_app=None,
         solution_name=None,
         extrusion_length=None,
         enable_cable_modeling=True,
         default_matrix="Original",
         tline_port="",
-        comp_name=None,
+        name=None,
     ):
         """Add a subcircuit from `HFSS`, `Q3d` or `2D Extractor` in circuit design.
 
         Parameters
         ----------
         pyaedt_app : :class:`pyaedt.q3d.Q3d` or :class:`pyaedt.q3d.Q2d` or :class:`pyaedt.q3d.Hfss`.
             pyaedt application object to include. It could be an Hfss object, a Q3d object or a Q2d.
@@ -1450,15 +1448,15 @@
             Extrusion length for 2D Models (q2d or Hfss) in model units. Default is `None`.
         enable_cable_modeling : bool, optional
             Either if the Hfss Cable modeling has to be enabled for 2D subcircuits.
         default_matrix : str, optional
             Matrix to link to the subcircuit. Default to `"Original"`. It only applies to 2D Extractor and Q3D.
         tline_port : str, optional
             Port to be used for tramsission line. Only applies to Hfss.
-        comp_name : str, optional
+        name : str, optional
             Component name.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
@@ -1466,33 +1464,33 @@
         ----------
 
         >>> oModelManager.Add
         >>> oComponentManager.Add
         >>> oDesign.AddCompInstance
         >>> oDesign.AddDynamicLink
         """
-        if not comp_name:
-            comp_name = generate_unique_name(pyaedt_app.design_name)
+        if not name:
+            name = generate_unique_name(pyaedt_app.design_name)
         source_project_path = pyaedt_app.project_file
         source_design_name = pyaedt_app.design_name
         if not solution_name:
             solution_name = pyaedt_app.nominal_sweep
         self._app.odesign.AddDynamicLink(
             source_design_name,
             source_project_path,
-            comp_name,
+            name,
             solution_name,
             tline_port,
             default_matrix,
             enable_cable_modeling,
             "Pyaedt Dynamic Link",
         )
         self.refresh_all_ids()
         for el in self.components:
-            if comp_name in self.components[el].composed_name:
+            if name in self.components[el].composed_name:
                 if extrusion_length:
                     _, units = decompose_variable_value(self.components[el].parameters["Length"])
                     self.components[el].set_property("Length", self.number_with_units(extrusion_length, units))
                 if tline_port and extrusion_length:
                     _, units = decompose_variable_value(self.components[el].parameters["TLineLength"])
                     self.components[el].set_property("TLineLength", self.number_with_units(extrusion_length, units))
                 return self.components[el]
@@ -1567,17 +1565,17 @@
             model = "2dext"
             owner = "2DExtractor"
             icon_file = "2dextractor.bmp"
         elif model_type.lower() == "siwave":
             model = "siwave"
             owner = "Siwave"
             icon_file = ""
-        designer_customization = self.get_comp_custom_settings(1, 0, 0, 1, 0, 0, "False", "", 1)
-        nexxim_customization = self.get_comp_custom_settings(2, 3, 1, 3, 0, 0, "False", "", 2)
-        hspice_customization = self.get_comp_custom_settings(3, 1, 2, 3, 0, 0, "False", "", 3)
+        designer_customization = self._get_comp_custom_settings(1, 0, 0, 1, 0, 0, "False", "", 1)
+        nexxim_customization = self._get_comp_custom_settings(2, 3, 1, 3, 0, 0, "False", "", 2)
+        hspice_customization = self._get_comp_custom_settings(3, 1, 2, 3, 0, 0, "False", "", 3)
 
         if image_subcircuit_path:
             _, file_extension = os.path.splitext(image_subcircuit_path)
             if file_extension != ".gif" or file_extension != ".bmp" or file_extension != ".jpg":
                 image_subcircuit_path = None
                 warnings.warn("Image extension is not valid. Use default image instead.")
         if not image_subcircuit_path:
@@ -1874,164 +1872,157 @@
         arg1.append(arg2)
         arg1.append(arg3)
         arg.append(arg1)
 
         self._app._oproject.ChangeProperty(arg)
         return True
 
-    @pyaedt_function_handler()
-    def refresh_dynamic_link(self, component_name):
+    @pyaedt_function_handler(component_name="name")
+    def refresh_dynamic_link(self, name):
         """Refresh a dynamic link component.
 
         Parameters
         ----------
-        component_name : str
+        name : str
             Name of the dynamic link component.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oComponentManager.UpdateDynamicLink
         """
-        if "@" in component_name:
-            component_name = component_name.split("@")[1]
-        component_name = component_name.split(";")[0]
-        self.o_component_manager.UpdateDynamicLink(component_name)
+        if "@" in name:
+            name = name.split("@")[1]
+        name = name.split(";")[0]
+        self.o_component_manager.UpdateDynamicLink(name)
         return True
 
     @pyaedt_function_handler()
     def _parse_spice_model(self, model_path):
         models = []
         with open_file(model_path, "r") as f:
             for line in f:
                 if ".subckt" in line.lower():
                     pinNames = [i.strip() for i in re.split(" |\t", line) if i]
                     models.append(pinNames[1])
         return models
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(model_path="input_file", model_name="model", symbol_name="symbol")
     def create_component_from_spicemodel(
         self,
-        model_path,
-        model_name=None,
+        input_file,
+        model=None,
         create_component=True,
         location=None,
         symbol_path="Nexxim Circuit Elements\\Nexxim_symbols:",
-        symbol_name="",
+        symbol="",
     ):
         """Create and place a new component based on a spice .lib file.
 
         Parameters
         ----------
-        model_path : str
+        input_file : str
             Path to .lib file.
-        model_name : str, optional
+        model : str, optional
             Model name to import. If `None` the first subckt in the lib file will be placed.
         create_component : bool, optional
             If set to ``True``, create a spice model component. Otherwise, only import the spice model.
         location : list, optional
             Position in the schematic of the new component.
         symbol_path : str, optional
             Path to the symbol library.
             Default value is ``"Nexxim Circuit Elements\\Nexxim_symbols:"``.
-        symbol_name : str, optional
+        symbol : str, optional
             Symbol name to replace the spice model with.
             Default value is an empty string which means the default symbol for spice is used.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
 
         Examples
         --------
         >>> from pyaedt import Circuit
         >>> cir = Circuit(specified_version="2023.2")
         >>> model = os.path.join("Your path", "test.lib")
-        >>> cir.modeler.schematic.create_component_from_spicemodel(model_path=model,
-        >>>                                                        model_name="GRM1234",
-        >>>                                                        symbol_name="nexx_cap")
+        >>> cir.modeler.schematic.create_component_from_spicemodel(input_file=model,model="GRM1234",symbol="nexx_cap")
         >>> cir.release_desktop(False, False)
         """
-        models = self._parse_spice_model(model_path)
-        if not model_name and models:
-            model_name = models[0]
-        elif model_name not in models:
+        models = self._parse_spice_model(input_file)
+        if not model and models:
+            model = models[0]
+        elif model not in models:
             return False
         arg = ["NAME:Options", "Mode:=", 2, "Overwrite:=", False, "SupportsSimModels:=", False, "LoadOnly:=", False]
         arg2 = ["NAME:Models"]
         for el in models:
             arg2.append(el + ":=")
-            if el == model_name:
-                if symbol_path and symbol_name:
-                    arg2.append([True, symbol_path + symbol_name, "", False])
+            if el == model:
+                if symbol_path and symbol:
+                    arg2.append([True, symbol_path + symbol, "", False])
                 else:
                     arg2.append([True, "", "", False])
             else:
                 arg2.append([False, "", "", False])
         arg.append(arg2)
-        self.o_component_manager.ImportModelsFromFile(model_path.replace("\\", "/"), arg)
+        self.o_component_manager.ImportModelsFromFile(input_file.replace("\\", "/"), arg)
 
         if create_component:
-            return self.create_component(
-                None,
-                component_library=None,
-                component_name=model_name,
-                location=location,
-            )
+            return self.create_component(None, component_library=None, component_name=model, location=location)
         else:
             return True
 
-    @pyaedt_function_handler()
-    def add_siwave_dynamic_link(self, model_path, solution_name=None, simulate_solutions=False):
+    @pyaedt_function_handler(model_path="input_file", solution_name="solution")
+    def add_siwave_dynamic_link(self, input_file, solution=None, simulate_solutions=False):
         """Add a siwave dinamyc link object.
 
         Parameters
         ----------
-        model_path : str
+        input_file : str
             Full path to the .siw file.
-        solution_name : str, optional
+        solution : str, optional
             Solution name.
         simulate_solutions : bool, optional
             Either if simulate or interpolate existing solutions.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dcircuit.CircuitComponent`
             Circuit Component Object.
         """
-        assert os.path.exists(model_path), "Project file doesn't exist"
-        comp_name = os.path.splitext(os.path.basename(model_path))[0]
-        results_path = model_path + "averesults"
-        solution = os.path.join(results_path, comp_name + ".asol")
+        assert os.path.exists(input_file), "Project file doesn't exist"
+        comp_name = os.path.splitext(os.path.basename(input_file))[0]
+        results_path = input_file + "averesults"
+        solution_path = os.path.join(results_path, comp_name + ".asol")
         # out = load_entire_aedt_file(solution)
-        out = load_keyword_in_aedt_file(solution, "Solutions")
-        if not solution_name:
-            solution_name = list(out["Solutions"]["SYZSolutions"].keys())[0]
+        out = load_keyword_in_aedt_file(solution_path, "Solutions")
+        if not solution:
+            solution = list(out["Solutions"]["SYZSolutions"].keys())[0]
         results_folder = os.path.join(
             results_path,
-            out["Solutions"]["SYZSolutions"][solution_name]["DiskName"],
-            out["Solutions"]["SYZSolutions"][solution_name]["DiskName"] + ".syzinfo",
+            out["Solutions"]["SYZSolutions"][solution]["DiskName"],
+            out["Solutions"]["SYZSolutions"][solution]["DiskName"] + ".syzinfo",
         )
 
         pin_names = []
         with open_file(results_folder, "r") as f:
             lines = f.read().splitlines()
             for line in lines:
                 if line[:4] == "PORT":
                     line_spit = line.split(" ")
                     pin_names.append(line_spit[1].strip('"'))
 
         return self._add_subcircuit_link(
             comp_name,
             pin_names,
-            model_path,
+            input_file,
             comp_name,
-            solution_name=solution_name,
+            solution_name=solution,
             model_type="siwave",
             simulate_solutions=simulate_solutions,
         )
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/PrimitivesTwinBuilder.py`

 * *Files 3% similar despite different names*

```diff
@@ -75,21 +75,21 @@
         -------
         :class:`pyaedt.modeler.PrimitivesCircuit.ComponentCatalog`
         """
         if not self._components_catalog:
             self._components_catalog = ComponentCatalog(self)
         return self._components_catalog
 
-    @pyaedt_function_handler()
-    def create_resistor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_resistor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a resistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the resistor. The default value is ``None``.
         value : float, optional
             Value for the resistor. The default value is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default value is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default value is ``0``.
@@ -106,33 +106,33 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Passive Elements",
             component_name="R",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("R", value)
 
         return id
 
-    @pyaedt_function_handler()
-    def create_inductor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_inductor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create an inductor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the inductor. The default is ``None``.
         value : float, optional
             Value for the inductor. The default is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
@@ -149,32 +149,32 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Passive Elements",
             component_name="L",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("L", value)
         return id
 
-    @pyaedt_function_handler()
-    def create_capacitor(self, compname=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_capacitor(self, name=None, value=50, location=None, angle=0, use_instance_id_netlist=False):
         """Create a capacitor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the capacitor. The default value is ``None``.
         value : float, optional
             Value for the capacitor. The default value is ``50``.
         location : list of float, optional
             Position on the X axis and Y axis. The default value is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default value is ``0``.
@@ -191,35 +191,35 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Passive Elements",
             component_name="C",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         id.set_property("C", value)
         id.set_property("UseInitialConditions", True)
         return id
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(compname="name")
     def create_voltage_source(
-        self, compname=None, type="E", amplitude=326, freq=50, location=None, angle=0, use_instance_id_netlist=False
+        self, name=None, type="E", amplitude=326, freq=50, location=None, angle=0, use_instance_id_netlist=False
     ):
         """Create a voltage source (conservative electrical output).
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the voltage source. The default is ``None``.
         type  : str, optional
             Type of the source. The default is ``E``.
         amplitude : float, optional
             Amplitude of the waveform if periodic. The default is ``326V``
         freq : float, optional
             Frequency of the periodic waveform. The default is ``50Hz``.
@@ -240,15 +240,15 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Sources",
             component_name="E",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
@@ -260,21 +260,21 @@
             id.set_property("AMPL", amplitude)
             id.set_property("FREQ", freq)
             id.set_property("TPERIO", "Tend+1")
             id.set_property("PERIO", 1)
 
         return id
 
-    @pyaedt_function_handler()
-    def create_diode(self, compname=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_diode(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a diode.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the diode. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis. The default value is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
@@ -289,30 +289,30 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Semiconductors System Level",
             component_name="D",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
         return id
 
-    @pyaedt_function_handler()
-    def create_npn(self, compname=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_npn(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create an NPN transistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the NPN transistor. The default value is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis. The default value is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
@@ -327,30 +327,30 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Semiconductors System Level",
             component_name="BJT",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
         return id
 
-    @pyaedt_function_handler()
-    def create_pnp(self, compname=None, location=None, angle=0, use_instance_id_netlist=False):
+    @pyaedt_function_handler(compname="name")
+    def create_pnp(self, name=None, location=None, angle=0, use_instance_id_netlist=False):
         """Create a PNP transistor.
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the PNP transistor. The default is ``None``.
         location : list of float, optional
             Position on the X axis and Y axis. The default value is ``None``.
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         use_instance_id_netlist : bool, optional
             Whether to use the instance ID in the net list. The default is ``False``.
@@ -365,28 +365,28 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Circuit\\Semiconductors System Level",
             component_name="BJT",
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
 
         return id
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(compname="name")
     def create_periodic_waveform_source(
         self,
-        compname=None,
+        name=None,
         type="SINE",
         amplitude=100,
         freq=50,
         phase=0,
         offset=0,
         delay=0,
         location=None,
@@ -394,15 +394,15 @@
         use_instance_id_netlist=False,
     ):
         """
         Create a periodic waveform source (non conservative real output).
 
         Parameters
         ----------
-        compname : str, optional
+        name : str, optional
             Name of the voltage source. The default is ``None``.
         type  : str, optional
             Type of the source [SINE, PULSE, TRAING, SAWTOOTH]. The default is ``SINE``.
         amplitude : float, optional
             Amplitude of the waveform if periodic. The default is ``100V``
         freq : float, optional
             Frequency of the periodic waveform. The default is ``50Hz``.
@@ -429,15 +429,15 @@
 
         >>> oEditor.CreateComponent
         """
         if location == None:
             location = []
 
         id = self.create_component(
-            compname,
+            name,
             component_library="Basic Elements\\Tools\\Time Functions",
             component_name=type,
             location=location,
             angle=angle,
             use_instance_id_netlist=use_instance_id_netlist,
         )
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/circuits/object3dcircuit.py` & `pyaedt-0.8.9/pyaedt/modeler/circuits/object3dcircuit.py`

 * *Files 4% similar despite different names*

```diff
@@ -127,23 +127,23 @@
             deltax = point[0]
         if move_y:
             deltay = point[1] + delta
         else:
             deltay = point[1]
         return deltax, deltay
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(component_pin="assignment")
     def connect_to_component(
-        self, component_pin, page_name=None, use_wire=False, wire_name="", clearance_units=1, page_port_angle=None
+        self, assignment, page_name=None, use_wire=False, wire_name="", clearance_units=1, page_port_angle=None
     ):
         """Connect schematic components.
 
         Parameters
         ----------
-        component_pin : :class:`pyaedt.modeler.circuits.PrimitivesNexxim.CircuitPins`
+        assignment : :class:`pyaedt.modeler.circuits.PrimitivesNexxim.CircuitPins`
            Component pin to attach.
         page_name : str, optional
             Page port name. The default value is ``None``, in which case
             a name is automatically generated.
         use_wire : bool, optional
             Whether to use wires or a page port to connect the pins.
             The default is ``False``, in which case a page port is used. Note
@@ -163,22 +163,22 @@
 
         References
         ----------
 
         >>> oPadstackManager.CreatePagePort
         """
         tol = 1e-8
-        if not isinstance(component_pin, list):
-            component_pin = [component_pin]
+        if not isinstance(assignment, list):
+            assignment = [assignment]
         if use_wire:
             direction = (180 + self.angle + self._circuit_comp.angle) * math.pi / 180
             points = [self.location]
             cangles = [self._circuit_comp.angle]
             negative = 0.0 >= direction >= (math.pi)
-            for cpin in component_pin:
+            for cpin in assignment:
                 prev = [i for i in points[-1]]
                 act = [i for i in cpin.location]
                 pins_x = [i.location[0] for i in self._circuit_comp.pins if i.name != self.name]
                 pins_x += [i.location[0] for i in cpin._circuit_comp.pins if i.name != cpin.name]
                 pins_y = [i.location[1] for i in self._circuit_comp.pins if i.name != self.name]
                 pins_y += [i.location[1] for i in cpin._circuit_comp.pins if i.name != cpin.name]
                 pins = [[i, j, 0] for i, j in zip(pins_x, pins_y)]
@@ -244,15 +244,15 @@
                         self._add_point(pins, points, delta, [p1, act[1]])
                     else:
                         points.append([p1, act[1]])
                     if points[-1][0] != act[0] or points[-1][1] != act[1]:
                         points.append(act)
 
                 cangles.append(cpin._circuit_comp.angle)
-            self._circuit_comp._circuit_components.create_wire(points, wire_name=wire_name)
+            self._circuit_comp._circuit_components.create_wire(points, name=wire_name)
             return True
         comp_angle = self._circuit_comp.angle * math.pi / 180
         if len(self._circuit_comp.pins) == 2:
             comp_angle += math.pi / 2
         if page_name is None:
             page_name = "{}_{}".format(
                 self._circuit_comp.composed_name.replace("CompInst@", "").replace(";", "_"), self.name
@@ -260,15 +260,15 @@
 
         if "Port" in self._circuit_comp.composed_name:
             try:
                 page_name = self._circuit_comp.name.split("@")[1].replace(";", "_")
             except Exception:
                 pass
         else:
-            for cmp in component_pin:
+            for cmp in assignment:
                 if "Port" in cmp._circuit_comp.composed_name:
                     try:
                         page_name = cmp._circuit_comp.name.split("@")[1].replace(";", "_")
                         break
                     except Exception:
                         continue
         try:
@@ -280,15 +280,15 @@
         if page_port_angle is not None:
             angle = page_port_angle * math.pi / 180
         elif self.location[0] < x_loc:
             angle = comp_angle
         else:
             angle = math.pi + comp_angle
         ret1 = self._circuit_comp._circuit_components.create_page_port(page_name, self.location, angle=angle)
-        for cmp in component_pin:
+        for cmp in assignment:
             try:
                 x_loc = AEDT_UNITS["Length"][decompose_variable_value(cmp._circuit_comp.location[0])[1]] * float(
                     decompose_variable_value(cmp._circuit_comp.location[0])[0]
                 )
             except Exception:
                 x_loc = float(cmp._circuit_comp.location[0])
             comp_pin_angle = cmp._circuit_comp.angle * math.pi / 180
@@ -711,106 +711,104 @@
         Returns
         -------
 
         """
         vMaterial = ["NAME:Component Mirror", "Value:=", mirror_value]
         self.change_property(vMaterial)
 
-    @pyaedt_function_handler()
-    def set_use_symbol_color(self, symbol_color=None):
+    @pyaedt_function_handler(symbol_color="color")
+    def set_use_symbol_color(self, color=None):
         """Set symbol color usage.
 
         Parameters
         ----------
-        symbol_color : bool, optional
+        color : bool, optional
             The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        if not symbol_color:
-            symbol_color = self.usesymbolcolor
-        vMaterial = ["NAME:Use Symbol Color", "Value:=", symbol_color]
+        if not color:
+            color = self.usesymbolcolor
+        vMaterial = ["NAME:Use Symbol Color", "Value:=", color]
         self.change_property(vMaterial)
         return True
 
-    @pyaedt_function_handler()
-    def set_color(self, R=255, G=128, B=0):
+    @pyaedt_function_handler(R="red", G="green", B="blue")
+    def set_color(self, red=255, green=128, blue=0):
         """Set symbol color.
 
         Parameters
         ----------
-        R : int, optional
+        red : int, optional
             Red color value. The default is ``255``.
-        G : int, optional
+        green : int, optional
             Green color value. The default is ``128``.
-        B : int, optional
+        blue : int, optional
             Blue color value. The default is ``0``
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        vMaterial = ["NAME:Component Color", "R:=", R, "G:=", G, "B:=", B]
+        vMaterial = ["NAME:Component Color", "R:=", red, "G:=", green, "B:=", blue]
         self.change_property(vMaterial)
         return True
 
-    @pyaedt_function_handler()
-    def set_property(self, property_name, property_value):
+    @pyaedt_function_handler(property_name="name", property_value="value")
+    def set_property(self, name, value):
         """Set a part property.
 
         Parameters
         ----------
-        property_name : str
+        name : str
             Name of the property.
-        property_value :
+        value :
             Value for the property.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        if isinstance(property_name, list):
-            for p, v in zip(property_name, property_value):
+        if isinstance(name, list):
+            for p, v in zip(name, value):
                 v_prop = ["NAME:" + p, "Value:=", v]
                 self.change_property(v_prop)
                 if self.__dict__.get("_parameters", None) and p in self.__dict__["_parameters"]:
                     self.__dict__["_parameters"][p] = v
                 else:
                     self.__dict__[p] = v
         else:
-            v_prop = ["NAME:" + property_name, "Value:=", property_value]
+            v_prop = ["NAME:" + name, "Value:=", value]
             self.change_property(v_prop)
-            if self.__dict__.get("_parameters", None) and property_name in self.__dict__["_parameters"]:
-                self.__dict__["_parameters"][property_name] = property_value
-            elif self.__dict__.get("_component_info", None) and property_name in self.__dict__.get(
-                "_component_info", None
-            ):
-                self.__dict__["_component_info"][property_name] = property_value
+            if self.__dict__.get("_parameters", None) and name in self.__dict__["_parameters"]:
+                self.__dict__["_parameters"][name] = value
+            elif self.__dict__.get("_component_info", None) and name in self.__dict__.get("_component_info", None):
+                self.__dict__["_component_info"][name] = value
             else:
-                self.__dict__[property_name] = property_value
+                self.__dict__[name] = value
         return True
 
     @pyaedt_function_handler()
     def _add_property(self, property_name, property_value):
         """Add a property.
 
         Parameters
@@ -826,48 +824,48 @@
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         self.__dict__[property_name] = property_value
         return True
 
-    @pyaedt_function_handler()
-    def change_property(self, vPropChange, names_list=None):
+    @pyaedt_function_handler(vPropChange="property", names_list="names")
+    def change_property(self, property_name, names=None):
         """Modify a property.
 
         Parameters
         ----------
-        vPropChange :
-
-        names_list : list, optional
+        property_name : list
+            Property value in AEDT syntax.
+        names : list, optional
              The default is ``None``.
 
         Returns
         -------
         bool
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         >>> oEditor.ChangeProperty
         """
-        vChangedProps = ["NAME:ChangedProps", vPropChange]
-        if names_list:
+        vChangedProps = ["NAME:ChangedProps", property_name]
+        if names:
             vPropServers = ["NAME:PropServers"]
-            for el in names_list:
+            for el in names:
                 vPropServers.append(el)
         else:
             vPropServers = ["NAME:PropServers", self.composed_name]
         tabname = None
-        if vPropChange[0][5:] in self._oeditor.GetProperties(self.tabname, self.composed_name):
+        if property_name[0][5:] in self._oeditor.GetProperties(self.tabname, self.composed_name):
             tabname = self.tabname
-        elif vPropChange[0][5:] in self._oeditor.GetProperties("PassedParameterTab", self.composed_name):
+        elif property_name[0][5:] in self._oeditor.GetProperties("PassedParameterTab", self.composed_name):
             tabname = "PassedParameterTab"
-        elif vPropChange[0][5:] in self._oeditor.GetProperties("BaseElementTab", self.composed_name):
+        elif property_name[0][5:] in self._oeditor.GetProperties("BaseElementTab", self.composed_name):
             tabname = "BaseElementTab"
         if tabname:
             vGeo3dlayout = ["NAME:" + tabname, vPropServers, vChangedProps]
             vOut = ["NAME:AllTabs", vGeo3dlayout]
             if "NAME:Component Location" in str(vChangedProps) and "PagePort" not in self.composed_name:
                 self._oeditor.ChangeProperty(vOut)
             return self._oeditor.ChangeProperty(vOut)
@@ -898,22 +896,22 @@
         """List of all schematic wires in the design."""
         wire_names = []
         for wire in self._oeditor.GetAllElements():
             if "Wire" in wire:
                 wire_names.append(wire)
         return wire_names
 
-    @pyaedt_function_handler()
-    def display_wire_properties(self, wire_name="", property_to_display="NetName", visibility="Name", location="Top"):
+    @pyaedt_function_handler(wire_name="name")
+    def display_wire_properties(self, name="", property_to_display="NetName", visibility="Name", location="Top"):
         """
         Display wire properties.
 
         Parameters
         ----------
-        wire_name : str, optional
+        name : str, optional
             Wire name to display.
             Default value is ``""``.
         property_to_display : str, optional
             Property to display. Choices are: ``"NetName"``, ``"PinCount"``, ``"AlignMicrowavePorts"``,
             ``"SchematicID"``, ``"Segment0"``.
             Default value is ``"NetName"``.
         visibility : str, optional
@@ -928,29 +926,29 @@
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         try:
             wire_exists = False
             for wire in self.wires:
-                if wire_name == wire.split("@")[1].split(";")[0]:
+                if name == wire.split("@")[1].split(";")[0]:
                     wire_id = wire.split("@")[1].split(";")[1].split(":")[0]
                     wire_exists = True
                     break
                 else:
                     continue
             if not wire_exists:
                 raise ValueError("Invalid wire name provided.")
 
             self._oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:PropDisplayPropTab",
-                        ["NAME:PropServers", "Wire@{};{};{}".format(wire_name, wire_id, 1)],
+                        ["NAME:PropServers", "Wire@{};{};{}".format(name, wire_id, 1)],
                         [
                             "NAME:NewProps",
                             ["NAME:" + property_to_display, "Format:=", visibility, "Location:=", location],
                         ],
                     ],
                 ]
             )
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/geometry_operators.py` & `pyaedt-0.8.9/pyaedt/modeler/geometry_operators.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modeler/modeler2d.py` & `pyaedt-0.8.9/pyaedt/modeler/modeler2d.py`

 * *Files 11% similar despite different names*

```diff
@@ -69,21 +69,21 @@
 
         """
         mess = "`primitives` is deprecated.\n"
         mess += " Use `app.modeler` directly to instantiate primitives methods."
         warn(mess, DeprecationWarning)
         return self._primitives
 
-    @pyaedt_function_handler()
-    def calculate_radius_2D(self, object_name, inner=False):
+    @pyaedt_function_handler(object_name="assignment")
+    def calculate_radius_2D(self, assignment, inner=False):
         """Calculate the extremity of an object in the radial direction.
 
         Parameters
         ----------
-        object_name : str
+        assignment : str
             name of the object from which to calculate the radius.
         inner : bool, optional
             The default is ``False``.
 
         Returns
         -------
         float
@@ -91,15 +91,15 @@
 
             .. note::
                 If ``inner=True``, then the maximum is returned; otherwise,
                 the minimum is returned.
 
         """
         radius = 0
-        oVertexIDs = self[object_name].vertices
+        oVertexIDs = self[assignment].vertices
         if oVertexIDs:
             if inner:
                 radius = 0
             else:
                 radius = 1e9
 
             for vertex in oVertexIDs:
@@ -107,16 +107,16 @@
                 vertex_radius = math.sqrt(float(pos[0]) ** 2 + float(pos[1]) ** 2)
                 if inner:
                     if vertex_radius > radius:
                         radius = vertex_radius
                 else:
                     if vertex_radius < radius:
                         radius = vertex_radius
-        elif self[object_name].edges:
-            radius = self[object_name].edges[0].length / (2 * math.pi)
+        elif self[assignment].edges:
+            radius = self[assignment].edges[0].length / (2 * math.pi)
 
         return radius
 
     @pyaedt_function_handler()
     def radial_split_2D(self, radius, name):
         """Split the stator and rotor for mesh refinement.
 
@@ -129,15 +129,15 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
 
-        cir = self.create_circle([0, 0, 0], 3, name=name + "_split", matname="vacuum")
+        cir = self.create_circle([0, 0, 0], 3, name=name + "_split", material="vacuum")
         self.oeditor.Copy(["NAME:Selections", "Selections:=", name])
         objects = [i for i in self.object_names]
         self.oeditor.Paste()
         name1 = [i for i in self.object_names if i not in objects]
         self.intersect([name1[0], cir.name], keep_originals=False)
         self.subtract(name, name1[0])
         return True
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/modeler3d.py` & `pyaedt-0.8.9/pyaedt/modeler/modeler3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -1091,46 +1091,42 @@
             self.logger.reset_timer()
             self.logger.info("Loading solids")
             for solid_pid in nas_to_dict["Solids"]:
                 for solid in nas_to_dict["Solids"][solid_pid]:
                     points = [nas_to_dict["Points"][id] for id in solid[1:]]
                     if solid[0] == "CPENTA":
                         element1 = self._app.modeler.create_polyline(
-                            position_list=[points[0], points[1], points[2]], close_surface=True, cover_surface=True
+                            points=[points[0], points[1], points[2]], cover_surface=True, close_surface=True
                         )
                         element2 = self._app.modeler.create_polyline(
-                            position_list=[points[3], points[4], points[5]], close_surface=True, cover_surface=True
+                            points=[points[3], points[4], points[5]], cover_surface=True, close_surface=True
                         )
                         self._app.modeler.connect([element1.name, element2.name])
                         element1.group_name = "PID_" + str(solid_pid)
                     elif solid[0] == "CHEXA":
                         element1 = self._app.modeler.create_polyline(
-                            position_list=[points[0], points[1], points[2], points[3]],
-                            close_surface=True,
-                            cover_surface=True,
+                            points=[points[0], points[1], points[2], points[3]], cover_surface=True, close_surface=True
                         )
                         element2 = self._app.modeler.create_polyline(
-                            position_list=[points[4], points[5], points[6], points[7]],
-                            close_surface=True,
-                            cover_surface=True,
+                            points=[points[4], points[5], points[6], points[7]], cover_surface=True, close_surface=True
                         )
                         self._app.modeler.connect([element1.name, element2.name])
                         element1.group_name = "PID_" + str(solid_pid)
                     elif solid[0] == "CTETRA":
                         element1 = self._app.modeler.create_polyline(
-                            position_list=[points[0], points[1], points[2]], close_surface=True, cover_surface=True
+                            points=[points[0], points[1], points[2]], cover_surface=True, close_surface=True
                         )
                         element2 = self._app.modeler.create_polyline(
-                            position_list=[points[0], points[1], points[3]], close_surface=True, cover_surface=True
+                            points=[points[0], points[1], points[3]], cover_surface=True, close_surface=True
                         )
                         element3 = self._app.modeler.create_polyline(
-                            position_list=[points[0], points[2], points[3]], close_surface=True, cover_surface=True
+                            points=[points[0], points[2], points[3]], cover_surface=True, close_surface=True
                         )
                         element4 = self._app.modeler.create_polyline(
-                            position_list=[points[1], points[2], points[3]], close_surface=True, cover_surface=True
+                            points=[points[1], points[2], points[3]], cover_surface=True, close_surface=True
                         )
                         self._app.modeler.unite([element1.name, element2.name, element3.name, element4.name])
                         element1.group_name = "PID_" + str(solid_pid)
 
             self.logger.info_timer("Solids loaded")
 
         objs_after = [i for i in self.object_names]
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/modelerpcb.py` & `pyaedt-0.8.9/pyaedt/modeler/modelerpcb.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,29 +186,29 @@
 
         """
         mess = "`primitives` is deprecated.\n"
         mess += " Use `app.modeler` directly to instantiate primitives methods."
         warn(mess, DeprecationWarning)
         return self._primitives
 
-    @pyaedt_function_handler
-    def obounding_box(self, object_name):
+    @pyaedt_function_handler(object_name="assignment")
+    def obounding_box(self, assignment):
         """Bounding box of a specified object.
 
         Returns
         -------
         list
             List of [LLx, LLy, URx, URy] coordinates.
 
         References
         ----------
 
         >>> oEditor.GetBBox
         """
-        bb = self.oeditor.GetBBox(object_name)
+        bb = self.oeditor.GetBBox(assignment)
         pll = bb.BBoxLL()
         pur = bb.BBoxUR()
         return [pll.GetX(), pll.GetY(), pur.GetX(), pur.GetY()]
 
     @pyaedt_function_handler()
     def _arg_with_dim(self, value, units=None):
         if units is None:
@@ -232,107 +232,109 @@
         if len(pos) < 3:
             zpos = self._arg_with_dim(0, units)
         else:
             zpos = self._arg_with_dim(pos[2], units)
 
         return xpos, ypos, zpos
 
-    @pyaedt_function_handler()
-    def change_property(self, property_object, property_name, property_value, property_tab="BaseElementTab"):
+    @pyaedt_function_handler(
+        property_object="assignment", property_name="name", property_value="value", property_tab="aedt_tab"
+    )
+    def change_property(self, assignment, name, value, aedt_tab="BaseElementTab"):
         """Change an oeditor property.
 
         Parameters
         ----------
-        property_object : str
+        assignment : str
             Name of the property object. It can be the name of an excitation or field reporter.
             For example, ``Excitations:Port1`` or ``FieldsReporter:Mag_H``.
-        property_name : str
+        name : str
             Name of the property. For example, ``Rotation Angle``.
-        property_value : str, list
+        value : str, list
             Value of the property. It is a string for a single value and a list of three elements for
             ``[x,y,z]`` coordianates.
-        property_tab : str
+        aedt_tab : str
             Name of the tab to update. Options are ``BaseElementTab``, ``EM Design``, and
             ``FieldsPostProcessorTab``. The default is ``BaseElementTab``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        if isinstance(property_value, list) and len(property_value) == 3:
-            xpos, ypos, zpos = self._pos_with_arg(property_value)
+        if isinstance(value, list) and len(value) == 3:
+            xpos, ypos, zpos = self._pos_with_arg(value)
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
-                        "NAME:" + property_tab,
-                        ["NAME:PropServers", property_object],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "X:=", xpos, "Y:=", ypos, "Z:=", zpos]],
+                        "NAME:" + aedt_tab,
+                        ["NAME:PropServers", assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "X:=", xpos, "Y:=", ypos, "Z:=", zpos]],
                     ],
                 ]
             )
-        elif isinstance(property_value, bool):
+        elif isinstance(value, bool):
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
-                        "NAME:" + property_tab,
-                        ["NAME:PropServers", property_object],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
+                        "NAME:" + aedt_tab,
+                        ["NAME:PropServers", assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "Value:=", value]],
                     ],
                 ]
             )
-        elif isinstance(property_value, (float, int)):
-            xpos = self._arg_with_dim(property_value, self.model_units)
+        elif isinstance(value, (float, int)):
+            xpos = self._arg_with_dim(value, self.model_units)
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
-                        "NAME:" + property_tab,
-                        ["NAME:PropServers", property_object],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", xpos]],
+                        "NAME:" + aedt_tab,
+                        ["NAME:PropServers", assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "Value:=", xpos]],
                     ],
                 ]
             )
-        elif isinstance(property_value, str):
+        elif isinstance(value, str):
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
-                        "NAME:" + property_tab,
-                        ["NAME:PropServers", property_object],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
+                        "NAME:" + aedt_tab,
+                        ["NAME:PropServers", assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "Value:=", value]],
                     ],
                 ]
             )
         else:
             self.logger.error("Wrong Property Value")
             return False
-        self.logger.info("Property {} Changed correctly.".format(property_name))
+        self.logger.info("Property {} Changed correctly.".format(name))
         return True
 
-    @pyaedt_function_handler()
-    def merge_design(self, merged_design=None, pos_x="0.0", pos_y="0.0", pos_z="0.0", rotation="0.0"):
+    @pyaedt_function_handler(pos_x="x", pos_y="y", pos_z="z")
+    def merge_design(self, merged_design=None, x="0.0", y="0.0", z="0.0", rotation="0.0"):
         """Merge a design into another.
 
         Parameters
         ----------
         merged_design : :class:`pyaedt.hfss3dlayout.Hfss3dLayout`
             Design to merge.
-        pos_x : float, str
+        x : float, str
             X Offset.
-        pos_y : float, str
+        y : float, str
             Y Offset.
-        pos_z : float, str
+        z : float, str
             Z Offset.
         rotation : float, str
             Rotation angle in deg.
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.ComponentsSubCircuit3DLayout`
@@ -352,52 +354,52 @@
                 continue
         if not comp_name:
             return False
         comp = ComponentsSubCircuit3DLayout(self, comp_name)
         self.components_3d[comp_name] = comp
         comp.is_3d_placement = True
         comp.local_origin = [0.0, 0.0, 0.0]
-        pos_x = self._arg_with_dim(pos_x)
-        pos_y = self._arg_with_dim(pos_y)
-        pos_z = self._arg_with_dim(pos_z)
+        x = self._arg_with_dim(x)
+        y = self._arg_with_dim(y)
+        z = self._arg_with_dim(z)
         rotation = self._arg_with_dim(rotation, "deg")
         comp.angle = rotation
-        comp.location = [pos_x, pos_y, pos_z]
+        comp.location = [x, y, z]
         return comp
 
-    @pyaedt_function_handler()
-    def change_clip_plane_position(self, clip_name, position):
+    @pyaedt_function_handler(clip_name="name", position="location")
+    def change_clip_plane_position(self, name, location):
         """Change the clip plane position.
 
         Parameters
         ----------
-        clip_name : str
+        name : str
             Name of the clip plane.
-        position : list
+        location : list
             List of ``[x,y,z]`` coordinates for the new position.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        return self.change_property(clip_name, "Location", position)
+        return self.change_property(name, "Location", location)
 
-    @pyaedt_function_handler()
-    def colinear_heal(self, selection, tolerance=0.1):
+    @pyaedt_function_handler(selection="assignment")
+    def colinear_heal(self, assignment, tolerance=0.1):
         """Remove small edges of one or more primitives.
 
         Parameters
         ----------
-        selection : str or list
+        assignment : str or list
             One or more primitives to heal.
         tolerance :  float, optional
             Tolerance value. The default is ``0.1``.
 
         Returns
         -------
         bool
@@ -411,43 +413,43 @@
 
 
         Examples
         --------
         >>> from pyaedt import Hfss3dLayout
         >>> h3d=Hfss3dLayout(specified_version="2021.2")
         >>> h3d.modeler.layers.add_layer("TOP")
-        >>> l1=h3d.modeler.create_line("TOP", [[0,0],[100,0]],  0.5, name="poly_1")
-        >>> l2=h3d.modeler.create_line("TOP", [[100,0],[120,-35]],  0.5, name="poly_2")
+        >>> l1=h3d.modeler.create_line("TOP",[[0,0],[100,0]],0.5)
+        >>> l2=h3d.modeler.create_line("TOP",[[100,0],[120,-35]],0.5)
         >>> h3d.modeler.unite([l1,l2])
-        >>> h3d.modeler.colinear_heal("poly_2", 0.25)
+        >>> h3d.modeler.colinear_heal("poly_2",0.25)
         True
         """
-        if isinstance(selection, str):
-            selection = [selection]
+        if isinstance(assignment, str):
+            assignment = [assignment]
         self.oeditor.Heal(
             [
                 "NAME:Repair",
                 "Selection:=",
-                selection,
+                assignment,
                 "Type:=",
                 "Colinear",
                 "Tol:=",
                 self.number_with_units(tolerance),
             ]
         )
 
         return True
 
-    @pyaedt_function_handler()
-    def expand(self, object_to_expand, size=1, expand_type="ROUND", replace_original=False):
+    @pyaedt_function_handler(object_to_expand="assignment")
+    def expand(self, assignment, size=1, expand_type="ROUND", replace_original=False):
         """Expand the object by a specific size.
 
         Parameters
         ----------
-        object_to_expand : str
+        assignment : str
             Name of the object.
         size : float, optional
             Size of the expansion. The default is ``1``.
         expand_type : str, optional
             Type of the expansion. Options are ``"ROUND"``, ``"MITER"``, and
             ``"CORNER"``. The default is ``"ROUND"``.
         replace_original : bool, optional
@@ -467,72 +469,70 @@
 
         Examples
         --------
         >>> from pyaedt import Hfss3dLayout
         >>> h3d=Hfss3dLayout(specified_version="2021.2")
         >>> h3d.modeler.layers.add_layer("TOP")
         >>> h3d.modeler.create_rectangle("TOP", [20,20],[50,50], name="rect_1")
-        >>> h3d.modeler.create_line("TOP",[[25,25],[40,40]], name="line_3")
+        >>> h3d.modeler.create_line("TOP",[[25,25],[40,40]])
         >>> out1 = h3d.modeler.expand("line_3")
         >>> print(out1)
         line_4
 
         """
-        object_to_expand = self.convert_to_selections(object_to_expand)
+        assignment = self.convert_to_selections(assignment)
         self.cleanup_objects()
-        layer = self.oeditor.GetPropertyValue("BaseElementTab", object_to_expand, "PlacementLayer")
-        poly = self.oeditor.GetPolygonDef(object_to_expand).GetPoints()
+        layer = self.oeditor.GetPropertyValue("BaseElementTab", assignment, "PlacementLayer")
+        poly = self.oeditor.GetPolygonDef(assignment).GetPoints()
         pos = [poly[0].GetX(), poly[0].GetY()]
         geom_names = self.oeditor.FindObjectsByPoint(self.oeditor.Point().Set(pos[0], pos[1]), layer)
-        self.oeditor.Expand(
-            self.number_with_units(size), expand_type, replace_original, ["NAME:elements", object_to_expand]
-        )
+        self.oeditor.Expand(self.number_with_units(size), expand_type, replace_original, ["NAME:elements", assignment])
         self.cleanup_objects()
         if not replace_original:
             new_geom_names = [
                 i
                 for i in self.oeditor.FindObjectsByPoint(self.oeditor.Point().Set(pos[0], pos[1]), layer)
                 if i not in geom_names
             ]
             return new_geom_names[0]
-        return object_to_expand
+        return assignment
 
-    @pyaedt_function_handler()
-    def import_cadence_brd(self, brd_filename, edb_path=None, edb_name=None):
+    @pyaedt_function_handler(brd_filename="input_file", edb_path="output_dir", edb_name="name")
+    def import_cadence_brd(self, input_file, output_dir=None, name=None):
         """Import a cadence board.
 
         Parameters
         ----------
-        brd_filename : str
+        input_file : str
             Full path and name of the BRD file to import.
-        edb_path : str, optional
+        output_dir : str, optional
             Path where the EDB is to be created. The default is ``None``, in which
             case the project directory is used.
-        edb_name : str, optional
+        name : str, optional
             Name of the EDB. The default is ``None``, in which
             case the board name is used.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oImportExport.ImportExtracta
         """
-        if not edb_path:
-            edb_path = self.projdir
-        if not edb_name:
-            name = os.path.basename(brd_filename)
-            edb_name = os.path.splitext(name)[0]
+        if not output_dir:
+            output_dir = self.projdir
+        if not name:
+            name = os.path.basename(input_file)
+            name = os.path.splitext(name)[0]
 
         self._oimportexport.ImportExtracta(
-            brd_filename, os.path.join(edb_path, edb_name + ".aedb"), os.path.join(edb_path, edb_name + ".xml")
+            input_file, os.path.join(output_dir, name + ".aedb"), os.path.join(output_dir, name + ".xml")
         )
         self._app.__init__(self._app._desktop.GetActiveProject().GetName())
         return True
 
     @pyaedt_function_handler()
     def modeler_variable(self, value):
         """Retrieve a modeler variable.
@@ -546,47 +546,47 @@
 
         """
         if isinstance(value, str):
             return value
         else:
             return str(value) + self.model_units
 
-    @pyaedt_function_handler()
-    def import_ipc2581(self, ipc_filename, edb_path=None, edb_name=None):
+    @pyaedt_function_handler(ipc_filename="input_file", edb_path="output_dir", edb_name="name")
+    def import_ipc2581(self, input_file, output_dir=None, name=None):
         """Import an IPC file.
 
         Parameters
         ----------
-        ipc_filename : str
+        input_file : str
             Full path and name of the IPC file.
-        edb_path : str, optional
+        output_dir : str, optional
             Path where the EDB is to be created. The default is ``None``, in which
             case the project directory is used.
-        edb_name : str, optional
+        name : str, optional
             Name of the EDB. The default is ``None``, in which
             case the board name is used.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oImportExport.ImportIPC
         """
-        if not edb_path:
-            edb_path = self.projdir
-        if not edb_name:
-            name = os.path.basename(ipc_filename)
-            edb_name = os.path.splitext(name)[0]
+        if not output_dir:
+            output_dir = self.projdir
+        if not name:
+            name = os.path.basename(input_file)
+            name = os.path.splitext(name)[0]
 
         self._oimportexport.ImportIPC(
-            ipc_filename, os.path.join(edb_path, edb_name + ".aedb"), os.path.join(edb_path, edb_name + ".xml")
+            input_file, os.path.join(output_dir, name + ".aedb"), os.path.join(output_dir, name + ".xml")
         )
         self._app.__init__(self._app._desktop.GetActiveProject().GetName())
         return True
 
     @pyaedt_function_handler()
     def subtract(self, blank, tool):
         """Subtract objects from one or more names.
@@ -615,175 +615,173 @@
         for el in tool:
             vArg1.append(el)
 
         if self.oeditor is not None:
             self.oeditor.Subtract(vArg1)
         return self.cleanup_objects()
 
-    @pyaedt_function_handler()
-    def convert_to_selections(self, objects_to_split, return_list=False):
+    @pyaedt_function_handler(objects_to_split="assignment")
+    def convert_to_selections(self, assignment, return_list=False):
         """Convert one or more object to selections.
 
         Parameters
         ----------
-        objects_to_split : str, int, list
+        assignment : str, int, list
             One or more objects to convert to selections. A list can contain
             both strings (object names) and integers (object IDs).
         return_list : bool, option
             Whether to return a list of the selections. The default is
             ``False``, in which case a string of the selections is returned.
             If ``True``, a list of the selections is returned.
 
         Returns
         -------
         str or list
            String or list of the selections.
 
         """
 
-        if not isinstance(objects_to_split, list):
-            objects_to_split = [objects_to_split]
+        if not isinstance(assignment, list):
+            assignment = [assignment]
         objnames = []
-        for el in objects_to_split:
+        for el in assignment:
             if isinstance(el, str):
                 objnames.append(el)
             elif "name" in dir(el):
                 objnames.append(el.name)
             else:
                 pass
         if return_list:
             return objnames
         else:
             return ",".join(objnames)
 
-    @pyaedt_function_handler()
-    def unite(self, objectlists):
+    @pyaedt_function_handler(objectlists="assignment")
+    def unite(self, assignment):
         """Unite objects from names.
 
         Parameters
         ----------
-        objectlists : list
+        assignment : list
             List of objects to unite.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Unite
         """
 
         vArg1 = ["NAME:primitives"]
-        if len(objectlists) >= 2:
-            objectlists = self.convert_to_selections(objectlists, True)
+        if len(assignment) >= 2:
+            assignment = self.convert_to_selections(assignment, True)
             self.cleanup_objects()
 
-            for el in objectlists:
+            for el in assignment:
                 vArg1.append(el)
             self.oeditor.Unite(vArg1)
             return self.cleanup_objects()
         else:
             self.logger.error("Input list must contain at least two elements.")
             return False
 
-    @pyaedt_function_handler()
-    def intersect(self, objectlists):
+    @pyaedt_function_handler(objectlists="assignment")
+    def intersect(self, assignment):
         """Intersect objects from names.
 
         Parameters
         ----------
-        objectlists : list
+        assignment : list
             List of objects to intersect.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Intersect
         """
         vArg1 = ["NAME:primitives"]
-        if len(objectlists) >= 2:
-            objectlists = self.convert_to_selections(objectlists, True)
+        if len(assignment) >= 2:
+            assignment = self.convert_to_selections(assignment, True)
             self.cleanup_objects()
 
-            for el in objectlists:
+            for el in assignment:
                 vArg1.append(el)
             self.oeditor.Intersect(vArg1)
             return self.cleanup_objects()
         else:
             self.logger.error("Input list must contain at least two elements.")
             return False
 
-    @pyaedt_function_handler()
-    def duplicate(self, objectlists, count, direction_vector):
+    @pyaedt_function_handler(objectlists="assignment", direction_vector="vector")
+    def duplicate(self, assignment, count, vector):
         """Duplicate one or more elements along a vector.
 
         Parameters
         ----------
-        objectlists : list
+        assignment : list
             List of elements to duplicate.
         count : int
 
-        direction_vector : list
+        vector : list
             List of ``[x,y]`` coordinates for the direction vector.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Duplicate
         """
-        objectlists = self.convert_to_selections(objectlists, True)
+        assignment = self.convert_to_selections(assignment, True)
 
         self.cleanup_objects()
-        if isinstance(objectlists, str):
-            objectlists = [objectlists]
-        self.oeditor.Duplicate(
-            ["NAME:options", "count:=", count], ["NAME:elements", ",".join(objectlists)], direction_vector
-        )
+        if isinstance(assignment, str):
+            assignment = [assignment]
+        self.oeditor.Duplicate(["NAME:options", "count:=", count], ["NAME:elements", ",".join(assignment)], vector)
         return self.cleanup_objects()
 
-    @pyaedt_function_handler()
-    def duplicate_across_layers(self, objects, layers):
+    @pyaedt_function_handler(objects="assignment")
+    def duplicate_across_layers(self, assignment, layers):
         """Duplicate one or more elements along a vector.
 
         Parameters
         ----------
-        objects : list
+        assignment : list
             List of elements to duplicate.
         layers : str, list
             Layer name on which duplicate object.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.DuplicateAcrossLyrs
         """
-        objects = self.convert_to_selections(objects, True)
+        assignment = self.convert_to_selections(assignment, True)
         self.cleanup_objects()
 
         if isinstance(layers, str):
             layers = [layers]
-        varg1 = ["NAME:elements"] + objects
+        varg1 = ["NAME:elements"] + assignment
         varg2 = ["NAME:layers"] + layers
 
         self.oeditor.DuplicateAcrossLyrs(varg1, varg2)
         return self.cleanup_objects()
 
     @pyaedt_function_handler()
     def set_temperature_dependence(
@@ -837,23 +835,23 @@
         except Exception:
             self.logger.error("Failed to enable the temperature dependence.")
             return False
         else:
             self.logger.info("Assigned Objects Temperature")
             return True
 
-    @pyaedt_function_handler()
-    def set_spice_model(self, component_name, model_path, model_name=None, subcircuit_name=None, pin_map=None):
+    @pyaedt_function_handler(component_name="assignment", model_path="input_file")
+    def set_spice_model(self, assignment, input_file, model_name=None, subcircuit_name=None, pin_map=None):
         """Assign a Spice model to a component.
 
         Parameters
         ----------
-        component_name : str
+        assignment : str
             Name of the component.
-        model_path : str, optional
+        input_file : str, optional
             Full path to the model file. The default is ``None``.
         model_name : str, optional
             Name of the model. The default is ``None``, in which case the model name is the file name without an
             extension.
         subcircuit_name : str, optional
             Name of the subcircuit. The default is ``None``, in which case the subcircuit name is the model name.
         pin_map : list, optional
@@ -866,22 +864,19 @@
             ``True`` when successful, ``False`` when failed.
 
         Examples
         --------
 
         >>> from pyaedt import Hfss3dLayout
         >>> h3d = Hfss3dLayout("myproject")
-        >>> h3d.modeler.set_spice_model(component_name="A1",
-        ...                             modelpath="pathtospfile",
-        ...                             modelname="spicemodelname",
-        ...                             subcircuit_name="SUBCK1")
+        >>> h3d.modeler.set_spice_model(assignment="A1",input_file=,subcircuit_name="SUBCK1")
 
         """
         if not model_name:
-            model_name = get_filename_without_extension(model_path)
+            model_name = get_filename_without_extension(input_file)
         if model_name not in list(self.o_model_manager.GetNames()):
             args = [
                 "NAME:" + model_name,
                 "Name:=",
                 model_name,
                 "ModTime:=",
                 1643711258,
@@ -896,29 +891,29 @@
                 "ImageFile:=",
                 "",
                 "SymbolPinConfiguration:=",
                 0,
                 ["NAME:PortInfoBlk"],
                 ["NAME:PortOrderBlk"],
                 "filename:=",
-                model_path,
+                input_file,
                 "modelname:=",
                 model_name,
             ]
             self.o_model_manager.Add(args)
         if not subcircuit_name:
             subcircuit_name = model_name
-        with open_file(model_path, "r") as f:
+        with open_file(input_file, "r") as f:
             for line in f:
                 if "subckt" in line.lower():
                     pinNames = [i.strip() for i in re.split(" |\t", line) if i]
                     pinNames.remove(pinNames[0])
                     pinNames.remove(pinNames[0])
                     break
-        componentPins = list(self.components[component_name].pins.keys())
+        componentPins = list(self.components[assignment].pins.keys())
         componentPins.reverse()
         if not pin_map:
             pin_map = []
             i = 0
             if len(componentPins) >= len(pinNames):
                 for pn in pinNames:
                     pin_map.append(pn + ":=")
@@ -934,26 +929,26 @@
             "CompPropType:=",
             0,
             "PinPairRLC:=",
             [
                 "RLCModelType:=",
                 4,
                 "SPICE_file_path:=",
-                model_path,
+                input_file,
                 "SPICE_model_name:=",
                 model_name,
                 "SPICE_subckt:=",
                 subcircuit_name,
                 "terminal_pin_map:=",
                 pin_map,
             ],
         ]
-        args = ["NAME:ModelChanges", ["NAME:UpdateModel0", ["NAME:ComponentNames", component_name], "Prop:=", args2]]
+        args = ["NAME:ModelChanges", ["NAME:UpdateModel0", ["NAME:ComponentNames", assignment], "Prop:=", args2]]
         self.oeditor.UpdateModels(args)
-        self.logger.info("Spice Model Correctly assigned to {}.".format(component_name))
+        self.logger.info("Spice Model Correctly assigned to {}.".format(assignment))
         return True
 
     @pyaedt_function_handler()
     def clip_plane(self):
         """Create a clip plane in the layout.
 
         .. note::
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/pcb/Primitives3DLayout.py` & `pyaedt-0.8.9/pyaedt/modeler/pcb/Primitives3DLayout.py`

 * *Files 5% similar despite different names*

```diff
@@ -161,21 +161,21 @@
             geom[k] = v
         for k, v in self.lines_voids.items():
             geom[k] = v
         for k, v in self.circles_voids.items():
             geom[k] = v
         return geom
 
-    @pyaedt_function_handler()
-    def objects_by_layer(self, layer_name, object_filter=None, include_voids=False):
+    @pyaedt_function_handler(layer_name="layer", object_filter="filter")
+    def objects_by_layer(self, layer, object_filter=None, include_voids=False):
         """Retrieve the list of objects that belongs to a specific layer.
 
         Parameters
         ----------
-        layer_name : str
+        layer : str
             Name of the layer to filter.
         object_filter : str, list, optional
             Name of the category to include in search. Options are `"poly"`, `"circle"`,
             `"rect"`,`"line"`,`"arc"`, `"via"`,`"pin"` and `"component"`.
         include_voids : bool, optional
             Either if include or not the voids in search.
 
@@ -188,32 +188,32 @@
         objs = []
         if object_filter:
             if isinstance(object_filter, str):
                 object_filter = [object_filter]
 
             for poly in object_filter:
                 objs = self.modeler.oeditor.FilterObjectList(
-                    "Type", poly, self.modeler.oeditor.FindObjects("Layer", layer_name)
+                    "Type", poly, self.modeler.oeditor.FindObjects("Layer", layer)
                 )
                 if include_voids:
                     objs = self.modeler.oeditor.FilterObjectList(
-                        "Type", poly + " void", self.modeler.oeditor.FindObjects("Layer", layer_name)
+                        "Type", poly + " void", self.modeler.oeditor.FindObjects("Layer", layer)
                     )
 
         else:
-            objs = self.modeler.oeditor.FindObjects("Layer", layer_name)
+            objs = self.modeler.oeditor.FindObjects("Layer", layer)
         return objs
 
-    @pyaedt_function_handler()
-    def objects_by_net(self, net_name, object_filter=None, include_voids=False):
+    @pyaedt_function_handler(net_name="net")
+    def objects_by_net(self, net, object_filter=None, include_voids=False):
         """Retrieve the list of objects that belongs to a specific net.
 
         Parameters
         ----------
-        net_name : str
+        net : str
             Name of the net to filter.
         object_filter : str, list, optional
             Name of the category to include in search. Options are `"poly"`, `"circle"`,
             `"rect"`,`"line"`,`"arc"`, `"via"`,`"pin"` and `"component"`.
         include_voids : bool, optional
             Either if include or not the voids in search.
 
@@ -225,24 +225,22 @@
 
         objs = []
         if object_filter:
             if isinstance(object_filter, str):
                 object_filter = [object_filter]
 
             for poly in object_filter:
-                objs = self.modeler.oeditor.FilterObjectList(
-                    "Type", poly, self.modeler.oeditor.FindObjects("Net", net_name)
-                )
+                objs = self.modeler.oeditor.FilterObjectList("Type", poly, self.modeler.oeditor.FindObjects("Net", net))
                 if include_voids:
                     objs = self.modeler.oeditor.FilterObjectList(
-                        "Type", poly + " void", self.modeler.oeditor.FindObjects("Net", net_name)
+                        "Type", poly + " void", self.modeler.oeditor.FindObjects("Net", net)
                     )
 
         else:
-            objs = self.modeler.oeditor.FindObjects("Net", net_name)
+            objs = self.modeler.oeditor.FindObjects("Net", net)
         return objs
 
     @pyaedt_function_handler()
     def _get_names(self, categories):
         names = []
         for category in categories:
             names.extend(self.modeler.oeditor.FindObjects("Type", category))
@@ -779,15 +777,15 @@
                     if prop[0] == "NAME:pds":
                         layers_num = len(prop) - 1
                         i = 1
                         while i <= layers_num:
                             lay = prop[i]
                             lay_name = lay[2]
                             lay_id = int(lay[4])
-                            self._padstacks[name].add_layer(layername=lay_name, layer_id=lay_id)
+                            self._padstacks[name].add_layer(layer=lay_name, layer_id=lay_id)
                             self._padstacks[name].layers[lay_name].layername = lay_name
                             self._padstacks[name].layers[lay_name].pad = self._padstacks[name].add_hole(
                                 lay[6][1], list(lay[6][3]), lay[6][5], lay[6][7], lay[6][9]
                             )
                             self._padstacks[name].layers[lay_name].antipad = self._padstacks[name].add_hole(
                                 lay[8][1], list(lay[8][3]), lay[8][5], lay[8][7], lay[8][9]
                             )
@@ -800,21 +798,21 @@
                             i += 1
                         pass
                 except Exception:
                     pass
 
         return self._padstacks
 
-    @pyaedt_function_handler()
-    def change_net_visibility(self, netlist=None, visible=False):
+    @pyaedt_function_handler(netlist="assignment")
+    def change_net_visibility(self, assignment=None, visible=False):
         """Change the visibility of one or more nets.
 
         Parameters
         ----------
-        netlist : str  or list, optional
+        assignment : str  or list, optional
             One or more nets to visualize. The default is ``None``.
             If no nets are provided all the nets in the design will be selected.
         visible : bool, optional
             Whether to make the selected nets visible.
             The default value is ``False``.
 
         Returns
@@ -824,36 +822,36 @@
 
         References
         ----------
 
         >>> oEditor.SetNetVisible
         """
         nets_dictionary = {}
-        if not netlist:
-            netlist = self.nets
-        elif [x for x in netlist if x not in self.nets]:
+        if not assignment:
+            assignment = self.nets
+        elif [x for x in assignment if x not in self.nets]:
             self.logger.error("Selected net doesn't exist in current design.")
             return False
-        if isinstance(netlist, str):
-            netlist = [netlist]
+        if isinstance(assignment, str):
+            assignment = [assignment]
 
         if isinstance(visible, str):
             if visible.lower() == "true":
                 visible = True
             elif visible.lower() == "false":
                 visible = False
             else:
                 self.logger.error("Provide a valid string value for visibility.")
                 return False
         elif not isinstance(visible, bool):
             self.logger.error("Provide a valid type value for visibility.")
             return False
 
         for net in self.nets:
-            if net not in netlist:
+            if net not in assignment:
                 nets_dictionary[net] = not visible
             else:
                 nets_dictionary[net] = visible
 
         args = ["NAME:Args"]
         try:
             for key in nets_dictionary:
@@ -863,26 +861,26 @@
                 args.append(nets_dictionary[key])
             self.oeditor.SetNetVisible(args)
             return True
         except Exception:
             self.logger.error("Couldn't change nets visibility.")
             return False
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(netname="net")
     def create_via(
         self,
         padstack="PlanarEMVia",
         x=0,
         y=0,
         rotation=0,
         hole_diam=None,
         top_layer=None,
         bot_layer=None,
         name=None,
-        netname=None,
+        net=None,
     ):
         # type: (str, float | str, float | str, float, float, str, str, str, str) -> Pins3DLayout
         """Create a via based on an existing padstack.
 
         Parameters
         ----------
         padstack : str, optional
@@ -898,15 +896,15 @@
             in which case the override is disabled.
         top_layer : str, optional
             Top layer. If ``None`` the first layer is taken.
         bot_layer : str, optional
             Bottom layer. If ``None`` the last layer is taken.
         name : str, optional
             Name of the via. If ``None`` a random name is generated.
-        netname : str, optional
+        net : str, optional
             Name of the net. The default is ``None``, in which case no
             name is assigned.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dlayout.Pins3DLayout` or bool
             Object via created when successful, ``False`` when failed.
@@ -943,182 +941,164 @@
                 arg.append("hole diameter:="), arg.append([self.number_with_units(1)])
 
             arg.append("Pin:="), arg.append(False)
             arg.append("highest_layer:="), arg.append(top_layer)
             arg.append("lowest_layer:="), arg.append(bot_layer)
 
             self.oeditor.CreateVia(arg)
-            if netname:
+            if net:
                 self.oeditor.ChangeProperty(
                     [
                         "NAME:AllTabs",
                         [
                             "NAME:BaseElementTab",
                             ["NAME:PropServers", name],
-                            ["NAME:ChangedProps", ["NAME:Net", "Value:=", netname]],
+                            ["NAME:ChangedProps", ["NAME:Net", "Value:=", net]],
                         ],
                     ]
                 )
             self._cleanup_vias(pins=False)
             return self.vias[name]
         except ValueError as e:
             self.logger.error(str(e))
             return False
 
-    @pyaedt_function_handler()
-    def create_circle(self, layername, x, y, radius, name=None, net_name=None, **kwargs):
+    @pyaedt_function_handler(layername="layer", netname="net", net_name="net")
+    def create_circle(self, layer, x, y, radius, name=None, net=None, **kwargs):
         """Create a circle on a layer.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer.
         x : float
             Position on the X axis.
         y : float
             Position on the Y axis.
         radius : float
             Radius of the circle.
         name : str, optional
             Name of the circle. The default is ``None``, in which case the
             default name is assigned.
-        net_name : str, optional
+        net : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dlayout.Circle3dLayout`
             Objects of the circle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreateCircle
         """
-        if "netname" in kwargs:
-            warnings.warn(
-                "`netname` is deprecated. Use `net_name` instead.",
-                DeprecationWarning,
-            )
-            net_name = kwargs["netname"]
         if not name:
             name = _uname()
         else:
             listnames = self.oeditor.FindObjects("Name", name)
             if listnames:
                 name = _uname(name)
 
         vArg1 = ["NAME:Contents", "circleGeometry:="]
         vArg2 = []
         vArg2.append("Name:="), vArg2.append(name)
-        vArg2.append("LayerName:="), vArg2.append(layername)
+        vArg2.append("LayerName:="), vArg2.append(layer)
         vArg2.append("lw:="), vArg2.append("0")
         vArg2.append("x:="), vArg2.append(self.number_with_units(x))
         vArg2.append("y:="), vArg2.append(self.number_with_units(y))
         vArg2.append("r:="), vArg2.append(self.number_with_units(radius))
         vArg1.append(vArg2)
         self.oeditor.CreateCircle(vArg1)
         primitive = Circle3dLayout(self, name, False)
         self._circles[name] = primitive
 
-        if net_name:
-            primitive.change_property(property_val=["NAME:Net", "Value:=", net_name])
+        if net:
+            primitive.change_property(value=["NAME:Net", "Value:=", net])
 
         return primitive
 
-    @pyaedt_function_handler()
-    def create_rectangle(
-        self, layername, origin, dimensions, corner_radius=0, angle=0, name=None, net_name=None, **kwargs
-    ):
+    @pyaedt_function_handler(layername="layer", dimensions="sizes", net_name="net", netname="net")
+    def create_rectangle(self, layer, origin, sizes, corner_radius=0, angle=0, name=None, net=None, **kwargs):
         """Create a rectangle on a layer.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer.
         origin : list
             Origin of the coordinate system in a list of ``[x, y]`` coordinates.
-        dimensions : list
+        sizes : list
             Dimensions for the box in a list of ``[x, y]`` coordinates.
         corner_radius : float, optional
         angle : float, optional
             Angle rotation in degrees. The default is ``0``.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case the
             default name is assigned.
-        net_name : str, optional
+        net : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dlayout.Rect3dLayout`
             Name of the rectangle created when successful.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
         """
-        if "netname" in kwargs:
-            warnings.warn(
-                "`netname` is deprecated. Use `net_name` instead.",
-                DeprecationWarning,
-            )
-            net_name = kwargs["netname"]
         if not name:
             name = _uname()
         else:
             listnames = self.oeditor.FindObjects("Name", name)
             if listnames:
                 name = _uname(name)
 
         vArg1 = ["NAME:Contents", "rectGeometry:="]
         vArg2 = []
         vArg2.append("Name:="), vArg2.append(name)
-        vArg2.append("LayerName:="), vArg2.append(layername)
+        vArg2.append("LayerName:="), vArg2.append(layer)
         vArg2.append("lw:="), vArg2.append("0")
         vArg2.append("Ax:="), vArg2.append(self.number_with_units(origin[0]))
         vArg2.append("Ay:="), vArg2.append(self.number_with_units(origin[1]))
-        vArg2.append("Bx:="), vArg2.append(
-            self.number_with_units(origin[0]) + "+" + self.number_with_units(dimensions[0])
-        )
-        vArg2.append("By:="), vArg2.append(
-            self.number_with_units(origin[1]) + "+" + self.number_with_units(dimensions[1])
-        )
+        vArg2.append("Bx:="), vArg2.append(self.number_with_units(origin[0]) + "+" + self.number_with_units(sizes[0]))
+        vArg2.append("By:="), vArg2.append(self.number_with_units(origin[1]) + "+" + self.number_with_units(sizes[1]))
         vArg2.append("cr:="), vArg2.append(self.number_with_units(corner_radius))
         vArg2.append("ang:=")
         vArg2.append(self.number_with_units(angle, "deg"))
         vArg1.append(vArg2)
         self.oeditor.CreateRectangle(vArg1)
         primitive = Rect3dLayout(self, name, False)
         self._rectangles[name] = primitive
 
-        if net_name:
-            primitive.change_property(property_val=["NAME:Net", "Value:=", net_name])
+        if net:
+            primitive.change_property(value=["NAME:Net", "Value:=", net])
 
         return primitive
 
-    @pyaedt_function_handler()
-    def create_polygon(self, layername, point_list, units=None, name=None, net_name=None):
+    @pyaedt_function_handler(layername="layer", net_name="net")
+    def create_polygon(self, layer, point_list, units=None, name=None, net=None):
         """Create a polygon on a specified layer.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer.
         point_list : list
             Origin of the coordinate system in a list of ``[x, y]`` coordinates.
         units : str, optional
             Polygon units. Default is modeler units.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case the
             default name is assigned.
-        net_name : str, optional
+        net : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dlayout.Polygons3DLayout`
             Object of the rectangle created when successful.
@@ -1134,42 +1114,42 @@
             listnames = self.oeditor.FindObjects("Name", name)
             if listnames:
                 name = _uname(name)
 
         vArg1 = ["NAME:Contents", "polyGeometry:="]
         vArg2 = []
         vArg2.append("Name:="), vArg2.append(name)
-        vArg2.append("LayerName:="), vArg2.append(layername)
+        vArg2.append("LayerName:="), vArg2.append(layer)
         vArg2.append("lw:="), vArg2.append("0")
         vArg2.append("n:="), vArg2.append(len(point_list))
         vArg2.append("U:="), vArg2.append(units if units else self.model_units)
         for point in point_list:
             vArg2.append("x:="), vArg2.append(point[0])
             vArg2.append("y:="), vArg2.append(point[1])
         vArg1.append(vArg2)
         self.oeditor.CreatePolygon(vArg1)
         primitive = Polygons3DLayout(self, name, is_void=False)
         self._polygons[name] = primitive
 
-        if net_name:
-            primitive.change_property(property_val=["NAME:Net", "Value:=", net_name])
+        if net:
+            primitive.change_property(value=["NAME:Net", "Value:=", net])
 
         return primitive
 
-    @pyaedt_function_handler()
-    def create_polygon_void(self, layername, point_list, object_owner, units=None, name=None):
+    @pyaedt_function_handler(layername="layer", point_list="points", object_owner="assignment")
+    def create_polygon_void(self, layer, points, assignment, units=None, name=None):
         """Create a polygon void on a specified layer.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer.
-        point_list : list
+        points : list
             List of points in a list of ``[x, y]`` coordinates.
-        object_owner : str
+        assignment : str
             Object Owner.
         units : str, optional
             Polygon units. Default is modeler units.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case the
             default name is assigned.
 
@@ -1185,47 +1165,49 @@
         """
         if not name:
             name = _uname()
         else:
             listnames = self.oeditor.FindObjects("Name", name)
             if listnames:
                 name = _uname(name)
-        if not self.oeditor.FindObjects("Name", object_owner):
+        if not self.oeditor.FindObjects("Name", assignment):
             self._app.logger.error("Owner Polygon not found.")
             return False
 
-        vArg1 = ["NAME:Contents", "owner:=", object_owner, "poly voidGeometry:="]
+        vArg1 = ["NAME:Contents", "owner:=", assignment, "poly voidGeometry:="]
         vArg2 = []
         vArg2.append("Name:="), vArg2.append(name)
-        vArg2.append("LayerName:="), vArg2.append(layername)
+        vArg2.append("LayerName:="), vArg2.append(layer)
         vArg2.append("lw:="), vArg2.append("0")
-        vArg2.append("n:="), vArg2.append(len(point_list))
+        vArg2.append("n:="), vArg2.append(len(points))
         vArg2.append("U:="), vArg2.append(units if units else self.model_units)
-        for point in point_list:
+        for point in points:
             vArg2.append("x:="), vArg2.append(point[0])
             vArg2.append("y:="), vArg2.append(point[1])
         vArg1.append(vArg2)
         self.oeditor.CreatePolygonVoid(vArg1)
         primitive = Polygons3DLayout(self, name, is_void=True)
         self._polygons[name] = primitive
 
         return primitive
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(
+        layername="layer", center_line_list="center_line_coordinates", net_name="net", netname="net"
+    )
     def create_line(
-        self, layername, center_line_list, lw=1, start_style=0, end_style=0, name=None, net_name=None, **kwargs
+        self, layer, center_line_coordinates, lw=1, start_style=0, end_style=0, name=None, net=None, **kwargs
     ):
         # type: (str, list, float|str, int, int, str, str, any) -> Line3dLayout
         """Create a line based on a list of points.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer to create the line on.
-        center_line_list : list
+        center_line_coordinates : list
             List of centerline coordinates in the form of ``[x, y]``.
         lw : float, optional
             Line width. The default is ``1``.
         start_style :
             Starting style of the line. Options are:
 
             * ``0`` - Flat
@@ -1235,15 +1217,15 @@
             The default is ``0``.
         end_style :
             Ending style of the line. The options are the same as
             those for ``start_style``. The default is ``0``.
         name : str, optional
             Name  of the line. The default is ``None``, in which case the
             default name is assigned.
-        net_name : str, optional
+        net : str, optional
             Name of the net. The default is ``None``, in which case the
             default name is assigned.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3dlayout.Line3dLayout`
             Object of the line created when successful.
@@ -1254,76 +1236,53 @@
         >>> oEditor.CreateLine
         """
         if "netname" in kwargs:
             warnings.warn(
                 "`netname` is deprecated. Use `net_name` instead.",
                 DeprecationWarning,
             )
-            net_name = kwargs["netname"]
+            net = kwargs["netname"]
         if not name:
             name = _uname()
         else:
             listnames = self.oeditor.FindObjects("Name", name)
             if listnames:
                 name = _uname(name)
         arg = ["NAME:Contents", "lineGeometry:="]
         arg2 = [
             "Name:=",
             name,
             "LayerName:=",
-            layername,
+            layer,
             "lw:=",
             self.number_with_units(lw),
             "endstyle:=",
             end_style,
             "StartCap:=",
             start_style,
             "n:=",
-            len(center_line_list),
+            len(center_line_coordinates),
             "U:=",
             self.model_units,
         ]
-        for a in center_line_list:
+        for a in center_line_coordinates:
             arg2.append("x:=")
             arg2.append(a[0])
             arg2.append("y:=")
             arg2.append(a[1])
         arg.append(arg2)
         self.oeditor.CreateLine(arg)
         primitive = Line3dLayout(self, name, False)
         self._lines[name] = primitive
 
-        if net_name:
-            primitive.change_property(property_val=["NAME:Net", "Value:=", net_name])
+        if net:
+            primitive.change_property(value=["NAME:Net", "Value:=", net])
         return primitive
 
     @pyaedt_function_handler()
-    def arg_with_dim(self, Value, sUnits=None):
-        """Format arguments with dimensions.
-
-        .. deprecated:: 0.6.56
-           Use :func:`number_with_units` instead.
-
-        Parameters
-        ----------
-        Value :
-            The value of the quantity.
-        sUnits :
-             The default is ``None``.
-
-        Returns
-        -------
-        str
-            String containing the value or value and the units if `sUnits` is not ``None``.
-
-        """
-        warnings.warn("Use :func:`number_with_units` instead.", DeprecationWarning)
-        return self._app.number_with_units(Value, sUnits)
-
-    @pyaedt_function_handler()
     def number_with_units(self, value, units=None):
         """Convert a number to a string with units.
 
         If value is a string, it's returned as is.
 
         Parameters
         ----------
@@ -1336,15 +1295,15 @@
         -------
         str
            String concatenating the value and unit.
 
         """
         return self._app.number_with_units(value, units)
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def place_3d_component(
         self,
         component_path,
         number_of_terminals=1,
         placement_layer=None,
         component_name=None,
         pos_x=0,
@@ -1532,24 +1491,25 @@
                 "elements:=",
                 pins,
             ]
         )
         comp = Components3DLayout(self, comp_name.split(";")[-1])
         return comp
 
-    def create_text(self, text, position, placement_layer="PostProcessing", angle=0, font_size=12):
+    @pyaedt_function_handler(placement_layer="layer")
+    def create_text(self, text, position, layer="PostProcessing", angle=0, font_size=12):
         """Create a text primitive object.
 
         Parameters
         ----------
         text : str
             Name for the text primitive object.
         position : list
             Position of the text.
-        placement_layer : str, optional
+        layer : str, optional
             Layer where text will be placed. The default value is ``"PostProcessing"``.
         angle : float, optional
             Angle of the text. The default value is ``0``.
         font_size : int, optional
             Font size. The default value is ``12``.
 
         Returns
@@ -1561,15 +1521,15 @@
         args = [
             "NAME:Contents",
             "textGeometry:=",
             [
                 "Name:=",
                 name,
                 "LayerName:=",
-                placement_layer,
+                layer,
                 "x:=",
                 position[0],
                 "y:=",
                 position[1],
                 "ang:=",
                 angle,
                 "isPlot:=",
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/pcb/object3dlayout.py` & `pyaedt-0.8.9/pyaedt/modeler/pcb/object3dlayout.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,70 +36,70 @@
 
         Returns
         -------
         str
         """
         return self._primitives.model_units
 
-    @pyaedt_function_handler()
-    def change_property(self, property_val, names_list=None):
+    @pyaedt_function_handler(property_val="value", names_list="names")
+    def change_property(self, value, names=None):
         """Modify a property.
 
         Parameters
         ----------
-        property_val : list
+        value : list
 
-        names_list : list, optional
+        names : list, optional
              The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        vChangedProps = ["NAME:ChangedProps", property_val]
-        if names_list:  # pragma: no cover
+        vChangedProps = ["NAME:ChangedProps", value]
+        if names:  # pragma: no cover
             vPropServers = ["NAME:PropServers"]
-            for el in names_list:
+            for el in names:
                 vPropServers.append(el)
         else:
             vPropServers = ["NAME:PropServers", self.name]
         vGeo3dlayout = ["NAME:BaseElementTab", vPropServers, vChangedProps]
         vOut = ["NAME:AllTabs", vGeo3dlayout]
 
         self._oeditor.ChangeProperty(vOut)
         return True
 
-    @pyaedt_function_handler()
-    def set_property_value(self, property_name, property_value):
+    @pyaedt_function_handler(property_name="name", property_value="value")
+    def set_property_value(self, name, value):
         """Set a property value.
 
         Parameters
         ----------
-        property_name : str
+        name : str
             Name of the property.
-        property_value :
+        value :
             Value of the property.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
-        vProp = ["NAME:" + property_name, "Value:=", property_value]
+        vProp = ["NAME:" + name, "Value:=", value]
         return self.change_property(vProp)
 
     @property
     def angle(self):
         """Get/Set the circle radius.
 
         Returns
@@ -1040,34 +1040,34 @@
         -------
         int
             Edge number.
         """
         result = [(edge[0][1] + edge[1][1]) for edge in self.edges]
         return result.index(max(result))
 
-    @pyaedt_function_handler()
-    def get_property_value(self, propertyname):
+    @pyaedt_function_handler(propertyname="name")
+    def get_property_value(self, name):
         """Retrieve a property value.
 
         Parameters
         ----------
-        propertyname : str
+        name : str
             Name of the property
 
         Returns
         -------
         type
             Value of the property.
 
         References
         ----------
 
         >>> oEditor.GetPropertyValue
         """
-        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, propertyname)
+        return self._oeditor.GetPropertyValue("BaseElementTab", self.name, name)
 
     @property
     def negative(self):
         """Get/Set the negative.
 
         Parameters
         ----------
@@ -1527,32 +1527,25 @@
         """Add a new point to the center line.
 
         Parameters
         ----------
         point : list
             [x,y] coordinate point to add.
         position : int, optional
-            Position of the new point.
+            Position of the new point in the geometry.
 
         Returns
         -------
         :class:`pyaedt.modeler.pcb.object3dlayout.Line3dLayout`
         """
         points = [
             [self._primitives.number_with_units(j, self.object_units) for j in i] for i in (self.center_line.values())
         ]
         points.insert(position, [self._primitives.number_with_units(j, self.object_units) for j in point])
-        line = self._primitives.create_line(
-            self.placement_layer,
-            points,
-            lw=self.width,
-            start_style=self.start_cap_type,
-            end_style=self.end_cap_type,
-            net_name=self.net_name,
-        )
+        line = self._primitives.create_line(self.placement_layer, points)
         line_name = self.name
         self._primitives.oeditor.Delete([self.name])
         line.name = line_name
         self._primitives._lines[self.name] = line
         return line
 
     @pyaedt_function_handler()
@@ -1572,22 +1565,15 @@
         if isinstance(point, str):
             point = [point]
         points = [
             [self._primitives.number_with_units(j, self.object_units) for j in v]
             for i, v in self.center_line.items()
             if i not in point
         ]
-        line = self._primitives.create_line(
-            self.placement_layer,
-            points,
-            lw=self.width,
-            start_style=self.start_cap_type,
-            end_style=self.end_cap_type,
-            net_name=self.net_name,
-        )
+        line = self._primitives.create_line(self.placement_layer, points)
         line_name = self.name
         self._primitives.oeditor.Delete([self.name])
         line.name = line_name
         self._primitives._lines[self.name] = line
         return line
 
     @pyaedt_function_handler()
@@ -1649,30 +1635,30 @@
         List
         """
         if self.is_arc:
             return [self.point.GetX()]
         else:
             return [self.point.GetX(), self.point.GetY()]
 
-    @pyaedt_function_handler()
-    def move(self, new_position):
+    @pyaedt_function_handler(new_position="location")
+    def move(self, location):
         """Move actual point to new location.
 
         Parameters
         ----------
-        new_position : List
+        location : List
             New point location.
 
         Returns
         -------
         bool
             ``True`` if the point was moved to the new location.
 
         """
-        if self.point.Move(self._primitives.oeditor.Point().Set(new_position[0], new_position[1])):
+        if self.point.Move(self._primitives.oeditor.Point().Set(location[0], location[1])):
             return True
 
 
 class ComponentsSubCircuit3DLayout(Object3DLayout, object):
     """Contains 3d Components in HFSS 3D Layout.
 
     Parameters
@@ -2065,31 +2051,31 @@
         arg2.append("sbn:=")
         arg2.append(self.solder_mat)
         arg.append(arg2)
         arg.append("ppl:=")
         arg.append([])
         return arg
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(layername="layer")
     def add_layer(
         self,
-        layername="Start",
+        layer="Start",
         pad_hole=None,
         antipad_hole=None,
         thermal_hole=None,
         connx=0,
         conny=0,
         conndir=0,
         layer_id=None,
     ):
         """Create a layer in the padstack.
 
         Parameters
         ----------
-        layername : str, optional
+        layer : str, optional
             Name of layer. The default is ``"Start"``.
         pad_hole : pyaedt.modeler.Object3d.Object3d.PDSHole
             Pad hole object, which you can create with the :func:`add_hole` method.
             The default is ``None``.
         antipad_hole :
             Antipad hole object, which you can create with the :func:`add_hole` method.
             The default is ``None``.
@@ -2105,37 +2091,36 @@
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        layer_id = None
-        if layername in self.layers:
+        if layer in self.layers:
             return False
         else:
             if not layer_id:
                 layer_id = len(list(self.layers.keys())) + 1
-            new_layer = self.PDSLayer(layername, layer_id)
+            new_layer = self.PDSLayer(layer, layer_id)
             new_layer.pad = pad_hole
             new_layer.antipad = antipad_hole
             new_layer.thermal = thermal_hole
             new_layer.connectionx = connx
             new_layer.connectiony = conny
             new_layer.connectiondir = conndir
-            self.layers[layername] = new_layer
+            self.layers[layer] = new_layer
             return True
 
-    @pyaedt_function_handler()
-    def add_hole(self, holetype="Cir", sizes=[1], xpos=0, ypos=0, rot=0):
+    @pyaedt_function_handler(holetype="hole_type", xpos="x", ypos="y", rot="rotation")
+    def add_hole(self, hole_type="Cir", sizes=None, x=0, y=0, rotation=0):
         """Add a hole.
 
         Parameters
         ----------
-        holetype : str, optional
+        hole_type : str, optional
             Type of the hole. Options are:
 
             * No" - no pad
             * "Cir" - Circle
             * "Sq" - Square
             * "Rct" - Rectangle
             * "Ov" - Oval
@@ -2146,34 +2131,36 @@
             * "S45" - Square 45 thermal
             * "S90" - Square 90 thermal
 
             The default is ``"Cir"``.
         sizes : array, optional
             Array of sizes, which depends on the object. For example, a circle ias an array
             of one element. The default is ``[1]``.
-        xpos :
+        x :
             Position on the X axis. The default is ``0``.
-        ypos :
+        y :
             Position on the Y axis. The default is ``0``.
-        rot : float, optional
+        rotation : float, optional
             Angle rotation in degrees. The default is ``0``.
 
         Returns
         -------
         :class:`pyaedt.modeler.Object3d.Object3d.PDSHole`
             Hole object to be passed to padstack or layer.
 
         """
+        if sizes is None:
+            sizes = [1]
         hole = self.PDSHole()
-        hole.shape = holetype
+        hole.shape = hole_type
         sizes = [_dim_arg(i, self.units) for i in sizes if type(i) is int or float]
         hole.sizes = sizes
-        hole.x = _dim_arg(xpos, self.units)
-        hole.y = _dim_arg(ypos, self.units)
-        hole.rot = _dim_arg(rot, "deg")
+        hole.x = _dim_arg(x, self.units)
+        hole.y = _dim_arg(y, self.units)
+        hole.rot = _dim_arg(rotation, "deg")
         return hole
 
     @pyaedt_function_handler()
     def create(self):
         """Create a padstack in AEDT.
 
         Returns
```

### Comparing `pyaedt-0.8.8/pyaedt/modeler/schematic.py` & `pyaedt-0.8.9/pyaedt/modeler/schematic.py`

 * *Files 8% similar despite different names*

```diff
@@ -86,28 +86,33 @@
         References
         ----------
 
         >>> oEditor.ZoomToFit
         """
         self.oeditor.ZoomToFit()
 
-    @pyaedt_function_handler()
-    def connect_schematic_components(self, firstcomponent, secondcomponent, pinnum_first=2, pinnum_second=1):
+    @pyaedt_function_handler(
+        firstcomponent="starting_component",
+        secondcomponent="ending_component",
+        pinnum_first="pin_starting",
+        pinnum_second="pin_ending",
+    )
+    def connect_schematic_components(self, starting_component, ending_component, pin_starting=2, pin_ending=1):
         """Connect schematic components.
 
         Parameters
         ----------
-        firstcomponent : str
+        starting_component : str
            Starting (right) component.
-        secondcomponent : str
+        ending_component : str
            Ending (left) component for the connection line.
-        pinnum_first : str, optional
+        pin_starting : str, optional
              Number of the pin at which to terminate the connection from the right end of the
              starting component. The default is ``2``.
-        pinnum_second : str, optional
+        pin_ending : str, optional
              Number of the pin at which to terminate the connection from the left end of the
              ending component. The default is ``1``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
@@ -115,42 +120,42 @@
         References
         ----------
 
         >>> oEditor.CreateWire
         """
         if self._app.design_type == "Maxwell Circuit":
             components = self.schematic.components
-            obj1 = components[firstcomponent]
+            obj1 = components[starting_component]
         else:
             components = self.components
-            obj1 = components[firstcomponent]
+            obj1 = components[starting_component]
         if "Port" in obj1.composed_name:
             pos1 = self.oeditor.GetPropertyValue("BaseElementTab", obj1.composed_name, "Component Location").split(", ")
             pos1 = [float(i.strip()[:-3]) * 0.0000254 for i in pos1]
             if "GPort" in obj1.composed_name:
                 pos1[1] += 0.00254
         else:
             if self._app.design_type == "Maxwell Circuit":
                 pos1 = [float(re.sub(r"[^0-9.\-]", "", x)) * 0.0000254 for x in obj1.location]
             else:
-                pins1 = components.get_pins(firstcomponent)
-                pos1 = components.get_pin_location(firstcomponent, pins1[pinnum_first - 1])
-        obj2 = components[secondcomponent]
+                pins1 = components.get_pins(starting_component)
+                pos1 = components.get_pin_location(starting_component, pins1[pin_starting - 1])
+        obj2 = components[ending_component]
         if "Port" in obj2.composed_name:
             pos2 = self.oeditor.GetPropertyValue("BaseElementTab", obj2.composed_name, "Component Location").split(", ")
             pos2 = [float(i.strip()[:-3]) * 0.0000254 for i in pos2]
             if "GPort" in obj2.composed_name:
                 pos2[1] += 0.00254
 
         else:
             if self._app.design_type == "Maxwell Circuit":
                 pos2 = [float(re.sub(r"[^0-9.\-]", "", x)) * 0.0000254 for x in obj2.location]
             else:
-                pins2 = components.get_pins(secondcomponent)
-                pos2 = components.get_pin_location(secondcomponent, pins2[pinnum_second - 1])
+                pins2 = components.get_pins(ending_component)
+                pos2 = components.get_pin_location(ending_component, pins2[pin_ending - 1])
         try:
             self.schematic.create_wire([pos1, pos2])
             return True
         except Exception:
             return False
 
     @pyaedt_function_handler()
@@ -322,110 +327,106 @@
                 )
                 self.change_text_property(str(text_id), "Rectangle BorderColor", [r3, g3, b3])
                 self.change_text_property(str(text_id), "Rectangle FillStyle", fill[rect_fill])
             return text_out
         except Exception:
             return False
 
-    @pyaedt_function_handler
-    def change_text_property(self, property_id, property_name, property_value):  # pragma: no cover
+    @pyaedt_function_handler(property_id="assignment", property_name="name", property_value="value")
+    def change_text_property(self, assignment, name, value):
         """Change an oeditor property.
 
         Parameters
         ----------
-        property_id : str
+        assignment : str
             Object id.
-        property_name : str
+        name : str
             Name of the property. For example, ``Text``.
-        property_value : str, list, int
+        value : str, list, int
             Value of the property. It can be a string, an int for a single value, a list of three elements for
             ``[r,g,b]`` color values or a list of two elements for ``[x, y]`` coordinates.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.ChangeProperty
         """
         graphics_id = [id.split("@")[1] for id in self.oeditor.GetAllGraphics()]
-        if property_id not in graphics_id:
+        if assignment not in graphics_id:
             self.logger.error("Invalid id.")
             return False
-        if isinstance(property_value, list) and len(property_value) == 3:
-            if (
-                not isinstance(property_value[0], int)
-                or not isinstance(property_value[1], int)
-                or not isinstance(property_value[2], int)
-            ):
+        if isinstance(value, list) and len(value) == 3:
+            if not isinstance(value[0], int) or not isinstance(value[1], int) or not isinstance(value[2], int):
                 self.logger.error("Invalid RGB values for color")
                 return False
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:BaseElementTab",
-                        ["NAME:PropServers", "SchObj@" + property_id],
+                        ["NAME:PropServers", "SchObj@" + assignment],
                         [
                             "NAME:ChangedProps",
                             [
-                                "NAME:" + property_name,
+                                "NAME:" + name,
                                 "R:=",
-                                property_value[0],
+                                value[0],
                                 "G:=",
-                                property_value[1],
+                                value[1],
                                 "B:=",
-                                property_value[2],
+                                value[2],
                             ],
                         ],
                     ],
                 ]
             )
-        elif isinstance(property_value, list) and len(property_value) == 2:
-            xpos = self._arg_with_dim(property_value[0])
-            ypos = self._arg_with_dim(property_value[1])
+        elif isinstance(value, list) and len(value) == 2:
+            xpos = self._arg_with_dim(value[0])
+            ypos = self._arg_with_dim(value[1])
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:BaseElementTab",
-                        ["NAME:PropServers", "SchObj@" + property_id],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "X:=", xpos, "Y:=", ypos]],
+                        ["NAME:PropServers", "SchObj@" + assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "X:=", xpos, "Y:=", ypos]],
                     ],
                 ]
             )
-        elif isinstance(property_value, bool):
+        elif isinstance(value, bool):
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:BaseElementTab",
-                        ["NAME:PropServers", "SchObj@" + property_id],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
+                        ["NAME:PropServers", "SchObj@" + assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "Value:=", value]],
                     ],
                 ]
             )
-        elif isinstance(property_value, (str, float, int)):
+        elif isinstance(value, (str, float, int)):
             self.oeditor.ChangeProperty(
                 [
                     "NAME:AllTabs",
                     [
                         "NAME:BaseElementTab",
-                        ["NAME:PropServers", "SchObj@" + property_id],
-                        ["NAME:ChangedProps", ["NAME:" + property_name, "Value:=", property_value]],
+                        ["NAME:PropServers", "SchObj@" + assignment],
+                        ["NAME:ChangedProps", ["NAME:" + name, "Value:=", value]],
                     ],
                 ]
             )
         else:
             self.logger.error("Wrong Property Value")
             return False
-        self.logger.debug("Property {} Changed correctly.".format(property_name))
+        self.logger.debug("Property {} Changed correctly.".format(name))
         return True
 
     @pyaedt_function_handler()
     def _get_components_selections(self, selections, return_as_list=True):
         sels = []
         if not isinstance(selections, list):
             selections = [selections]
@@ -563,47 +564,47 @@
 
     @model_units.setter
     def model_units(self, units):
         """Set the model units as a string e.g. "mm"."""
         assert units in AEDT_UNITS["Length"], "Invalid units string {0}".format(units)
         self.oeditor.SetActivelUnits(["NAME:Units Parameter", "Units:=", units, "Rescale:=", False])
 
-    @pyaedt_function_handler()
-    def move(self, selections, pos, units=None):
+    @pyaedt_function_handler(selections="assignment", pos="offset")
+    def move(self, assignment, offset, units=None):
         """Move the selections by the specified ``[x, y]`` coordinates.
 
         Parameters
         ----------
-        selections : list
+        assignment : list
             List of the selections.
-        pos : list
+        offset : list
             Offset for the ``[x, y]`` axis.
         units : str
             Units of the movement. The default is ``meter``. If ``None``, ``schematic_units`` are used.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Move
         """
-        sels = self._get_components_selections(selections)
+        sels = self._get_components_selections(assignment)
         if not sels:
             self.logger.error("No Component Found.")
             return False
         if units:
-            x_location = AEDT_UNITS["Length"][units] * float(pos[0])
-            y_location = AEDT_UNITS["Length"][units] * float(pos[1])
+            x_location = AEDT_UNITS["Length"][units] * float(offset[0])
+            y_location = AEDT_UNITS["Length"][units] * float(offset[1])
         else:
-            x_location = AEDT_UNITS["Length"][self.schematic_units] * float(pos[0])
-            y_location = AEDT_UNITS["Length"][self.schematic_units] * float(pos[1])
+            x_location = AEDT_UNITS["Length"][self.schematic_units] * float(offset[0])
+            y_location = AEDT_UNITS["Length"][self.schematic_units] * float(offset[1])
         self.oeditor.Move(
             ["NAME:Selections", "Selections:=", sels],
             [
                 "NAME:MoveParameters",
                 "xdelta:=",
                 x_location,
                 "ydelta:=",
@@ -612,36 +613,36 @@
                 False,
                 "Rubberband:=",
                 False,
             ],
         )
         return True
 
-    @pyaedt_function_handler()
-    def rotate(self, selections, degrees=90):
+    @pyaedt_function_handler(selections="assignment")
+    def rotate(self, assignment, degrees=90):
         """Rotate the selections by degrees.
 
         Parameters
         ----------
-        selections : list
+        assignment : list
             List of the selections.
         degrees : optional
             Angle rotation in degrees. The default is ``90``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oEditor.Rotate
         """
-        sels = self._get_components_selections(selections)
+        sels = self._get_components_selections(assignment)
         if not sels:
             self.logger.error("No Component Found.")
             return False
 
         self.oeditor.Rotate(
             ["NAME:Selections", "Selections:=", sels],
             [
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/AdvancedPostProcessing.py` & `pyaedt-0.8.9/pyaedt/modules/AdvancedPostProcessing.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/Boundary.py` & `pyaedt-0.8.9/pyaedt/modules/Boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,16 +346,16 @@
 
     Create a cylinder at the XY working plane and assign a copper coating of 0.2 mm to it. The Coating is a boundary
     operation and coat will return a ``pyaedt.modules.Boundary.BoundaryObject``
 
     >>> from pyaedt import Hfss
     >>> hfss =Hfss()
     >>> origin = hfss.modeler.Position(0, 0, 0)
-    >>> inner = hfss.modeler.create_cylinder(hfss.PLANE.XY, origin, 3, 200, 0, "inner")
-    >>> inner_id = hfss.modeler.get_obj_id("inner")
+    >>> inner = hfss.modeler.create_cylinder(hfss.PLANE.XY,origin,3,200,0,"inner")
+    >>> inner_id = hfss.modeler.get_obj_id("inner",)
     >>> coat = hfss.assign_coating([inner_id],"copper",use_thickness=True,thickness="0.2mm")
     """
 
     def __init__(self, app, name, props=None, boundarytype=None, auto_update=True):
         self.auto_update = False
         self._app = app
         self._name = name
@@ -871,16 +871,16 @@
     Examples
     --------
 
     Create a matrix in Maxwell3D return a ``pyaedt.modules.Boundary.BoundaryObject``
 
     >>> from pyaedt import Maxwell2d
     >>> maxwell_2d = Maxwell2d()
-    >>> coil1 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0], [8, 3], True, "Coil_1", "vacuum")
-    >>> coil2 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0], [8, 3], True, "Coil_2", "vacuum")
+    >>> coil1 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0],[8, 3],True,"Coil_1","vacuum")
+    >>> coil2 = maxwell_2d.modeler.create_rectangle([8.5,1.5, 0],[8, 3],True,"Coil_2","vacuum")
     >>> maxwell_2d.assign_matrix(["Coil_1", "Coil_2"])
     """
 
     def __init__(self, app, name, props=None, boundarytype=None):
         self.auto_update = False
         self._app = app
         self._name = name
@@ -3611,15 +3611,15 @@
                     new_list.append(page_net_list)
                 else:
                     new_list.append(self._clean_list(item))
             else:
                 new_list.append(item)
         return new_list
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def create(self):
         """
         Create network in AEDT.
 
         Returns
         -------
         bool:
@@ -3641,15 +3641,15 @@
 
         args = self._get_args()
 
         clean_args = self._clean_list(args)
         self._app.oboundary.AssignNetworkBoundary(clean_args)
         return True
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _update_from_props(self):
         nodes = self.props.get("Nodes", None)
         if nodes is not None:
             nd_name_list = [node.name for node in self._nodes]
             for node_name, node_dict in nodes.items():
                 if node_name not in nd_name_list:
                     nd_type = node_dict.get("NodeType", None)
@@ -4006,24 +4006,24 @@
     @pyaedt_function_handler()
     def _add_to_props(self, new_node, type_dict="Nodes"):
         try:
             self.props[type_dict].update({new_node.name: new_node.props})
         except KeyError:
             self.props[type_dict] = {new_node.name: new_node.props}
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(face_id="assignment")
     def add_face_node(
-        self, face_id, name=None, thermal_resistance="NoResistance", material=None, thickness=None, resistance=None
+        self, assignment, name=None, thermal_resistance="NoResistance", material=None, thickness=None, resistance=None
     ):
         """
         Create a face node in the network.
 
         Parameters
         ----------
-        face_id : int
+        assignment : int
             Face ID.
         name : str, optional
             Name of the node. Default is ``None``.
         thermal_resistance : str
             Thermal resistance value and unit. Default is ``"NoResistance"``.
         material : str, optional
             Material specification (required if ``thermal_resistance="Compute"``).
@@ -4042,23 +4042,23 @@
 
         Examples
         --------
 
         >>> import pyaedt
         >>> app = pyaedt.Icepak()
         >>> network = pyaedt.modules.Boundary.Network(app)
-        >>> box = app.modeler.create_box([5, 5, 5], [20, 50, 80])
+        >>> box = app.modeler.create_box([5, 5, 5],[20, 50, 80])
         >>> faces_ids = [face.id for face in box.faces]
         >>> network.add_face_node(faces_ids[0])
-        >>> network.add_face_node(faces_ids[1], name="TestNode", thermal_resistance="Compute",
-        >>>                       material="Al-Extruded", thickness="2mm")
-        >>> network.add_face_node(faces_ids[2], name="TestNode", thermal_resistance="Specified", resistance=2)
+        >>> network.add_face_node(faces_ids[1],name="TestNode",thermal_resistance="Compute",
+        ...                       material="Al-Extruded",thickness="2mm")
+        >>> network.add_face_node(faces_ids[2],name="TestNode",thermal_resistance="Specified",resistance=2)
         """
         props_dict = OrderedDict({})
-        props_dict["FaceID"] = face_id
+        props_dict["FaceID"] = assignment
         if thermal_resistance is not None:
             if thermal_resistance == "Compute":
                 if resistance is not None:
                     self._app.logger.info(
                         '``resistance`` assignment is incompatible with ``thermal_resistance="Compute"``'
                         "and it is ignored."
                     )
@@ -4086,28 +4086,28 @@
                     props_dict["Resistance"] = resistance
                 else:  # pragma : no cover
                     raise AttributeError(
                         'If ``thermal_resistance="Specified"``, ``resistance`` argument must be prescribed.'
                     )
 
         if name is None:
-            name = "FaceID" + str(face_id)
+            name = "FaceID" + str(assignment)
         new_node = self._Node(name, self._app, node_type="FaceNode", props=props_dict, network=self)
         self._nodes.append(new_node)
         self._add_to_props(new_node)
         return new_node
 
-    @pyaedt_function_handler()
-    def add_nodes_from_dictionaries(self, nodes_dict):
+    @pyaedt_function_handler(nodes_dict="nodes")
+    def add_nodes_from_dictionaries(self, nodes):
         """
         Add nodes to the network from dictionary.
 
         Parameters
         ----------
-        nodes_dict : list or dict
+        nodes : list or dict
             A dictionary or list of dictionaries containing nodes to add to the network. Different
             node types require different key and value pairs:
 
             - Face nodes must contain the ``"ID"`` key associated with an integer containing the face ID.
               Optional keys and values pairs are:
 
               - ``"ThermalResistance"``: a string specifying the type of thermal resistance.
@@ -4162,31 +4162,31 @@
 
         Examples
         --------
 
         >>> import pyaedt
         >>> app = pyaedt.Icepak()
         >>> network = pyaedt.modules.Boundary.Network(app)
-        >>> box = app.modeler.create_box([5, 5, 5], [20, 50, 80])
+        >>> box = app.modeler.create_box([5, 5, 5],[20, 50, 80])
         >>> faces_ids = [face.id for face in box.faces]
         >>> nodes_dict = [
         >>>         {"FaceID": faces_ids[0]},
         >>>         {"Name": "TestNode", "FaceID": faces_ids[1],
         >>>          "ThermalResistance": "Compute", "Thickness": "2mm"},
         >>>         {"FaceID": faces_ids[2], "ThermalResistance": "Specified", "Resistance": "2cel_per_w"},
         >>>         {"Name": "Junction", "Power": "1W"}]
         >>> network.add_nodes_from_dictionaries(nodes_dict)
 
         """
-        if isinstance(nodes_dict, dict):
-            nodes_dict = [nodes_dict]
-        for node_dict in nodes_dict:
+        if isinstance(nodes, dict):
+            nodes = [nodes]
+        for node_dict in nodes:
             if "FaceID" in node_dict.keys():
                 self.add_face_node(
-                    face_id=node_dict["FaceID"],
+                    assignment=node_dict["FaceID"],
                     name=node_dict.get("Name", None),
                     thermal_resistance=node_dict.get("ThermalResistance", None),
                     material=node_dict.get("Material", None),
                     thickness=node_dict.get("Thickness", None),
                     resistance=node_dict.get("Resistance", None),
                 )
             elif "ValueType" in node_dict.keys():
@@ -4232,15 +4232,15 @@
 
         Examples
         --------
 
         >>> import pyaedt
         >>> app = pyaedt.Icepak()
         >>> network = pyaedt.modules.Boundary.Network(app)
-        >>> box = app.modeler.create_box([5, 5, 5], [20, 50, 80])
+        >>> box = app.modeler.create_box([5, 5, 5],[20, 50, 80])
         >>> faces_ids = [face.id for face in box.faces]
         >>> connection = {"Name": "LinkTest", "Connection": [faces_ids[1], faces_ids[0]], "Value": "1cel_per_w"}
         >>> network.add_links_from_dictionaries(connection)
 
         """
         if name is None:
             new_name = True
@@ -4277,15 +4277,15 @@
 
         Examples
         --------
 
         >>> import pyaedt
         >>> app = pyaedt.Icepak()
         >>> network = pyaedt.modules.Boundary.Network(app)
-        >>> box = app.modeler.create_box([5, 5, 5], [20, 50, 80])
+        >>> box = app.modeler.create_box([5, 5, 5],[20, 50, 80])
         >>> faces_ids = [face.id for face in box.faces]
         >>> [network.add_face_node(faces_ids[i]) for i in range(2)]
         >>> connection = {"Name": "LinkTest", "Link": [faces_ids[1], faces_ids[0], "1cel_per_w"]}
         >>> network.add_links_from_dictionaries(connection)
 
         """
         if isinstance(connections, dict):
@@ -4380,15 +4380,15 @@
             list
                 First two elements of the list are the node names that the link connects,
                 the third element is the link type while the fourth contains the value
                 associated with the link.
             """
             return [self.node_1, self.node_2] + self._link_type + [self.value]
 
-        @pyaedt_function_handler
+        @pyaedt_function_handler()
         def delete_link(self):
             """
             Delete link from network.
             """
             self._network.props["Links"].pop(self.name)
             self._network._links.remove(self)
 
@@ -4397,15 +4397,15 @@
             self.name = name
             self._type = node_type
             self._app = app
             self._props = props
             self._node_props()
             self._network = network
 
-        @pyaedt_function_handler
+        @pyaedt_function_handler()
         def delete_node(self):
             """
             Delete node from network.
             """
             self._network.props["Nodes"].pop(self.name)
             self._network._nodes.remove(self)
 
@@ -4566,15 +4566,15 @@
             "Values": self._parse_value(),
         }
 
     @abstractmethod
     def _parse_value(self):
         pass  # pragma : no cover
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def __getitem__(self, k):
         return self.props.get(k)
 
 
 class LinearDictionary(BoundaryDictionary):
     """
     Manages linear conditions assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4593,15 +4593,15 @@
     """
 
     def __init__(self, intercept, slope):
         super().__init__("Transient", "Linear")
         self.intercept = intercept
         self.slope = slope
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.slope, self.intercept]
 
 
 class PowerLawDictionary(BoundaryDictionary):
     """
     Manages power law condition assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4624,15 +4624,15 @@
 
     def __init__(self, intercept, coefficient, scaling_exponent):
         super().__init__("Transient", "Power Law")
         self.intercept = intercept
         self.coefficient = coefficient
         self.scaling_exponent = scaling_exponent
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.intercept, self.coefficient, self.scaling_exponent]
 
 
 class ExponentialDictionary(BoundaryDictionary):
     """
     Manages exponential condition assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4655,15 +4655,15 @@
 
     def __init__(self, vertical_offset, coefficient, exponent_coefficient):
         super().__init__("Transient", "Exponential")
         self.vertical_offset = vertical_offset
         self.coefficient = coefficient
         self.exponent_coefficient = exponent_coefficient
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.vertical_offset, self.coefficient, self.exponent_coefficient]
 
 
 class SinusoidalDictionary(BoundaryDictionary):
     """
     Manages sinusoidal condition assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4690,15 +4690,15 @@
     def __init__(self, vertical_offset, vertical_scaling, period, period_offset):
         super().__init__("Transient", "Sinusoidal")
         self.vertical_offset = vertical_offset
         self.vertical_scaling = vertical_scaling
         self.period = period
         self.period_offset = period_offset
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.vertical_offset, self.vertical_scaling, self.period, self.period_offset]
 
 
 class SquareWaveDictionary(BoundaryDictionary):
     """
     Manages square wave condition assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4721,15 +4721,15 @@
         super().__init__("Transient", "Square Wave")
         self.on_value = on_value
         self.initial_time_off = initial_time_off
         self.on_time = on_time
         self.off_time = off_time
         self.off_value = off_value
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.on_value, self.initial_time_off, self.on_time, self.off_time, self.off_value]
 
 
 class PieceWiseLinearDictionary(BoundaryDictionary):
     """
     Manages dataset condition assignments, which are children of the ``BoundaryDictionary`` class.
@@ -4747,14 +4747,14 @@
 
     def __init__(self, assignment_type, ds, scale):
         super().__init__(assignment_type, "Piecewise Linear")
         self.scale = scale
         self._assignment_type = assignment_type
         self.dataset = ds
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler()
     def _parse_value(self):
         return [self.scale, self.dataset.name]
 
     @property
     def dataset_name(self):
         return self.dataset.name
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/CableModeling.py` & `pyaedt-0.8.9/pyaedt/modules/CableModeling.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/CircuitTemplates.py` & `pyaedt-0.8.9/pyaedt/modules/CircuitTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/DesignXPloration.py` & `pyaedt-0.8.9/pyaedt/modules/DesignXPloration.py`

 * *Files 2% similar despite different names*

```diff
@@ -500,37 +500,37 @@
         elif self.soltype == "OptiParametric":
             self._app.activate_variable_tuning(variable_name)
         elif self.soltype == "OptiSensitivity":
             self._app.activate_variable_sensitivity(variable_name)
         elif self.soltype == "OptiStatistical":
             self._app.activate_variable_statistical(variable_name)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(num_cores="cores", num_tasks="tasks", num_gpu="gpus")
     def analyze(
         self,
-        num_cores=1,
-        num_tasks=1,
-        num_gpu=0,
+        cores=1,
+        tasks=1,
+        gpus=0,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
         revert_to_initial_mesh=False,
     ):
         """Solve the active design.
 
         Parameters
         ----------
-        num_cores : int, optional
-            Number of simulation cores. Default is ``1``.
-        num_tasks : int, optional
-            Number of simulation tasks. Default is ``1``.
-        num_gpu : int, optional
-            Number of simulation graphic processing units to use. Default is ``0``.
+        cores : int, optional
+            Number of simulation cores. The default is ``1``.
+        tasks : int, optional
+            Number of simulation tasks. The default is ``1``.
+        gpus : int, optional
+            Number of simulation graphic processing units to use. The default is ``0``.
         acf_file : str, optional
             Full path to the custom ACF file.
         use_auto_settings : bool, optional
             Set ``True`` to use automatic settings for HPC. The option is only considered for setups
             that support automatic settings.
         solve_in_batch : bool, optional
             Whether to solve the project in batch or not.
@@ -550,18 +550,18 @@
 
         References
         ----------
 
         >>> oDesign.Analyze
         """
         return self._app.analyze(
-            setup_name=self.name,
-            num_cores=num_cores,
-            num_tasks=num_tasks,
-            num_gpu=num_gpu,
+            name=self.name,
+            cores=cores,
+            tasks=tasks,
+            gpus=gpus,
             acf_file=acf_file,
             use_auto_settings=use_auto_settings,
             solve_in_batch=solve_in_batch,
             machine=machine,
             run_in_thread=run_in_thread,
             revert_to_initial_mesh=revert_to_initial_mesh,
         )
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/LayerStackup.py` & `pyaedt-0.8.9/pyaedt/modules/LayerStackup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1381,25 +1381,25 @@
                     o._user = True
                     o._SRMdl = infosdict["SideRoughness0 Type"]
                     o._SNR = infosdict["SideRoughness0"].split(", ")[0]
                     o._SHRatio = decompose_variable_value(infosdict["SideRoughness0"].split(", ")[1])[0]
             layers[o.id] = o
         return layers
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(layername="layer", layertype="layer_type")
     def add_layer(
-        self, layername, layertype="signal", thickness="0mm", elevation="0mm", material="copper", isnegative=False
+        self, layer, layer_type="signal", thickness="0mm", elevation="0mm", material="copper", isnegative=False
     ):
         """Add a layer.
 
         Parameters
         ----------
-        layername : str
+        layer : str
             Name of the layer.
-        layertype : str, optional
+        layer_type : str, optional
             Type of the layer. The default is ``"signal"``.
         thickness : str, optional
             Thickness with units. The default is ``"0mm"``.
         elevation : str, optional
             Elevation with units. The default is ``"0mm"``.
         material : str, optional
             Name of the material. The default is ``"copper"``.
@@ -1407,16 +1407,16 @@
             If ``True``, the geometry on the layer is cut away from the layer. The default is ``False``.
 
         Returns
         -------
         :class:`pyaedt.modules.LayerStackup.Layer`
             Layer object.
         """
-        newlayer = Layer(self, layertype, isnegative)
-        newlayer.name = layername
+        newlayer = Layer(self, layer_type, isnegative)
+        newlayer.name = layer
         newlayer._thickness = thickness
 
         if elevation == "0mm":
             el = (
                 0
                 if list(self.layers.values())[0].type not in ["dielectric", "signal", "via"]
                 else "{}{}".format(
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/Material.py` & `pyaedt-0.8.9/pyaedt/modules/Material.py`

 * *Files 3% similar despite different names*

```diff
@@ -606,21 +606,21 @@
         >>> hfss = Hfss(specified_version="2021.2")
         >>> mat1 = hfss.materials.add_material("new_copper2")
         >>> mat1.add_thermal_modifier_free_form("if(Temp > 1000cel, 1, if(Temp < -273.15cel, 1, 1))")
         """
         self._property_value[index].thermalmodifier = formula
         return self._add_thermal_modifier(formula, index)
 
-    @pyaedt_function_handler()
-    def add_thermal_modifier_dataset(self, dataset_name, index=0):
+    @pyaedt_function_handler(dataset_name="dataset")
+    def add_thermal_modifier_dataset(self, dataset, index=0):
         """Add a thermal modifier to a material property using an existing dataset.
 
         Parameters
         ----------
-        dataset_name : str
+        dataset : str
             Name of the project dataset.
         index : int, optional
             Value for the index. The default is ``0``.
 
         Returns
         -------
         bool
@@ -637,15 +637,15 @@
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss(specified_version="2021.2")
         >>> mat1 = hfss.materials.add_material("new_copper2")
         >>> mat1.add_thermal_modifier_dataset("$ds1")
         """
 
-        formula = "pwl({}, Temp)".format(dataset_name)
+        formula = "pwl({}, Temp)".format(dataset)
         self._property_value[index].thermalmodifier = formula
         return self._add_thermal_modifier(formula, index)
 
     @pyaedt_function_handler()
     def add_thermal_modifier_closed_form(
         self, tref=22, c1=0.0001, c2=1e-6, tl=-273.15, tu=1000, units="cel", auto_calc=True, tml=1000, tmu=1000, index=0
     ):
@@ -1053,21 +1053,21 @@
         >>> hfss = Hfss(specified_version="2021.2")
         >>> mat1 = hfss.materials.add_material("new_copper2")
         >>> mat1.add_spatial_modifier_free_form("if(X > 1mm, 1, if(X < 1mm, 2, 1))")
         """
         self._property_value[index].spatialmodifier = formula
         return self._add_spatial_modifier(formula, index)
 
-    @pyaedt_function_handler()
-    def add_spatial_modifier_dataset(self, dataset_name, index=0):
+    @pyaedt_function_handler(dataset_name="dataset")
+    def add_spatial_modifier_dataset(self, dataset, index=0):
         """Add a spatial modifier to a material property using an existing dataset.
 
         Parameters
         ----------
-        dataset_name : str
+        dataset : str
             Name of the project dataset.
         index : int, optional
             Value for the index. The default is ``0``.
 
         Returns
         -------
         bool
@@ -1084,15 +1084,15 @@
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss(specified_version="2021.2")
         >>> mat1 = hfss.materials.add_material("new_copper2")
         >>> mat1.add_spatial_modifier_dataset("$ds1")
         """
 
-        formula = "clp({}, X,Y,Z)".format(dataset_name)
+        formula = "clp({}, X,Y,Z)".format(dataset)
         self._property_value[index].spatialmodifier = formula
         return self._add_spatial_modifier(formula, index)
 
 
 class CommonMaterial(object):
     """Manages datasets with frequency-dependent materials.
 
@@ -2022,28 +2022,28 @@
                 "DirComp1": str(x),
                 "DirComp2": str(y),
                 "DirComp3": str(z),
             }
         )
         return self.update()
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(points_list_at_freq="points_at_frequency")
     def get_core_loss_coefficients(
         self,
-        points_list_at_freq,
+        points_at_frequency,
         core_loss_model_type="Electrical Steel",
         thickness="0.5mm",
         conductivity=0,
         coefficient_setup="w_per_cubic_meter",
     ):
         """Get electrical steel or power ferrite core loss coefficients at a given frequency.
 
         Parameters
         ----------
-        points_list_at_freq : dict
+        points_at_frequency : dict
             Dictionary where keys are the frequencies (in Hz) and values are lists of points (BP curve).
             If the core loss model is calculated at one frequency, this parameter must be provided as a
             dictionary with one key (single frequency in Hz) and values are lists of points at
             that specific frequency (BP curve).
         core_loss_model_type : str, optional
             Core loss model type. The default value is ``"Electrical Steel"``.
             Options are ``"Electrical Steel"`` and ``"Power Ferrite"``.
@@ -2068,102 +2068,101 @@
 
         Examples
         --------
         This example shows how to get core loss coefficients for Electrical Steel core loss model.
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> box = m3d.modeler.create_box([-10, -10, 0], [20, 20, 20], "box_to_split")
+        >>> box = m3d.modeler.create_box([-10, -10, 0],[20, 20, 20],"box_to_split")
         >>> box.material = "magnesium"
         >>> coefficients = m3d.materials["magnesium"].get_core_loss_coefficients(
-        ...                                                        points_list_at_freq={60 : [[0, 0], [1, 3], [2, 7]]},
-        ...                                                        thickness="0.5mm",
-        ...                                                        conductivity=0)
+        ...                                                         points_at_frequency={60 : [[0, 0], [1, 3], [2, 7]]},
+        ...                                                         thickness="0.5mm",conductivity=0)
         >>> print(coefficients)
         >>> m3d.release_desktop(True, True)
         """
-        if not isinstance(points_list_at_freq, dict):
+        if not isinstance(points_at_frequency, dict):
             raise TypeError("Points list at frequency must be provided as a dictionary.")
         if not isinstance(thickness, str):
             raise TypeError("Thickness must be provided as a string with value and unit.")
         else:
             value, unit = decompose_variable_value(thickness)
             if not is_number(value) and not unit:
                 raise TypeError("Thickness must be provided as a string with value and unit.")
-        if len(points_list_at_freq) <= 1 and core_loss_model_type == "Power Ferrite":
+        if len(points_at_frequency) <= 1 and core_loss_model_type == "Power Ferrite":
             raise ValueError("At least 2 frequencies must be included.")
         props = OrderedDict({})
-        freq_keys = list(points_list_at_freq.keys())
+        freq_keys = list(points_at_frequency.keys())
         for i in range(0, len(freq_keys)):
             if isinstance(freq_keys[i], str):
                 value, unit = decompose_variable_value(freq_keys[i])
                 if unit != "Hz":
                     value = unit_converter(values=value, unit_system="Freq", input_units=unit, output_units="Hz")
-                points_list_at_freq[value] = points_list_at_freq[freq_keys[i]]
-                del points_list_at_freq[freq_keys[i]]
+                points_at_frequency[value] = points_at_frequency[freq_keys[i]]
+                del points_at_frequency[freq_keys[i]]
 
-        if len(points_list_at_freq) == 1:
+        if len(points_at_frequency) == 1:
             props["CoefficientSetupData"] = OrderedDict({})
             props["CoefficientSetupData"]["property_data"] = "coreloss_data"
             props["CoefficientSetupData"]["coefficient_setup"] = coefficient_setup
-            frequency = list(points_list_at_freq.keys())[0]
+            frequency = list(points_at_frequency.keys())[0]
             props["CoefficientSetupData"]["Frequency"] = "{}Hz".format(frequency)
             props["CoefficientSetupData"]["Thickness"] = thickness
             props["CoefficientSetupData"]["Conductivity"] = str(conductivity)
-            points = [i for p in points_list_at_freq[frequency] for i in p]
+            points = [i for p in points_at_frequency[frequency] for i in p]
             props["CoefficientSetupData"]["Coordinates"] = OrderedDict({"DimUnits": ["", ""], "Points": points})
-        elif len(points_list_at_freq) > 1:
+        elif len(points_at_frequency) > 1:
             props["CoreLossMultiCurveData"] = OrderedDict({})
             props["CoreLossMultiCurveData"]["property_data"] = "coreloss_multi_curve_data"
             props["CoreLossMultiCurveData"]["coreloss_unit"] = coefficient_setup
 
             props["CoreLossMultiCurveData"]["AllCurves"] = OrderedDict({})
             props["CoreLossMultiCurveData"]["AllCurves"]["OneCurve"] = []
-            for freq in points_list_at_freq.keys():
-                points = [i for p in points_list_at_freq[freq] for i in p]
+            for freq in points_at_frequency.keys():
+                points = [i for p in points_at_frequency[freq] for i in p]
                 one_curve = OrderedDict(
                     {
                         "Frequency": "{}Hz".format(freq),
                         "Coordinates": OrderedDict({"DimUnits": ["", ""], "Points": points}),
                     }
                 )
                 props["CoreLossMultiCurveData"]["AllCurves"]["OneCurve"].append(one_curve)
 
         props = self._get_args(props)
         props.pop(0)
-        if len(points_list_at_freq) == 1:
+        if len(points_at_frequency) == 1:
             props[0][-1][2] = "NAME:Points"
             points = props[0][-1].pop(2)
             props[0][-1][2].insert(0, points)
         else:
             for p in props[0][-1]:
                 if isinstance(p, list):
                     p[3].pop(2)
                     p[3][2].insert(0, "NAME:Points")
         coefficients = self.odefinition_manager.ComputeCoreLossCoefficients(
             core_loss_model_type, self.mass_density.evaluated_value, props[0]
         )
         return list(coefficients)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(points_list_at_freq="points_at_frequency")
     def set_coreloss_at_frequency(
         self,
-        points_list_at_freq,
+        points_at_frequency,
         kdc=0,
         cut_depth="1mm",
         thickness="0.5mm",
         conductivity=0,
         coefficient_setup="w_per_cubic_meter",
         core_loss_model_type="Electrical Steel",
     ):
         """Set electrical steel or power ferrite core loss model at one single frequency or at multiple frequencies.
 
         Parameters
         ----------
-        points_list_at_freq : dict
+        points_at_frequency : dict
             Dictionary where keys are the frequencies (in Hz) and values are lists of points (BP curve).
             If the core loss model is calculated at one frequency, this parameter must be provided as a
             dictionary with one key (single frequency in Hz) and values are lists of points at
             that specific frequency (BP curve).
         kdc : float
             Coefficient considering the DC flux bias effects
         cut_depth : str, optional
@@ -2198,90 +2197,90 @@
         --------
         This example shows how to set a core loss model for a material in case material properties are calculated for
         core losses at one frequency or core losses versus frequencies (core losses multicurve data).
         The first case shows how to set properties for core losses at one frequency:
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> box = m3d.modeler.create_box([-10, -10, 0], [20, 20, 20], "box_to_split")
+        >>> box = m3d.modeler.create_box([-10, -10, 0],[20, 20, 20],"box_to_split")
         >>> box.material = "magnesium"
         >>> m3d.materials["magnesium"].set_coreloss_at_frequency(
-                                                    ... points_list_at_freq={60 : [[0,0], [1,3.5], [2,7.4]]}
+                                                    ... points_at_frequency={60 : [[0,0], [1,3.5], [2,7.4]]}
                                                     ... )
         >>> m3d.release_desktop(True, True)
 
         The second case shows how to set properties for core losses versus frequencies:
 
         >>> from pyaedt import Maxwell3d
         >>> m3d = Maxwell3d()
-        >>> box = m3d.modeler.create_box([-10, -10, 0], [20, 20, 20], "box_to_split")
+        >>> box = m3d.modeler.create_box([-10, -10, 0],[20, 20, 20],"box_to_split")
         >>> box.material = "magnesium"
         >>> m3d.materials["magnesium"].set_coreloss_at_frequency(
-                                                    ... points_list_at_freq={60 : [[0,0], [1,3.5], [2,7.4]],
+                                                    ... points_at_frequency={60 : [[0,0], [1,3.5], [2,7.4]],
                                                     ...                      100 : [[0,0], [1,8], [2,9]],
                                                     ...                      150 : [[0,0], [1,10], [2,19]]}
                                                     ... )
         >>> m3d.release_desktop(True, True)
 
         """
-        if not isinstance(points_list_at_freq, dict):
+        if not isinstance(points_at_frequency, dict):
             raise TypeError("Points list at frequency must be provided as a dictionary.")
-        if len(points_list_at_freq) <= 1 and core_loss_model_type == "Power Ferrite":
+        if len(points_at_frequency) <= 1 and core_loss_model_type == "Power Ferrite":
             raise ValueError("At least 2 frequencies must be included.")
-        freq_keys = list(points_list_at_freq.keys())
+        freq_keys = list(points_at_frequency.keys())
         for i in range(0, len(freq_keys)):
             if isinstance(freq_keys[i], str):
                 value, unit = decompose_variable_value(freq_keys[i])
                 if unit != "Hz":
                     value = unit_converter(values=value, unit_system="Freq", input_units=unit, output_units="Hz")
-                points_list_at_freq[value] = points_list_at_freq[freq_keys[i]]
-                del points_list_at_freq[freq_keys[i]]
+                points_at_frequency[value] = points_at_frequency[freq_keys[i]]
+                del points_at_frequency[freq_keys[i]]
         if "core_loss_type" not in self._props:
             choice = "Electrical Steel" if core_loss_model_type == "Electrical Steel" else "Power Ferrite"
             self._props["core_loss_type"] = OrderedDict({"property_type": "ChoiceProperty", "Choice": choice})
         else:
             self._props.pop("core_loss_cm", None)
             self._props.pop("core_loss_x", None)
             self._props.pop("core_loss_y", None)
             self._props.pop("core_loss_hci", None)
             self._props.pop("core_loss_br", None)
             self._props.pop("core_loss_hkc", None)
             self._props.pop("core_loss_curves", None)
             self._props["core_loss_type"]["Choice"] = core_loss_model_type
-        if len(points_list_at_freq) == 1:
+        if len(points_at_frequency) == 1:
             self._props["AttachedData"]["CoefficientSetupData"] = OrderedDict({})
             self._props["AttachedData"]["CoefficientSetupData"]["property_data"] = "coreloss_data"
             self._props["AttachedData"]["CoefficientSetupData"]["coefficient_setup"] = coefficient_setup
-            frequency = list(points_list_at_freq.keys())[0]
+            frequency = list(points_at_frequency.keys())[0]
             self._props["AttachedData"]["CoefficientSetupData"]["Frequency"] = "{}Hz".format(frequency)
             self._props["AttachedData"]["CoefficientSetupData"]["Thickness"] = thickness
             self._props["AttachedData"]["CoefficientSetupData"]["Conductivity"] = str(conductivity)
-            points = [i for p in points_list_at_freq[frequency] for i in p]
+            points = [i for p in points_at_frequency[frequency] for i in p]
             self._props["AttachedData"]["CoefficientSetupData"]["Coordinates"] = OrderedDict(
                 {"DimUnits": ["", ""], "Points": points}
             )
-        elif len(points_list_at_freq) > 1:
+        elif len(points_at_frequency) > 1:
             self._props["AttachedData"]["CoreLossMultiCurveData"] = OrderedDict({})
             self._props["AttachedData"]["CoreLossMultiCurveData"]["property_data"] = "coreloss_multi_curve_data"
             self._props["AttachedData"]["CoreLossMultiCurveData"]["coreloss_unit"] = coefficient_setup
 
             self._props["AttachedData"]["CoreLossMultiCurveData"]["AllCurves"] = OrderedDict({})
             self._props["AttachedData"]["CoreLossMultiCurveData"]["AllCurves"]["OneCurve"] = []
-            for freq in points_list_at_freq.keys():
-                points = [i for p in points_list_at_freq[freq] for i in p]
+            for freq in points_at_frequency.keys():
+                points = [i for p in points_at_frequency[freq] for i in p]
                 one_curve = OrderedDict(
                     {
                         "Frequency": "{}Hz".format(freq),
                         "Coordinates": OrderedDict({"DimUnits": ["", ""], "Points": points}),
                     }
                 )
                 self._props["AttachedData"]["CoreLossMultiCurveData"]["AllCurves"]["OneCurve"].append(one_curve)
 
         coefficients = self.get_core_loss_coefficients(
-            points_list_at_freq, thickness=thickness, conductivity=conductivity
+            points_at_frequency, thickness=thickness, conductivity=conductivity
         )
         if core_loss_model_type == "Electrical Steel":
             self._props["core_loss_kh"] = str(coefficients[0])
             self._props["core_loss_kc"] = str(coefficients[1])
             self._props["core_loss_ke"] = str(coefficients[2])
         else:
             self._props["core_loss_cm"] = str(coefficients[0])
@@ -2409,27 +2408,27 @@
         self._props["core_loss_cm"] = "{}A_per_meter".format(cm)
         self._props["core_loss_x"] = "{}tesla".format(x)
         self._props["core_loss_y"] = str(y)
         self._props["core_loss_kdc"] = str(kdc)
         self._props["core_loss_equiv_cut_depth"] = "{}meter".format(cut_depth)
         return self.update()
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(point_list="points", punit="units")
     def set_bp_curve_coreloss(
-        self, point_list, kdc=0, cut_depth=0.0001, punit="kw/m^3", bunit="tesla", frequency=60, thickness="0.5mm"
+        self, points, kdc=0, cut_depth=0.0001, units="kw/m^3", bunit="tesla", frequency=60, thickness="0.5mm"
     ):
         """Set B-P Type Core Loss.
 
         Parameters
         ----------
-        point_list : list of list
+        points : list of list
             List of [x,y] points.
         kdc : float
         cut_depth : float
-        punit : str
+        units : str
             Core loss unit. The default is ``"kw/m^3"``.
         bunit : str
             Magnetic field unit. The default is ``"tesla"``.
         frequency : float
         thickness : str, optional
             Lamination thickness. The default is ``"0.5mm"``.
 
@@ -2451,23 +2450,23 @@
             self._props.pop("core_loss_hkc", None)
             self._props.pop("core_loss_curves", None)
             self._props["core_loss_type"]["Choice"] = "B-P Curve"
         self._props["core_loss_kdc"] = str(kdc)
         self._props["core_loss_equiv_cut_depth"] = "{}meter".format(cut_depth)
         self._props["core_loss_curves"] = OrderedDict({})
         self._props["core_loss_curves"]["property_type"] = "nonlinear"
-        self._props["core_loss_curves"]["PUnit"] = punit
+        self._props["core_loss_curves"]["PUnit"] = units
         self._props["core_loss_curves"]["BUnit"] = bunit
         self._props["core_loss_curves"]["Frequency"] = "{}Hz".format(frequency)
         self._props["core_loss_curves"]["Thickness"] = thickness
         self._props["core_loss_curves"]["IsTemperatureDependent"] = False
 
         self._props["core_loss_curves"]["BPCoordinates"] = OrderedDict({})
         self._props["core_loss_curves"]["BPCoordinates"]["Point"] = []
-        for points in point_list:
+        for points in points:
             self._props["core_loss_curves"]["BPCoordinates"]["Point"].append(points)
         return self.update()
 
     @pyaedt_function_handler()
     def get_curve_coreloss_type(self):
         """Return the curve core loss type assigned to material.
 
@@ -2592,47 +2591,49 @@
         Returns
         -------
         bool
             ``True`` when the material is dielectric, ``False`` otherwise.
         """
         return not self.is_conductor(threshold)
 
-    @pyaedt_function_handler
+    @pyaedt_function_handler(i_freq="frequency")
     def set_djordjevic_sarkar_model(
         self,
         dk=4,
         df=0.02,
-        i_freq=1e9,
+        frequency=1e9,
         sigma_dc=1e-12,
         freq_hi=159.15494e9,
     ):
         """Set Djordjevic-Sarkar model.
 
         Parameters
         ----------
         dk : int, float, str, optional
             Dielectric constant at input frequency.
         df : int, float, str, optional
             Loss tangent at input frequency.
-        i_freq : int, float, optional.
+        frequency : int, float, optional.
             Input frequency in Hz.
         sigma_dc : int, float, optional
             Conductivity at DC. The default is ``1e-12``.
         freq_hi : int, float, optional
             High-frequency corner in Hz. The default is ``159.15494e9``.
 
         Returns
         -------
         bool
             ``True`` if successful, ``False`` otherwise.
         """
 
         # K = f"({dk} * {df} - {sigma_dc} / (2 * pi * {i_freq} * e0)) / atan({freq_hi} / {i_freq})"
-        K = "({} * {} - {} / (2 * pi * {} * e0)) / atan({} / {})".format(dk, df, sigma_dc, i_freq, freq_hi, i_freq)
-        epsilon_inf = "({} - {} / 2 * ln({}**2 / {}**2 + 1))".format(dk, K, freq_hi, i_freq)
+        K = "({} * {} - {} / (2 * pi * {} * e0)) / atan({} / {})".format(
+            dk, df, sigma_dc, frequency, freq_hi, frequency
+        )
+        epsilon_inf = "({} - {} / 2 * ln({}**2 / {}**2 + 1))".format(dk, K, freq_hi, frequency)
         freq_low = "({} / exp(10 * {} * {} / ({})))".format(freq_hi, df, epsilon_inf, K)
         ds_er = "{} + {} / 2 * ln(({}**2 + Freq**2) / ({}**2 + Freq**2))".format(epsilon_inf, K, freq_hi, freq_low)
         cond = "{} + 2 * pi * Freq * e0 * ({}) * (atan(Freq / ({})) - atan(Freq / {}))".format(
             sigma_dc, K, freq_low, freq_hi
         )
         # ds_tande = "{} / (e0 * {} * 2 * pi * Freq)".format(cond, ds_er)
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/MaterialLib.py` & `pyaedt-0.8.9/pyaedt/modules/MaterialLib.py`

 * *Files 4% similar despite different names*

```diff
@@ -209,87 +209,87 @@
                     self._app.project_properties["AnsoftProject"]["Definitions"]["SurfaceMaterials"][ds],
                     material_update=False,
                 )
         except Exception:
             pass
         return mats
 
-    @pyaedt_function_handler()
-    def checkifmaterialexists(self, mat):
+    @pyaedt_function_handler(mat="material")
+    def checkifmaterialexists(self, material):
         """Check if a material exists in AEDT or PyAEDT Definitions.
 
         Parameters
         ----------
-        mat : str
+        material : str
             Name of the material. If the material exists and is not in the materials database,
             it is added to this database.
 
         Returns
         -------
         :class:`pyaedt.modules.Material.Material`
             Material object if present, ``False`` when failed.
 
         References
         ----------
 
         >>> oDefinitionManager.GetProjectMaterialNames
         >>> oMaterialManager.GetData
         """
-        if isinstance(mat, Material):
-            if mat.name.lower() in self.material_keys:
-                return mat
+        if isinstance(material, Material):
+            if material.name.lower() in self.material_keys:
+                return material
             else:
                 return False
-        if mat.lower() in self.material_keys:
-            if mat.lower() in self.mat_names_aedt_lower:
-                return self.material_keys[mat.lower()]
-            if mat.lower() not in list(self.odefinition_manager.GetProjectMaterialNames()):
-                self.material_keys[mat.lower()].update()
-            return self.material_keys[mat.lower()]
-        elif mat.lower() in self.mat_names_aedt_lower:
-            return self._aedmattolibrary(mat)
+        if material.lower() in self.material_keys:
+            if material.lower() in self.mat_names_aedt_lower:
+                return self.material_keys[material.lower()]
+            if material.lower() not in list(self.odefinition_manager.GetProjectMaterialNames()):
+                self.material_keys[material.lower()].update()
+            return self.material_keys[material.lower()]
+        elif material.lower() in self.mat_names_aedt_lower:
+            return self._aedmattolibrary(material)
         elif settings.remote_api or settings.remote_rpc_session:
-            return self._aedmattolibrary(mat)
+            return self._aedmattolibrary(material)
         return False
 
-    @pyaedt_function_handler()
-    def check_thermal_modifier(self, mat):
+    @pyaedt_function_handler(mat="material")
+    def check_thermal_modifier(self, material):
         """Check a material to see if it has any thermal modifiers.
 
         Parameters
         ----------
-        mat : str
+        material : str
             Name of the material. All properties for this material are checked
             for thermal modifiers.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
-        omat = self.checkifmaterialexists(mat)
+        omat = self.checkifmaterialexists(material)
         if omat:
             for el in MatProperties.aedtname:
                 if omat.__dict__["_" + el].thermalmodifier:
                     return True
         return False
 
-    @pyaedt_function_handler()
-    def add_material(self, materialname, props=None):
+    @pyaedt_function_handler(materialname="name", props="properties")
+    def add_material(self, name, properties=None):
         """Add a material with default values.
 
         When the added material object is returned, you can customize
         the material. This method does not update the material.
 
         Parameters
         ----------
-        materialname : str
+        name : str
             Name of the material.
-        props : dict, optional
+        properties : dict, optional
             Material property dictionary. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Material.Material`
 
         References
@@ -305,41 +305,41 @@
         >>> mat = hfss.materials.add_material("MyMaterial")
         >>> print(mat.conductivity.value)
 
         >>> oDefinitionManager.GetProjectMaterialNames
         >>> oMaterialManager.GetData
 
         """
-        materialname = materialname
-        self.logger.info("Adding new material to the Project Library: " + materialname)
-        if materialname.lower() in self.material_keys:
+        name = name
+        self.logger.info("Adding new material to the Project Library: " + name)
+        if name.lower() in self.material_keys:
             self.logger.warning("Warning. The material is already in the database. Change or edit the name.")
-            return self.material_keys[materialname.lower()]
-        elif self._get_aedt_case_name(materialname):
-            return self._aedmattolibrary(self._get_aedt_case_name(materialname))
+            return self.material_keys[name.lower()]
+        elif self._get_aedt_case_name(name):
+            return self._aedmattolibrary(self._get_aedt_case_name(name))
         else:
-            material = Material(self, materialname, props, material_update=True)
+            material = Material(self, name, properties, material_update=True)
             material._update_material()
             if material:
                 self.logger.info("Material has been added. Edit it to update in Desktop.")
-                self.material_keys[materialname.lower()] = material
-                self._mats.append(materialname)
-                return self.material_keys[materialname.lower()]
+                self.material_keys[name.lower()] = material
+                self._mats.append(name)
+                return self.material_keys[name.lower()]
         return False
 
-    @pyaedt_function_handler()
-    def add_surface_material(self, material_name, emissivity=None):
+    @pyaedt_function_handler(material_name="name")
+    def add_surface_material(self, name, emissivity=None):
         """Add a surface material.
 
         In AEDT, base properties are loaded from the XML database file ``amat.xml``
         or from the emissivity.
 
         Parameters
         ----------
-        material_name : str
+        name : str
             Name of the surface material.
         emissivity : float, optional
             Emissivity value.
 
         Returns
         -------
         :class:`pyaedt.modules.SurfaceMaterial`
@@ -350,31 +350,31 @@
         >>> oDefinitionManager.AddSurfaceMaterial
 
         Examples
         --------
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> mat = hfss.materials.add_surface_material("Steel", 0.85)
+        >>> mat = hfss.materials.add_surface_material("Steel",0.85)
         >>> print(mat.emissivity.value)
 
         """
-        self.logger.info("Adding a surface material to the project library: " + material_name)
-        if material_name.lower() in self.surface_material_keys:
+        self.logger.info("Adding a surface material to the project library: " + name)
+        if name.lower() in self.surface_material_keys:
             self.logger.warning("Warning. The material is already in the database. Change the name or edit it.")
-            return self.surface_material_keys[material_name.lower()]
+            return self.surface_material_keys[name.lower()]
         else:
-            material = SurfaceMaterial(self._app, material_name, material_update=False)
+            material = SurfaceMaterial(self._app, name, material_update=False)
             if emissivity:
                 material.emissivity = emissivity
             material.update()
             material._material_update = True
             self.logger.info("Material has been added. Edit it to update in Desktop.")
-            self.surface_material_keys[material_name.lower()] = material
-            return self.surface_material_keys[material_name.lower()]
+            self.surface_material_keys[name.lower()] = material
+            return self.surface_material_keys[name.lower()]
 
     @pyaedt_function_handler()
     def _create_mat_project_vars(self, matlist):
         matprop = {}
         tol = 1e-12
         for prop in MatProperties.aedtname:
             matprop[prop] = []
@@ -388,23 +388,23 @@
                 a = sum(matprop[prop])
                 if a < tol:
                     del matprop[prop]
             except Exception:
                 pass
         return matprop
 
-    @pyaedt_function_handler()
-    def add_material_sweep(self, materials_list, material_name):
+    @pyaedt_function_handler(materials_list="assignment", material_name="name")
+    def add_material_sweep(self, assignment, name):
         """Create a sweep material made of an array of materials.
 
         Parameters
         ----------
-        materials_list : list
+        assignment : list
             List of materials to merge into a single sweep material.
-        material_name : str
+        name : str
             Name of the sweep material.
 
         Returns
         -------
         int
             Index of the project variable.
 
@@ -416,52 +416,52 @@
         Examples
         --------
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> hfss.materials.add_material("MyMaterial")
         >>> hfss.materials.add_material("MyMaterial2")
-        >>> hfss.materials.add_material_sweep(["MyMaterial", "MyMaterial2"], "Sweep_copper")
+        >>> hfss.materials.add_material_sweep(["MyMaterial", "MyMaterial2"],"Sweep_copper")
         """
         matsweep = []
-        for mat in materials_list:
+        for mat in assignment:
             matobj = self.checkifmaterialexists(mat)
             if matobj:
                 matsweep.append(matobj)
 
         mat_dict = self._create_mat_project_vars(matsweep)
 
-        newmat = Material(self, material_name, material_update=False)
+        newmat = Material(self, name, material_update=False)
         newmat._update_material()
-        index = "$ID" + material_name
+        index = "$ID" + name
         newmat.is_sweep_material = True
         self._app[index] = 0
         for el in mat_dict:
             if el in list(mat_dict.keys()):
-                array_var_name = "$" + material_name + "_" + el
+                array_var_name = "$" + name + "_" + el
                 self._app[array_var_name] = mat_dict[el]
                 newmat.__dict__["_" + el].value = array_var_name + "[" + index + "]"
                 newmat._update_props(el, array_var_name + "[" + index + "]", False)
 
         newmat.update()
-        self.material_keys[material_name.lower()] = newmat
+        self.material_keys[name.lower()] = newmat
         return index
 
-    @pyaedt_function_handler()
-    def duplicate_material(self, material_name, new_name=None, props=None):
+    @pyaedt_function_handler(material_name="material", new_name="name", props="properties")
+    def duplicate_material(self, material, name=None, properties=None):
         """Duplicate a material.
 
         Parameters
         ----------
-        material_name : str
+        material : str
             Name of the material.
-        new_name : str
+        name : str
             Name for the copy of the material. If a new name is not specified,
             the new material name is ``material_name`` plusa  "_clone"`` suffix.
-        props : list
+        properties : list
             List of properties to parameterize when the material is duplicated.
             Parameterized properties have project scope. Options are:
 
             - `'permittivity'`
             - `'permeability'`
             - `'conductivity'`
             - '`dielectric_loss_tan'`
@@ -479,73 +479,73 @@
 
         Examples
         --------
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> hfss.materials.add_material("MyMaterial")
-        >>> hfss.materials.duplicate_material("MyMaterial", "MyMaterial2")
+        >>> hfss.materials.duplicate_material("MyMaterial","MyMaterial2")
 
         """
         # Special characters must be removed from material names to make
         # valid strings for parameter names.
         replace_characters = [(" ", "_"), ("(", ""), (")", ""), ("/", "_"), ("-", "_"), (".", "_"), (",", "_")]
         valid_prop_names = (
             "permittivity",
             "permeability",
             "conductivity",
             "dielectric_loss_tangent",
             "magnetic_loss_tangent",
         )
 
         # Get the material definition.
-        material_in_aedt = material_name.lower() in list(self.mat_names_aedt_lower)
-        material_in_project = material_name.lower() in list(self.material_keys.keys())
+        material_in_aedt = material.lower() in list(self.mat_names_aedt_lower)
+        material_in_project = material.lower() in list(self.material_keys.keys())
         if not (material_in_aedt or material_in_project):  # Check for material definition
-            self.logger.error("Material {} is not present".format(material_name))
+            self.logger.error("Material {} is not present".format(material))
             return False
         if not material_in_project:
-            material = self._aedmattolibrary(material_name)
+            material = self._aedmattolibrary(material)
         else:
-            material = self.material_keys[material_name.lower()]
+            material = self.material_keys[material.lower()]
 
-        if not new_name:
-            new_name = material_name + "_clone"
-        new_material = Material(self, new_name, material._props, material_update=False)
+        if not name:
+            name = material + "_clone"
+        new_material = Material(self, name, material._props, material_update=False)
         new_material._update_material()
 
         # Parameterize material properties if these were passed.
-        if props:
-            for p in props:
+        if properties:
+            for p in properties:
                 if p in valid_prop_names:
-                    var_name = "$" + new_name + "_" + p
+                    var_name = "$" + name + "_" + p
                     for r in replace_characters:
                         var_name = var_name.replace(r[0], r[1])
                     self._app[var_name] = getattr(
                         material, p
                     ).value  # Assign default value to parameterized material parameter.
                     try:
                         setattr(new_material, p, var_name)
                     except TypeError:
                         print("p = {}".format(p))
         new_material.update()
         new_material._material_update = True
-        self._mats.append(new_name)
-        self.material_keys[new_name.lower()] = new_material
+        self._mats.append(name)
+        self.material_keys[name.lower()] = new_material
         return new_material
 
-    @pyaedt_function_handler()
-    def duplicate_surface_material(self, material, new_name):
+    @pyaedt_function_handler(new_name="name")
+    def duplicate_surface_material(self, material, name):
         """Duplicate a surface material.
 
         Parameters
         ----------
          material : str
             Name of the surface material.
-        new_name : str
+        name : str
             Name for the copy of the surface material.
 
         Returns
         -------
         :class:`pyaedt.modules.SurfaceMaterial`
 
         References
@@ -555,23 +555,23 @@
 
         Examples
         --------
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
         >>> hfss.materials.add_surface_material("MyMaterial")
-        >>> hfss.materials.duplicate_surface_material("MyMaterial", "MyMaterial2")
+        >>> hfss.materials.duplicate_surface_material("MyMaterial","MyMaterial2")
         """
         if not material.lower() in list(self.surface_material_keys.keys()):
             self.logger.error("Material {} is not present".format(material))
             return False
         newmat = SurfaceMaterial(
-            self, new_name.lower(), self.surface_material_keys[material.lower()]._props, material_update=True
+            self, name.lower(), self.surface_material_keys[material.lower()]._props, material_update=True
         )
-        self.surface_material_keys[new_name.lower()] = newmat
+        self.surface_material_keys[name.lower()] = newmat
         return newmat
 
     @pyaedt_function_handler()
     def remove_material(self, material, library="Project"):
         """Remove a material.
 
         Parameters
@@ -676,21 +676,21 @@
         first_value = next(value_iterator)
         newmat = Material(self, matname, first_value, material_update=False)
         newmat._update_material()
         newmat._material_update = True
         self.material_keys[matname.lower()] = newmat
         return self.material_keys[matname.lower()]
 
-    @pyaedt_function_handler()
-    def export_materials_to_file(self, full_json_path):
+    @pyaedt_function_handler(full_json_path="output_file")
+    def export_materials_to_file(self, output_file):
         """Export all materials to a JSON  or TOML file.
 
         Parameters
         ----------
-        full_json_path : str
+        output_file : str
             Full path and name of the JSON file to export to.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -746,51 +746,51 @@
                             )
                         }
                     )
         json_dict = {}
         json_dict["materials"] = output_dict
         if datasets:
             json_dict["datasets"] = datasets
-        return write_configuration_file(json_dict, full_json_path)
+        return write_configuration_file(json_dict, output_file)
 
-    @pyaedt_function_handler()
-    def import_materials_from_file(self, full_path=None, **kwargs):
+    @pyaedt_function_handler(full_path="input_file")
+    def import_materials_from_file(self, input_file=None, **kwargs):
         """Import and create materials from a JSON or AMAT file.
 
         Parameters
         ----------
-        full_path : str
+        input_file : str
             Full path and name for the JSON or AMAT file.
 
         Returns
         -------
         List of :class:`pyaedt.modules.Material.Material`
 
         """
 
         if "full_json_path" in kwargs and kwargs["full_json_path"] is not None:  # pragma: no cover
             warnings.warn(
                 "``full_json_path`` was deprecated in 0.8.1. Use ``full_path`` instead.",
                 DeprecationWarning,
             )
-            full_path = kwargs["full_json_path"]
+            input_file = kwargs["full_json_path"]
 
-        if full_path is None or not os.path.exists(full_path):
+        if input_file is None or not os.path.exists(input_file):
             self.logger.error("Incorrect path provided.")
             return False
 
-        _, file_extension = os.path.splitext(full_path)
+        _, file_extension = os.path.splitext(input_file)
         json_flag = True
         datasets = {}
         if file_extension.lower() == ".json":
-            data = read_json(full_path)
+            data = read_json(input_file)
             if "datasets" in list(data.keys()):
                 datasets = data["datasets"]
         elif file_extension.lower() == ".amat":
-            data = load_entire_aedt_file(full_path)
+            data = load_entire_aedt_file(input_file)
             json_flag = False
             new_data = {}
 
             for mat_name in data:
                 if "MaterialDef" in data[mat_name] and mat_name in data[mat_name]["MaterialDef"]:
                     new_data[mat_name] = data[mat_name]["MaterialDef"][mat_name]
                 else:
@@ -851,27 +851,27 @@
                     continue
                 if mat_name.lower() in list(self.material_keys.keys()):
                     newname = generate_unique_name(mat_name)
                     self.logger.warning("Material %s already exists. Renaming to %s", mat_name, newname)
                 else:
                     newname = mat_name
 
-                newmat = self.add_material(newname, props=data[mat_name])
+                newmat = self.add_material(newname, properties=data[mat_name])
                 newmat._props = data[mat_name]
                 newmat._update_material()
                 materials_added.append(newmat)
         return materials_added
 
-    @pyaedt_function_handler()
-    def import_materials_from_excel(self, material_file):
+    @pyaedt_function_handler(material_file="input_file")
+    def import_materials_from_excel(self, input_file):
         """Import and create materials from a csv or excel file.
 
         Parameters
         ----------
-        material_file : str
+        input_file : str
             Full path and name for the csv or xlsx file.
 
         Returns
         -------
         List of :class:`pyaedt.modules.Material.Material`
 
         """
@@ -881,18 +881,18 @@
             self.logger.error("Pandas is needed. Install it.")
             return False
         materials_added = []
         props = {}
         if is_ironpython:
             self.logger.error("This method only works with CPython.")
             return False
-        if os.path.splitext(material_file)[1] == ".csv":
-            df = pd.read_csv(material_file, index_col=0)
-        elif os.path.splitext(material_file)[1] == ".xlsx":
-            df = pd.read_excel(material_file, index_col=0)
+        if os.path.splitext(input_file)[1] == ".csv":
+            df = pd.read_csv(input_file, index_col=0)
+        elif os.path.splitext(input_file)[1] == ".xlsx":
+            df = pd.read_excel(input_file, index_col=0)
         else:
             self.logger.error("Only csv and xlsx are supported.")
             return False
         keys = [i.lower() for i in list(df.keys())]
         for el, val in df[::-1].iterrows():
             if isinstance(el, float):
                 break
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/Mesh.py` & `pyaedt-0.8.9/pyaedt/modules/Mesh.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,15 +320,15 @@
 
     Examples
     --------
     Basic usage demonstrated with an HFSS design:
 
     >>> from pyaedt import Hfss
     >>> hfss = Hfss()
-    >>> cylinder = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+    >>> cylinder = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
     >>> model_resolution = hfss.mesh.assign_model_resolution(cylinder,1e-4,"ModelRes1")
     """
 
     def __init__(self, app):
         app.logger.reset_timer()
         self._app = app
         self._odesign = self._app.odesign
@@ -355,15 +355,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> cylinder = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> cylinder = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> mr1 = hfss.mesh.assign_model_resolution(cylinder,1e-4,"ModelRes1")
         >>> mr2 = hfss.mesh[mr1.name]
         """
 
         if part_id in self.meshoperation_names:
             mesh_op_selected = [mesh_op for mesh_op in self.meshoperations if mesh_op.name == part_id]
             return mesh_op_selected[0]
@@ -381,15 +381,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> o = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> o = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> mr1 = hfss.mesh.assign_model_resolution(o,1e-4,"ModelRes1")
         >>> mesh_operations_list = hfss.mesh.meshoperations
         """
         if self._meshoperations is None:
             self._meshoperations = self._get_design_mesh_operations()
         return self._meshoperations
 
@@ -411,15 +411,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> o = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> o = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> mr1 = hfss.mesh.assign_model_resolution(o,1e-4,"ModelRes1")
         >>> mr2 = hfss.mesh.assign_model_resolution(o,1e-2,"ModelRes2")
         >>> mesh_operations_names = hfss.mesh.meshoperation_names
         """
         if self._app._is_object_oriented_enabled():
             return list(self._app.odesign.GetChildObject("Mesh").GetChildNames())
         return []
@@ -561,15 +561,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> o = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> o = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> surface = hfss.mesh.assign_surface_mesh(o.id,3,"Surface")
         """
         assignment = self.modeler.convert_to_selections(assignment, True)
         if name:
             for m in self.meshoperations:
                 if name == m.name:
                     name = generate_unique_name(name)
@@ -626,15 +626,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> o = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> o = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> surface = hfss.mesh.assign_surface_mesh_manual(o.id,1e-6,aspect_ratio=3,name="Surface_Manual")
         """
         assignment = self.modeler.convert_to_selections(assignment, True)
         if name:
             for m in self.meshoperations:
                 if name == m.name:
                     name = generate_unique_name(name)
@@ -703,15 +703,15 @@
 
         Examples
         --------
         Basic usage demonstrated with an HFSS design:
 
         >>> from pyaedt import Hfss
         >>> hfss = Hfss()
-        >>> o = hfss.modeler.create_cylinder(0, [0, 0, 0], 3, 20, 0)
+        >>> o = hfss.modeler.create_cylinder(0,[0, 0, 0],3,20,0)
         >>> surface = hfss.mesh.assign_model_resolution(o,1e-4,"ModelRes1")
         """
         assignment = self.modeler.convert_to_selections(assignment, True)
         if name:
             for m in self.meshoperations:
                 if name == m.name:
                     name = generate_unique_name(name)
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/Mesh3DLayout.py` & `pyaedt-0.8.9/pyaedt/modules/Mesh3DLayout.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/MeshIcepak.py` & `pyaedt-0.8.9/pyaedt/modules/MeshIcepak.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,39 +337,39 @@
             Name to assign to the subregion.
         parts : list of str
             Parts to be included in the subregion.
 
          Returns
         -------
         bool
-            True if successful, else False
+            ``True`` when successful, ``False`` when failed.
         """
         try:
             if (
                 self.object is not None and self._app.modeler.objects_by_name.get(self.object.name, False)
             ) or self._app.modeler.objects_by_name.get(region_name, False):
                 self._app.logger.error("{} already exists in the design.".format(self.object.name))
                 return False
             if not isinstance(parts, list):
                 objects = [parts]
                 if not isinstance(objects[0], str):
                     objects = [o.name for o in objects]
             self._app.modeler.create_subregion(padding_values, padding_types, parts, region_name)
             return True
-        except:
+        except Exception:
             return False
 
     def delete(self):
         """
         Delete the subregion object.
 
          Returns
         -------
         bool
-            True if successful, else False
+           ``True`` when successful, ``False`` when failed.
         """
         try:
             self.object.delete()
             self._app.mesh.meshregions.remove(
                 [mo for mo in self._app.mesh.meshregions.values() if mo.subregion == self][0]
             )
             return True
@@ -536,17 +536,17 @@
     """
     Manages Icepak mesh region settings.
 
     Attributes:
         name : str
             Name of the mesh region.
         manual_settings : bool
-            Whether to use manual settings or automatic ones.
-        settings : ::class::modules.MeshIcepak.MeshSettings
-            Dictionary-like object to handle settings
+            Whether to use manual settings. If ``False``, automatic settings are used.
+        settings : :class:`modules.MeshIcepak.MeshSettings`
+            Dictionary-like object to handle settings.
     """
 
     def __init__(self, units, app, name):
         self.manual_settings = False
         self.settings = MeshSettings(self, app)
         self._name = name
         self._model_units = units
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/OptimetricsTemplates.py` & `pyaedt-0.8.9/pyaedt/modules/OptimetricsTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/PostProcessor.py` & `pyaedt-0.8.9/pyaedt/modules/PostProcessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -3036,14 +3036,15 @@
         quantity,
         setup,
         intrinsics,
         list_type,
         plot_name=None,
         filter_boxes=None,
         field_type=None,
+        create_plot=True,
     ):
         if not list_type.startswith("Layer") and self._app.design_type != "HFSS 3D Layout Design":
             assignment = self._app.modeler.convert_to_selections(assignment, True)
         if not setup:
             setup = self._app.existing_analysis_sweeps[0]
         if not intrinsics:
             for i in self._app.setups:
@@ -3079,22 +3080,21 @@
                 layer_plot_type=list_type,
             )
         if self._app.design_type == "Q3D Extractor":  # pragma: no cover
             plot.field_type = field_type
         plot.name = plot_name
         plot.plot_folder = plot_name
         plot.filter_boxes = filter_boxes
-        plt = plot.create()
-        if "Maxwell" in self._app.design_type and "Transient" in self.post_solution_type:
-            self.ofieldsreporter.SetPlotsViewSolutionContext([plot_name], setup, "Time:" + intrinsics["Time"])
-        if plt:
-            self.field_plots[plot_name] = plot
-            return plot
-        else:
-            return False
+        if create_plot:
+            plt = plot.create()
+            if plt:
+                return plot
+            else:
+                return False
+        return plot
 
     @pyaedt_function_handler(quantityName="quantity", setup_name="setup")
     def _create_fieldplot_line_traces(
         self,
         seeding_faces_ids,
         in_volume_tracing_ids,
         surface_tracing_ids,
@@ -3290,28 +3290,188 @@
             "FieldLineTrace",
             setup,
             intrinsics,
             plot_name,
             field_type=field_type,
         )
 
+    @pyaedt_function_handler()
+    def _get_3dl_layers_nets(self, layers, nets, setup):
+        lst_faces = []
+        new_layers = []
+        if not layers:
+            new_layers.extend(["{}".format(i) for i in self._app.modeler.edb.stackup.dielectric_layers.keys()])
+            for layer in self._app.modeler.edb.stackup.signal_layers.keys():
+                if not nets:
+                    nets = list(self._app.modeler.edb.nets.nets.keys())
+                for el in nets:
+                    try:
+                        get_ids = self._odesign.GetGeometryIdsForNetLayerCombination(el, layer, setup)
+                    except:
+                        get_ids = []
+                    if isinstance(get_ids, (tuple, list)) and len(get_ids) > 2:
+                        lst_faces.extend([int(i) for i in get_ids[2:]])
+
+        else:
+            for layer in layers:
+                if layer in self._app.modeler.edb.stackup.dielectric_layers:
+                    new_layers.append("{}".format(layer))
+                elif layer in self._app.modeler.edb.stackup.signal_layers:
+                    if not nets:
+                        nets = list(self._app.modeler.edb.nets.nets.keys())
+                    for el in nets:
+                        try:
+                            get_ids = self._odesign.GetGeometryIdsForNetLayerCombination(el, layer, setup)
+                        except:
+                            get_ids = []
+                        if isinstance(get_ids, (tuple, list)) and len(get_ids) > 2:
+                            lst_faces.extend([int(i) for i in get_ids[2:]])
+        return lst_faces, new_layers
+
+    @pyaedt_function_handler()
+    def _get_3d_layers_nets(self, layers, nets):
+        dielectrics = []
+        new_layers = []
+        for k, v in self._app.modeler.user_defined_components.items():
+            if v.layout_component:
+                if not layers and not nets:
+                    new_layers.extend(
+                        [
+                            "{}:{}#t=fill".format(k, i)
+                            for i in v.layout_component.edb_object.stackup.signal_layers.keys()
+                        ]
+                    )
+                    new_layers.extend(
+                        ["{}:{}".format(k, i) for i in v.layout_component.edb_object.stackup.dielectric_layers.keys()]
+                    )
+                elif not nets:
+                    for layer in layers:
+                        if layer in v.layout_component.edb_object.stackup.signal_layers:
+                            new_layers.append("{}:{}#t=fill".format(k, layer))
+                        elif layer in v.layout_component.edb_object.stackup.dielectric_layers:
+                            new_layers.append("{}:{}".format(k, layer))
+                elif not layers:
+                    for v in self._app.modeler.user_defined_components.values():
+                        new_layers.extend(
+                            [[i] + nets for i in v.layout_component.edb_object.stackup.signal_layers.keys()]
+                        )
+                else:
+                    for layer in layers:
+                        if layer in v.layout_component.edb_object.stackup.signal_layers:
+                            new_layers.append([layer] + nets)
+                        elif layer in v.layout_component.edb_object.stackup.dielectric_layers:
+                            dielectrics.append("{}:{}".format(k, layer))
+        return dielectrics, new_layers
+
+    @pyaedt_function_handler()
+    def create_fieldplot_layers(
+        self, layers, quantity, setup=None, nets=None, plot_on_surface=True, intrinsics=None, name=None
+    ):
+        # type: (list, str, str, list, bool, dict, str) -> FieldPlot
+        """Create a field plot of stacked layer plot.
+        This plot is valid from AEDT 2023 R2 and later in HFSS 3D Layout.
+        It will also work when a layout components in 3d modeler is used.
+        In order to plot on signal layers use the method ``create_fieldplot_layers_nets``.
+
+        Parameters
+        ----------
+        layers : list
+            List of layers to plot. For example:
+            ``["Layer1","Layer2"]``. If empty list is provided
+            all layers will be considered.
+        quantity : str
+            Name of the quantity to plot.
+        setup : str, optional
+            Name of the setup. The default is ``None``, in which case the ``nominal_adaptive``
+            setup is used. Make sure to build a setup string in the form of
+            ``"SetupName : SetupSweep"``, where ``SetupSweep`` is the sweep name to
+            use in the export or ``LastAdaptive``.
+        nets : list, optional
+            List of nets to filter the field plot. Optional.
+        intrinsics : dict, optional
+            Dictionary containing all intrinsic variables.
+            The default is ``None``.
+        name : str, optional
+            Name of the field plot to create.
+
+        Returns
+        -------
+        :class:``pyaedt.modules.solutions.FieldPlot`` or bool
+            Plot object.
+
+        References
+        ----------
+
+        >>> oModule.CreateFieldPlot
+        """
+        if not setup:
+            setup = self._app.existing_analysis_sweeps[0]
+        if nets is None:
+            nets = []
+        if not (
+            "APhi" in self.post_solution_type and settings.aedt_version >= "2023.2"
+        ) and not self._app.design_type in ["HFSS", "HFSS 3D Layout Design"]:
+            self.logger.error("This method requires AEDT 2023 R2 and Maxwell 3D Transient APhi Formulation.")
+            return False
+        if intrinsics is None:
+            intrinsics = {}
+        if name and name in list(self.field_plots.keys()):
+            self.logger.info("Plot {} exists. returning the object.".format(name))
+            return self.field_plots[name]
+
+        if self._app.design_type in ["HFSS 3D Layout Design"]:
+            lst_faces, new_layers = self._get_3dl_layers_nets(layers, nets, setup)
+            if new_layers:
+                plt = self._create_fieldplot(
+                    new_layers, quantity, setup, intrinsics, "ObjList", name, create_plot=False
+                )
+                plt.surfaces = lst_faces
+                out = plt.create()
+                if out:
+                    return plt
+                return False
+            else:
+                return self._create_fieldplot(lst_faces, quantity, setup, intrinsics, "FacesList", name)
+        else:
+            dielectrics, new_layers = self._get_3d_layers_nets(layers, nets)
+            if nets and plot_on_surface:
+                plot_type = "LayerNetsExtFace"
+            elif nets:
+                plot_type = "LayerNets"
+            else:
+                plot_type = "ObjList"
+            if new_layers:
+                plt = self._create_fieldplot(
+                    new_layers, quantity, setup, intrinsics, plot_type, name, create_plot=False
+                )
+                if dielectrics:
+                    plt.volumes = dielectrics
+                out = plt.create()
+                if out:
+                    return plt
+            elif dielectrics:
+                return self._create_fieldplot(dielectrics, quantity, setup, intrinsics, "ObjList", name)
+            return False
+
     @pyaedt_function_handler(quantity_name="quantity", setup_name="setup")
     def create_fieldplot_layers_nets(
         self, layers_nets, quantity, setup=None, intrinsics=None, plot_on_surface=True, plot_name=None
-    ):  # pragma: no cover
+    ):
         # type: (list, str, str, dict, bool, str) -> FieldPlot
         """Create a field plot of stacked layer plot.
         This plot is valid from AEDT 2023 R2 and later in HFSS 3D Layout
         and any modeler where a layout component is used.
 
         Parameters
         ----------
         layers_nets : list
             List of layers and nets to plot. For example:
-            ``[["Layer1", "GND", "PWR"], ["Layer2", "VCC"], ...]``.
+            ``[["Layer1", "GND", "PWR"], ["Layer2", "VCC"], ...]``. If ``"no-layer"`` is provided as first argument,
+            all layers will be considered. If ``"no-net"`` is provided or the list contains only layer name, all the
+            nets will be automatically considered.
         quantity : str
             Name of the quantity to plot.
         setup : str, optional
             Name of the setup. The default is ``None``, in which case the ``nominal_adaptive``
             setup is used. Make sure to build a setup string in the form of
             ``"SetupName : SetupSweep"``, where ``SetupSweep`` is the sweep name to
             use in the export or ``LastAdaptive``.
@@ -3329,14 +3489,15 @@
             Plot object.
 
         References
         ----------
 
         >>> oModule.CreateFieldPlot
         """
+
         if not (
             "APhi" in self.post_solution_type and settings.aedt_version >= "2023.2"
         ) and not self._app.design_type in ["HFSS", "HFSS 3D Layout Design"]:
             self.logger.error("This method requires AEDT 2023 R2 and Maxwell 3D Transient APhi Formulation.")
             return False
         if intrinsics is None:
             intrinsics = {}
@@ -3349,19 +3510,35 @@
             lst = []
             for layer in layers_nets:
                 for el in layer[1:]:
                     get_ids = self._odesign.GetGeometryIdsForNetLayerCombination(el, layer[0], setup)
                     if isinstance(get_ids, (tuple, list)) and len(get_ids) > 2:
                         lst.extend([int(i) for i in get_ids[2:]])
             return self._create_fieldplot(lst, quantity, setup, intrinsics, "FacesList", plot_name)
-        if plot_on_surface:
-            plot_type = "LayerNetsExtFace"
         else:
-            plot_type = "LayerNets"
-        return self._create_fieldplot(layers_nets, quantity, setup, intrinsics, plot_type, plot_name)
+            new_list = []
+            for layer in layers_nets:
+                if "no-layer" in layer[0]:
+                    for v in self._app.modeler.user_defined_components.values():
+                        new_list.extend(
+                            [[i] + layer[1:] for i in v.layout_component.edb_object.stackup.signal_layers.keys()]
+                        )
+                else:
+                    new_list.append(layer)
+            layers_nets = new_list
+            for layer in layers_nets:
+                if len(layer) == 1 or "no-net" in layer[1]:
+                    for v in self._app.modeler.user_defined_components.values():
+                        if layer[0] in v.layout_component.edb_object.stackup.stackup_layers:
+                            layer.extend(list(v.layout_component.edb_object.nets.nets.keys()))
+            if plot_on_surface:
+                plot_type = "LayerNetsExtFace"
+            else:
+                plot_type = "LayerNets"
+            return self._create_fieldplot(layers_nets, quantity, setup, intrinsics, plot_type, plot_name)
 
     @pyaedt_function_handler(
         objlist="assignment", quantityName="quantity", IntrinsincDict="intrinsics", setup_name="setup"
     )
     def create_fieldplot_surface(
         self, assignment, quantity, setup=None, intrinsics=None, plot_name=None, field_type="DC R/L Fields"
     ):
@@ -3874,15 +4051,15 @@
             return files_exported
         else:
             fname = os.path.join(export_path, "Model_AllObjs_AllMats.obj")
             self._app.modeler.oeditor.ExportModelMeshToFile(fname, assignment)
             return [[fname, "aquamarine", 0.3]]
 
     @pyaedt_function_handler(setup_name="setup")
-    def export_mesh_obj(self, setup=None, intrinsics=None):
+    def export_mesh_obj(self, setup=None, intrinsics=None, export_air_objects=False, on_surfaces=True):
         """Export the mesh in AEDTPLT format.
         The mesh has to be available in the selected setup.
         If a parametric model is provided, you can choose the mesh to export by providing a specific set of variations.
         This method applies only to ``Hfss``, ``Q3d``, ``Q2D``, ``Maxwell3d``, ``Maxwell2d``, ``Icepak``
         and ``Mechanical`` objects. This method is calling ``create_fieldplot_surface`` to create a mesh plot and
         ``export_field_plot`` to export it as ``aedtplt`` file.
 
@@ -3893,14 +4070,19 @@
             setup is used. Be sure to build a setup string in the form of
             ``"SetupName : SetupSweep"``, where ``SetupSweep`` is the sweep name to
             use in the export or ``LastAdaptive``.
         intrinsics : dict, optional.
             Intrinsic dictionary that is needed for the export.
             The default is ``None``, which assumes that no variables are present in
             the dictionary or nominal values are used.
+        export_air_objects : bool, optional
+            Whether to include vacuum objects for the copied objects.
+            The default is ``False``.
+        on_surfaces : bool, optional
+            Whether to create a mesh on surfaces or on the volume.  The default is ``True``.
 
         Returns
         -------
         str
             File Generated with full path.
 
         Examples
@@ -3915,21 +4097,29 @@
         """
         if intrinsics is None:
             intrinsics = {}
         project_path = self._app.working_directory
 
         if not setup:
             setup = self._app.nominal_adaptive
-        face_lists = []
+        mesh_list = []
         obj_list = self._app.modeler.object_names
         for el in obj_list:
             object3d = self._app.modeler[el]
-            if not object3d.is3d or object3d.material_name not in ["vacuum", "air"]:
-                face_lists += [i.id for i in object3d.faces]
-        plot = self.create_fieldplot_surface(face_lists, "Mesh", setup, intrinsics)
+            if on_surfaces:
+                if not object3d.is3d or (not export_air_objects and object3d.material_name not in ["vacuum", "air"]):
+                    mesh_list += [i.id for i in object3d.faces]
+            else:
+                if not object3d.is3d or (not export_air_objects and object3d.material_name not in ["vacuum", "air"]):
+                    mesh_list.append(el)
+        if on_surfaces:
+            plot = self.create_fieldplot_surface(mesh_list, "Mesh", setup, intrinsics)
+        else:
+            plot = self.create_fieldplot_volume(mesh_list, "Mesh", setup, intrinsics)
+
         if plot:
             file_to_add = self.export_field_plot(plot.name, project_path)
             plot.delete()
             return file_to_add
         return None
 
     @pyaedt_function_handler()
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/SetupTemplates.py` & `pyaedt-0.8.9/pyaedt/modules/SetupTemplates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/SolveSetup.py` & `pyaedt-0.8.9/pyaedt/modules/SolveSetup.py`

 * *Files 2% similar despite different names*

```diff
@@ -66,38 +66,38 @@
             elif i == "Time":
                 intr[i] = "0s"
         return intr
 
     def __repr__(self):
         return "SetupName " + self.name + " with " + str(len(self.sweeps)) + " Sweeps"
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(num_cores="cores", num_tasks="tasks", num_gpu="gpus")
     def analyze(
         self,
-        num_cores=1,
-        num_tasks=1,
-        num_gpu=0,
+        cores=1,
+        tasks=1,
+        gpus=0,
         acf_file=None,
         use_auto_settings=True,
         solve_in_batch=False,
         machine="localhost",
         run_in_thread=False,
         revert_to_initial_mesh=False,
         blocking=True,
     ):
         """Solve the active design.
 
         Parameters
         ----------
-        num_cores : int, optional
-            Number of simulation cores. Default is ``1``.
-        num_tasks : int, optional
-            Number of simulation tasks. Default is ``1``.
-        num_gpu : int, optional
-            Number of simulation graphic processing units to use. Default is ``0``.
+        cores : int, optional
+            Number of simulation cores. The default is ``1``.
+        tasks : int, optional
+            Number of simulation tasks. The default is ``1``.
+        gpus : int, optional
+            Number of simulation graphic processing units to use. The default is ``0``.
         acf_file : str, optional
             Full path to the custom ACF file.
         use_auto_settings : bool, optional
             Set ``True`` to use automatic settings for HPC. The option is only considered for setups
             that support automatic settings.
         solve_in_batch : bool, optional
             Whether to solve the project in batch or not.
@@ -120,18 +120,18 @@
 
         References
         ----------
 
         >>> oDesign.Analyze
         """
         self._app.analyze(
-            setup_name=self.name,
-            num_cores=num_cores,
-            num_tasks=num_tasks,
-            num_gpu=num_gpu,
+            name=self.name,
+            cores=cores,
+            tasks=tasks,
+            gpus=gpus,
             acf_file=acf_file,
             use_auto_settings=use_auto_settings,
             solve_in_batch=solve_in_batch,
             machine=machine,
             run_in_thread=run_in_thread,
             revert_to_initial_mesh=revert_to_initial_mesh,
             blocking=blocking,
@@ -470,38 +470,38 @@
         """
         soltype = SetupKeys.SetupNames[self.setuptype]
         arg = ["NAME:" + self.name]
         _dict2arg(self.props, arg)
         self.omodule.InsertSetup(soltype, arg)
         return arg
 
-    @pyaedt_function_handler()
-    def update(self, update_dictionary=None):
+    @pyaedt_function_handler(update_dictionary="properties")
+    def update(self, properties=None):
         """Update the setup based on either the class argument or a dictionary.
 
         Parameters
         ----------
-        update_dictionary : optional
+        properties : optional
             Dictionary to use to update the setup. The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.EditSetup
         """
         legacy_update = self.auto_update
         self.auto_update = False
-        if update_dictionary:
-            for el in update_dictionary:
-                self.props[el] = update_dictionary[el]
+        if properties:
+            for el in properties:
+                self.props[el] = properties[el]
         self.auto_update = legacy_update
         arg = ["NAME:" + self.name]
         _dict2arg(self.props, arg)
 
         self.omodule.EditSetup(self.name, arg)
         return True
 
@@ -1092,21 +1092,21 @@
             elif soltype == "NexximAMI":
                 self.omodule.EditAMIAnalysis(self.name, arg)
 
             else:
                 raise NotImplementedError("Solution type '{}' is not implemented yet".format(soltype))
         return True
 
-    @pyaedt_function_handler()
-    def update(self, update_dictionary=None):
+    @pyaedt_function_handler(update_dictionary="properties")
+    def update(self, properties=None):
         """Update the setup based on the class arguments or a dictionary.
 
         Parameters
         ----------
-        update_dictionary : dict, optional
+        properties : dict, optional
             Dictionary of settings to apply. The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
@@ -1118,17 +1118,17 @@
         >>> oModule.EditTransient
         >>> oModule.EditQuickEyeAnalysis
         >>> oModule.EditVerifEyeAnalysis
         >>> oModule.EditAMIAnalysis
         """
         legacy_update = self.auto_update
         self.auto_update = False
-        if update_dictionary:
-            for el in update_dictionary:
-                self.props[el] = update_dictionary[el]
+        if properties:
+            for el in properties:
+                self.props[el] = properties[el]
         arg = ["NAME:SimSetup"]
         soltype = SetupKeys.SetupNames[self.setuptype]
         _dict2arg(self.props, arg)
         self._setup(soltype, arg, False)
         self.auto_update = legacy_update
         return True
 
@@ -1172,35 +1172,37 @@
             if isinstance(el, (int, float)):
                 sweeps.append(str(el) + units)
             else:
                 sweeps.append(el)
         lin_data = " ".join(sweeps)
         return self._add_sweep(sweep_variable, lin_data, override_existing_sweep)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(start_point="start", end_point="stop")
     def add_sweep_count(
         self,
         sweep_variable="Freq",
-        start_point=1,
-        end_point=100,
+        start=1,
+        stop=100,
         count=100,
         units="GHz",
         count_type="Linear",
         override_existing_sweep=True,
     ):
         """Add a step sweep to existing Circuit Setup. It can be ``"Linear"``, ``"Decade"`` or ``"Octave"``.
 
         Parameters
         ----------
         sweep_variable : str, optional
-            Variable to which the sweep belongs. Default is ``"Freq``.
-        start_point : float or str, optional
-            Start Point of Linear Count sweep. If ``str`` then no units will be applied.
-        end_point : float or str, optional
-            End Point of Linear Count sweep. If ``str`` then no units will be applied.
+            Variable that the sweep belongs to. The default is ``"Freq``.
+        start : float or str, optional
+            Start point of the linear count sweep. The default is ``1``.
+            If a string ``str`` is specified, no units are applied.
+        stop : float or str, optional
+            End point of the linear count sweep. The default is ``100``.
+            If a string is specified, no units are applied.
         count :  int, optional
             Number of points. Default is ``100``.
         units : str, optional
             Sweeps Units. It will be ignored if strings are provided as start_point or end_point.
         count_type : str, optional
             Count Type. Default is ``"Linear"``. It can be also ``"Decade"`` or ``"Octave"``.
         override_existing_sweep : bool, optional
@@ -1217,50 +1219,53 @@
         >>> oModule.EditLinearNetworkAnalysis
         >>> oModule.EditDCAnalysis
         >>> oModule.EditTransient
         >>> oModule.EditQuickEyeAnalysis
         >>> oModule.EditVerifEyeAnalysis
         >>> oModule.EditAMIAnalysis
         """
-        if isinstance(start_point, (int, float)):
-            start_point = str(start_point) + units
-        if isinstance(end_point, (int, float)):
-            end_point = str(end_point) + units
+        if isinstance(start, (int, float)):
+            start = str(start) + units
+        if isinstance(stop, (int, float)):
+            stop = str(stop) + units
         lin_in = "LINC"
         if count_type.lower() == "decade":
             lin_in = "DEC"
         elif count_type.lower() == "octave":
             lin_in = "OCT"
-        lin_data = "{} {} {} {}".format(lin_in, start_point, end_point, count)
+        lin_data = "{} {} {} {}".format(lin_in, start, stop, count)
         return self._add_sweep(sweep_variable, lin_data, override_existing_sweep)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(start_point="start", end_point="stop")
     def add_sweep_step(
         self,
         sweep_variable="Freq",
-        start_point=1,
-        end_point=100,
+        start=1,
+        stop=100,
         step_size=1,
         units="GHz",
         override_existing_sweep=True,
     ):
         """Add a linear count sweep to existing Circuit Setup.
 
         Parameters
         ----------
         sweep_variable : str, optional
             Variable to which the sweep belongs. Default is ``"Freq``.
-        start_point : float or str, optional
-            Start Point of Linear Count sweep. If ``str`` then no units will be applied.
-        end_point : float or str, optional
-            End Point of Linear Count sweep. If ``str`` then no units will be applied.
+        start : float or str, optional
+            Start point of the linear count sweep. The default is ``1``.
+            If a string ``str`` is specified, no units are applied.
+        stop : float or str, optional
+            End point of the linear count sweep. The default is ``100``.
+            If a string is specified, no units are applied.
         step_size :  float or str, optional
-            Step Size of sweep. If ``str`` then no units will be applied.
+            Step size of the sweep. The default is ``1``.
+            If a string is specified, no units are applied.
         units : str, optional
-            Sweeps Units. It will be ignored if strings are provided as start_point or end_point
+            Sweeps Units. It will be ignored if strings are provided as start_point or end_point.
         override_existing_sweep : bool, optional
             Define if existing sweep on the same variable has to be overridden or kept and added to this new sweep.
 
         Returns
         -------
         bool
             ``True`` is succeeded.
@@ -1271,21 +1276,21 @@
         >>> oModule.EditLinearNetworkAnalysis
         >>> oModule.EditDCAnalysis
         >>> oModule.EditTransient
         >>> oModule.EditQuickEyeAnalysis
         >>> oModule.EditVerifEyeAnalysis
         >>> oModule.EditAMIAnalysis
         """
-        if isinstance(start_point, (int, float)):
-            start_point = str(start_point) + units
-        if isinstance(end_point, (int, float)):
-            end_point = str(end_point) + units
+        if isinstance(start, (int, float)):
+            start = str(start) + units
+        if isinstance(stop, (int, float)):
+            stop = str(stop) + units
         if isinstance(step_size, (int, float)):
             step_size = str(step_size) + units
-        linc_data = "LIN {} {} {}".format(start_point, end_point, step_size)
+        linc_data = "LIN {} {} {}".format(start, stop, step_size)
         return self._add_sweep(sweep_variable, linc_data, override_existing_sweep)
 
     @pyaedt_function_handler()
     def _add_sweep(self, sweep_variable, equation, override_existing_sweep):
         if isinstance(self.props["SweepDefinition"], list):
             for sw in self.props["SweepDefinition"]:
                 if sw["Variable"] == sweep_variable:
@@ -1774,36 +1779,36 @@
         >>> oModule.Add
         """
         arg = ["NAME:" + self.name]
         _dict2arg(self.props, arg)
         self.omodule.Add(arg)
         return True
 
-    @pyaedt_function_handler()
-    def update(self, update_dictionary=None):
+    @pyaedt_function_handler(update_dictionary="properties")
+    def update(self, properties=None):
         """Update the setup based on the class arguments or a dictionary.
 
         Parameters
         ----------
-        update_dictionary : dict, optional
+        properties : dict, optional
             Dictionary of settings to apply.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.Edit
         """
-        if update_dictionary:
-            for el in update_dictionary:
-                self.props._setitem_without_update(el, update_dictionary[el])
+        if properties:
+            for el in properties:
+                self.props._setitem_without_update(el, properties[el])
         arg = ["NAME:" + self.name]
         _dict2arg(self.props, arg)
         self.omodule.Edit(self.name, arg)
         return True
 
     @pyaedt_function_handler()
     def enable(self):
@@ -1847,23 +1852,23 @@
 
         >>> oModule.Edit
         """
         self.props["Properties"]["Enable"] = "false"
         self.update()
         return True
 
-    @pyaedt_function_handler()
-    def export_to_hfss(self, file_fullname, keep_net_name=False):
-        """Export the HFSS 3D Layout design to HFSS 3D design.
+    @pyaedt_function_handler(file_fullname="output_file")
+    def export_to_hfss(self, output_file, keep_net_name=False):
+        """Export the HFSS 3D Layout design to an HFSS 3D design.
 
         This method is not supported with IronPython.
 
         Parameters
         ----------
-        file_fullname : str
+        output_file : str
             Full path and file name for exporting the project.
 
         keep_net_name : bool
             Keep net name in 3D export when ``True`` or by default when ``False``. Default value is ``False``.
 
         Returns
         -------
@@ -1872,27 +1877,27 @@
 
         References
         ----------
 
         >>> oModule.ExportToHfss
         """
 
-        file_fullname = file_fullname
-        if not os.path.isdir(os.path.dirname(file_fullname)):
+        output_file = output_file
+        if not os.path.isdir(os.path.dirname(output_file)):
             return False
-        file_fullname = os.path.splitext(file_fullname)[0] + ".aedt"
+        output_file = os.path.splitext(output_file)[0] + ".aedt"
         info_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 0))
         error_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 2))
-        self.omodule.ExportToHfss(self.name, file_fullname)
-        succeeded = self._check_export_log(info_messages, error_messages, file_fullname)
+        self.omodule.ExportToHfss(self.name, output_file)
+        succeeded = self._check_export_log(info_messages, error_messages, output_file)
         if succeeded and keep_net_name:
             if not is_ironpython:
                 from pyaedt import Hfss
 
-                self._get_net_names(Hfss, file_fullname)
+                self._get_net_names(Hfss, output_file)
             else:
                 self.p_app.logger.error("Exporting layout while keeping net name is not supported with IronPython")
         return succeeded
 
     @pyaedt_function_handler()
     def _get_net_names(self, app, file_fullname):
         primitives_3d_pts_per_nets = self._get_primitives_points_per_net()
@@ -1936,31 +1941,31 @@
                             pad_objs = aedtapp.modeler.get_bodynames_from_position(pad_pos, None, False)
                             for pad_obj in pad_objs:
                                 if pad_obj in metal_object:
                                     pad_ind = aedtapp.modeler.objects[pad_obj].id
                                     if pad_ind not in obj_dict:
                                         obj_dict[pad_ind] = aedtapp.modeler.objects[pad_ind]
             obj_list = list(obj_dict.values())
+            net = net.replace(".", "_")
             if len(obj_list) == 1:
                 net = net.replace("-", "m")
                 net = net.replace("+", "p")
                 net_name = re.sub("[^a-zA-Z0-9 .\n]", "_", net)
                 obj_list[0].name = net_name
                 obj_list[0].color = [randrange(255), randrange(255), randrange(255)]
             elif len(obj_list) > 1:
                 united_object = aedtapp.modeler.unite(obj_list, purge=True)
                 obj_ind = aedtapp.modeler.objects[united_object].id
-                try:
+                if obj_ind:
                     net = net.replace("-", "m")
                     net = net.replace("+", "p")
                     net_name = re.sub("[^a-zA-Z0-9 .\n]", "_", net)
                     aedtapp.modeler.objects[obj_ind].name = net_name
                     aedtapp.modeler.objects[obj_ind].color = [randrange(255), randrange(255), randrange(255)]
-                except Exception:
-                    pass
+
         if aedtapp.design_type == "Q3D Extractor":
             aedtapp.auto_identify_nets()
         aedtapp.close_project(save_project=True)
 
     @pyaedt_function_handler()
     def _get_primitives_points_per_net(self):
         edb = self.p_app.modeler.edb
@@ -2075,52 +2080,54 @@
             if infos_errors:
                 for message in infos_errors:
                     self.p_app.logger.error(message)
                 break
             time.sleep(2)
         return succeeded
 
-    @pyaedt_function_handler()
-    def export_to_q3d(self, file_fullname, keep_net_name=False):
-        """Export the HFSS 3DLayout design to Q3D design.
+    @pyaedt_function_handler(file_fullname="output_file")
+    def export_to_q3d(self, output_file, keep_net_name=False):
+        """Export the HFSS 3D Layout design to a Q3D design.
 
         Parameters
         ----------
-        file_fullname : str
+        output_file : str
             Full path and file name for exporting the project.
+        keep_net_name : bool
+            Whether to keep the net name in the 3D export, The default is ``False``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         keep_net_name : bool
             Keep net name in 3D export when ``True`` or by default when ``False``. Default value is ``False``.
 
         References
         ----------
 
         >>> oModule.ExportToQ3d
         """
 
-        if not os.path.isdir(os.path.dirname(file_fullname)):
+        if not os.path.isdir(os.path.dirname(output_file)):
             return False
-        file_fullname = os.path.splitext(file_fullname)[0] + ".aedt"
-        if os.path.exists(file_fullname):
-            os.unlink(file_fullname)
+        output_file = os.path.splitext(output_file)[0] + ".aedt"
+        if os.path.exists(output_file):
+            os.unlink(output_file)
         info_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 0))
         error_messages = list(self.p_app.odesktop.GetMessages(self.p_app.project_name, self.p_app.design_name, 2))
-        self.omodule.ExportToQ3d(self.name, file_fullname)
-        succeeded = self._check_export_log(info_messages, error_messages, file_fullname)
+        self.omodule.ExportToQ3d(self.name, output_file)
+        succeeded = self._check_export_log(info_messages, error_messages, output_file)
         if succeeded and keep_net_name:
             if not is_ironpython:
                 from pyaedt import Q3d
 
-                self._get_net_names(Q3d, file_fullname)
+                self._get_net_names(Q3d, output_file)
             else:
-                self.p_app.logger.error("Exporting layout while keeping net name is not supported with IronPython")
+                self.p_app.logger.error("Exporting layout while keeping net name is not supported with IronPython.")
         return succeeded
 
     @pyaedt_function_handler(sweepname="name", sweeptype="sweep_type")
     def add_sweep(self, name=None, sweep_type="Interpolating"):
         """Add a frequency sweep.
 
         Parameters
@@ -3706,37 +3713,37 @@
 
     @dc_resistance_only.setter
     def dc_resistance_only(self, value):
         if self.dc_enabled:
             self.props["DC"]["SolveResOnly"] = value
 
     @pyaedt_function_handler()
-    def update(self, update_dictionary=None):
+    def update(self, properties=None):
         """Update the setup based on either the class argument or a dictionary.
 
         Parameters
         ----------
-        update_dictionary : optional
+        properties : optional
             Dictionary to use to update the setup. The default is ``None``.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         References
         ----------
 
         >>> oModule.EditSetup
         """
         legacy_update = self.auto_update
         self.auto_update = False
-        if update_dictionary:
-            for el in update_dictionary:
-                self.props[el] = update_dictionary[el]
+        if properties:
+            for el in properties:
+                self.props[el] = properties[el]
         self.auto_update = legacy_update
         arg = ["NAME:" + self.name]
         props1 = {i: v for i, v in self.props.items()}
         if not self.capacitance_enabled:
             del props1["Cap"]
         if not self.ac_rl_enabled:
             del props1["AC"]
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/SolveSweeps.py` & `pyaedt-0.8.9/pyaedt/modules/SolveSweeps.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/monitor_icepak.py` & `pyaedt-0.8.9/pyaedt/modules/monitor_icepak.py`

 * *Files 0% similar despite different names*

```diff
@@ -387,16 +387,15 @@
         >>> oModule.AssignFaceMonitor
 
         Examples
         --------
 
         Create a rectangle named ``"Surface1"`` and assign a temperature monitor to that surface.
 
-        >>> surface = icepak.modeler.create_rectangle(icepak.PLANE.XY,
-        ...                                           [0, 0, 0], [10, 20], name="Surface1")
+        >>> surface = icepak.modeler.create_rectangle(icepak.PLANE.XY,[0, 0, 0],[10, 20],name="Surface1")
         >>> icepak.assign_surface_monitor("Surface1", monitor_name="monitor")
         'monitor'
         """
         if isinstance(surface_name, str):
             surface_name = [surface_name]
         if isinstance(monitor_quantity, str):
             monitor_quantity = [monitor_quantity]
@@ -491,15 +490,15 @@
         >>> oModule.AssignPointMonitor
 
         Examples
         --------
 
         Create a box named ``"BlockBox1"`` and assign a temperature monitor point to that object.
 
-        >>> box = icepak.modeler.create_box([1, 1, 1], [3, 3, 3], "BlockBox1", "copper")
+        >>> box = icepak.modeler.create_box([1, 1, 1],[3, 3, 3],"BlockBox1","copper")
         >>> icepak.assign_point_monitor(box.name, monitor_name="monitor2")
         "'monitor2'
         """
         if not isinstance(name, list):
             name = [name]
         if not isinstance(monitor_quantity, list):
             monitor_quantity = [monitor_quantity]
```

### Comparing `pyaedt-0.8.8/pyaedt/modules/report_templates.py` & `pyaedt-0.8.9/pyaedt/modules/report_templates.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/modules/solutions.py` & `pyaedt-0.8.9/pyaedt/modules/solutions.py`

 * *Files 1% similar despite different names*

```diff
@@ -3109,14 +3109,22 @@
 
         """
         try:
             if self.seeding_faces:
                 self.oField.CreateFieldPlot(self.surfacePlotInstructionLineTraces, "FieldLineTrace")
             else:
                 self.oField.CreateFieldPlot(self.surfacePlotInstruction, "Field")
+            if (
+                "Maxwell" in self._postprocessor._app.design_type
+                and "Transient" in self._postprocessor.post_solution_type
+            ):
+                self._postprocessor.ofieldsreporter.SetPlotsViewSolutionContext(
+                    [self.name], self.solution, "Time:" + self.intrinsics["Time"]
+                )
+            self._postprocessor.field_plots[self.name] = self
             return True
         except Exception:
             return False
 
     @pyaedt_function_handler()
     def update(self):
         """Update the field plot.
```

### Comparing `pyaedt-0.8.8/pyaedt/q3d.py` & `pyaedt-0.8.9/pyaedt/q3d.py`

 * *Files 2% similar despite different names*

```diff
@@ -96,61 +96,61 @@
 
         Returns
         -------
         List
         """
         return self.matrices[matrix_index].sources(is_gc_sources=is_gc_sources)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(source_names="assignment", rm_name="reduced_matrix")
     def insert_reduced_matrix(
         self,
         operation_name,
-        source_names=None,
-        rm_name=None,
+        assignment=None,
+        reduced_matrix=None,
         new_net_name=None,
         new_source_name=None,
         new_sink_name=None,
     ):
         """Insert a new reduced matrix.
 
         Parameters
         ----------
         operation_name : str
             Name of the operation to create.
-        source_names : list, str, optional
+        assignment : list, str, optional
             List of sources or nets or arguments needed for the operation. The default
             is ``None``.
-        rm_name : str, optional
+        reduced_matrix : str, optional
             Name of the reduced matrix. The default is ``None``.
         new_net_name : str, optional
             Name of the new net. The default is ``None``.
         new_source_name : str, optional
             Name of the new source. The default is ``None``.
         new_sink_name : str, optional
             Name of the new sink. The default is ``None``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.Matrix`
             Matrix object.
         """
-        if not rm_name:
-            rm_name = generate_unique_name(operation_name)
-        matrix = Matrix(self, rm_name, operation_name)
+        if not reduced_matrix:
+            reduced_matrix = generate_unique_name(operation_name)
+        matrix = Matrix(self, reduced_matrix, operation_name)
 
         if not new_net_name:
             new_net_name = generate_unique_name("Net")
 
         if not new_source_name:
             new_source_name = generate_unique_name("Source")
 
         if not new_sink_name:
             new_sink_name = generate_unique_name("Sink")
 
-        if matrix.create(source_names, new_net_name, new_source_name, new_sink_name):
+        if matrix.create(assignment, new_net_name, new_source_name, new_sink_name):
             self.matrices.append(matrix)
         return matrix
 
     @pyaedt_function_handler()
     def get_all_sources(self):
         """Get all setup sources.
 
@@ -883,20 +883,19 @@
 
         >>> oModule.ExportCircuit
 
         Examples
         --------
         >>> from pyaedt import Q3d
         >>> aedtapp = Q3d()
-        >>> box = aedtapp.modeler.create_box([30, 30, 30], [10, 10, 10], name="mybox")
-        >>> net = aedtapp.assign_net(box, "my_net")
+        >>> box = aedtapp.modeler.create_box([30, 30, 30],[10, 10, 10],name="mybox")
+        >>> net = aedtapp.assign_net(box,"my_net")
         >>> source = aedtapp.assign_source_to_objectface(box.bottom_face_z.id, axisdir=0,
         ...     source_name="Source1", net_name=net.name)
-        >>> sink = aedtapp.assign_sink_to_objectface(box.top_face_z.id, axisdir=0,
-        ...     sink_name="Sink1", net_name=net.name)
+        >>> sink = aedtapp.assign_sink_to_objectface(box.top_face_z.id,direction=0,name="Sink1",net_name=net.name)
         >>> aedtapp["d"] = "20mm"
         >>> aedtapp.modeler.duplicate_along_line(objid="Box1",vector=[0, "d", 0])
         >>> mysetup = aedtapp.create_setup()
         >>> aedtapp.analyze_setup(mysetup.name)
         >>> aedtapp.export_equivalent_circuit(file_name="test_export_circuit.cir",
         ...     setup_name=mysetup.name,
         ...     sweep="LastAdaptive",
@@ -1321,40 +1320,40 @@
         """Delete all nets in the design."""
         net_names = self.nets[::]
         for i in self.boundaries[::]:
             if i.name in net_names:
                 i.delete()
         return True
 
-    @pyaedt_function_handler()
-    def objects_from_nets(self, nets, materials=None):
+    @pyaedt_function_handler(nets="assignment")
+    def objects_from_nets(self, assignment, materials=None):
         """Find the objects that belong to one or more nets. You can filter by materials.
 
         Parameters
         ----------
-        nets : str, list
+        assignment : str, list
             One or more nets to search for. The search is case-insensitive.
         materials : str, list, optional
             One or more materials for filtering the net objects. The default
             is ``None``. The search is case insensitive.
 
         Returns
         -------
         dict
             Dictionary of net name and objects that belongs to it.
         """
-        if isinstance(nets, str):
-            nets = [nets]
+        if isinstance(assignment, str):
+            assignment = [assignment]
         if isinstance(materials, str):
             materials = [materials]
         elif not materials:
             materials = []
         materials = [i.lower() for i in materials]
         objects = {}
-        for net in nets:
+        for net in assignment:
             for bound in self.boundaries:
                 if net.lower() == bound.name.lower() and "Net" in bound.type:
                     obj_list = self.modeler.convert_to_selections(bound.props.get("Objects", []), True)
                     if materials:
                         obj_list = [
                             self.modeler[i].name for i in obj_list if self.modeler[i].material_name.lower() in materials
                         ]
@@ -1451,21 +1450,21 @@
             self._boundaries[bound.name] = bound
         if new_nets:
             self.logger.info("{} Nets have been identified: {}".format(len(new_nets), ", ".join(new_nets)))
         else:
             self.logger.info("No new nets identified")
         return True
 
-    @pyaedt_function_handler()
-    def assign_net(self, objects, net_name=None, net_type="Signal"):
+    @pyaedt_function_handler(objects="assignment")
+    def assign_net(self, assignment, net_name=None, net_type="Signal"):
         """Assign a net to a list of objects.
 
         Parameters
         ----------
-        objects : list, str
+        assignment : list, str
             List of objects to assign the net to. It can be a single object.
         net_name : str, optional
             Name of the net. The default is ```None``, in which case the
             default name is used.
         net_type : str, bool
             Type of net to create. Options are ``"Signal"``, ``"Ground"`` and ``"Floating"``.
             The default is ``"Signal"``.
@@ -1482,44 +1481,44 @@
         >>> oModule.AssignGroundNet
         >>> oModule.AssignFloatingNet
 
         Examples
         --------
         >>> from pyaedt import Q3d
         >>> q3d = Q3d()
-        >>> box = q3d.modeler.create_box([30, 30, 30], [10, 10, 10], name="mybox")
+        >>> box = q3d.modeler.create_box([30, 30, 30],[10, 10, 10],name="mybox")
         >>> net_name = "my_net"
-        >>> net = q3d.assign_net(box, net_name)
+        >>> net = q3d.assign_net(box,net_name)
         """
-        objects = self.modeler.convert_to_selections(objects, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
         if not net_name:
             net_name = generate_unique_name("Net")
-        props = OrderedDict({"Objects": objects})
+        props = OrderedDict({"Objects": assignment})
         type_bound = "SignalNet"
         if net_type.lower() == "ground":
             type_bound = "GroundNet"
         elif net_type.lower() == "floating":
             type_bound = "FloatingNet"
         bound = BoundaryObject(self, net_name, props, type_bound)
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def source(self, objects=None, axisdir=0, name=None, net_name=None, terminal_type="voltage"):
+    @pyaedt_function_handler(objects="assignment", axisdir="direction")
+    def source(self, assignment=None, direction=0, name=None, net_name=None, terminal_type="voltage"):
         """Generate a source on a face of an object or a group of faces or face ids.
         The face ID is selected based on the axis direction. It is the face that
         has the maximum/minimum in this axis direction.
 
         Parameters
         ----------
-        objects : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
+        assignment : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name of the object or face ID or face ID list.
-        axisdir : int, optional
+        direction : int, optional
             Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
         name : str, optional
             Name of the source. The default is ``None``.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
         terminal_type : str
             Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
@@ -1530,28 +1529,28 @@
             Source object.
 
         References
         ----------
 
         >>> oModule.AssignSource
         """
-        return self._assign_source_or_sink(objects, axisdir, name, net_name, terminal_type, "Source")
+        return self._assign_source_or_sink(assignment, direction, name, net_name, terminal_type, "Source")
 
-    @pyaedt_function_handler()
-    def sink(self, objects=None, axisdir=0, name=None, net_name=None, terminal_type="voltage"):
+    @pyaedt_function_handler(objects="assignment", axisdir="direction")
+    def sink(self, assignment=None, direction=0, name=None, net_name=None, terminal_type="voltage"):
         """Generate a sink on a face of an object or a group of faces or face ids.
 
         The face ID is selected based on the axis direction. It is the face that
         has the maximum/minimum in this axis direction.
 
         Parameters
         ----------
-        objects : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
+        assignment : str, int or list or :class:`pyaedt.modeler.cad.object3d.Object3d`
             Name of the object or face ID or face ID list.
-        axisdir : int, optional
+        direction : int, optional
             Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
         name : str, optional
             Name of the source. The default is ``None``.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
         terminal_type : str
             Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
@@ -1562,26 +1561,26 @@
             Sink object.
 
         References
         ----------
 
         >>> oModule.AssignSource
         """
-        return self._assign_source_or_sink(objects, axisdir, name, net_name, terminal_type, "Sink")
+        return self._assign_source_or_sink(assignment, direction, name, net_name, terminal_type, "Sink")
 
-    @pyaedt_function_handler()
-    def _assign_source_or_sink(self, objects, axisdir, name, net_name, terminal_type, exc_type):
+    @pyaedt_function_handler(objects="assignment", axisdir="direction")
+    def _assign_source_or_sink(self, assignment, direction, name, net_name, terminal_type, exc_type):
         if not name:
             name = generate_unique_name(exc_type)
-        objects = self.modeler.convert_to_selections(objects, True)
+        assignment = self.modeler.convert_to_selections(assignment, True)
         sheets = []
         is_face = True
-        for object_name in objects:
+        for object_name in assignment:
             if isinstance(object_name, str) and object_name in self.modeler.solid_names:
-                sheets.append(self.modeler._get_faceid_on_axis(object_name, axisdir))
+                sheets.append(self.modeler._get_faceid_on_axis(object_name, direction))
                 if not net_name:
                     for net in self.nets:
                         if object_name in self.objects_from_nets(net):
                             net_name = net
             elif isinstance(object_name, str):
                 is_face = False
                 sheets.append(object_name)
@@ -1603,179 +1602,116 @@
             props["Net"] = net_name
         bound = BoundaryObject(self, name, props, exc_type)
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_source_to_objectface(self, object_name, axisdir=0, source_name=None, net_name=None):
-        """Generate a source on a face of an object.
-
-        .. deprecated:: 0.6.70
-           Use :func:`source` method instead.
-
-        The face ID is selected based on the axis direction. It is the face that
-        has the maximum/minimum in this axis direction.
-
-        Parameters
-        ----------
-        object_name : str, int
-            Name of the object or face ID.
-        axisdir : int, optional
-            Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
-        source_name : str, optional
-            Name of the source. The default is ``None``.
-        net_name : str, optional
-            Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
-
-        Returns
-        -------
-        :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Source object.
-
-        References
-        ----------
-
-        >>> oModule.AssignSource
-        """
-        warnings.warn("Use :func:`source` method instead.", DeprecationWarning)
-        return self.source(objects=object_name, axisdir=0, name=source_name, net_name=net_name)
-
-    @pyaedt_function_handler()
-    def assign_source_to_sheet(
-        self, sheetname, objectname=None, netname=None, sourcename=None, terminal_type="voltage"
-    ):
-        """Generate a source on a sheet.
-
-        .. deprecated:: 0.6.70
-           Use :func:`source` method instead.
-
-        Parameters
-        ----------
-        sheetname : str, int or list
-            Name of the sheets to create the source on.
-        objectname :  str, optional
-            Name of the parent object. The default is ``None``.
-        netname : str, optional
-            Name of the net. The default is ``None``.
-        sourcename : str,  optional
-            Name of the source. The default is ``None``.
-        terminal_type : str
-            Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
-
-        Returns
-        -------
-        :class:`pyaedt.modules.Boundary.BoundaryObject`
-            Source object.
-
-        References
-        ----------
-
-        >>> oModule.AssignSource
-        """
-        warnings.warn("Use :func:`source` method instead.", DeprecationWarning)
-        return self.source(objects=sheetname, name=sourcename, net_name=netname, terminal_type=terminal_type)
-
-    @pyaedt_function_handler()
-    def assign_sink_to_objectface(self, object_name, axisdir=0, sink_name=None, net_name=None):
+    @pyaedt_function_handler(
+        object_name="assignment",
+        axisdir="direction",
+        sink_name="name",
+    )
+    def assign_sink_to_objectface(self, assignment, direction=0, name=None, net_name=None):
         """Generate a sink on a face of an object.
 
         The face ID is selected based on the axis direction. It is the face that has
         the maximum or minimum in this axis direction.
 
         Parameters
         ----------
-        object_name : str, int
+        assignment : str, int
             Name of the object or face ID.
-        axisdir : int, optional
+        direction : int, optional
             Initial axis direction. Options are ``0`` to ``5``. The default is ``0``.
-        sink_name : str, optional
+        name : str, optional
             Name of the sink. The default is ``None``.
         net_name : str, optional
             Name of the net. The default is ``None``, in which case the ``object_name`` is considered.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Sink object.
 
         References
         ----------
 
         >>> oModule.AssignSink
         """
-        object_name = self.modeler.convert_to_selections(object_name, True)[0]
-        if isinstance(object_name, int):
-            a = object_name
-            object_name = self.modeler.oeditor.GetObjectNameByFaceID(a)
+        assignment = self.modeler.convert_to_selections(assignment, True)[0]
+        if isinstance(assignment, int):
+            a = assignment
+            assignment = self.modeler.oeditor.GetObjectNameByFaceID(a)
         else:
-            a = self.modeler._get_faceid_on_axis(object_name, axisdir)
-        if not sink_name:
-            sink_name = generate_unique_name("Sink")
+            a = self.modeler._get_faceid_on_axis(assignment, direction)
+        if not name:
+            name = generate_unique_name("Sink")
         if not net_name:
-            net_name = object_name
+            net_name = assignment
         if a:
             props = OrderedDict(
-                {"Faces": [a], "ParentBndID": object_name, "TerminalType": "ConstantVoltage", "Net": net_name}
+                {"Faces": [a], "ParentBndID": assignment, "TerminalType": "ConstantVoltage", "Net": net_name}
             )
-            bound = BoundaryObject(self, sink_name, props, "Sink")
+            bound = BoundaryObject(self, name, props, "Sink")
             if bound.create():
                 self._boundaries[bound.name] = bound
                 return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_sink_to_sheet(self, sheetname, objectname=None, netname=None, sinkname=None, terminal_type="voltage"):
+    @pyaedt_function_handler(sheetname="assignment", objectname="object_name", netname="net_name", sinkname="sink_name")
+    def assign_sink_to_sheet(
+        self, assignment, object_name=None, net_name=None, sink_name=None, terminal_type="voltage"
+    ):
         """Generate a sink on a sheet.
 
         Parameters
         ----------
-        sheetname :
+        assignment :
             Name of the sheet to create the sink on.
-        objectname : str, optional
+        object_name : str, optional
             Name of the parent object. The default is ``None``.
-        netname : str, optional
+        net_name : str, optional
             Name of the net. The default is ``None``.
-        sinkname : str, optional
+        sink_name : str, optional
             Name of the sink. The default is ``None``.
         terminal_type : str
             Type of the terminal. Options are ``voltage`` and ``current``. The default is ``voltage``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Source object.
 
         References
         ----------
 
         >>> oModule.AssignSink
         """
-        if not sinkname:
-            sinkname = generate_unique_name("Sink")
-        sheetname = self.modeler.convert_to_selections(sheetname, True)[0]
-        if isinstance(sheetname, int):
-            props = OrderedDict({"Faces": [sheetname]})
-        else:
-            props = OrderedDict({"Objects": [sheetname]})
-        if objectname:
-            props["ParentBndID"] = objectname
+        if not sink_name:
+            sink_name = generate_unique_name("Sink")
+        assignment = self.modeler.convert_to_selections(assignment, True)[0]
+        if isinstance(assignment, int):
+            props = OrderedDict({"Faces": [assignment]})
+        else:
+            props = OrderedDict({"Objects": [assignment]})
+        if object_name:
+            props["ParentBndID"] = object_name
 
         if terminal_type == "current":
             terminal_str = "UniformCurrent"
         else:
             terminal_str = "ConstantVoltage"
 
         props["TerminalType"] = terminal_str
 
-        if netname:
-            props["Net"] = netname
+        if net_name:
+            props["Net"] = net_name
 
-        bound = BoundaryObject(self, sinkname, props, "Sink")
+        bound = BoundaryObject(self, sink_name, props, "Sink")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
     @pyaedt_function_handler()
     def create_frequency_sweep(self, setupname, units=None, freqstart=0, freqstop=1, freqstep=None, sweepname=None):
@@ -2136,105 +2072,105 @@
             aedt_process_id,
         )
         self.MATRIXOPERATIONS = MATRIXOPERATIONSQ2D()
 
     def _init_from_design(self, *args, **kwargs):
         self.__init__(*args, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_rectangle(self, position, dimension_list, name="", matname=""):
+    @pyaedt_function_handler(position="origin", dimension_list="sizes", matname="material")
+    def create_rectangle(self, origin, sizes, name="", material=""):
         """Create a rectangle.
 
         Parameters
         ----------
-        position : list
+        origin : list
             List of ``[x, y]`` coordinates for the starting point of the rectangle.
-        dimension_list : list
+        sizes : list
             List of ``[width, height]`` dimensions.
         name : str, optional
             Name of the rectangle. The default is ``None``, in which case
             the default name is assigned.
-        matname : str, optional
+        material : str, optional
             Name of the material. The default is ``None``, in which case
             the default material is used.
 
         Returns
         -------
         :class:`pyaedt.modeler.cad.object3d.Object3d`
             3D object.
 
         References
         ----------
 
         >>> oEditor.CreateRectangle
         """
-        return self.modeler.create_rectangle(position, dimension_list=dimension_list, name=name, matname=matname)
+        return self.modeler.create_rectangle(origin=origin, sizes=sizes, name=name, material=material)
 
-    @pyaedt_function_handler()
-    def assign_single_signal_line(self, target_objects, name="", solve_option="SolveInside", thickness=None, unit="um"):
+    @pyaedt_function_handler(target_objects="assignment", unit="units")
+    def assign_single_signal_line(self, assignment, name="", solve_option="SolveInside", thickness=None, units="um"):
         """Assign the conductor type to sheets.
 
         Parameters
         ----------
-        target_objects : list
+        assignment : list
             List of Object3D.
         name : str, optional
             Name of the conductor. The default is ``""``, in which case the default name is used.
         solve_option : str, optional
             Method for solving. Options are ``"SolveInside"``, ``"SolveOnBoundary"``, and ``"Automatic"``.
             The default is ``"SolveInside"``.
         thickness : float, optional
             Conductor thickness. The default is ``None``, in which case the conductor thickness
             is obtained by dividing the conductor's area by its perimeter (A/p). If multiple
             conductors are selected, the average conductor thickness is used.
-        unit : str, optional
+        units : str, optional
             Thickness unit. The default is ``"um"``.
 
         References
         ----------
 
         >>> oModule.AssignSingleSignalLine
         >>> oModule.AssignSingleReferenceGround
         """
 
         warnings.warn(
             "`assign_single_signal_line` is deprecated. Use `assign_single_conductor` instead.", DeprecationWarning
         )
-        self.assign_single_conductor(target_objects, name, "SignalLine", solve_option, thickness, unit)
+        self.assign_single_conductor(assignment, name, "SignalLine", solve_option, thickness, units)
 
-    @pyaedt_function_handler()
+    @pyaedt_function_handler(target_objects="assignment", unit="units")
     def assign_single_conductor(
         self,
-        target_objects,
+        assignment,
         name="",
         conductor_type="SignalLine",
         solve_option="SolveInside",
         thickness=None,
-        unit="um",
+        units="um",
     ):
         """
         Assign the conductor type to sheets.
 
         Parameters
         ----------
-        target_objects : list
+        assignment : list
             List of Object3D.
         name : str, optional
             Name of the conductor. The default is ``""``, in which case the default name is used.
         conductor_type : str
             Type of the conductor. Options are ``"SignalLine"`` and ``"ReferenceGround"``. The default is
             ``"SignalLine"``.
         solve_option : str, optional
             Method for solving. Options are ``"SolveInside"``, ``"SolveOnBoundary"``, and ``"Automatic"``.
             The default is ``"SolveInside"``.
         thickness : float, optional
             Conductor thickness. The default is ``None``, in which case the conductor thickness is obtained by dividing
             the conductor's area by its perimeter (A/p). If multiple conductors are selected, the average conductor
             thickness is used.
-        unit : str, optional
+        units : str, optional
             Thickness unit. The default is ``"um"``.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
             Source object.
 
@@ -2243,49 +2179,49 @@
 
         >>> oModule.AssignSingleSignalLine
         >>> oModule.AssignSingleReferenceGround
         """
         if not name:
             name = generate_unique_name(name)
 
-        if isinstance(target_objects, list):
-            a = target_objects
-            obj_names = [i.name for i in target_objects]
+        if isinstance(assignment, list):
+            a = assignment
+            obj_names = [i.name for i in assignment]
         else:
-            a = [target_objects]
-            obj_names = [target_objects.name]
+            a = [assignment]
+            obj_names = [assignment.name]
 
         if not thickness:
             t_list = []
             for t_obj in a:
                 perimeter = 0
                 for edge in t_obj.edges:
                     perimeter = perimeter + edge.length
                 t_list.append(t_obj.faces[0].area / perimeter)
             thickness = sum(t_list) / len(t_list)
 
-        props = OrderedDict({"Objects": obj_names, "SolveOption": solve_option, "Thickness": str(thickness) + unit})
+        props = OrderedDict({"Objects": obj_names, "SolveOption": solve_option, "Thickness": str(thickness) + units})
 
         bound = BoundaryObject(self, name, props, conductor_type)
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
         return False
 
-    @pyaedt_function_handler()
-    def assign_huray_finitecond_to_edges(self, edges, radius, ratio, unit="um", name=""):
+    @pyaedt_function_handler(edges="assignment", unit="units")
+    def assign_huray_finitecond_to_edges(self, assignment, radius, ratio, units="um", name=""):
         """
         Assign the Huray surface roughness model to edges.
 
         Parameters
         ----------
-        edges :
+        assignment :
         radius :
         ratio :
-        unit : str, optional
+        units : str, optional
             The default is ``"um"``.
         name : str, optional
             The default is ``""``, in which case the default name is used.
 
         Returns
         -------
         :class:`pyaedt.modules.Boundary.BoundaryObject`
@@ -2296,19 +2232,19 @@
 
         >>> oMdoule.AssignFiniteCond
         """
         if not name:
             name = generate_unique_name(name)
 
         if not isinstance(radius, str):
-            ra = str(radius) + unit
+            ra = str(radius) + units
         else:
             ra = radius
 
-        a = self.modeler.convert_to_selections(edges, True)
+        a = self.modeler.convert_to_selections(assignment, True)
 
         props = OrderedDict({"Edges": a, "UseCoating": False, "Radius": ra, "Ratio": str(ratio)})
 
         bound = BoundaryObject(self, name, props, "Finite Conductivity")
         if bound.create():
             self._boundaries[bound.name] = bound
             return bound
@@ -2458,34 +2394,34 @@
                             )
                             exported_files.append(export_path)
                             self.logger.info("Exported W-element: %s", export_path)
                         except Exception:  # pragma: no cover
                             self.logger.warning("Export W-element failed")
         return exported_files
 
-    @pyaedt_function_handler()
-    def toggle_conductor_type(self, conductor_name, new_type):
+    @pyaedt_function_handler(conductor_name="assignment")
+    def toggle_conductor_type(self, assignment, new_type):
         """Change the conductor type.
 
         Parameters
         ----------
-        conductor_name : str
+        assignment : str
             Name of the conductor to update.
         new_type : str
             New conductor type.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
         """
         try:
-            self.oboundary.ToggleConductor(conductor_name, new_type)
+            self.oboundary.ToggleConductor(assignment, new_type)
             for bound in self.boundaries:
-                if bound.name == conductor_name:
+                if bound.name == assignment:
                     bound.type = new_type
             self.logger.info("Conductor type correctly updated")
             return True
         except Exception:
             self.logger.error("Error in updating conductor type")
             return False
```

### Comparing `pyaedt-0.8.8/pyaedt/rmxprt.py` & `pyaedt-0.8.9/pyaedt/rmxprt.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/rpc/rpyc_services.py` & `pyaedt-0.8.9/pyaedt/rpc/rpyc_services.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/hdm_parser.py` & `pyaedt-0.8.9/pyaedt/sbrplus/hdm_parser.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/hdm_utils.py` & `pyaedt-0.8.9/pyaedt/sbrplus/hdm_utils.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/HdmObject.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/HdmObject.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/SbrBounceType.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/SbrBounceType.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/StopWatch.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/StopWatch.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/add_3dlight.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/add_3dlight.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/draw_rays1.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/draw_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/draw_wfobj.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/draw_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/filter_rays1.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/filter_rays1.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/filtered_tracks.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/filtered_tracks.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/ld_sbrplushdm.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/ld_sbrplushdm.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/ld_wfobj.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/ld_wfobj.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/matlab/validate_sfields.m` & `pyaedt-0.8.9/pyaedt/sbrplus/matlab/validate_sfields.m`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/sbrplus/plot.py` & `pyaedt-0.8.9/pyaedt/sbrplus/plot.py`

 * *Files identical despite different names*

### Comparing `pyaedt-0.8.8/pyaedt/twinbuilder.py` & `pyaedt-0.8.9/pyaedt/twinbuilder.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,43 +123,43 @@
             port,
             aedt_process_id,
         )
 
     def _init_from_design(self, *args, **kwargs):
         self.__init__(*args, **kwargs)
 
-    @pyaedt_function_handler()
-    def create_schematic_from_netlist(self, file_to_import):
+    @pyaedt_function_handler(file_to_import="input_file")
+    def create_schematic_from_netlist(self, input_file):
         """Create a circuit schematic from an HSpice net list.
 
         Supported currently are:
 
         * R
         * L
         * C
         * Diodes
         * Bjts
         * Discrete components with syntax ``Uxxx net1 net2 ... netn modname``
 
         Parameters
         ----------
-        file_to_import : str
+        input_file : str
             Full path to the HSpice file.
 
         Returns
         -------
         bool
             ``True`` when successful, ``False`` when failed.
 
         """
         xpos = 0
         ypos = 0
         delta = 0.0508
         use_instance = True
-        with open_file(file_to_import, "r") as f:
+        with open_file(input_file, "r") as f:
             for line in f:
                 mycomp = None
                 fields = line.split(" ")
                 name = fields[0]
                 if fields[0][0] == "R":
                     value = fields[3][fields[3].find("=") + 1 :].strip()
                     mycomp = self.modeler.schematic.create_resistor(
@@ -267,21 +267,21 @@
         ----------
 
         >>> oDesign.ChangeProperty
         """
         self.set_sim_setup_parameter("Hmax", expression)
         return True
 
-    @pyaedt_function_handler()
-    def set_sim_setup_parameter(self, var_str, expression, analysis_name="TR"):
+    @pyaedt_function_handler(var_str="variable")
+    def set_sim_setup_parameter(self, variable, expression, analysis_name="TR"):
         """Set simulation setup parameters.
 
         Parameters
         ----------
-        var_str : string
+        variable : string
             Name of the variable.
         expression :
 
         analysis_name : str, optional
             Name of the analysis. The default is ``"TR"``.
 
         Returns
@@ -304,15 +304,15 @@
 
         self._odesign.ChangeProperty(
             [
                 "NAME:AllTabs",
                 [
                     "NAME:BaseElementTab",
                     ["NAME:PropServers", analysis_name],
-                    ["NAME:ChangedProps", ["NAME:" + var_str, "Value:=", value_str]],
+                    ["NAME:ChangedProps", ["NAME:" + variable, "Value:=", value_str]],
                 ],
             ]
         )
         return True
 
     @pyaedt_function_handler(setup_name="setup", sweep_name="sweep")
     def add_q3d_dynamic_component(
```

### Comparing `pyaedt-0.8.8/pyproject.toml` & `pyaedt-0.8.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -82,18 +82,18 @@
     "pypandoc>=1.10.0,<1.14",
     #"pytest-sphinx",
     "pyvista>=0.38.0,<0.44",
     "recommonmark",
     #"scikit-learn",
     "scikit-rf>=0.30.0,<0.33",
     "Sphinx==5.3.0; python_version == '3.7'",
-    "Sphinx>=7.1.0,<7.3; python_version > '3.7'",
+    "Sphinx>=7.1.0,<7.4; python_version > '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.8'",
-    "sphinx-autobuild==2024.4.13; python_version > '3.8'",
+    "sphinx-autobuild==2024.4.16; python_version > '3.8'",
     #"sphinx-autodoc-typehints",
     "sphinx-copybutton>=0.5.0,<0.6",
     "sphinx-gallery>=0.14.0,<0.16",
     "sphinx-jinja>=2.0,<2.1",
     #"sphinx-notfound-page",
     "sphinx_design>=0.4.0,<0.6",
     #"sphinxcontrib-websupport",
@@ -104,18 +104,18 @@
 doc-noexamples = [
     "ansys-sphinx-theme>=0.10.0,<0.16",
     "imageio>=2.30.0,<2.35",
     #"imageio-ffmpeg",
     "numpydoc>=1.5.0,<1.8",
     # "recommonmark",
     "Sphinx==5.3.0; python_version == '3.7'",
-    "Sphinx>=7.1.0,<7.3; python_version > '3.7'",
+    "Sphinx>=7.1.0,<7.4; python_version > '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.7'",
     "sphinx-autobuild==2021.3.14; python_version == '3.8'",
-    "sphinx-autobuild==2024.4.13; python_version > '3.8'",
+    "sphinx-autobuild==2024.4.16; python_version > '3.8'",
     #"sphinx-autodoc-typehints",
     "sphinx-copybutton>=0.5.0,<0.6",
     "sphinx-gallery>=0.14.0,<0.16",
     #"sphinx-notfound-page",
     #"sphinxcontrib-websupport",
     "sphinx_design>=0.4.0,<0.6",
     "sphinx-jinja>=2.0,<2.1",
```

### Comparing `pyaedt-0.8.8/PKG-INFO` & `pyaedt-0.8.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyaedt
-Version: 0.8.8
+Version: 0.8.9
 Summary: Higher-Level Pythonic Ansys Electronics Desktop Framework
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: PyAEDT developers <massimo.capodiferro@ansys.com>
 Requires-Python: >=3.7,<4
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
@@ -46,33 +46,33 @@
 Requires-Dist: openpyxl>=3.0.0,<3.2 ; extra == "doc"
 Requires-Dist: osmnx>=1.1.0,<1.10 ; extra == "doc"
 Requires-Dist: pypandoc>=1.10.0,<1.14 ; extra == "doc"
 Requires-Dist: pyvista>=0.38.0,<0.44 ; extra == "doc"
 Requires-Dist: recommonmark ; extra == "doc"
 Requires-Dist: scikit-rf>=0.30.0,<0.33 ; extra == "doc"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc" and ( python_version == '3.7')
-Requires-Dist: Sphinx>=7.1.0,<7.3 ; extra == "doc" and ( python_version > '3.7')
+Requires-Dist: Sphinx>=7.1.0,<7.4 ; extra == "doc" and ( python_version > '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc" and ( python_version == '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc" and ( python_version == '3.8')
-Requires-Dist: sphinx-autobuild==2024.4.13 ; extra == "doc" and ( python_version > '3.8')
+Requires-Dist: sphinx-autobuild==2024.4.16 ; extra == "doc" and ( python_version > '3.8')
 Requires-Dist: sphinx-copybutton>=0.5.0,<0.6 ; extra == "doc"
 Requires-Dist: sphinx-gallery>=0.14.0,<0.16 ; extra == "doc"
 Requires-Dist: sphinx-jinja>=2.0,<2.1 ; extra == "doc"
 Requires-Dist: sphinx_design>=0.4.0,<0.6 ; extra == "doc"
 Requires-Dist: SRTM.py ; extra == "doc"
 Requires-Dist: utm ; extra == "doc"
 Requires-Dist: vtk==9.2.6 ; extra == "doc"
 Requires-Dist: ansys-sphinx-theme>=0.10.0,<0.16 ; extra == "doc-noexamples"
 Requires-Dist: imageio>=2.30.0,<2.35 ; extra == "doc-noexamples"
 Requires-Dist: numpydoc>=1.5.0,<1.8 ; extra == "doc-noexamples"
 Requires-Dist: Sphinx==5.3.0 ; extra == "doc-noexamples" and ( python_version == '3.7')
-Requires-Dist: Sphinx>=7.1.0,<7.3 ; extra == "doc-noexamples" and ( python_version > '3.7')
+Requires-Dist: Sphinx>=7.1.0,<7.4 ; extra == "doc-noexamples" and ( python_version > '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc-noexamples" and ( python_version == '3.7')
 Requires-Dist: sphinx-autobuild==2021.3.14 ; extra == "doc-noexamples" and ( python_version == '3.8')
-Requires-Dist: sphinx-autobuild==2024.4.13 ; extra == "doc-noexamples" and ( python_version > '3.8')
+Requires-Dist: sphinx-autobuild==2024.4.16 ; extra == "doc-noexamples" and ( python_version > '3.8')
 Requires-Dist: sphinx-copybutton>=0.5.0,<0.6 ; extra == "doc-noexamples"
 Requires-Dist: sphinx-gallery>=0.14.0,<0.16 ; extra == "doc-noexamples"
 Requires-Dist: sphinx_design>=0.4.0,<0.6 ; extra == "doc-noexamples"
 Requires-Dist: sphinx-jinja>=2.0,<2.1 ; extra == "doc-noexamples"
 Requires-Dist: ansys-pythonnet>=3.1.0rc3 ; extra == "dotnet"
 Requires-Dist: cffi==1.15.1 ; extra == "dotnet" and ( platform_system=='Linux' and python_version == '3.7')
 Requires-Dist: cffi>=1.16.0,<1.17 ; extra == "dotnet" and ( platform_system=='Linux' and python_version > '3.7')
```
