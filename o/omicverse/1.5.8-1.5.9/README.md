# Comparing `tmp/omicverse-1.5.8.tar.gz` & `tmp/omicverse-1.5.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "omicverse-1.5.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "omicverse-1.5.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `omicverse-1.5.8.tar` & `omicverse-1.5.9.tar`

### file list

```diff
@@ -1,252 +1,262 @@
--rw-r--r--   0        0        0    35823 2022-09-03 17:16:03.066315 omicverse-1.5.8/LICENSE
--rw-r--r--   0        0        0     9309 2024-02-07 18:05:42.433784 omicverse-1.5.8/README.md
--rw-r--r--   0        0        0    14340 2024-01-10 14:32:56.132386 omicverse-1.5.8/omicverse/.DS_Store
--rw-r--r--   0        0        0      320 2022-09-07 04:15:30.431190 omicverse-1.5.8/omicverse/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     6148 2024-01-10 14:32:56.133683 omicverse-1.5.8/omicverse/CEFCON/.DS_Store
--rw-r--r--   0        0        0     5763 2024-01-10 14:32:23.544885 omicverse-1.5.8/omicverse/CEFCON/CEFCON.py
--rw-r--r--   0        0        0      578 2024-01-10 14:32:23.545017 omicverse-1.5.8/omicverse/CEFCON/__init__.py
--rw-r--r--   0        0        0    20088 2024-01-10 15:37:22.257813 omicverse-1.5.8/omicverse/CEFCON/cefcon_result_object.py
--rw-r--r--   0        0        0    25206 2024-02-07 18:05:42.434153 omicverse-1.5.8/omicverse/CEFCON/cell_lineage_GRN.py
--rw-r--r--   0        0        0    12749 2024-01-10 14:32:23.545595 omicverse-1.5.8/omicverse/CEFCON/datasets.py
--rw-r--r--   0        0        0    19274 2024-01-10 14:32:23.545769 omicverse-1.5.8/omicverse/CEFCON/driver_regulators.py
--rw-r--r--   0        0        0    10834 2024-01-10 14:32:23.545914 omicverse-1.5.8/omicverse/CEFCON/eval_utils.py
--rw-r--r--   0        0        0     1447 2024-01-10 14:32:23.546152 omicverse-1.5.8/omicverse/CEFCON/resources/__init__.py
--rw-r--r--   0        0        0    10200 2024-01-10 14:32:23.546316 omicverse-1.5.8/omicverse/CEFCON/resources/hs_hgnc_tfs_animaltfdb4.txt
--rw-r--r--   0        0        0    10199 2024-01-10 14:32:23.546477 omicverse-1.5.8/omicverse/CEFCON/resources/hs_hgnc_tfs_lambert2018.txt
--rw-r--r--   0        0        0    10775 2024-01-10 14:32:23.546633 omicverse-1.5.8/omicverse/CEFCON/resources/mm_mgi_tfs.txt
--rw-r--r--   0        0        0    10219 2024-01-10 14:32:23.546795 omicverse-1.5.8/omicverse/CEFCON/resources/mm_mgi_tfs_animaltfdb4.txt
--rw-r--r--   0        0        0    18943 2024-01-10 14:32:23.546975 omicverse-1.5.8/omicverse/CEFCON/utils.py
--rw-r--r--   0        0        0     1987 2023-09-10 17:39:18.150175 omicverse-1.5.8/omicverse/SEACells/Rscripts/chromVAR.R
--rw-r--r--   0        0        0       87 2023-09-10 17:39:18.150264 omicverse-1.5.8/omicverse/SEACells/Rscripts/tanay.R
--rw-r--r--   0        0        0       43 2024-01-03 07:00:21.024604 omicverse-1.5.8/omicverse/SEACells/__init__.py
--rwxr-xr-x   0        0        0     4422 2023-09-10 17:39:18.150400 omicverse-1.5.8/omicverse/SEACells/accessibility.py
--rw-r--r--   0        0        0     6700 2023-09-10 17:39:18.150670 omicverse-1.5.8/omicverse/SEACells/build_graph.py
--rw-r--r--   0        0        0     8749 2024-01-03 16:51:27.839894 omicverse-1.5.8/omicverse/SEACells/core.py
--rw-r--r--   0        0        0    28399 2024-02-23 20:47:29.546398 omicverse-1.5.8/omicverse/SEACells/cpu.py
--rw-r--r--   0        0        0    20804 2024-02-23 20:47:20.015169 omicverse-1.5.8/omicverse/SEACells/cpu_dense.py
--rw-r--r--   0        0        0     4565 2023-09-10 17:39:18.330939 omicverse-1.5.8/omicverse/SEACells/domainadapt.py
--rw-r--r--   0        0        0     5112 2024-01-05 09:29:13.339566 omicverse-1.5.8/omicverse/SEACells/evaluate.py
--rw-r--r--   0        0        0    12141 2024-02-23 20:48:32.048983 omicverse-1.5.8/omicverse/SEACells/genescores.py
--rw-r--r--   0        0        0    28340 2024-02-23 20:49:35.440996 omicverse-1.5.8/omicverse/SEACells/gpu.py
--rw-r--r--   0        0        0     5030 2023-09-10 17:39:18.331369 omicverse-1.5.8/omicverse/SEACells/plot.py
--rw-r--r--   0        0        0      302 2023-09-10 17:39:18.331431 omicverse-1.5.8/omicverse/SEACells/preprocess.py
--rw-r--r--   0        0        0     8601 2023-09-10 17:39:18.331539 omicverse-1.5.8/omicverse/SEACells/tfactivity.py
--rw-r--r--   0        0        0     3220 2024-02-23 20:50:14.766727 omicverse-1.5.8/omicverse/SEACells/utils.py
--rw-r--r--   0        0        0      119 2023-09-10 17:39:18.331687 omicverse-1.5.8/omicverse/SEACells/version.py
--rw-r--r--   0        0        0     1624 2023-11-19 13:27:17.805455 omicverse-1.5.8/omicverse/STAGATE_pyG/STAGATE.py
--rw-r--r--   0        0        0     3096 2023-11-19 13:27:17.805588 omicverse-1.5.8/omicverse/STAGATE_pyG/Train_STAGATE.py
--rw-r--r--   0        0        0      373 2023-11-19 13:27:17.805702 omicverse-1.5.8/omicverse/STAGATE_pyG/__init__.py
--rw-r--r--   0        0        0     9355 2023-11-19 14:32:48.008093 omicverse-1.5.8/omicverse/STAGATE_pyG/gat_conv.py
--rw-r--r--   0        0        0     9881 2023-11-19 13:46:14.331564 omicverse-1.5.8/omicverse/STAGATE_pyG/utils.py
--rw-r--r--   0        0        0     1629 2024-01-02 05:35:04.424748 omicverse-1.5.8/omicverse/STAligner/STALIGNER.py
--rw-r--r--   0        0        0    13944 2024-01-02 05:35:04.424887 omicverse-1.5.8/omicverse/STAligner/ST_utils.py
--rw-r--r--   0        0        0    11855 2024-01-10 14:32:23.547613 omicverse-1.5.8/omicverse/STAligner/gat_conv.py
--rw-r--r--   0        0        0     4830 2024-01-10 17:53:56.421303 omicverse-1.5.8/omicverse/STAligner/mnn_utils.py
--rw-r--r--   0        0        0    16871 2024-01-02 05:35:04.425259 omicverse-1.5.8/omicverse/STAligner/train_STAligner.py
--rw-r--r--   0        0        0      857 2024-02-22 10:39:31.491805 omicverse-1.5.8/omicverse/__init__.py
--rw-r--r--   0        0        0     6148 2023-04-03 18:27:15.377061 omicverse-1.5.8/omicverse/bulk/.DS_Store
--rw-r--r--   0        0        0    25320 2024-02-21 16:43:28.536550 omicverse-1.5.8/omicverse/bulk/_Deseq2.py
--rw-r--r--   0        0        0    21289 2024-02-07 18:05:42.434835 omicverse-1.5.8/omicverse/bulk/_Enrichment.py
--rw-r--r--   0        0        0    29240 2023-07-14 07:39:35.883647 omicverse-1.5.8/omicverse/bulk/_Gene_module.py
--rw-r--r--   0        0        0      629 2023-08-09 05:33:15.892865 omicverse-1.5.8/omicverse/bulk/__init__.py
--rw-r--r--   0        0        0   633338 2023-04-03 07:50:58.899031 omicverse-1.5.8/omicverse/bulk/_chm13.py
--rw-r--r--   0        0        0      502 2023-08-09 05:33:18.082174 omicverse-1.5.8/omicverse/bulk/_combat.py
--rw-r--r--   0        0        0     1633 2022-09-06 14:17:42.730883 omicverse-1.5.8/omicverse/bulk/_df_apply.py
--rw-r--r--   0        0        0    42804 2022-09-06 14:17:42.731609 omicverse-1.5.8/omicverse/bulk/_dynamicTree.py
--rw-r--r--   0        0        0     6919 2023-07-12 17:29:32.278344 omicverse-1.5.8/omicverse/bulk/_network.py
--rw-r--r--   0        0        0    12290 2023-04-05 17:42:26.435325 omicverse-1.5.8/omicverse/bulk/_tcga.py
--rw-r--r--   0        0        0      275 2023-05-27 07:42:00.305669 omicverse-1.5.8/omicverse/bulk2single/__init__.py
--rw-r--r--   0        0        0    17858 2023-11-13 14:58:09.745576 omicverse-1.5.8/omicverse/bulk2single/_bulk2single.py
--rw-r--r--   0        0        0      829 2023-09-07 10:19:48.804560 omicverse-1.5.8/omicverse/bulk2single/_bulkdeconvolve.py
--rw-r--r--   0        0        0    15889 2024-01-10 14:43:25.330930 omicverse-1.5.8/omicverse/bulk2single/_bulktrajblend.py
--rw-r--r--   0        0        0    29806 2023-05-06 16:11:04.140905 omicverse-1.5.8/omicverse/bulk2single/_map_utils.py
--rw-r--r--   0        0        0    24978 2023-05-17 10:51:23.881340 omicverse-1.5.8/omicverse/bulk2single/_map_utils1.py
--rw-r--r--   0        0        0    12746 2023-04-14 09:44:12.354770 omicverse-1.5.8/omicverse/bulk2single/_single2spatial.py
--rw-r--r--   0        0        0    10462 2023-05-14 07:19:07.135859 omicverse-1.5.8/omicverse/bulk2single/_utils.py
--rw-r--r--   0        0        0     8560 2023-04-06 07:00:58.204356 omicverse-1.5.8/omicverse/bulk2single/_vae.py
--rw-r--r--   0        0        0       48 2023-05-30 08:00:53.496990 omicverse-1.5.8/omicverse/cylib/README.rst
--rw-r--r--   0        0        0       25 2023-05-31 17:51:38.764877 omicverse-1.5.8/omicverse/cylib/__init__.py
--rw-r--r--   0        0        0     3338 2023-05-31 17:55:48.200546 omicverse-1.5.8/omicverse/cylib/fast_utils.py
--rw-r--r--   0        0        0     1313 2023-05-30 08:00:53.497082 omicverse-1.5.8/omicverse/data_files/README.md
--rw-r--r--   0        0        0      613 2023-05-30 08:00:53.497137 omicverse-1.5.8/omicverse/data_files/apoptosis_human.gmt
--rw-r--r--   0        0        0      598 2023-05-30 08:00:53.497199 omicverse-1.5.8/omicverse/data_files/apoptosis_mouse.gmt
--rw-r--r--   0        0        0  1277787 2023-05-30 08:00:53.501091 omicverse-1.5.8/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt
--rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501212 omicverse-1.5.8/omicverse/data_files/cell_cycle_human.gmt
--rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501283 omicverse-1.5.8/omicverse/data_files/cell_cycle_mouse.gmt
--rw-r--r--   0        0        0      222 2023-05-30 08:00:53.501354 omicverse-1.5.8/omicverse/data_files/emt_human.gmt
--rw-r--r--   0        0        0      230 2023-05-30 08:00:53.501426 omicverse-1.5.8/omicverse/data_files/gender_human.gmt
--rw-r--r--   0        0        0      142 2023-05-30 08:00:53.501498 omicverse-1.5.8/omicverse/data_files/gender_mouse.gmt
--rw-r--r--   0        0        0    48244 2023-05-30 08:00:53.501752 omicverse-1.5.8/omicverse/data_files/h.all.v7.5.1.symbols.gmt
--rw-r--r--   0        0        0     2725 2023-05-30 08:00:53.501840 omicverse-1.5.8/omicverse/data_files/human_lung.gmt
--rw-r--r--   0        0        0      743 2023-05-30 08:00:53.501906 omicverse-1.5.8/omicverse/data_files/human_t_cell_markers.gmt
--rw-r--r--   0        0        0      929 2023-05-30 08:00:53.502035 omicverse-1.5.8/omicverse/data_files/mitochondrial_genes_human.gmt
--rw-r--r--   0        0        0      930 2023-05-30 08:00:53.502100 omicverse-1.5.8/omicverse/data_files/mitochondrial_genes_mouse.gmt
--rw-r--r--   0        0        0      706 2023-05-30 08:00:53.502165 omicverse-1.5.8/omicverse/data_files/mouse_brain.gmt
--rw-r--r--   0        0        0     1931 2023-05-30 08:00:53.502238 omicverse-1.5.8/omicverse/data_files/mouse_liver.gmt
--rw-r--r--   0        0        0     4068 2023-05-30 08:00:53.502316 omicverse-1.5.8/omicverse/data_files/mouse_lung.gmt
--rw-r--r--   0        0        0      787 2023-05-30 08:00:53.502394 omicverse-1.5.8/omicverse/data_files/ribosomal_genes_human.gmt
--rw-r--r--   0        0        0      801 2023-05-30 08:00:53.502468 omicverse-1.5.8/omicverse/data_files/ribosomal_genes_mouse.gmt
--rw-r--r--   0        0        0       55 2022-09-07 09:33:07.470218 omicverse-1.5.8/omicverse/mofapy2/__init__.py
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.470284 omicverse-1.5.8/omicverse/mofapy2/build_model/__init__.py
--rw-r--r--   0        0        0    13189 2022-09-07 10:12:11.559603 omicverse-1.5.8/omicverse/mofapy2/build_model/build_model.py
--rw-r--r--   0        0        0    28425 2022-09-07 10:12:16.240298 omicverse-1.5.8/omicverse/mofapy2/build_model/init_model.py
--rw-r--r--   0        0        0    25076 2022-09-07 10:12:21.681277 omicverse-1.5.8/omicverse/mofapy2/build_model/save_model.py
--rw-r--r--   0        0        0      637 2022-09-07 10:12:26.660116 omicverse-1.5.8/omicverse/mofapy2/build_model/train_model.py
--rw-r--r--   0        0        0     3366 2022-09-07 10:12:30.366961 omicverse-1.5.8/omicverse/mofapy2/build_model/utils.py
--rw-r--r--   0        0        0      405 2022-09-07 09:33:07.470940 omicverse-1.5.8/omicverse/mofapy2/config.py
--rw-r--r--   0        0        0    26036 2022-09-07 10:13:08.257046 omicverse-1.5.8/omicverse/mofapy2/core/BayesNet.py
--rw-r--r--   0        0        0       21 2022-09-07 09:33:07.471206 omicverse-1.5.8/omicverse/mofapy2/core/__init__.py
--rw-r--r--   0        0        0      448 2022-09-07 09:33:07.471309 omicverse-1.5.8/omicverse/mofapy2/core/distributions/__init__.py
--rw-r--r--   0        0        0     3923 2022-09-07 09:33:07.471393 omicverse-1.5.8/omicverse/mofapy2/core/distributions/basic_distributions.py
--rw-r--r--   0        0        0     1301 2022-09-07 10:20:27.422096 omicverse-1.5.8/omicverse/mofapy2/core/distributions/bernoulli.py
--rw-r--r--   0        0        0     4709 2022-09-07 10:20:18.413617 omicverse-1.5.8/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py
--rw-r--r--   0        0        0     1859 2022-09-07 10:20:33.345355 omicverse-1.5.8/omicverse/mofapy2/core/distributions/beta.py
--rw-r--r--   0        0        0     1928 2022-09-07 10:20:37.394428 omicverse-1.5.8/omicverse/mofapy2/core/distributions/binomial.py
--rw-r--r--   0        0        0     2061 2022-09-07 10:20:40.951879 omicverse-1.5.8/omicverse/mofapy2/core/distributions/gamma.py
--rw-r--r--   0        0        0    38150 2022-09-07 09:33:07.471983 omicverse-1.5.8/omicverse/mofapy2/core/distributions/multi_task_GP.py
--rw-r--r--   0        0        0    16083 2022-09-07 10:20:53.092939 omicverse-1.5.8/omicverse/mofapy2/core/distributions/multivariate_gaussian.py
--rw-r--r--   0        0        0     1663 2022-09-07 10:20:57.661446 omicverse-1.5.8/omicverse/mofapy2/core/distributions/poisson.py
--rw-r--r--   0        0        0     2223 2022-09-07 10:21:03.520320 omicverse-1.5.8/omicverse/mofapy2/core/distributions/univariate_gaussian.py
--rw-r--r--   0        0        0     5591 2022-09-07 09:33:07.472344 omicverse-1.5.8/omicverse/mofapy2/core/gp_utils.py
--rw-r--r--   0        0        0     1765 2022-09-07 09:33:07.472409 omicverse-1.5.8/omicverse/mofapy2/core/gpu_utils.py
--rw-r--r--   0        0        0     6291 2022-09-07 09:33:07.472554 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Alpha_nodes.py
--rw-r--r--   0        0        0     4646 2022-09-07 10:16:08.287697 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Kc_node.py
--rw-r--r--   0        0        0     3581 2022-09-07 10:16:52.659105 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Kg_node.py
--rw-r--r--   0        0        0    49309 2022-09-07 10:22:30.858460 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Sigma_node.py
--rwxr-xr-x   0        0        0     5327 2022-09-07 10:18:15.524786 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Tau_nodes.py
--rw-r--r--   0        0        0     6551 2022-09-07 09:33:07.473126 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Theta_nodes.py
--rw-r--r--   0        0        0     7911 2022-09-07 10:18:33.209503 omicverse-1.5.8/omicverse/mofapy2/core/nodes/U_nodes.py
--rwxr-xr-x   0        0        0    10037 2022-09-07 10:18:50.380099 omicverse-1.5.8/omicverse/mofapy2/core/nodes/W_nodes.py
--rw-r--r--   0        0        0     3577 2022-09-07 10:18:59.577240 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Y_nodes.py
--rwxr-xr-x   0        0        0    15625 2022-09-07 10:19:28.866210 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes.py
--rw-r--r--   0        0        0     9248 2022-09-07 10:19:17.982574 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes_GP.py
--rw-r--r--   0        0        0     8127 2022-09-07 10:19:10.770163 omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py
--rw-r--r--   0        0        0     7505 2022-09-07 10:19:37.520420 omicverse-1.5.8/omicverse/mofapy2/core/nodes/ZgU_node.py
--rw-r--r--   0        0        0      581 2022-09-07 09:33:07.473827 omicverse-1.5.8/omicverse/mofapy2/core/nodes/__init__.py
--rw-r--r--   0        0        0     3812 2022-09-07 10:14:43.810952 omicverse-1.5.8/omicverse/mofapy2/core/nodes/basic_nodes.py
--rw-r--r--   0        0        0     6837 2022-09-07 09:33:07.473999 omicverse-1.5.8/omicverse/mofapy2/core/nodes/multiview_nodes.py
--rw-r--r--   0        0        0    21096 2022-09-07 10:17:25.117004 omicverse-1.5.8/omicverse/mofapy2/core/nodes/nongaussian_nodes.py
--rw-r--r--   0        0        0    11994 2022-09-07 10:18:40.408370 omicverse-1.5.8/omicverse/mofapy2/core/nodes/variational_nodes.py
--rw-r--r--   0        0        0     3764 2022-09-07 09:33:07.474508 omicverse-1.5.8/omicverse/mofapy2/core/utils.py
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.474782 omicverse-1.5.8/omicverse/mofapy2/run/__init__.py
--rw-r--r--   0        0        0    70968 2023-05-18 07:48:53.001053 omicverse-1.5.8/omicverse/mofapy2/run/entry_point.py
--rw-r--r--   0        0        0   324931 2022-09-07 09:33:07.476317 omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_0.txt
--rw-r--r--   0        0        0   324642 2022-09-07 09:33:07.477843 omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_1.txt
--rw-r--r--   0        0        0   324951 2022-09-07 09:33:07.478979 omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_2.txt
--rw-r--r--   0        0        0   996145 2022-09-07 09:33:07.483410 omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_0.txt
--rw-r--r--   0        0        0   996423 2022-09-07 09:33:07.486212 omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_1.txt
--rw-r--r--   0        0        0   995502 2022-09-07 09:33:07.486904 omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_2.txt
--rw-r--r--   0        0        0        0 2022-09-07 09:33:07.486988 omicverse-1.5.8/omicverse/mofapy2/simulate/__init__.py
--rw-r--r--   0        0        0     6509 2022-09-07 10:10:46.603319 omicverse-1.5.8/omicverse/mofapy2/simulate/simulate_mofa.py
--rw-r--r--   0        0        0       22 2022-09-07 09:33:07.487160 omicverse-1.5.8/omicverse/mofapy2/version.py
--rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py
--rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py
--rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py
--rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.078134 omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0      120 2022-09-07 04:15:14.079001 omicverse-1.5.8/omicverse/nocd/__init__.py
--rw-r--r--   0        0        0     2163 2022-09-07 04:15:14.083601 omicverse-1.5.8/omicverse/nocd/data.py
--rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.5.8/omicverse/nocd/generate.py
--rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.5.8/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py
--rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.085633 omicverse-1.5.8/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py
--rw-r--r--   0        0        0       54 2022-09-07 04:15:14.086034 omicverse-1.5.8/omicverse/nocd/metrics/__init__.py
--rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.5.8/omicverse/nocd/metrics/supervised.py
--rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.089087 omicverse-1.5.8/omicverse/nocd/metrics/unsupervised.py
--rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py
--rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py
--rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py
--rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.5.8/omicverse/nocd/nn/__init__.py
--rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.5.8/omicverse/nocd/nn/decoder.py
--rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.5.8/omicverse/nocd/nn/gcn.py
--rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.5.8/omicverse/nocd/nn/imrpoved_gcn.py
--rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.5.8/omicverse/nocd/sampler.py
--rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.5.8/omicverse/nocd/train.py
--rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.093413 omicverse-1.5.8/omicverse/nocd/utils.py
--rw-r--r--   0        0        0      306 2023-11-16 15:26:26.581114 omicverse-1.5.8/omicverse/palantir/__init__.py
--rw-r--r--   0        0        0      248 2023-11-16 15:35:54.712851 omicverse-1.5.8/omicverse/palantir/config.py
--rw-r--r--   0        0        0    20843 2023-11-16 15:37:03.805608 omicverse-1.5.8/omicverse/palantir/core.py
--rw-r--r--   0        0        0     3481 2023-11-16 15:32:44.282139 omicverse-1.5.8/omicverse/palantir/io.py
--rw-r--r--   0        0        0    73306 2023-11-16 15:36:17.002907 omicverse-1.5.8/omicverse/palantir/plot.py
--rw-r--r--   0        0        0     1459 2023-11-16 15:26:26.581668 omicverse-1.5.8/omicverse/palantir/preprocess.py
--rw-r--r--   0        0        0    20923 2023-11-16 15:35:47.772593 omicverse-1.5.8/omicverse/palantir/presults.py
--rw-r--r--   0        0        0    33510 2023-11-16 20:46:00.233185 omicverse-1.5.8/omicverse/palantir/utils.py
--rw-r--r--   0        0        0     5570 2023-11-16 15:26:26.582123 omicverse-1.5.8/omicverse/palantir/validation.py
--rw-r--r--   0        0        0      107 2023-11-19 13:09:57.850190 omicverse-1.5.8/omicverse/palantir/version.py
--rw-r--r--   0        0        0      137 2024-02-21 16:16:00.957288 omicverse-1.5.8/omicverse/pl/__init__.py
--rw-r--r--   0        0        0    10364 2024-02-23 20:33:22.783257 omicverse-1.5.8/omicverse/pl/_bulk.py
--rw-r--r--   0        0        0      330 2024-01-29 14:46:01.259775 omicverse-1.5.8/omicverse/pl/_general.py
--rw-r--r--   0        0        0    13984 2024-02-21 15:37:30.787564 omicverse-1.5.8/omicverse/pl/_heatmap.py
--rw-r--r--   0        0        0     7298 2024-02-12 10:18:03.192092 omicverse-1.5.8/omicverse/pl/_multi.py
--rw-r--r--   0        0        0     2921 2024-02-15 15:09:29.425724 omicverse-1.5.8/omicverse/pl/_palette.py
--rw-r--r--   0        0        0    26187 2024-02-21 15:36:25.350638 omicverse-1.5.8/omicverse/pl/_single.py
--rw-r--r--   0        0        0      600 2024-01-30 10:48:56.294041 omicverse-1.5.8/omicverse/pp/__init__.py
--rw-r--r--   0        0        0    27228 2024-01-30 10:48:44.037699 omicverse-1.5.8/omicverse/pp/_preprocess.py
--rw-r--r--   0        0        0    17176 2024-02-10 13:56:53.047422 omicverse-1.5.8/omicverse/pp/_qc.py
--rw-r--r--   0        0        0     6148 2023-07-05 12:55:01.552000 omicverse-1.5.8/omicverse/single/.DS_Store
--rw-r--r--   0        0        0     8790 2022-09-03 17:16:03.070397 omicverse-1.5.8/omicverse/single/README.md
--rw-r--r--   0        0        0    61426 2023-06-26 23:50:36.692480 omicverse-1.5.8/omicverse/single/_SCSA.py
--rw-r--r--   0        0        0     1215 2024-02-23 21:29:48.898564 omicverse-1.5.8/omicverse/single/__init__.py
--rw-r--r--   0        0        0    28030 2023-12-28 10:37:02.673733 omicverse-1.5.8/omicverse/single/_anno.py
--rw-r--r--   0        0        0    10196 2023-08-15 09:58:12.551350 omicverse-1.5.8/omicverse/single/_atac.py
--rw-r--r--   0        0        0     9656 2024-01-10 14:32:23.549507 omicverse-1.5.8/omicverse/single/_aucell.py
--rw-r--r--   0        0        0     3407 2023-12-12 07:25:16.476686 omicverse-1.5.8/omicverse/single/_batch.py
--rw-r--r--   0        0        0    19489 2024-01-10 14:56:03.811609 omicverse-1.5.8/omicverse/single/_cefcon.py
--rw-r--r--   0        0        0    32142 2024-02-20 07:59:48.545882 omicverse-1.5.8/omicverse/single/_cellfategenie.py
--rwxr-xr-x   0        0        0    21100 2022-09-07 05:59:40.809184 omicverse-1.5.8/omicverse/single/_cosg.py
--rw-r--r--   0        0        0    12142 2023-07-04 04:23:59.889080 omicverse-1.5.8/omicverse/single/_cpdb.py
--rw-r--r--   0        0        0    32028 2023-08-28 19:22:48.553542 omicverse-1.5.8/omicverse/single/_ltnn.py
--rw-r--r--   0        0        0    20556 2024-01-30 09:16:15.392857 omicverse-1.5.8/omicverse/single/_mdic3.py
--rw-r--r--   0        0        0     5551 2024-02-23 21:27:18.590762 omicverse-1.5.8/omicverse/single/_metacell.py
--rw-r--r--   0        0        0    38177 2023-08-08 08:04:00.711068 omicverse-1.5.8/omicverse/single/_mofa.py
--rw-r--r--   0        0        0    11678 2024-01-10 14:44:12.836094 omicverse-1.5.8/omicverse/single/_nocd.py
--rw-r--r--   0        0        0     4589 2023-07-23 08:19:07.196675 omicverse-1.5.8/omicverse/single/_scannorl.py
--rw-r--r--   0        0        0    18135 2023-04-03 15:03:48.751508 omicverse-1.5.8/omicverse/single/_scdrug.py
--rw-r--r--   0        0        0    13608 2023-07-08 08:47:26.522256 omicverse-1.5.8/omicverse/single/_scgsea.py
--rw-r--r--   0        0        0        0 2023-08-19 13:26:01.097674 omicverse-1.5.8/omicverse/single/_seacells.py
--rw-r--r--   0        0        0     7303 2024-01-30 10:37:15.236907 omicverse-1.5.8/omicverse/single/_simba.py
--rw-r--r--   0        0        0    18296 2023-07-11 04:31:16.370357 omicverse-1.5.8/omicverse/single/_tosica.py
--rw-r--r--   0        0        0     4218 2023-11-16 20:07:20.519890 omicverse-1.5.8/omicverse/single/_traj.py
--rw-r--r--   0        0        0    76688 2024-02-19 20:43:08.500848 omicverse-1.5.8/omicverse/single/_via.py
--rw-r--r--   0        0        0      149 2024-01-06 19:48:26.581590 omicverse-1.5.8/omicverse/space/__init__.py
--rw-r--r--   0        0        0     4913 2024-01-06 19:47:57.665850 omicverse-1.5.8/omicverse/space/_cluster.py
--rw-r--r--   0        0        0    12205 2024-01-10 14:32:23.549911 omicverse-1.5.8/omicverse/space/_integrate.py
--rw-r--r--   0        0        0     7451 2024-02-07 18:05:42.436346 omicverse-1.5.8/omicverse/space/_spaceflow.py
--rw-r--r--   0        0        0     3292 2023-12-12 07:25:30.770192 omicverse-1.5.8/omicverse/space/_tangram.py
--rw-r--r--   0        0        0    27318 2024-02-07 18:05:42.436550 omicverse-1.5.8/omicverse/spaceflow/_SpaceFlow.py
--rw-r--r--   0        0        0       54 2024-02-07 18:05:42.436663 omicverse-1.5.8/omicverse/spaceflow/__init__.py
--rw-r--r--   0        0        0      361 2024-02-07 18:05:42.436756 omicverse-1.5.8/omicverse/spaceflow/_util.py
--rw-r--r--   0        0        0      108 2023-11-13 14:40:19.151431 omicverse-1.5.8/omicverse/tape/__init__.py
--rw-r--r--   0        0        0     7521 2023-09-28 09:40:35.361223 omicverse-1.5.8/omicverse/tape/deconvolution.py
--rw-r--r--   0        0        0     7953 2023-09-28 09:40:50.694373 omicverse-1.5.8/omicverse/tape/model.py
--rw-r--r--   0        0        0     6097 2023-09-28 09:41:17.053043 omicverse-1.5.8/omicverse/tape/simulation.py
--rw-r--r--   0        0        0     6726 2023-09-28 09:41:28.452046 omicverse-1.5.8/omicverse/tape/train.py
--rw-r--r--   0        0        0     6585 2023-09-28 14:24:10.730906 omicverse-1.5.8/omicverse/tape/utils.py
--rw-r--r--   0        0        0    11399 2023-07-08 08:54:04.442016 omicverse-1.5.8/omicverse/tosica/TOSICA_model.py
--rw-r--r--   0        0        0      184 2023-07-05 16:39:57.238794 omicverse-1.5.8/omicverse/tosica/__init__.py
--rw-r--r--   0        0        0     5669 2023-07-05 12:56:02.375603 omicverse-1.5.8/omicverse/tosica/customized_linear.py
--rw-r--r--   0        0        0    11304 2023-07-05 15:46:55.560572 omicverse-1.5.8/omicverse/tosica/pre.py
--rw-r--r--   0        0        0    13384 2023-07-11 04:33:48.020024 omicverse-1.5.8/omicverse/tosica/train.py
--rw-r--r--   0        0        0     1111 2023-12-04 20:09:51.594263 omicverse-1.5.8/omicverse/utils/__init__.py
--rw-r--r--   0        0        0     6217 2024-01-04 17:08:18.979832 omicverse-1.5.8/omicverse/utils/_cluster.py
--rw-r--r--   0        0        0    21401 2023-08-28 19:25:33.751561 omicverse-1.5.8/omicverse/utils/_data.py
--rw-r--r--   0        0        0     2343 2023-06-01 08:49:06.326555 omicverse-1.5.8/omicverse/utils/_enum.py
--rw-r--r--   0        0        0    20217 2023-07-08 08:44:29.300351 omicverse-1.5.8/omicverse/utils/_genomics.py
--rw-r--r--   0        0        0    20837 2023-08-18 14:13:31.420310 omicverse-1.5.8/omicverse/utils/_heatmap.py
--rw-r--r--   0        0        0     5370 2023-08-08 16:27:48.029476 omicverse-1.5.8/omicverse/utils/_knn.py
--rw-r--r--   0        0        0     2520 2023-05-27 07:38:06.457609 omicverse-1.5.8/omicverse/utils/_mde.py
--rw-r--r--   0        0        0    16487 2023-09-26 17:14:22.181959 omicverse-1.5.8/omicverse/utils/_paga.py
--rw-r--r--   0        0        0    38859 2024-02-23 20:30:28.817553 omicverse-1.5.8/omicverse/utils/_plot.py
--rw-r--r--   0        0        0     5008 2023-08-31 10:23:54.166327 omicverse-1.5.8/omicverse/utils/_roe.py
--rw-r--r--   0        0        0    48995 2024-01-29 13:46:13.992761 omicverse-1.5.8/omicverse/utils/_scatterplot.py
--rw-r--r--   0        0        0     4169 2023-09-26 16:51:08.413978 omicverse-1.5.8/omicverse/utils/_syn.py
--rw-r--r--   0        0        0     5765 2023-12-04 20:09:39.026475 omicverse-1.5.8/omicverse/utils/_venn.py
--rw-r--r--   0        0        0      441 2023-04-07 07:58:16.954693 omicverse-1.5.8/omicverse/via/.idea/VIA.iml
--rw-r--r--   0        0        0      143 2023-04-07 07:58:16.954828 omicverse-1.5.8/omicverse/via/__init__.py
--rw-r--r--   0        0        0   195095 2024-02-21 15:13:58.278501 omicverse-1.5.8/omicverse/via/core.py
--rw-r--r--   0        0        0    10436 2023-07-04 11:16:15.075797 omicverse-1.5.8/omicverse/via/datasets_via.py
--rw-r--r--   0        0        0   160696 2024-02-21 15:13:19.841598 omicverse-1.5.8/omicverse/via/examples.py
--rw-r--r--   0        0        0   145530 2023-04-07 16:00:02.788869 omicverse-1.5.8/omicverse/via/plotting_via.py
--rw-r--r--   0        0        0    75612 2023-10-17 15:06:18.715265 omicverse-1.5.8/omicverse/via/utils_via.py
--rw-r--r--   0        0        0     7987 2023-04-07 07:58:16.958047 omicverse-1.5.8/omicverse/via/windmap.py
--rw-r--r--   0        0        0     1942 2024-02-15 16:47:09.906339 omicverse-1.5.8/pyproject.toml
--rw-r--r--   0        0        0    11314 1970-01-01 00:00:00.000000 omicverse-1.5.8/PKG-INFO
+-rw-r--r--   0        0        0    35823 2022-09-03 17:16:03.066315 omicverse-1.5.9/LICENSE
+-rw-r--r--   0        0        0     9783 2024-05-07 07:32:17.353765 omicverse-1.5.9/README.md
+-rw-r--r--   0        0        0    14340 2024-04-04 13:18:25.816042 omicverse-1.5.9/omicverse/.DS_Store
+-rw-r--r--   0        0        0      320 2022-09-07 04:15:30.431190 omicverse-1.5.9/omicverse/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     6148 2024-01-10 14:32:56.133683 omicverse-1.5.9/omicverse/CEFCON/.DS_Store
+-rw-r--r--   0        0        0     5763 2024-01-10 14:32:23.544885 omicverse-1.5.9/omicverse/CEFCON/CEFCON.py
+-rw-r--r--   0        0        0      578 2024-01-10 14:32:23.545017 omicverse-1.5.9/omicverse/CEFCON/__init__.py
+-rw-r--r--   0        0        0    20088 2024-01-10 15:37:22.257813 omicverse-1.5.9/omicverse/CEFCON/cefcon_result_object.py
+-rw-r--r--   0        0        0    25206 2024-02-07 18:05:42.434153 omicverse-1.5.9/omicverse/CEFCON/cell_lineage_GRN.py
+-rw-r--r--   0        0        0    12749 2024-01-10 14:32:23.545595 omicverse-1.5.9/omicverse/CEFCON/datasets.py
+-rw-r--r--   0        0        0    19274 2024-01-10 14:32:23.545769 omicverse-1.5.9/omicverse/CEFCON/driver_regulators.py
+-rw-r--r--   0        0        0    10834 2024-01-10 14:32:23.545914 omicverse-1.5.9/omicverse/CEFCON/eval_utils.py
+-rw-r--r--   0        0        0     1447 2024-01-10 14:32:23.546152 omicverse-1.5.9/omicverse/CEFCON/resources/__init__.py
+-rw-r--r--   0        0        0    10200 2024-01-10 14:32:23.546316 omicverse-1.5.9/omicverse/CEFCON/resources/hs_hgnc_tfs_animaltfdb4.txt
+-rw-r--r--   0        0        0    10199 2024-01-10 14:32:23.546477 omicverse-1.5.9/omicverse/CEFCON/resources/hs_hgnc_tfs_lambert2018.txt
+-rw-r--r--   0        0        0    10775 2024-01-10 14:32:23.546633 omicverse-1.5.9/omicverse/CEFCON/resources/mm_mgi_tfs.txt
+-rw-r--r--   0        0        0    10219 2024-01-10 14:32:23.546795 omicverse-1.5.9/omicverse/CEFCON/resources/mm_mgi_tfs_animaltfdb4.txt
+-rw-r--r--   0        0        0    18943 2024-01-10 14:32:23.546975 omicverse-1.5.9/omicverse/CEFCON/utils.py
+-rw-r--r--   0        0        0     1987 2023-09-10 17:39:18.150175 omicverse-1.5.9/omicverse/SEACells/Rscripts/chromVAR.R
+-rw-r--r--   0        0        0       87 2023-09-10 17:39:18.150264 omicverse-1.5.9/omicverse/SEACells/Rscripts/tanay.R
+-rw-r--r--   0        0        0       43 2024-01-03 07:00:21.024604 omicverse-1.5.9/omicverse/SEACells/__init__.py
+-rwxr-xr-x   0        0        0     4422 2023-09-10 17:39:18.150400 omicverse-1.5.9/omicverse/SEACells/accessibility.py
+-rw-r--r--   0        0        0     6700 2023-09-10 17:39:18.150670 omicverse-1.5.9/omicverse/SEACells/build_graph.py
+-rw-r--r--   0        0        0     8749 2024-01-03 16:51:27.839894 omicverse-1.5.9/omicverse/SEACells/core.py
+-rw-r--r--   0        0        0    28399 2024-02-23 20:47:29.546398 omicverse-1.5.9/omicverse/SEACells/cpu.py
+-rw-r--r--   0        0        0    20804 2024-02-23 20:47:20.015169 omicverse-1.5.9/omicverse/SEACells/cpu_dense.py
+-rw-r--r--   0        0        0     4565 2023-09-10 17:39:18.330939 omicverse-1.5.9/omicverse/SEACells/domainadapt.py
+-rw-r--r--   0        0        0     5112 2024-01-05 09:29:13.339566 omicverse-1.5.9/omicverse/SEACells/evaluate.py
+-rw-r--r--   0        0        0    12141 2024-02-23 20:48:32.048983 omicverse-1.5.9/omicverse/SEACells/genescores.py
+-rw-r--r--   0        0        0    28340 2024-02-23 20:49:35.440996 omicverse-1.5.9/omicverse/SEACells/gpu.py
+-rw-r--r--   0        0        0     5030 2023-09-10 17:39:18.331369 omicverse-1.5.9/omicverse/SEACells/plot.py
+-rw-r--r--   0        0        0      302 2023-09-10 17:39:18.331431 omicverse-1.5.9/omicverse/SEACells/preprocess.py
+-rw-r--r--   0        0        0     8601 2023-09-10 17:39:18.331539 omicverse-1.5.9/omicverse/SEACells/tfactivity.py
+-rw-r--r--   0        0        0     3220 2024-02-23 20:50:14.766727 omicverse-1.5.9/omicverse/SEACells/utils.py
+-rw-r--r--   0        0        0      119 2023-09-10 17:39:18.331687 omicverse-1.5.9/omicverse/SEACells/version.py
+-rw-r--r--   0        0        0     1624 2023-11-19 13:27:17.805455 omicverse-1.5.9/omicverse/STAGATE_pyG/STAGATE.py
+-rw-r--r--   0        0        0     3096 2023-11-19 13:27:17.805588 omicverse-1.5.9/omicverse/STAGATE_pyG/Train_STAGATE.py
+-rw-r--r--   0        0        0      373 2023-11-19 13:27:17.805702 omicverse-1.5.9/omicverse/STAGATE_pyG/__init__.py
+-rw-r--r--   0        0        0     9355 2023-11-19 14:32:48.008093 omicverse-1.5.9/omicverse/STAGATE_pyG/gat_conv.py
+-rw-r--r--   0        0        0     9881 2023-11-19 13:46:14.331564 omicverse-1.5.9/omicverse/STAGATE_pyG/utils.py
+-rw-r--r--   0        0        0     1629 2024-01-02 05:35:04.424748 omicverse-1.5.9/omicverse/STAligner/STALIGNER.py
+-rw-r--r--   0        0        0    13944 2024-01-02 05:35:04.424887 omicverse-1.5.9/omicverse/STAligner/ST_utils.py
+-rw-r--r--   0        0        0    11855 2024-01-10 14:32:23.547613 omicverse-1.5.9/omicverse/STAligner/gat_conv.py
+-rw-r--r--   0        0        0     4830 2024-01-10 17:53:56.421303 omicverse-1.5.9/omicverse/STAligner/mnn_utils.py
+-rw-r--r--   0        0        0    16871 2024-01-02 05:35:04.425259 omicverse-1.5.9/omicverse/STAligner/train_STAligner.py
+-rw-r--r--   0        0        0      896 2024-04-30 10:03:30.078204 omicverse-1.5.9/omicverse/__init__.py
+-rw-r--r--   0        0        0      800 2024-04-30 10:18:31.122841 omicverse-1.5.9/omicverse/_settings.py
+-rw-r--r--   0        0        0     6148 2023-04-03 18:27:15.377061 omicverse-1.5.9/omicverse/bulk/.DS_Store
+-rw-r--r--   0        0        0    25320 2024-02-21 16:43:28.536550 omicverse-1.5.9/omicverse/bulk/_Deseq2.py
+-rw-r--r--   0        0        0    21289 2024-02-07 18:05:42.434835 omicverse-1.5.9/omicverse/bulk/_Enrichment.py
+-rw-r--r--   0        0        0    29240 2023-07-14 07:39:35.883647 omicverse-1.5.9/omicverse/bulk/_Gene_module.py
+-rw-r--r--   0        0        0      629 2023-08-09 05:33:15.892865 omicverse-1.5.9/omicverse/bulk/__init__.py
+-rw-r--r--   0        0        0   633338 2023-04-03 07:50:58.899031 omicverse-1.5.9/omicverse/bulk/_chm13.py
+-rw-r--r--   0        0        0      502 2023-08-09 05:33:18.082174 omicverse-1.5.9/omicverse/bulk/_combat.py
+-rw-r--r--   0        0        0     1633 2022-09-06 14:17:42.730883 omicverse-1.5.9/omicverse/bulk/_df_apply.py
+-rw-r--r--   0        0        0    42804 2022-09-06 14:17:42.731609 omicverse-1.5.9/omicverse/bulk/_dynamicTree.py
+-rw-r--r--   0        0        0     6919 2023-07-12 17:29:32.278344 omicverse-1.5.9/omicverse/bulk/_network.py
+-rw-r--r--   0        0        0    12290 2023-04-05 17:42:26.435325 omicverse-1.5.9/omicverse/bulk/_tcga.py
+-rw-r--r--   0        0        0      275 2023-05-27 07:42:00.305669 omicverse-1.5.9/omicverse/bulk2single/__init__.py
+-rw-r--r--   0        0        0    17858 2023-11-13 14:58:09.745576 omicverse-1.5.9/omicverse/bulk2single/_bulk2single.py
+-rw-r--r--   0        0        0      829 2023-09-07 10:19:48.804560 omicverse-1.5.9/omicverse/bulk2single/_bulkdeconvolve.py
+-rw-r--r--   0        0        0    15889 2024-01-10 14:43:25.330930 omicverse-1.5.9/omicverse/bulk2single/_bulktrajblend.py
+-rw-r--r--   0        0        0    29806 2023-05-06 16:11:04.140905 omicverse-1.5.9/omicverse/bulk2single/_map_utils.py
+-rw-r--r--   0        0        0    24978 2023-05-17 10:51:23.881340 omicverse-1.5.9/omicverse/bulk2single/_map_utils1.py
+-rw-r--r--   0        0        0    12746 2023-04-14 09:44:12.354770 omicverse-1.5.9/omicverse/bulk2single/_single2spatial.py
+-rw-r--r--   0        0        0    10462 2023-05-14 07:19:07.135859 omicverse-1.5.9/omicverse/bulk2single/_utils.py
+-rw-r--r--   0        0        0     8560 2023-04-06 07:00:58.204356 omicverse-1.5.9/omicverse/bulk2single/_vae.py
+-rw-r--r--   0        0        0       48 2023-05-30 08:00:53.496990 omicverse-1.5.9/omicverse/cylib/README.rst
+-rw-r--r--   0        0        0       25 2023-05-31 17:51:38.764877 omicverse-1.5.9/omicverse/cylib/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-31 17:55:48.200546 omicverse-1.5.9/omicverse/cylib/fast_utils.py
+-rw-r--r--   0        0        0     1313 2023-05-30 08:00:53.497082 omicverse-1.5.9/omicverse/data_files/README.md
+-rw-r--r--   0        0        0      613 2023-05-30 08:00:53.497137 omicverse-1.5.9/omicverse/data_files/apoptosis_human.gmt
+-rw-r--r--   0        0        0      598 2023-05-30 08:00:53.497199 omicverse-1.5.9/omicverse/data_files/apoptosis_mouse.gmt
+-rw-r--r--   0        0        0  1277787 2023-05-30 08:00:53.501091 omicverse-1.5.9/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt
+-rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501212 omicverse-1.5.9/omicverse/data_files/cell_cycle_human.gmt
+-rw-r--r--   0        0        0      597 2023-05-30 08:00:53.501283 omicverse-1.5.9/omicverse/data_files/cell_cycle_mouse.gmt
+-rw-r--r--   0        0        0      222 2023-05-30 08:00:53.501354 omicverse-1.5.9/omicverse/data_files/emt_human.gmt
+-rw-r--r--   0        0        0      230 2023-05-30 08:00:53.501426 omicverse-1.5.9/omicverse/data_files/gender_human.gmt
+-rw-r--r--   0        0        0      142 2023-05-30 08:00:53.501498 omicverse-1.5.9/omicverse/data_files/gender_mouse.gmt
+-rw-r--r--   0        0        0    48244 2023-05-30 08:00:53.501752 omicverse-1.5.9/omicverse/data_files/h.all.v7.5.1.symbols.gmt
+-rw-r--r--   0        0        0     2725 2023-05-30 08:00:53.501840 omicverse-1.5.9/omicverse/data_files/human_lung.gmt
+-rw-r--r--   0        0        0      743 2023-05-30 08:00:53.501906 omicverse-1.5.9/omicverse/data_files/human_t_cell_markers.gmt
+-rw-r--r--   0        0        0      929 2023-05-30 08:00:53.502035 omicverse-1.5.9/omicverse/data_files/mitochondrial_genes_human.gmt
+-rw-r--r--   0        0        0      930 2023-05-30 08:00:53.502100 omicverse-1.5.9/omicverse/data_files/mitochondrial_genes_mouse.gmt
+-rw-r--r--   0        0        0      706 2023-05-30 08:00:53.502165 omicverse-1.5.9/omicverse/data_files/mouse_brain.gmt
+-rw-r--r--   0        0        0     1931 2023-05-30 08:00:53.502238 omicverse-1.5.9/omicverse/data_files/mouse_liver.gmt
+-rw-r--r--   0        0        0     4068 2023-05-30 08:00:53.502316 omicverse-1.5.9/omicverse/data_files/mouse_lung.gmt
+-rw-r--r--   0        0        0      787 2023-05-30 08:00:53.502394 omicverse-1.5.9/omicverse/data_files/ribosomal_genes_human.gmt
+-rw-r--r--   0        0        0      801 2023-05-30 08:00:53.502468 omicverse-1.5.9/omicverse/data_files/ribosomal_genes_mouse.gmt
+-rw-r--r--   0        0        0       55 2022-09-07 09:33:07.470218 omicverse-1.5.9/omicverse/mofapy2/__init__.py
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.470284 omicverse-1.5.9/omicverse/mofapy2/build_model/__init__.py
+-rw-r--r--   0        0        0    13189 2022-09-07 10:12:11.559603 omicverse-1.5.9/omicverse/mofapy2/build_model/build_model.py
+-rw-r--r--   0        0        0    28425 2022-09-07 10:12:16.240298 omicverse-1.5.9/omicverse/mofapy2/build_model/init_model.py
+-rw-r--r--   0        0        0    25076 2022-09-07 10:12:21.681277 omicverse-1.5.9/omicverse/mofapy2/build_model/save_model.py
+-rw-r--r--   0        0        0      637 2022-09-07 10:12:26.660116 omicverse-1.5.9/omicverse/mofapy2/build_model/train_model.py
+-rw-r--r--   0        0        0     3366 2022-09-07 10:12:30.366961 omicverse-1.5.9/omicverse/mofapy2/build_model/utils.py
+-rw-r--r--   0        0        0      405 2022-09-07 09:33:07.470940 omicverse-1.5.9/omicverse/mofapy2/config.py
+-rw-r--r--   0        0        0    26036 2022-09-07 10:13:08.257046 omicverse-1.5.9/omicverse/mofapy2/core/BayesNet.py
+-rw-r--r--   0        0        0       21 2022-09-07 09:33:07.471206 omicverse-1.5.9/omicverse/mofapy2/core/__init__.py
+-rw-r--r--   0        0        0      448 2022-09-07 09:33:07.471309 omicverse-1.5.9/omicverse/mofapy2/core/distributions/__init__.py
+-rw-r--r--   0        0        0     3923 2022-09-07 09:33:07.471393 omicverse-1.5.9/omicverse/mofapy2/core/distributions/basic_distributions.py
+-rw-r--r--   0        0        0     1301 2022-09-07 10:20:27.422096 omicverse-1.5.9/omicverse/mofapy2/core/distributions/bernoulli.py
+-rw-r--r--   0        0        0     4709 2022-09-07 10:20:18.413617 omicverse-1.5.9/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py
+-rw-r--r--   0        0        0     1859 2022-09-07 10:20:33.345355 omicverse-1.5.9/omicverse/mofapy2/core/distributions/beta.py
+-rw-r--r--   0        0        0     1928 2022-09-07 10:20:37.394428 omicverse-1.5.9/omicverse/mofapy2/core/distributions/binomial.py
+-rw-r--r--   0        0        0     2061 2022-09-07 10:20:40.951879 omicverse-1.5.9/omicverse/mofapy2/core/distributions/gamma.py
+-rw-r--r--   0        0        0    38150 2022-09-07 09:33:07.471983 omicverse-1.5.9/omicverse/mofapy2/core/distributions/multi_task_GP.py
+-rw-r--r--   0        0        0    16083 2022-09-07 10:20:53.092939 omicverse-1.5.9/omicverse/mofapy2/core/distributions/multivariate_gaussian.py
+-rw-r--r--   0        0        0     1663 2022-09-07 10:20:57.661446 omicverse-1.5.9/omicverse/mofapy2/core/distributions/poisson.py
+-rw-r--r--   0        0        0     2223 2022-09-07 10:21:03.520320 omicverse-1.5.9/omicverse/mofapy2/core/distributions/univariate_gaussian.py
+-rw-r--r--   0        0        0     5591 2022-09-07 09:33:07.472344 omicverse-1.5.9/omicverse/mofapy2/core/gp_utils.py
+-rw-r--r--   0        0        0     1765 2022-09-07 09:33:07.472409 omicverse-1.5.9/omicverse/mofapy2/core/gpu_utils.py
+-rw-r--r--   0        0        0     6291 2022-09-07 09:33:07.472554 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Alpha_nodes.py
+-rw-r--r--   0        0        0     4646 2022-09-07 10:16:08.287697 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Kc_node.py
+-rw-r--r--   0        0        0     3581 2022-09-07 10:16:52.659105 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Kg_node.py
+-rw-r--r--   0        0        0    49309 2022-09-07 10:22:30.858460 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Sigma_node.py
+-rwxr-xr-x   0        0        0     5327 2022-09-07 10:18:15.524786 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Tau_nodes.py
+-rw-r--r--   0        0        0     6551 2022-09-07 09:33:07.473126 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Theta_nodes.py
+-rw-r--r--   0        0        0     7911 2022-09-07 10:18:33.209503 omicverse-1.5.9/omicverse/mofapy2/core/nodes/U_nodes.py
+-rwxr-xr-x   0        0        0    10037 2022-09-07 10:18:50.380099 omicverse-1.5.9/omicverse/mofapy2/core/nodes/W_nodes.py
+-rw-r--r--   0        0        0     3577 2022-09-07 10:18:59.577240 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Y_nodes.py
+-rwxr-xr-x   0        0        0    15625 2022-09-07 10:19:28.866210 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes.py
+-rw-r--r--   0        0        0     9248 2022-09-07 10:19:17.982574 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes_GP.py
+-rw-r--r--   0        0        0     8127 2022-09-07 10:19:10.770163 omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py
+-rw-r--r--   0        0        0     7505 2022-09-07 10:19:37.520420 omicverse-1.5.9/omicverse/mofapy2/core/nodes/ZgU_node.py
+-rw-r--r--   0        0        0      581 2022-09-07 09:33:07.473827 omicverse-1.5.9/omicverse/mofapy2/core/nodes/__init__.py
+-rw-r--r--   0        0        0     3812 2022-09-07 10:14:43.810952 omicverse-1.5.9/omicverse/mofapy2/core/nodes/basic_nodes.py
+-rw-r--r--   0        0        0     6837 2022-09-07 09:33:07.473999 omicverse-1.5.9/omicverse/mofapy2/core/nodes/multiview_nodes.py
+-rw-r--r--   0        0        0    21096 2022-09-07 10:17:25.117004 omicverse-1.5.9/omicverse/mofapy2/core/nodes/nongaussian_nodes.py
+-rw-r--r--   0        0        0    11994 2022-09-07 10:18:40.408370 omicverse-1.5.9/omicverse/mofapy2/core/nodes/variational_nodes.py
+-rw-r--r--   0        0        0     3764 2022-09-07 09:33:07.474508 omicverse-1.5.9/omicverse/mofapy2/core/utils.py
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.474782 omicverse-1.5.9/omicverse/mofapy2/run/__init__.py
+-rw-r--r--   0        0        0    70968 2023-05-18 07:48:53.001053 omicverse-1.5.9/omicverse/mofapy2/run/entry_point.py
+-rw-r--r--   0        0        0   324931 2022-09-07 09:33:07.476317 omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_0.txt
+-rw-r--r--   0        0        0   324642 2022-09-07 09:33:07.477843 omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_1.txt
+-rw-r--r--   0        0        0   324951 2022-09-07 09:33:07.478979 omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_2.txt
+-rw-r--r--   0        0        0   996145 2022-09-07 09:33:07.483410 omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_0.txt
+-rw-r--r--   0        0        0   996423 2022-09-07 09:33:07.486212 omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_1.txt
+-rw-r--r--   0        0        0   995502 2022-09-07 09:33:07.486904 omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_2.txt
+-rw-r--r--   0        0        0        0 2022-09-07 09:33:07.486988 omicverse-1.5.9/omicverse/mofapy2/simulate/__init__.py
+-rw-r--r--   0        0        0     6509 2022-09-07 10:10:46.603319 omicverse-1.5.9/omicverse/mofapy2/simulate/simulate_mofa.py
+-rw-r--r--   0        0        0       22 2022-09-07 09:33:07.487160 omicverse-1.5.9/omicverse/mofapy2/version.py
+-rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py
+-rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py
+-rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py
+-rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.078134 omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0      120 2022-09-07 04:15:14.079001 omicverse-1.5.9/omicverse/nocd/__init__.py
+-rw-r--r--   0        0        0     2163 2022-09-07 04:15:14.083601 omicverse-1.5.9/omicverse/nocd/data.py
+-rw-r--r--   0        0        0     1301 2022-09-07 04:15:14.083982 omicverse-1.5.9/omicverse/nocd/generate.py
+-rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.5.9/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py
+-rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.085633 omicverse-1.5.9/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py
+-rw-r--r--   0        0        0       54 2022-09-07 04:15:14.086034 omicverse-1.5.9/omicverse/nocd/metrics/__init__.py
+-rw-r--r--   0        0        0     4068 2022-09-07 04:18:20.582316 omicverse-1.5.9/omicverse/nocd/metrics/supervised.py
+-rw-r--r--   0        0        0     3214 2022-09-07 04:15:14.089087 omicverse-1.5.9/omicverse/nocd/metrics/unsupervised.py
+-rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py
+-rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py
+-rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py
+-rw-r--r--   0        0        0       70 2022-09-07 04:15:14.090185 omicverse-1.5.9/omicverse/nocd/nn/__init__.py
+-rw-r--r--   0        0        0     4453 2022-09-07 04:15:14.092088 omicverse-1.5.9/omicverse/nocd/nn/decoder.py
+-rw-r--r--   0        0        0     3505 2022-09-07 04:17:34.429490 omicverse-1.5.9/omicverse/nocd/nn/gcn.py
+-rw-r--r--   0        0        0     3610 2022-09-07 04:17:50.594410 omicverse-1.5.9/omicverse/nocd/nn/imrpoved_gcn.py
+-rw-r--r--   0        0        0     1681 2022-09-07 04:15:14.092998 omicverse-1.5.9/omicverse/nocd/sampler.py
+-rw-r--r--   0        0        0     4558 2022-09-07 04:15:14.093212 omicverse-1.5.9/omicverse/nocd/train.py
+-rw-r--r--   0        0        0     5051 2022-09-07 04:15:14.093413 omicverse-1.5.9/omicverse/nocd/utils.py
+-rw-r--r--   0        0        0      306 2023-11-16 15:26:26.581114 omicverse-1.5.9/omicverse/palantir/__init__.py
+-rw-r--r--   0        0        0      248 2023-11-16 15:35:54.712851 omicverse-1.5.9/omicverse/palantir/config.py
+-rw-r--r--   0        0        0    20843 2023-11-16 15:37:03.805608 omicverse-1.5.9/omicverse/palantir/core.py
+-rw-r--r--   0        0        0     3481 2023-11-16 15:32:44.282139 omicverse-1.5.9/omicverse/palantir/io.py
+-rw-r--r--   0        0        0    73306 2023-11-16 15:36:17.002907 omicverse-1.5.9/omicverse/palantir/plot.py
+-rw-r--r--   0        0        0     1459 2023-11-16 15:26:26.581668 omicverse-1.5.9/omicverse/palantir/preprocess.py
+-rw-r--r--   0        0        0    20923 2023-11-16 15:35:47.772593 omicverse-1.5.9/omicverse/palantir/presults.py
+-rw-r--r--   0        0        0    33510 2023-11-16 20:46:00.233185 omicverse-1.5.9/omicverse/palantir/utils.py
+-rw-r--r--   0        0        0     5570 2023-11-16 15:26:26.582123 omicverse-1.5.9/omicverse/palantir/validation.py
+-rw-r--r--   0        0        0      107 2023-11-19 13:09:57.850190 omicverse-1.5.9/omicverse/palantir/version.py
+-rw-r--r--   0        0        0      137 2024-02-21 16:16:00.957288 omicverse-1.5.9/omicverse/pl/__init__.py
+-rw-r--r--   0        0        0    10364 2024-02-23 20:33:22.783257 omicverse-1.5.9/omicverse/pl/_bulk.py
+-rw-r--r--   0        0        0      330 2024-01-29 14:46:01.259775 omicverse-1.5.9/omicverse/pl/_general.py
+-rw-r--r--   0        0        0    13984 2024-02-21 15:37:30.787564 omicverse-1.5.9/omicverse/pl/_heatmap.py
+-rw-r--r--   0        0        0     7298 2024-02-12 10:18:03.192092 omicverse-1.5.9/omicverse/pl/_multi.py
+-rw-r--r--   0        0        0     2921 2024-02-15 15:09:29.425724 omicverse-1.5.9/omicverse/pl/_palette.py
+-rw-r--r--   0        0        0    26187 2024-02-21 15:36:25.350638 omicverse-1.5.9/omicverse/pl/_single.py
+-rw-r--r--   0        0        0      678 2024-04-30 11:31:45.659926 omicverse-1.5.9/omicverse/pp/__init__.py
+-rw-r--r--   0        0        0    30974 2024-04-30 12:06:54.390685 omicverse-1.5.9/omicverse/pp/_preprocess.py
+-rw-r--r--   0        0        0    21711 2024-04-30 11:51:57.135003 omicverse-1.5.9/omicverse/pp/_qc.py
+-rw-r--r--   0        0        0     6148 2023-07-05 12:55:01.552000 omicverse-1.5.9/omicverse/single/.DS_Store
+-rw-r--r--   0        0        0     8790 2022-09-03 17:16:03.070397 omicverse-1.5.9/omicverse/single/README.md
+-rw-r--r--   0        0        0    61426 2023-06-26 23:50:36.692480 omicverse-1.5.9/omicverse/single/_SCSA.py
+-rw-r--r--   0        0        0     1236 2024-04-17 10:50:05.940779 omicverse-1.5.9/omicverse/single/__init__.py
+-rw-r--r--   0        0        0    28030 2023-12-28 10:37:02.673733 omicverse-1.5.9/omicverse/single/_anno.py
+-rw-r--r--   0        0        0    10196 2023-08-15 09:58:12.551350 omicverse-1.5.9/omicverse/single/_atac.py
+-rw-r--r--   0        0        0     9656 2024-01-10 14:32:23.549507 omicverse-1.5.9/omicverse/single/_aucell.py
+-rw-r--r--   0        0        0     3407 2023-12-12 07:25:16.476686 omicverse-1.5.9/omicverse/single/_batch.py
+-rw-r--r--   0        0        0    19489 2024-01-10 14:56:03.811609 omicverse-1.5.9/omicverse/single/_cefcon.py
+-rw-r--r--   0        0        0    32142 2024-02-20 07:59:48.545882 omicverse-1.5.9/omicverse/single/_cellfategenie.py
+-rw-r--r--   0        0        0    47487 2024-05-07 07:15:29.550760 omicverse-1.5.9/omicverse/single/_cnmf.py
+-rwxr-xr-x   0        0        0    21100 2022-09-07 05:59:40.809184 omicverse-1.5.9/omicverse/single/_cosg.py
+-rw-r--r--   0        0        0    12142 2023-07-04 04:23:59.889080 omicverse-1.5.9/omicverse/single/_cpdb.py
+-rw-r--r--   0        0        0    32067 2024-03-21 07:08:44.438283 omicverse-1.5.9/omicverse/single/_ltnn.py
+-rw-r--r--   0        0        0    20556 2024-01-30 09:16:15.392857 omicverse-1.5.9/omicverse/single/_mdic3.py
+-rw-r--r--   0        0        0     5551 2024-02-23 21:27:18.590762 omicverse-1.5.9/omicverse/single/_metacell.py
+-rw-r--r--   0        0        0    38177 2023-08-08 08:04:00.711068 omicverse-1.5.9/omicverse/single/_mofa.py
+-rw-r--r--   0        0        0    11678 2024-01-10 14:44:12.836094 omicverse-1.5.9/omicverse/single/_nocd.py
+-rw-r--r--   0        0        0    33108 2024-03-25 17:13:26.339586 omicverse-1.5.9/omicverse/single/_pyslingshot.py
+-rw-r--r--   0        0        0     4589 2023-07-23 08:19:07.196675 omicverse-1.5.9/omicverse/single/_scannorl.py
+-rw-r--r--   0        0        0    18135 2023-04-03 15:03:48.751508 omicverse-1.5.9/omicverse/single/_scdrug.py
+-rw-r--r--   0        0        0    13608 2023-07-08 08:47:26.522256 omicverse-1.5.9/omicverse/single/_scgsea.py
+-rw-r--r--   0        0        0        0 2023-08-19 13:26:01.097674 omicverse-1.5.9/omicverse/single/_seacells.py
+-rw-r--r--   0        0        0     7303 2024-01-30 10:37:15.236907 omicverse-1.5.9/omicverse/single/_simba.py
+-rw-r--r--   0        0        0    18296 2023-07-11 04:31:16.370357 omicverse-1.5.9/omicverse/single/_tosica.py
+-rw-r--r--   0        0        0     4896 2024-03-25 17:06:42.669860 omicverse-1.5.9/omicverse/single/_traj.py
+-rw-r--r--   0        0        0    76688 2024-02-19 20:43:08.500848 omicverse-1.5.9/omicverse/single/_via.py
+-rw-r--r--   0        0        0      179 2024-04-09 17:03:49.791612 omicverse-1.5.9/omicverse/space/__init__.py
+-rw-r--r--   0        0        0     4913 2024-01-06 19:47:57.665850 omicverse-1.5.9/omicverse/space/_cluster.py
+-rw-r--r--   0        0        0    12205 2024-01-10 14:32:23.549911 omicverse-1.5.9/omicverse/space/_integrate.py
+-rw-r--r--   0        0        0     7451 2024-02-07 18:05:42.436346 omicverse-1.5.9/omicverse/space/_spaceflow.py
+-rw-r--r--   0        0        0     3609 2024-04-09 17:53:40.361589 omicverse-1.5.9/omicverse/space/_spatrio.py
+-rw-r--r--   0        0        0     3292 2023-12-12 07:25:30.770192 omicverse-1.5.9/omicverse/space/_tangram.py
+-rw-r--r--   0        0        0    27318 2024-02-07 18:05:42.436550 omicverse-1.5.9/omicverse/spaceflow/_SpaceFlow.py
+-rw-r--r--   0        0        0       54 2024-02-07 18:05:42.436663 omicverse-1.5.9/omicverse/spaceflow/__init__.py
+-rw-r--r--   0        0        0      361 2024-02-07 18:05:42.436756 omicverse-1.5.9/omicverse/spaceflow/_util.py
+-rwxr-xr-x   0        0        0      252 2024-04-04 13:09:51.808929 omicverse-1.5.9/omicverse/spatrio/__init__.py
+-rwxr-xr-x   0        0        0     8337 2024-04-04 13:09:51.809884 omicverse-1.5.9/omicverse/spatrio/evals.py
+-rwxr-xr-x   0        0        0    11019 2024-04-09 16:53:51.435252 omicverse-1.5.9/omicverse/spatrio/helper.py
+-rwxr-xr-x   0        0        0     1576 2024-04-04 13:09:51.810108 omicverse-1.5.9/omicverse/spatrio/simulation.py
+-rwxr-xr-x   0        0        0    25017 2024-04-09 17:30:56.121256 omicverse-1.5.9/omicverse/spatrio/spatrio.py
+-rwxr-xr-x   0        0        0     1771 2024-04-04 13:09:51.810274 omicverse-1.5.9/omicverse/spatrio/visualization.py
+-rw-r--r--   0        0        0      108 2023-11-13 14:40:19.151431 omicverse-1.5.9/omicverse/tape/__init__.py
+-rw-r--r--   0        0        0     7521 2023-09-28 09:40:35.361223 omicverse-1.5.9/omicverse/tape/deconvolution.py
+-rw-r--r--   0        0        0     7953 2023-09-28 09:40:50.694373 omicverse-1.5.9/omicverse/tape/model.py
+-rw-r--r--   0        0        0     6097 2023-09-28 09:41:17.053043 omicverse-1.5.9/omicverse/tape/simulation.py
+-rw-r--r--   0        0        0     6726 2023-09-28 09:41:28.452046 omicverse-1.5.9/omicverse/tape/train.py
+-rw-r--r--   0        0        0     6585 2023-09-28 14:24:10.730906 omicverse-1.5.9/omicverse/tape/utils.py
+-rw-r--r--   0        0        0    11399 2023-07-08 08:54:04.442016 omicverse-1.5.9/omicverse/tosica/TOSICA_model.py
+-rw-r--r--   0        0        0      184 2023-07-05 16:39:57.238794 omicverse-1.5.9/omicverse/tosica/__init__.py
+-rw-r--r--   0        0        0     5669 2023-07-05 12:56:02.375603 omicverse-1.5.9/omicverse/tosica/customized_linear.py
+-rw-r--r--   0        0        0    11304 2023-07-05 15:46:55.560572 omicverse-1.5.9/omicverse/tosica/pre.py
+-rw-r--r--   0        0        0    13384 2023-07-11 04:33:48.020024 omicverse-1.5.9/omicverse/tosica/train.py
+-rw-r--r--   0        0        0     1111 2023-12-04 20:09:51.594263 omicverse-1.5.9/omicverse/utils/__init__.py
+-rw-r--r--   0        0        0     6217 2024-01-04 17:08:18.979832 omicverse-1.5.9/omicverse/utils/_cluster.py
+-rw-r--r--   0        0        0    21598 2024-04-15 08:07:53.561238 omicverse-1.5.9/omicverse/utils/_data.py
+-rw-r--r--   0        0        0     2343 2023-06-01 08:49:06.326555 omicverse-1.5.9/omicverse/utils/_enum.py
+-rw-r--r--   0        0        0    20217 2023-07-08 08:44:29.300351 omicverse-1.5.9/omicverse/utils/_genomics.py
+-rw-r--r--   0        0        0    20837 2023-08-18 14:13:31.420310 omicverse-1.5.9/omicverse/utils/_heatmap.py
+-rw-r--r--   0        0        0     5370 2023-08-08 16:27:48.029476 omicverse-1.5.9/omicverse/utils/_knn.py
+-rw-r--r--   0        0        0     2520 2023-05-27 07:38:06.457609 omicverse-1.5.9/omicverse/utils/_mde.py
+-rw-r--r--   0        0        0    16487 2023-09-26 17:14:22.181959 omicverse-1.5.9/omicverse/utils/_paga.py
+-rw-r--r--   0        0        0    38859 2024-02-23 20:30:28.817553 omicverse-1.5.9/omicverse/utils/_plot.py
+-rw-r--r--   0        0        0     5008 2023-08-31 10:23:54.166327 omicverse-1.5.9/omicverse/utils/_roe.py
+-rw-r--r--   0        0        0    48995 2024-01-29 13:46:13.992761 omicverse-1.5.9/omicverse/utils/_scatterplot.py
+-rw-r--r--   0        0        0     4169 2023-09-26 16:51:08.413978 omicverse-1.5.9/omicverse/utils/_syn.py
+-rw-r--r--   0        0        0     5765 2023-12-04 20:09:39.026475 omicverse-1.5.9/omicverse/utils/_venn.py
+-rw-r--r--   0        0        0      441 2023-04-07 07:58:16.954693 omicverse-1.5.9/omicverse/via/.idea/VIA.iml
+-rw-r--r--   0        0        0      143 2023-04-07 07:58:16.954828 omicverse-1.5.9/omicverse/via/__init__.py
+-rw-r--r--   0        0        0   195095 2024-02-21 15:13:58.278501 omicverse-1.5.9/omicverse/via/core.py
+-rw-r--r--   0        0        0    10436 2023-07-04 11:16:15.075797 omicverse-1.5.9/omicverse/via/datasets_via.py
+-rw-r--r--   0        0        0   160696 2024-02-21 15:13:19.841598 omicverse-1.5.9/omicverse/via/examples.py
+-rw-r--r--   0        0        0   145530 2023-04-07 16:00:02.788869 omicverse-1.5.9/omicverse/via/plotting_via.py
+-rw-r--r--   0        0        0    75612 2023-10-17 15:06:18.715265 omicverse-1.5.9/omicverse/via/utils_via.py
+-rw-r--r--   0        0        0     7987 2023-04-07 07:58:16.958047 omicverse-1.5.9/omicverse/via/windmap.py
+-rw-r--r--   0        0        0     1958 2024-04-03 19:32:50.358055 omicverse-1.5.9/pyproject.toml
+-rw-r--r--   0        0        0    11804 1970-01-01 00:00:00.000000 omicverse-1.5.9/PKG-INFO
```

### Comparing `omicverse-1.5.8/LICENSE` & `omicverse-1.5.9/LICENSE`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/README.md` & `omicverse-1.5.9/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 <img src="https://raw.githubusercontent.com/Starlitnightly/omicverse/master/README.assets/logo.png" width="400">
 </h1><br>
 
 [![pypi-badge](https://img.shields.io/pypi/v/omicverse)](https://pypi.org/project/omicverse) [![Documentation Status](https://readthedocs.org/projects/omicverse/badge/?version=latest)](https://omicverse.readthedocs.io/en/latest/?badge=latest) [![pypiDownloads](https://static.pepy.tech/badge/omicverse)](https://pepy.tech/project/omicverse) [![condaDownloads](https://img.shields.io/conda/dn/conda-forge/omicverse?logo=Anaconda)](https://anaconda.org/conda-forge/omicverse) [![License:GPL](https://img.shields.io/badge/license-GNU-blue)](https://img.shields.io/apm/l/vim-mode) [![scverse](https://img.shields.io/badge/scverse-ecosystem-blue.svg?labelColor=yellow)](https://scverse.org/) [![Pytest](https://github.com/Starlitnightly/omicverse/workflows/py38|py39/badge.svg)](https://github.com/Starlitnightly/omicverse/) 
 
 OmicVerse is the fundamental package for multi omics included bulk and single cell analysis with Python. For more information, please read our paper: [OmicVerse: A single pipeline for exploring the entire transcriptome universe](https://www.biorxiv.org/content/10.1101/2023.06.06.543913v2)
 
+If you like **OmicVerse** and want to support our mission, please consider making a [donation](https://afdian.net/a/starlitnightly) to support our efforts.
+
+## Introduction
+
 The original name of the omicverse was [Pyomic](https://pypi.org/project/Pyomic/), but we wanted to address a whole universe of transcriptomics, so we changed the name to OmicVerse, it aimed to solve all task in RNA-seq.
 
 BulkTrajBlend algorithm in OmicVerse that combines Beta-Variational AutoEncoder for deconvolution and graph neural networks for overlapping community discovery to effectively interpolate and restore the continuity of “interrupted” cells in the original scRNA-seq data.
 
 ![omicverse-light](omicverse_guide/docs/img/omicverse.png#gh-light-mode-only)
 ![omicverse-dark](omicverse_guide/docs/img/omicverse_dark.png#gh-dark-mode-only)
 
@@ -75,14 +79,15 @@
 - [29] [CEFCON](https://github.com/WPZgithub/CEFCON) was originally published in [*Nature Communications*](https://www.nature.com/articles/s41467-023-44103-3)
 - [30] [PyComplexHeatmap](https://github.com/DingWB/PyComplexHeatmap) was originally published in [*iMeta*](https://doi.org/10.1002/imt2.115)
 
 ## Included Package not published or preprint
 
 - [1] [Cellula](https://github.com/andrecossa5/Cellula/) is to provide a toolkit for the exploration of scRNA-seq. These tools perform common single-cell analysis tasks
 - [2] [pegasus](https://github.com/lilab-bcb/pegasus/) is a tool for analyzing transcriptomes of millions of single cells. It is a command line tool, a python package and a base for Cloud-based analysis workflows.
+- [3] [cNMF](https://github.com/dylkot/cNMF) is an analysis pipeline for inferring gene expression programs from single-cell RNA-Seq (scRNA-Seq) data.
 
 ## Contact
 
 - Zehua Zeng ([starlitnightly@163.com](mailto:starlitnightly@163.com) or [zehuazeng@xs.ustb.edu.cn](mailto:zehuazeng@xs.ustb.edu.cn))
 - Lei Hu ([hulei@westlake.edu.cn](mailto:hulei@westlake.edu.cn))
 
 ## Developer Guild
@@ -93,9 +98,11 @@
 
 We would like to thank the following WeChat Official Accounts for promoting Omicverse.
 
 <p align="left"> <a href="http://www.biotrainee.com/" target="_blank" rel="noreferrer"> <img src="README.assets/image-20230701163953794.png" alt="linux" width="50" height="50"/> </a> <a href="https://zhuanlan.zhihu.com/c_1257815636945915904?page=3" target="_blank" rel="noreferrer"> <img src="README.assets/WechatIMG688.png" alt="linux" width="50" height="50"/> </a> </p>
 
 ## Other
 
+If you would like to sponsor the development of our project, you can go to the afdian website (https://afdian.net/a/starlitnightly) and sponsor us.
+
 <div>Logo made by <a href="https://www.designevo.com/" title="Free Online Logo Maker">DesignEvo free logo creator</a></div>
```

### Comparing `omicverse-1.5.8/omicverse/.DS_Store` & `omicverse-1.5.9/omicverse/.DS_Store`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 00000000: 0000 0001 4275 6431 0000 3000 0000 0800  ....Bud1..0.....
 00000010: 0000 3000 0000 100c 0000 0086 0000 200c  ..0........... .
 00000020: 0000 0000 0000 0000 0000 0000 0000 0800  ................
 00000030: 0000 0800 0000 0000 0000 0000 0000 0000  ................
-00000040: 0000 0000 0000 0003 0000 0001 0000 0023  ...............#
-00000050: 0000 0003 0000 1000 0046 0043 004f 004e  .........F.C.O.N
-00000060: 7653 726e 0000 0000 0000 0000 0000 0000  vSrn............
+00000040: 0000 0000 0000 0003 0000 0001 0000 0029  ...............)
+00000050: 0000 0003 0000 1000 006c 0069 0062 7653  .........l.i.bvS
+00000060: 726e 6c6f 0000 0000 0000 0000 0000 0000  rnlo............
 00000070: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000080: 0000 0000 0000 0002 0000 0001 0000 0004  ................
-00000090: 0000 0006 0043 0045 0046 0043 004f 004e  .....C.E.F.C.O.N
-000000a0: 7653 726e 6c6f 6e67 0000 0001 6f62 0000  vSrnlong....ob..
+00000090: 0000 0005 0063 0079 006c 0069 0062 7653  .....c.y.l.i.bvS
+000000a0: 726e 6c6f 6e67 0000 0001 626c 6f62 0000  rnlong....blob..
 000000b0: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
 000000c0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000d0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000e0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 000000f0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000100: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000110: 0000 0000 0000 0000 0000 0000 0000 0000  ................
@@ -250,271 +250,271 @@
 00000f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00000ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001000: 0000 0000 0000 0000 0000 0019 0000 0005  ................
-00001010: 0063 0079 006c 0069 0062 6277 7370 626c  .c.y.l.i.bbwspbl
-00001020: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
-00001030: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-00001040: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-00001050: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001060: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001070: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001080: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001090: 7208 0908 095f 1018 7b7b 3135 302c 2032  r...._..{{150, 2
-000010a0: 3330 7d2c 207b 3932 302c 2034 3336 7d7d  30}, {920, 436}}
-000010b0: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-000010c0: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-000010d0: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-000010e0: 0005 0063 0079 006c 0069 0062 7653 726e  ...c.y.l.i.bvSrn
-000010f0: 6c6f 6e67 0000 0001 0000 000a 0064 0061  long.........d.a
-00001100: 0074 0061 005f 0066 0069 006c 0065 0073  .t.a._.f.i.l.e.s
-00001110: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
-00001120: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
-00001130: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
-00001140: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
-00001150: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
-00001160: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
-00001170: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
-00001180: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
-00001190: 3135 302c 2032 3330 7d2c 207b 3932 302c  150, 230}, {920,
-000011a0: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
-000011b0: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
-000011c0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
-000011d0: 0000 008b 0000 000a 0064 0061 0074 0061  .........d.a.t.a
-000011e0: 005f 0066 0069 006c 0065 0073 6c73 7643  ._.f.i.l.e.slsvC
-000011f0: 626c 6f62 0000 0353 6270 6c69 7374 3030  blob...Sbplist00
-00001200: da01 0203 0405 0607 0809 0a0b 0c0d 1d57  ...............W
-00001210: 5859 5a0c 5c58 6963 6f6e 5369 7a65 5f10  XYZ.\XiconSize_.
-00001220: 0f73 686f 7749 636f 6e50 7265 7669 6577  .showIconPreview
-00001230: 5763 6f6c 756d 6e73 5f10 1163 616c 6375  Wcolumns_..calcu
-00001240: 6c61 7465 416c 6c53 697a 6573 5f10 0f73  lateAllSizes_..s
-00001250: 6372 6f6c 6c50 6f73 6974 696f 6e59 5874  crollPositionYXt
-00001260: 6578 7453 697a 655f 100f 7363 726f 6c6c  extSize_..scroll
-00001270: 506f 7369 7469 6f6e 585a 736f 7274 436f  PositionXZsortCo
-00001280: 6c75 6d6e 5f10 1075 7365 5265 6c61 7469  lumn_..useRelati
-00001290: 7665 4461 7465 735f 1012 7669 6577 4f70  veDates_..viewOp
-000012a0: 7469 6f6e 7356 6572 7369 6f6e 2340 3000  tionsVersion#@0.
-000012b0: 0000 0000 0009 ae0e 171f 2428 2d32 373c  ..........$(-27<
-000012c0: 4045 494d 51d4 0f10 1112 0c14 0c16 5776  @EIMQ.........Wv
-000012d0: 6973 6962 6c65 5577 6964 7468 5961 7363  isibleUwidthYasc
-000012e0: 656e 6469 6e67 5a69 6465 6e74 6966 6965  endingZidentifie
-000012f0: 7209 1101 2c09 546e 616d 65d4 1218 191a  r...,.Tname.....
-00001300: 1b1c 1d1d 5577 6964 7468 5961 7363 656e  ....UwidthYascen
-00001310: 6469 6e67 5776 6973 6962 6c65 5875 6269  dingWvisibleXubi
-00001320: 7175 6974 7910 2308 08d4 0f10 1112 0c21  quity.#........!
-00001330: 1d23 0910 b508 5c64 6174 654d 6f64 6966  .#....\dateModif
-00001340: 6965 64d4 0f10 1112 1d21 1d27 0808 5b64  ied......!.'..[d
-00001350: 6174 6543 7265 6174 6564 d40f 1011 120c  ateCreated......
-00001360: 2a1d 2c09 1061 0854 7369 7a65 d40f 1011  *.,..a.Tsize....
-00001370: 120c 2f0c 3109 1073 0954 6b69 6e64 d40f  ../.1..s.Tkind..
-00001380: 1011 121d 340c 3608 1064 0955 6c61 6265  ....4.6..d.Ulabe
-00001390: 6cd4 0f10 1112 1d39 0c3b 0810 4b09 5776  l......9.;..K.Wv
-000013a0: 6572 7369 6f6e d40f 1011 121d 140c 3f08  ersion........?.
-000013b0: 0958 636f 6d6d 656e 7473 d40f 1011 121d  .Xcomments......
-000013c0: 421d 4408 10c8 085e 6461 7465 4c61 7374  B.D....^dateLast
-000013d0: 4f70 656e 6564 d40f 1011 121d 421d 4808  Opened......B.H.
-000013e0: 085a 7368 6172 654f 776e 6572 d40f 1011  .ZshareOwner....
-000013f0: 121d 421d 4c08 085f 100f 7368 6172 654c  ..B.L.._..shareL
-00001400: 6173 7445 6469 746f 72d4 1218 191a 4e21  astEditor.....N!
-00001410: 1d1d 5964 6174 6541 6464 6564 0808 d41a  ..YdateAdded....
-00001420: 1819 121d 531d 5508 10d2 085f 1010 696e  ....S.U...._..in
-00001430: 7669 7461 7469 6f6e 5374 6174 7573 0823  vitationStatus.#
-00001440: 4043 8000 0000 0000 2340 2a00 0000 0000  @C......#@*.....
-00001450: 0023 0000 0000 0000 0000 546e 616d 6509  .#........Tname.
-00001460: 1400 0000 0000 0000 0000 0000 0000 0000  ................
-00001470: 0100 0800 1d00 2600 3800 4000 5400 6600  ......&.8.@.T.f.
-00001480: 6f00 8100 8c00 9f00 b400 bd00 be00 cd00  o...............
-00001490: d600 de00 e400 ee00 f900 fa00 fd00 fe01  ................
-000014a0: 0301 0c01 1201 1c01 2401 2d01 2f01 3001  ........$.-./.0.
-000014b0: 3101 3a01 3b01 3d01 3e01 4b01 5401 5501  1.:.;.=.>.K.T.U.
-000014c0: 5601 6201 6b01 6c01 6e01 6f01 7401 7d01  V.b.k.l.n.o.t.}.
-000014d0: 7e01 8001 8101 8601 8f01 9001 9201 9301  ~...............
-000014e0: 9901 a201 a301 a501 a601 ae01 b701 b801  ................
-000014f0: b901 c201 cb01 cc01 ce01 cf01 de01 e701  ................
-00001500: e801 e901 f401 fd01 fe01 ff02 1102 1a02  ................
-00001510: 2402 2502 2602 2f02 3002 3202 3302 4602  $.%.&./.0.2.3.F.
-00001520: 4702 5002 5902 6202 6702 6800 0000 0000  G.P.Y.b.g.h.....
-00001530: 0002 0100 0000 0000 0000 5d00 0000 0000  ..........].....
-00001540: 0000 0000 0000 0000 0002 7900 0000 0a00  ..........y.....
-00001550: 6400 6100 7400 6100 5f00 6600 6900 6c00  d.a.t.a._.f.i.l.
-00001560: 6500 736c 7376 7062 6c6f 6200 0002 ae62  e.slsvpblob....b
-00001570: 706c 6973 7430 30da 0102 0304 0506 0708  plist00.........
-00001580: 090a 0b0c 0d1f 4748 494a 0c4c 5869 636f  ......GHIJ.LXico
-00001590: 6e53 697a 655f 100f 7368 6f77 4963 6f6e  nSize_..showIcon
-000015a0: 5072 6576 6965 7757 636f 6c75 6d6e 735f  PreviewWcolumns_
-000015b0: 1011 6361 6c63 756c 6174 6541 6c6c 5369  ..calculateAllSi
-000015c0: 7a65 735f 100f 7363 726f 6c6c 506f 7369  zes_..scrollPosi
-000015d0: 7469 6f6e 5958 7465 7874 5369 7a65 5f10  tionYXtextSize_.
-000015e0: 0f73 6372 6f6c 6c50 6f73 6974 696f 6e58  .scrollPositionX
-000015f0: 5a73 6f72 7443 6f6c 756d 6e5f 1010 7573  ZsortColumn_..us
-00001600: 6552 656c 6174 6976 6544 6174 6573 5f10  eRelativeDates_.
-00001610: 1276 6965 774f 7074 696f 6e73 5665 7273  .viewOptionsVers
-00001620: 696f 6e23 4030 0000 0000 0000 09d9 0e0f  ion#@0..........
-00001630: 1011 1213 1415 1617 2025 2a2f 3438 3d41  ........ %*/48=A
-00001640: 5863 6f6d 6d65 6e74 7355 6c61 6265 6c57  XcommentsUlabelW
-00001650: 7665 7273 696f 6e5b 6461 7465 4372 6561  version[dateCrea
-00001660: 7465 6454 7369 7a65 5c64 6174 654d 6f64  tedTsize\dateMod
-00001670: 6966 6965 6454 6b69 6e64 546e 616d 655e  ifiedTkindTname^
-00001680: 6461 7465 4c61 7374 4f70 656e 6564 d418  dateLastOpened..
-00001690: 191a 1b1c 1d0c 1f55 696e 6465 7855 7769  .......UindexUwi
-000016a0: 6474 6859 6173 6365 6e64 696e 6757 7669  dthYascendingWvi
-000016b0: 7369 626c 6510 0711 012c 0908 d418 191a  sible....,......
-000016c0: 1b21 220c 1f10 0510 6409 08d4 1819 1a1b  .!".....d.......
-000016d0: 2627 0c1f 1006 104b 0908 d418 191a 1b2b  &'.....K.......+
-000016e0: 2c1f 1f10 0210 b508 08d4 1819 1a1b 3031  ,.............01
-000016f0: 1f0c 1003 1061 0809 d418 191a 1b35 2c1f  .....a.......5,.
-00001700: 0c10 0108 09d4 1819 1a1b 393a 0c0c 1004  ..........9:....
-00001710: 1073 0909 d418 191a 1b3e 1d0c 0c10 0009  .s.......>......
-00001720: 09d4 1819 1a1b 4243 1f1f 1008 10c8 0808  ......BC........
-00001730: 0823 4043 8000 0000 0000 2340 2a00 0000  .#@C......#@*...
-00001740: 0000 0023 0000 0000 0000 0000 546e 616d  ...#........Tnam
-00001750: 6509 1400 0000 0000 0000 0000 0000 0000  e...............
-00001760: 0000 0100 0800 1d00 2600 3800 4000 5400  ........&.8.@.T.
-00001770: 6600 6f00 8100 8c00 9f00 b400 bd00 be00  f.o.............
-00001780: d100 da00 e000 e800 f400 f901 0601 0b01  ................
-00001790: 1001 1f01 2801 2e01 3401 3e01 4601 4801  ....(...4.>.F.H.
-000017a0: 4b01 4c01 4d01 5601 5801 5a01 5b01 5c01  K.L.M.V.X.Z.[.\.
-000017b0: 6501 6701 6901 6a01 6b01 7401 7601 7801  e.g.i.j.k.t.v.x.
-000017c0: 7901 7a01 8301 8501 8701 8801 8901 9201  y.z.............
-000017d0: 9401 9501 9601 9f01 a101 a301 a401 a501  ................
-000017e0: ae01 b001 b101 b201 bb01 bd01 bf01 c001  ................
-000017f0: c101 c201 cb01 d401 dd01 e201 e300 0000  ................
-00001800: 0000 0002 0100 0000 0000 0000 4d00 0000  ............M...
-00001810: 0000 0000 0000 0000 0000 0001 f400 0000  ................
-00001820: 0a00 6400 6100 7400 6100 5f00 6600 6900  ..d.a.t.a._.f.i.
-00001830: 6c00 6500 7376 5372 6e6c 6f6e 6700 0000  l.e.svSrnlong...
-00001840: 0100 0000 0700 6d00 6f00 6600 6100 7000  ......m.o.f.a.p.
-00001850: 7900 3249 6c6f 6362 6c6f 6200 0000 1000  y.2Ilocblob.....
-00001860: 0000 4100 0000 9eff ffff ffff ff00 0000  ..A.............
-00001870: 0000 0700 6d00 6f00 6600 6100 7000 7900  ....m.o.f.a.p.y.
-00001880: 3262 7773 7062 6c6f 6200 0000 b862 706c  2bwspblob....bpl
-00001890: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-000018a0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000018b0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-000018c0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-000018d0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-000018e0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000018f0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00001900: 7b31 3839 2c20 3133 317d 2c20 7b39 3230  {189, 131}, {920
-00001910: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-00001920: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
-00001930: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001940: 0000 0000 8b00 0000 0700 6d00 6f00 6600  ..........m.o.f.
-00001950: 6100 7000 7900 3264 7363 6c62 6f6f 6c00  a.p.y.2dsclbool.
-00001960: 0000 0007 006d 006f 0066 0061 0070 0079  .....m.o.f.a.p.y
-00001970: 0032 7653 726e 6c6f 6e67 0000 0001 0000  .2vSrnlong......
-00001980: 0004 006e 006f 0063 0064 496c 6f63 626c  ...n.o.c.dIlocbl
-00001990: 6f62 0000 0010 0000 01f9 0000 002e ffff  ob..............
-000019a0: ffff ffff 0000 0000 0008 0070 0061 006c  ...........p.a.l
-000019b0: 0061 006e 0074 0069 0072 6277 7370 626c  .a.n.t.i.rbwspbl
-000019c0: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
-000019d0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-000019e0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-000019f0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00001a00: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00001a10: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00001a20: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00001a30: 7208 0908 095f 1018 7b7b 3139 312c 2031  r...._..{{191, 1
-00001a40: 3630 7d2c 207b 3932 302c 2034 3336 7d7d  60}, {920, 436}}
-00001a50: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-00001a60: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-00001a70: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-00001a80: 0008 0070 0061 006c 0061 006e 0074 0069  ...p.a.l.a.n.t.i
-00001a90: 0072 7653 726e 6c6f 6e67 0000 0001 0000  .rvSrnlong......
-00001aa0: 0008 0053 0045 0041 0043 0065 006c 006c  ...S.E.A.C.e.l.l
-00001ab0: 0073 6277 7370 626c 6f62 0000 00b7 6270  .sbwspblob....bp
-00001ac0: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
-00001ad0: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00001ae0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00001af0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00001b00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00001b10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00001b20: 6f77 5369 6465 6261 7208 0908 095f 1017  owSidebar...._..
-00001b30: 7b7b 3536 2c20 3138 337d 2c20 7b39 3631  {{56, 183}, {961
-00001b40: 2c20 3438 387d 7d09 0815 232f 3b52 5f6b  , 488}}...#/;R_k
-00001b50: 6c6d 6e6f 8900 0000 0000 0001 0100 0000  lmno............
-00001b60: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001b70: 0000 0000 8a00 0000 0800 5300 4500 4100  ..........S.E.A.
-00001b80: 4300 6500 6c00 6c00 7376 5372 6e6c 6f6e  C.e.l.l.svSrnlon
-00001b90: 6700 0000 0100 0000 0600 7300 6900 6e00  g.........s.i.n.
-00001ba0: 6700 6c00 6549 6c6f 6362 6c6f 6200 0000  g.l.eIlocblob...
-00001bb0: 1000 0001 8b00 0000 2eff ffff ffff ff00  ................
-00001bc0: 0000 0000 0600 7300 6900 6e00 6700 6c00  ......s.i.n.g.l.
-00001bd0: 6562 7773 7062 6c6f 6200 0000 b862 706c  ebwspblob....bpl
-00001be0: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00001bf0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00001c00: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00001c10: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00001c20: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00001c30: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00001c40: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00001c50: 7b35 3932 2c20 3231 367d 2c20 7b39 3230  {592, 216}, {920
-00001c60: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-00001c70: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
-00001c80: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00001c90: 0000 0000 8b00 0000 0600 7300 6900 6e00  ..........s.i.n.
-00001ca0: 6700 6c00 6564 7363 6c62 6f6f 6c00 0000  g.l.edsclbool...
-00001cb0: 0006 0073 0069 006e 0067 006c 0065 7653  ...s.i.n.g.l.evS
-00001cc0: 726e 6c6f 6e67 0000 0001 0000 000b 0053  rnlong.........S
-00001cd0: 0054 0041 0047 0041 0054 0045 005f 0070  .T.A.G.A.T.E._.p
-00001ce0: 0079 0047 6277 7370 626c 6f62 0000 00b8  .y.Gbwspblob....
-00001cf0: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-00001d00: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00001d10: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-00001d20: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00001d30: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00001d40: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00001d50: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-00001d60: 1018 7b7b 3139 302c 2031 3630 7d2c 207b  ..{{190, 160}, {
-00001d70: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
-00001d80: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
-00001d90: 0000 0000 0000 000d 0000 0000 0000 0000  ................
-00001da0: 0000 0000 0000 008b 0000 000b 0053 0054  .............S.T
-00001db0: 0041 0047 0041 0054 0045 005f 0070 0079  .A.G.A.T.E._.p.y
-00001dc0: 0047 7653 726e 6c6f 6e67 0000 0001 0000  .GvSrnlong......
-00001dd0: 0005 0075 0074 0069 006c 0073 496c 6f63  ...u.t.i.l.sIloc
-00001de0: 626c 6f62 0000 0010 0000 0267 0000 002e  blob.......g....
-00001df0: ffff ffff ffff 0000 0000 0003 0076 0069  .............v.i
-00001e00: 0061 496c 6f63 626c 6f62 0000 0010 0000  .aIlocblob......
-00001e10: 00af 0000 009e ffff ffff ffff 0000 0000  ................
-00001e20: 0003 0076 0069 0061 6277 7370 626c 6f62  ...v.i.abwspblob
-00001e30: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-00001e40: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
-00001e50: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00001e60: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00001e70: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00001e80: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00001e90: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00001ea0: 0908 095f 1018 7b7b 3531 302c 2031 3834  ..._..{{510, 184
-00001eb0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
-00001ec0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00001ed0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00001ee0: 0000 0000 0000 0000 0000 008b 0000 0003  ................
-00001ef0: 0076 0069 0061 7653 726e 6c6f 6e67 0000  .v.i.avSrnlong..
-00001f00: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00001f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00001f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00001000: 0000 0000 0000 0000 0000 001d 0000 000a  ................
+00001010: 0064 0061 0074 0061 005f 0066 0069 006c  .d.a.t.a._.f.i.l
+00001020: 0065 0073 6277 7370 626c 6f62 0000 00b8  .e.sbwspblob....
+00001030: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
+00001040: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
+00001050: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
+00001060: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
+00001070: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
+00001080: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
+00001090: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
+000010a0: 1018 7b7b 3135 302c 2032 3330 7d2c 207b  ..{{150, 230}, {
+000010b0: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
+000010c0: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
+000010d0: 0000 0000 0000 000d 0000 0000 0000 0000  ................
+000010e0: 0000 0000 0000 008b 0000 000a 0064 0061  .............d.a
+000010f0: 0074 0061 005f 0066 0069 006c 0065 0073  .t.a._.f.i.l.e.s
+00001100: 6c73 7643 626c 6f62 0000 0353 6270 6c69  lsvCblob...Sbpli
+00001110: 7374 3030 da01 0203 0405 0607 0809 0a0b  st00............
+00001120: 0c0d 1d57 5859 5a0c 5c58 6963 6f6e 5369  ...WXYZ.\XiconSi
+00001130: 7a65 5f10 0f73 686f 7749 636f 6e50 7265  ze_..showIconPre
+00001140: 7669 6577 5763 6f6c 756d 6e73 5f10 1163  viewWcolumns_..c
+00001150: 616c 6375 6c61 7465 416c 6c53 697a 6573  alculateAllSizes
+00001160: 5f10 0f73 6372 6f6c 6c50 6f73 6974 696f  _..scrollPositio
+00001170: 6e59 5874 6578 7453 697a 655f 100f 7363  nYXtextSize_..sc
+00001180: 726f 6c6c 506f 7369 7469 6f6e 585a 736f  rollPositionXZso
+00001190: 7274 436f 6c75 6d6e 5f10 1075 7365 5265  rtColumn_..useRe
+000011a0: 6c61 7469 7665 4461 7465 735f 1012 7669  lativeDates_..vi
+000011b0: 6577 4f70 7469 6f6e 7356 6572 7369 6f6e  ewOptionsVersion
+000011c0: 2340 3000 0000 0000 0009 ae0e 171f 2428  #@0...........$(
+000011d0: 2d32 373c 4045 494d 51d4 0f10 1112 0c14  -27<@EIMQ.......
+000011e0: 0c16 5776 6973 6962 6c65 5577 6964 7468  ..WvisibleUwidth
+000011f0: 5961 7363 656e 6469 6e67 5a69 6465 6e74  YascendingZident
+00001200: 6966 6965 7209 1101 2c09 546e 616d 65d4  ifier...,.Tname.
+00001210: 1218 191a 1b1c 1d1d 5577 6964 7468 5961  ........UwidthYa
+00001220: 7363 656e 6469 6e67 5776 6973 6962 6c65  scendingWvisible
+00001230: 5875 6269 7175 6974 7910 2308 08d4 0f10  Xubiquity.#.....
+00001240: 1112 0c21 1d23 0910 b508 5c64 6174 654d  ...!.#....\dateM
+00001250: 6f64 6966 6965 64d4 0f10 1112 1d21 1d27  odified......!.'
+00001260: 0808 5b64 6174 6543 7265 6174 6564 d40f  ..[dateCreated..
+00001270: 1011 120c 2a1d 2c09 1061 0854 7369 7a65  ....*.,..a.Tsize
+00001280: d40f 1011 120c 2f0c 3109 1073 0954 6b69  ....../.1..s.Tki
+00001290: 6e64 d40f 1011 121d 340c 3608 1064 0955  nd......4.6..d.U
+000012a0: 6c61 6265 6cd4 0f10 1112 1d39 0c3b 0810  label......9.;..
+000012b0: 4b09 5776 6572 7369 6f6e d40f 1011 121d  K.Wversion......
+000012c0: 140c 3f08 0958 636f 6d6d 656e 7473 d40f  ..?..Xcomments..
+000012d0: 1011 121d 421d 4408 10c8 085e 6461 7465  ....B.D....^date
+000012e0: 4c61 7374 4f70 656e 6564 d40f 1011 121d  LastOpened......
+000012f0: 421d 4808 085a 7368 6172 654f 776e 6572  B.H..ZshareOwner
+00001300: d40f 1011 121d 421d 4c08 085f 100f 7368  ......B.L.._..sh
+00001310: 6172 654c 6173 7445 6469 746f 72d4 1218  areLastEditor...
+00001320: 191a 4e21 1d1d 5964 6174 6541 6464 6564  ..N!..YdateAdded
+00001330: 0808 d41a 1819 121d 531d 5508 10d2 085f  ........S.U...._
+00001340: 1010 696e 7669 7461 7469 6f6e 5374 6174  ..invitationStat
+00001350: 7573 0823 4043 8000 0000 0000 2340 2a00  us.#@C......#@*.
+00001360: 0000 0000 0023 0000 0000 0000 0000 546e  .....#........Tn
+00001370: 616d 6509 1400 0000 0000 0000 0000 0000  ame.............
+00001380: 0000 0000 0100 0800 1d00 2600 3800 4000  ..........&.8.@.
+00001390: 5400 6600 6f00 8100 8c00 9f00 b400 bd00  T.f.o...........
+000013a0: be00 cd00 d600 de00 e400 ee00 f900 fa00  ................
+000013b0: fd00 fe01 0301 0c01 1201 1c01 2401 2d01  ............$.-.
+000013c0: 2f01 3001 3101 3a01 3b01 3d01 3e01 4b01  /.0.1.:.;.=.>.K.
+000013d0: 5401 5501 5601 6201 6b01 6c01 6e01 6f01  T.U.V.b.k.l.n.o.
+000013e0: 7401 7d01 7e01 8001 8101 8601 8f01 9001  t.}.~...........
+000013f0: 9201 9301 9901 a201 a301 a501 a601 ae01  ................
+00001400: b701 b801 b901 c201 cb01 cc01 ce01 cf01  ................
+00001410: de01 e701 e801 e901 f401 fd01 fe01 ff02  ................
+00001420: 1102 1a02 2402 2502 2602 2f02 3002 3202  ....$.%.&./.0.2.
+00001430: 3302 4602 4702 5002 5902 6202 6702 6800  3.F.G.P.Y.b.g.h.
+00001440: 0000 0000 0002 0100 0000 0000 0000 5d00  ..............].
+00001450: 0000 0000 0000 0000 0000 0000 0002 7900  ..............y.
+00001460: 0000 0a00 6400 6100 7400 6100 5f00 6600  ....d.a.t.a._.f.
+00001470: 6900 6c00 6500 736c 7376 7062 6c6f 6200  i.l.e.slsvpblob.
+00001480: 0002 ae62 706c 6973 7430 30da 0102 0304  ...bplist00.....
+00001490: 0506 0708 090a 0b0c 0d1f 4748 494a 0c4c  ..........GHIJ.L
+000014a0: 5869 636f 6e53 697a 655f 100f 7368 6f77  XiconSize_..show
+000014b0: 4963 6f6e 5072 6576 6965 7757 636f 6c75  IconPreviewWcolu
+000014c0: 6d6e 735f 1011 6361 6c63 756c 6174 6541  mns_..calculateA
+000014d0: 6c6c 5369 7a65 735f 100f 7363 726f 6c6c  llSizes_..scroll
+000014e0: 506f 7369 7469 6f6e 5958 7465 7874 5369  PositionYXtextSi
+000014f0: 7a65 5f10 0f73 6372 6f6c 6c50 6f73 6974  ze_..scrollPosit
+00001500: 696f 6e58 5a73 6f72 7443 6f6c 756d 6e5f  ionXZsortColumn_
+00001510: 1010 7573 6552 656c 6174 6976 6544 6174  ..useRelativeDat
+00001520: 6573 5f10 1276 6965 774f 7074 696f 6e73  es_..viewOptions
+00001530: 5665 7273 696f 6e23 4030 0000 0000 0000  Version#@0......
+00001540: 09d9 0e0f 1011 1213 1415 1617 2025 2a2f  ............ %*/
+00001550: 3438 3d41 5863 6f6d 6d65 6e74 7355 6c61  48=AXcommentsUla
+00001560: 6265 6c57 7665 7273 696f 6e5b 6461 7465  belWversion[date
+00001570: 4372 6561 7465 6454 7369 7a65 5c64 6174  CreatedTsize\dat
+00001580: 654d 6f64 6966 6965 6454 6b69 6e64 546e  eModifiedTkindTn
+00001590: 616d 655e 6461 7465 4c61 7374 4f70 656e  ame^dateLastOpen
+000015a0: 6564 d418 191a 1b1c 1d0c 1f55 696e 6465  ed.........Uinde
+000015b0: 7855 7769 6474 6859 6173 6365 6e64 696e  xUwidthYascendin
+000015c0: 6757 7669 7369 626c 6510 0711 012c 0908  gWvisible....,..
+000015d0: d418 191a 1b21 220c 1f10 0510 6409 08d4  .....!".....d...
+000015e0: 1819 1a1b 2627 0c1f 1006 104b 0908 d418  ....&'.....K....
+000015f0: 191a 1b2b 2c1f 1f10 0210 b508 08d4 1819  ...+,...........
+00001600: 1a1b 3031 1f0c 1003 1061 0809 d418 191a  ..01.....a......
+00001610: 1b35 2c1f 0c10 0108 09d4 1819 1a1b 393a  .5,...........9:
+00001620: 0c0c 1004 1073 0909 d418 191a 1b3e 1d0c  .....s.......>..
+00001630: 0c10 0009 09d4 1819 1a1b 4243 1f1f 1008  ..........BC....
+00001640: 10c8 0808 0823 4043 8000 0000 0000 2340  .....#@C......#@
+00001650: 2a00 0000 0000 0023 0000 0000 0000 0000  *......#........
+00001660: 546e 616d 6509 1400 0000 0000 0000 0000  Tname...........
+00001670: 0000 0000 0000 0100 0800 1d00 2600 3800  ............&.8.
+00001680: 4000 5400 6600 6f00 8100 8c00 9f00 b400  @.T.f.o.........
+00001690: bd00 be00 d100 da00 e000 e800 f400 f901  ................
+000016a0: 0601 0b01 1001 1f01 2801 2e01 3401 3e01  ........(...4.>.
+000016b0: 4601 4801 4b01 4c01 4d01 5601 5801 5a01  F.H.K.L.M.V.X.Z.
+000016c0: 5b01 5c01 6501 6701 6901 6a01 6b01 7401  [.\.e.g.i.j.k.t.
+000016d0: 7601 7801 7901 7a01 8301 8501 8701 8801  v.x.y.z.........
+000016e0: 8901 9201 9401 9501 9601 9f01 a101 a301  ................
+000016f0: a401 a501 ae01 b001 b101 b201 bb01 bd01  ................
+00001700: bf01 c001 c101 c201 cb01 d401 dd01 e201  ................
+00001710: e300 0000 0000 0002 0100 0000 0000 0000  ................
+00001720: 4d00 0000 0000 0000 0000 0000 0000 0001  M...............
+00001730: f400 0000 0a00 6400 6100 7400 6100 5f00  ......d.a.t.a._.
+00001740: 6600 6900 6c00 6500 7376 5372 6e6c 6f6e  f.i.l.e.svSrnlon
+00001750: 6700 0000 0100 0000 0700 6d00 6f00 6600  g.........m.o.f.
+00001760: 6100 7000 7900 3249 6c6f 6362 6c6f 6200  a.p.y.2Ilocblob.
+00001770: 0000 1000 0000 4100 0000 9eff ffff ffff  ......A.........
+00001780: ff00 0000 0000 0700 6d00 6f00 6600 6100  ........m.o.f.a.
+00001790: 7000 7900 3262 7773 7062 6c6f 6200 0000  p.y.2bwspblob...
+000017a0: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+000017b0: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+000017c0: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+000017d0: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+000017e0: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+000017f0: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00001800: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+00001810: 5f10 187b 7b31 3839 2c20 3133 317d 2c20  _..{{189, 131}, 
+00001820: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
+00001830: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+00001840: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00001850: 0000 0000 0000 0000 8b00 0000 0700 6d00  ..............m.
+00001860: 6f00 6600 6100 7000 7900 3264 7363 6c62  o.f.a.p.y.2dsclb
+00001870: 6f6f 6c00 0000 0007 006d 006f 0066 0061  ool......m.o.f.a
+00001880: 0070 0079 0032 7653 726e 6c6f 6e67 0000  .p.y.2vSrnlong..
+00001890: 0001 0000 0004 006e 006f 0063 0064 496c  .......n.o.c.dIl
+000018a0: 6f63 626c 6f62 0000 0010 0000 01f9 0000  ocblob..........
+000018b0: 002e ffff ffff ffff 0000 0000 0008 0070  ...............p
+000018c0: 0061 006c 0061 006e 0074 0069 0072 6277  .a.l.a.n.t.i.rbw
+000018d0: 7370 626c 6f62 0000 00b8 6270 6c69 7374  spblob....bplist
+000018e0: 3030 d601 0203 0405 0607 0807 080b 085d  00.............]
+000018f0: 5368 6f77 5374 6174 7573 4261 725b 5368  ShowStatusBar[Sh
+00001900: 6f77 546f 6f6c 6261 725b 5368 6f77 5461  owToolbar[ShowTa
+00001910: 6256 6965 775f 1014 436f 6e74 6169 6e65  bView_..Containe
+00001920: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00001930: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00001940: 6465 6261 7208 0908 095f 1018 7b7b 3139  debar...._..{{19
+00001950: 312c 2031 3630 7d2c 207b 3932 302c 2034  1, 160}, {920, 4
+00001960: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00001970: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00001980: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00001990: 008b 0000 0008 0070 0061 006c 0061 006e  .......p.a.l.a.n
+000019a0: 0074 0069 0072 7653 726e 6c6f 6e67 0000  .t.i.rvSrnlong..
+000019b0: 0001 0000 0008 0053 0045 0041 0043 0065  .......S.E.A.C.e
+000019c0: 006c 006c 0073 6277 7370 626c 6f62 0000  .l.l.sbwspblob..
+000019d0: 00b7 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+000019e0: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+000019f0: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
+00001a00: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00001a10: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00001a20: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00001a30: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+00001a40: 095f 1017 7b7b 3536 2c20 3138 337d 2c20  ._..{{56, 183}, 
+00001a50: 7b39 3631 2c20 3438 387d 7d09 0815 232f  {961, 488}}...#/
+00001a60: 3b52 5f6b 6c6d 6e6f 8900 0000 0000 0001  ;R_klmno........
+00001a70: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00001a80: 0000 0000 0000 0000 8a00 0000 0800 5300  ..............S.
+00001a90: 4500 4100 4300 6500 6c00 6c00 7376 5372  E.A.C.e.l.l.svSr
+00001aa0: 6e6c 6f6e 6700 0000 0100 0000 0600 7300  nlong.........s.
+00001ab0: 6900 6e00 6700 6c00 6549 6c6f 6362 6c6f  i.n.g.l.eIlocblo
+00001ac0: 6200 0000 1000 0001 8b00 0000 2eff ffff  b...............
+00001ad0: ffff ff00 0000 0000 0600 7300 6900 6e00  ..........s.i.n.
+00001ae0: 6700 6c00 6562 7773 7062 6c6f 6200 0000  g.l.ebwspblob...
+00001af0: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00001b00: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00001b10: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00001b20: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00001b30: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00001b40: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00001b50: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+00001b60: 5f10 187b 7b35 3932 2c20 3231 367d 2c20  _..{{592, 216}, 
+00001b70: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
+00001b80: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+00001b90: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00001ba0: 0000 0000 0000 0000 8b00 0000 0600 7300  ..............s.
+00001bb0: 6900 6e00 6700 6c00 6564 7363 6c62 6f6f  i.n.g.l.edsclboo
+00001bc0: 6c00 0000 0006 0073 0069 006e 0067 006c  l......s.i.n.g.l
+00001bd0: 0065 7653 726e 6c6f 6e67 0000 0001 0000  .evSrnlong......
+00001be0: 0007 0073 0070 0061 0074 0072 0069 006f  ...s.p.a.t.r.i.o
+00001bf0: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00001c00: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00001c10: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00001c20: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00001c30: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001c40: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001c50: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001c60: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00001c70: 3539 322c 2033 3132 7d2c 207b 3932 302c  592, 312}, {920,
+00001c80: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00001c90: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00001ca0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00001cb0: 0000 008b 0000 0007 0073 0070 0061 0074  .........s.p.a.t
+00001cc0: 0072 0069 006f 6c67 3153 636f 6d70 0000  .r.i.olg1Scomp..
+00001cd0: 0000 0001 581f 0000 0007 0073 0070 0061  ....X......s.p.a
+00001ce0: 0074 0072 0069 006f 6d6f 4444 626c 6f62  .t.r.i.omoDDblob
+00001cf0: 0000 0008 c1ee 78cc dddc c441 0000 0007  ......x....A....
+00001d00: 0073 0070 0061 0074 0072 0069 006f 6d6f  .s.p.a.t.r.i.omo
+00001d10: 6444 626c 6f62 0000 0008 c1ee 78cc dddc  dDblob......x...
+00001d20: c441 0000 0007 0073 0070 0061 0074 0072  .A.....s.p.a.t.r
+00001d30: 0069 006f 7068 3153 636f 6d70 0000 0000  .i.oph1Scomp....
+00001d40: 0001 f000 0000 0007 0073 0070 0061 0074  .........s.p.a.t
+00001d50: 0072 0069 006f 7653 726e 6c6f 6e67 0000  .r.i.ovSrnlong..
+00001d60: 0001 0000 000b 0053 0054 0041 0047 0041  .......S.T.A.G.A
+00001d70: 0054 0045 005f 0070 0079 0047 6277 7370  .T.E._.p.y.Gbwsp
+00001d80: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00001d90: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00001da0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00001db0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00001dc0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00001dd0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00001de0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00001df0: 6261 7208 0908 095f 1018 7b7b 3139 302c  bar...._..{{190,
+00001e00: 2031 3630 7d2c 207b 3932 302c 2034 3336   160}, {920, 436
+00001e10: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00001e20: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00001e30: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00001e40: 0000 000b 0053 0054 0041 0047 0041 0054  .....S.T.A.G.A.T
+00001e50: 0045 005f 0070 0079 0047 7653 726e 6c6f  .E._.p.y.GvSrnlo
+00001e60: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
+00001e70: 006c 0073 496c 6f63 626c 6f62 0000 0010  .l.sIlocblob....
+00001e80: 0000 0267 0000 002e ffff ffff ffff 0000  ...g............
+00001e90: 0000 0003 0076 0069 0061 496c 6f63 626c  .....v.i.aIlocbl
+00001ea0: 6f62 0000 0010 0000 00af 0000 009e ffff  ob..............
+00001eb0: ffff ffff 0000 0000 0003 0076 0069 0061  ...........v.i.a
+00001ec0: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00001ed0: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00001ee0: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00001ef0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00001f00: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00001f10: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00001f20: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00001f30: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00001f40: 3531 302c 2031 3834 7d2c 207b 3932 302c  510, 184}, {920,
+00001f50: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00001f60: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00001f70: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00001f80: 0000 008b 0000 0003 0076 0069 0061 7653  .........v.i.avS
+00001f90: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00001fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00001ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002000: 0000 0000 0000 0000 0000 0009 0000 000b  ................
+00002000: 0000 0000 0000 0000 0000 000b 0000 000b  ................
 00002010: 005f 005f 0069 006e 0069 0074 005f 005f  ._._.i.n.i.t._._
 00002020: 002e 0070 0079 496c 6f63 626c 6f62 0000  ...p.yIlocblob..
 00002030: 0010 0000 0041 0000 002e ffff ffff ffff  .....A..........
 00002040: 0000 0000 0004 0062 0075 006c 006b 496c  .......b.u.l.kIl
 00002050: 6f63 626c 6f62 0000 0010 0000 011d 0000  ocblob..........
 00002060: 002e ffff ffff ffff 0000 0000 0004 0062  ...............b
 00002070: 0075 006c 006b 6277 7370 626c 6f62 0000  .u.l.kbwspblob..
@@ -636,134 +636,134 @@
 000027b0: 5f10 1443 6f6e 7461 696e 6572 5368 6f77  _..ContainerShow
 000027c0: 5369 6465 6261 725c 5769 6e64 6f77 426f  Sidebar\WindowBo
 000027d0: 756e 6473 5b53 686f 7753 6964 6562 6172  unds[ShowSidebar
 000027e0: 0809 0809 5f10 187b 7b33 3235 2c20 3335  ...._..{{325, 35
 000027f0: 357d 2c20 7b39 3230 2c20 3433 367d 7d09  5}, {920, 436}}.
 00002800: 0815 232f 3b52 5f6b 6c6d 6e6f 8a00 0000  ..#/;R_klmno....
 00002810: 0000 0001 0100 0000 0000 0000 0d00 0000  ................
-00002820: 0000 0000 0000 0000 0000 0000 8b00 6900  ..............i.
-00002830: 6c00 6500 7376 5372 6e6c 6f6e 6700 0000  l.e.svSrnlong...
-00002840: 0100 0000 0700 6d00 6f00 6600 6100 7000  ......m.o.f.a.p.
-00002850: 7900 3249 6c6f 6362 6c6f 6200 0000 1000  y.2Ilocblob.....
-00002860: 0000 4100 0000 9eff ffff ffff ff00 0000  ..A.............
-00002870: 0000 0700 6d00 6f00 6600 6100 7000 7900  ....m.o.f.a.p.y.
-00002880: 3262 7773 7062 6c6f 6200 0000 b862 706c  2bwspblob....bpl
-00002890: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-000028a0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-000028b0: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-000028c0: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-000028d0: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-000028e0: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-000028f0: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00002900: 7b31 3839 2c20 3133 317d 2c20 7b39 3230  {189, 131}, {920
-00002910: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-00002920: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
-00002930: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00002940: 0000 0000 8b00 0000 0700 6d00 6f00 6600  ..........m.o.f.
-00002950: 6100 7000 7900 3264 7363 6c62 6f6f 6c00  a.p.y.2dsclbool.
-00002960: 0000 0007 006d 006f 0066 0061 0070 0079  .....m.o.f.a.p.y
-00002970: 0032 7653 726e 6c6f 6e67 0000 0001 0000  .2vSrnlong......
-00002980: 0004 006e 006f 0063 0064 496c 6f63 626c  ...n.o.c.dIlocbl
-00002990: 6f62 0000 0010 0000 01f9 0000 002e ffff  ob..............
-000029a0: ffff ffff 0000 0000 0008 0070 0061 006c  ...........p.a.l
-000029b0: 0061 006e 0074 0069 0072 6277 7370 626c  .a.n.t.i.rbwspbl
-000029c0: 6f62 0000 00b8 6270 6c69 7374 3030 d601  ob....bplist00..
-000029d0: 0203 0405 0607 0807 080b 085d 5368 6f77  ...........]Show
-000029e0: 5374 6174 7573 4261 725b 5368 6f77 546f  StatusBar[ShowTo
-000029f0: 6f6c 6261 725b 5368 6f77 5461 6256 6965  olbar[ShowTabVie
-00002a00: 775f 1014 436f 6e74 6169 6e65 7253 686f  w_..ContainerSho
-00002a10: 7753 6964 6562 6172 5c57 696e 646f 7742  wSidebar\WindowB
-00002a20: 6f75 6e64 735b 5368 6f77 5369 6465 6261  ounds[ShowSideba
-00002a30: 7208 0908 095f 1018 7b7b 3139 312c 2031  r...._..{{191, 1
-00002a40: 3630 7d2c 207b 3932 302c 2034 3336 7d7d  60}, {920, 436}}
-00002a50: 0908 1523 2f3b 525f 6b6c 6d6e 6f8a 0000  ...#/;R_klmno...
-00002a60: 0000 0000 0101 0000 0000 0000 000d 0000  ................
-00002a70: 0000 0000 0000 0000 0000 0000 008b 0000  ................
-00002a80: 0008 0070 0061 006c 0061 006e 0074 0069  ...p.a.l.a.n.t.i
-00002a90: 0072 7653 726e 6c6f 6e67 0000 0001 0000  .rvSrnlong......
-00002aa0: 0008 0053 0045 0041 0043 0065 006c 006c  ...S.E.A.C.e.l.l
-00002ab0: 0073 6277 7370 626c 6f62 0000 00b7 6270  .sbwspblob....bp
-00002ac0: 6c69 7374 3030 d601 0203 0405 0607 0807  list00..........
-00002ad0: 080b 085d 5368 6f77 5374 6174 7573 4261  ...]ShowStatusBa
-00002ae0: 725b 5368 6f77 546f 6f6c 6261 725b 5368  r[ShowToolbar[Sh
-00002af0: 6f77 5461 6256 6965 775f 1014 436f 6e74  owTabView_..Cont
-00002b00: 6169 6e65 7253 686f 7753 6964 6562 6172  ainerShowSidebar
-00002b10: 5c57 696e 646f 7742 6f75 6e64 735b 5368  \WindowBounds[Sh
-00002b20: 6f77 5369 6465 6261 7208 0908 095f 1017  owSidebar...._..
-00002b30: 7b7b 3536 2c20 3138 337d 2c20 7b39 3631  {{56, 183}, {961
-00002b40: 2c20 3438 387d 7d09 0815 232f 3b52 5f6b  , 488}}...#/;R_k
-00002b50: 6c6d 6e6f 8900 0000 0000 0001 0100 0000  lmno............
-00002b60: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00002b70: 0000 0000 8a00 0000 0800 5300 4500 4100  ..........S.E.A.
-00002b80: 4300 6500 6c00 6c00 7376 5372 6e6c 6f6e  C.e.l.l.svSrnlon
-00002b90: 6700 0000 0100 0000 0600 7300 6900 6e00  g.........s.i.n.
-00002ba0: 6700 6c00 6549 6c6f 6362 6c6f 6200 0000  g.l.eIlocblob...
-00002bb0: 1000 0001 8b00 0000 2eff ffff ffff ff00  ................
-00002bc0: 0000 0000 0600 7300 6900 6e00 6700 6c00  ......s.i.n.g.l.
-00002bd0: 6562 7773 7062 6c6f 6200 0000 b862 706c  ebwspblob....bpl
-00002be0: 6973 7430 30d6 0102 0304 0506 0708 0708  ist00...........
-00002bf0: 0b08 5d53 686f 7753 7461 7475 7342 6172  ..]ShowStatusBar
-00002c00: 5b53 686f 7754 6f6f 6c62 6172 5b53 686f  [ShowToolbar[Sho
-00002c10: 7754 6162 5669 6577 5f10 1443 6f6e 7461  wTabView_..Conta
-00002c20: 696e 6572 5368 6f77 5369 6465 6261 725c  inerShowSidebar\
-00002c30: 5769 6e64 6f77 426f 756e 6473 5b53 686f  WindowBounds[Sho
-00002c40: 7753 6964 6562 6172 0809 0809 5f10 187b  wSidebar...._..{
-00002c50: 7b35 3932 2c20 3231 367d 2c20 7b39 3230  {592, 216}, {920
-00002c60: 2c20 3433 367d 7d09 0815 232f 3b52 5f6b  , 436}}...#/;R_k
-00002c70: 6c6d 6e6f 8a00 0000 0000 0001 0100 0000  lmno............
-00002c80: 0000 0000 0d00 0000 0000 0000 0000 0000  ................
-00002c90: 0000 0000 8b00 0000 0600 7300 6900 6e00  ..........s.i.n.
-00002ca0: 6700 6c00 6564 7363 6c62 6f6f 6c00 0000  g.l.edsclbool...
-00002cb0: 0006 0073 0069 006e 0067 006c 0065 7653  ...s.i.n.g.l.evS
-00002cc0: 726e 6c6f 6e67 0000 0001 0000 000b 0053  rnlong.........S
-00002cd0: 0054 0041 0047 0041 0054 0045 005f 0070  .T.A.G.A.T.E._.p
-00002ce0: 0079 0047 6277 7370 626c 6f62 0000 00b8  .y.Gbwspblob....
-00002cf0: 6270 6c69 7374 3030 d601 0203 0405 0607  bplist00........
-00002d00: 0807 080b 085d 5368 6f77 5374 6174 7573  .....]ShowStatus
-00002d10: 4261 725b 5368 6f77 546f 6f6c 6261 725b  Bar[ShowToolbar[
-00002d20: 5368 6f77 5461 6256 6965 775f 1014 436f  ShowTabView_..Co
-00002d30: 6e74 6169 6e65 7253 686f 7753 6964 6562  ntainerShowSideb
-00002d40: 6172 5c57 696e 646f 7742 6f75 6e64 735b  ar\WindowBounds[
-00002d50: 5368 6f77 5369 6465 6261 7208 0908 095f  ShowSidebar...._
-00002d60: 1018 7b7b 3139 302c 2031 3630 7d2c 207b  ..{{190, 160}, {
-00002d70: 3932 302c 2034 3336 7d7d 0908 1523 2f3b  920, 436}}...#/;
-00002d80: 525f 6b6c 6d6e 6f8a 0000 0000 0000 0101  R_klmno.........
-00002d90: 0000 0000 0000 000d 0000 0000 0000 0000  ................
-00002da0: 0000 0000 0000 008b 0000 000b 0053 0054  .............S.T
-00002db0: 0041 0047 0041 0054 0045 005f 0070 0079  .A.G.A.T.E._.p.y
-00002dc0: 0047 7653 726e 6c6f 6e67 0000 0001 0000  .GvSrnlong......
-00002dd0: 0005 0075 0074 0069 006c 0073 496c 6f63  ...u.t.i.l.sIloc
-00002de0: 626c 6f62 0000 0010 0000 0267 0000 002e  blob.......g....
-00002df0: ffff ffff ffff 0000 0000 0003 0076 0069  .............v.i
-00002e00: 0061 496c 6f63 626c 6f62 0000 0010 0000  .aIlocblob......
-00002e10: 00af 0000 009e ffff ffff ffff 0000 0000  ................
-00002e20: 0003 0076 0069 0061 6277 7370 626c 6f62  ...v.i.abwspblob
-00002e30: 0000 00b8 6270 6c69 7374 3030 d601 0203  ....bplist00....
-00002e40: 0405 0607 0807 080b 085d 5368 6f77 5374  .........]ShowSt
-00002e50: 6174 7573 4261 725b 5368 6f77 546f 6f6c  atusBar[ShowTool
-00002e60: 6261 725b 5368 6f77 5461 6256 6965 775f  bar[ShowTabView_
-00002e70: 1014 436f 6e74 6169 6e65 7253 686f 7753  ..ContainerShowS
-00002e80: 6964 6562 6172 5c57 696e 646f 7742 6f75  idebar\WindowBou
-00002e90: 6e64 735b 5368 6f77 5369 6465 6261 7208  nds[ShowSidebar.
-00002ea0: 0908 095f 1018 7b7b 3531 302c 2031 3834  ..._..{{510, 184
-00002eb0: 7d2c 207b 3932 302c 2034 3336 7d7d 0908  }, {920, 436}}..
-00002ec0: 1523 2f3b 525f 6b6c 6d6e 6f8a 0000 0000  .#/;R_klmno.....
-00002ed0: 0000 0101 0000 0000 0000 000d 0000 0000  ................
-00002ee0: 0000 0000 0000 0000 0000 008b 0000 0003  ................
-00002ef0: 0076 0069 0061 7653 726e 6c6f 6e67 0000  .v.i.avSrnlong..
-00002f00: 0001 0000 0000 0000 0000 0000 0000 0000  ................
-00002f10: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f20: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f30: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f40: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f50: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f60: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f70: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f80: 0000 0000 0000 0000 0000 0000 0000 0000  ................
-00002f90: 0000 0000 0000 0000 0000 0000 0000 0000  ................
+00002820: 0000 0000 0000 0000 0000 0000 8b00 0000  ................
+00002830: 0600 4300 4500 4600 4300 4f00 4e76 5372  ..C.E.F.C.O.NvSr
+00002840: 6e6c 6f6e 6700 0000 0100 0000 0500 6300  nlong.........c.
+00002850: 7900 6c00 6900 6262 7773 7062 6c6f 6200  y.l.i.bbwspblob.
+00002860: 0000 b862 706c 6973 7430 30d6 0102 0304  ...bplist00.....
+00002870: 0506 0708 0708 0b08 5d53 686f 7753 7461  ........]ShowSta
+00002880: 7475 7342 6172 5b53 686f 7754 6f6f 6c62  tusBar[ShowToolb
+00002890: 6172 5b53 686f 7754 6162 5669 6577 5f10  ar[ShowTabView_.
+000028a0: 1443 6f6e 7461 696e 6572 5368 6f77 5369  .ContainerShowSi
+000028b0: 6465 6261 725c 5769 6e64 6f77 426f 756e  debar\WindowBoun
+000028c0: 6473 5b53 686f 7753 6964 6562 6172 0809  ds[ShowSidebar..
+000028d0: 0809 5f10 187b 7b31 3530 2c20 3233 307d  .._..{{150, 230}
+000028e0: 2c20 7b39 3230 2c20 3433 367d 7d09 0815  , {920, 436}}...
+000028f0: 232f 3b52 5f6b 6c6d 6e6f 8a00 0000 0000  #/;R_klmno......
+00002900: 0001 0100 0000 0000 0000 0d00 0000 0000  ................
+00002910: 0000 0000 0000 0000 0000 8b74 6169 6e65  ...........taine
+00002920: 7253 686f 7753 6964 6562 6172 5c57 696e  rShowSidebar\Win
+00002930: 646f 7742 6f75 6e64 735b 5368 6f77 5369  dowBounds[ShowSi
+00002940: 6465 6261 7208 0908 095f 1018 7b7b 3139  debar...._..{{19
+00002950: 312c 2031 3630 7d2c 207b 3932 302c 2034  1, 160}, {920, 4
+00002960: 3336 7d7d 0908 1523 2f3b 525f 6b6c 6d6e  36}}...#/;R_klmn
+00002970: 6f8a 0000 0000 0000 0101 0000 0000 0000  o...............
+00002980: 000d 0000 0000 0000 0000 0000 0000 0000  ................
+00002990: 008b 0000 0008 0070 0061 006c 0061 006e  .......p.a.l.a.n
+000029a0: 0074 0069 0072 7653 726e 6c6f 6e67 0000  .t.i.rvSrnlong..
+000029b0: 0001 0000 0008 0053 0045 0041 0043 0065  .......S.E.A.C.e
+000029c0: 006c 006c 0073 6277 7370 626c 6f62 0000  .l.l.sbwspblob..
+000029d0: 00b7 6270 6c69 7374 3030 d601 0203 0405  ..bplist00......
+000029e0: 0607 0807 080b 085d 5368 6f77 5374 6174  .......]ShowStat
+000029f0: 7573 4261 725b 5368 6f77 546f 6f6c 6261  usBar[ShowToolba
+00002a00: 725b 5368 6f77 5461 6256 6965 775f 1014  r[ShowTabView_..
+00002a10: 436f 6e74 6169 6e65 7253 686f 7753 6964  ContainerShowSid
+00002a20: 6562 6172 5c57 696e 646f 7742 6f75 6e64  ebar\WindowBound
+00002a30: 735b 5368 6f77 5369 6465 6261 7208 0908  s[ShowSidebar...
+00002a40: 095f 1017 7b7b 3536 2c20 3138 337d 2c20  ._..{{56, 183}, 
+00002a50: 7b39 3631 2c20 3438 387d 7d09 0815 232f  {961, 488}}...#/
+00002a60: 3b52 5f6b 6c6d 6e6f 8900 0000 0000 0001  ;R_klmno........
+00002a70: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00002a80: 0000 0000 0000 0000 8a00 0000 0800 5300  ..............S.
+00002a90: 4500 4100 4300 6500 6c00 6c00 7376 5372  E.A.C.e.l.l.svSr
+00002aa0: 6e6c 6f6e 6700 0000 0100 0000 0600 7300  nlong.........s.
+00002ab0: 6900 6e00 6700 6c00 6549 6c6f 6362 6c6f  i.n.g.l.eIlocblo
+00002ac0: 6200 0000 1000 0001 8b00 0000 2eff ffff  b...............
+00002ad0: ffff ff00 0000 0000 0600 7300 6900 6e00  ..........s.i.n.
+00002ae0: 6700 6c00 6562 7773 7062 6c6f 6200 0000  g.l.ebwspblob...
+00002af0: b862 706c 6973 7430 30d6 0102 0304 0506  .bplist00.......
+00002b00: 0708 0708 0b08 5d53 686f 7753 7461 7475  ......]ShowStatu
+00002b10: 7342 6172 5b53 686f 7754 6f6f 6c62 6172  sBar[ShowToolbar
+00002b20: 5b53 686f 7754 6162 5669 6577 5f10 1443  [ShowTabView_..C
+00002b30: 6f6e 7461 696e 6572 5368 6f77 5369 6465  ontainerShowSide
+00002b40: 6261 725c 5769 6e64 6f77 426f 756e 6473  bar\WindowBounds
+00002b50: 5b53 686f 7753 6964 6562 6172 0809 0809  [ShowSidebar....
+00002b60: 5f10 187b 7b35 3932 2c20 3231 367d 2c20  _..{{592, 216}, 
+00002b70: 7b39 3230 2c20 3433 367d 7d09 0815 232f  {920, 436}}...#/
+00002b80: 3b52 5f6b 6c6d 6e6f 8a00 0000 0000 0001  ;R_klmno........
+00002b90: 0100 0000 0000 0000 0d00 0000 0000 0000  ................
+00002ba0: 0000 0000 0000 0000 8b00 0000 0600 7300  ..............s.
+00002bb0: 6900 6e00 6700 6c00 6564 7363 6c62 6f6f  i.n.g.l.edsclboo
+00002bc0: 6c00 0000 0006 0073 0069 006e 0067 006c  l......s.i.n.g.l
+00002bd0: 0065 7653 726e 6c6f 6e67 0000 0001 0000  .evSrnlong......
+00002be0: 0007 0073 0070 0061 0074 0072 0069 006f  ...s.p.a.t.r.i.o
+00002bf0: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00002c00: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00002c10: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00002c20: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00002c30: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00002c40: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00002c50: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00002c60: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00002c70: 3539 322c 2033 3132 7d2c 207b 3932 302c  592, 312}, {920,
+00002c80: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00002c90: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00002ca0: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00002cb0: 0000 008b 0000 0007 0073 0070 0061 0074  .........s.p.a.t
+00002cc0: 0072 0069 006f 6c67 3153 636f 6d70 0000  .r.i.olg1Scomp..
+00002cd0: 0000 0001 581f 0000 0007 0073 0070 0061  ....X......s.p.a
+00002ce0: 0074 0072 0069 006f 6d6f 4444 626c 6f62  .t.r.i.omoDDblob
+00002cf0: 0000 0008 c1ee 78cc dddc c441 0000 0007  ......x....A....
+00002d00: 0073 0070 0061 0074 0072 0069 006f 6d6f  .s.p.a.t.r.i.omo
+00002d10: 6444 626c 6f62 0000 0008 c1ee 78cc dddc  dDblob......x...
+00002d20: c441 0000 0007 0073 0070 0061 0074 0072  .A.....s.p.a.t.r
+00002d30: 0069 006f 7068 3153 636f 6d70 0000 0000  .i.oph1Scomp....
+00002d40: 0001 f000 0000 0007 0073 0070 0061 0074  .........s.p.a.t
+00002d50: 0072 0069 006f 7653 726e 6c6f 6e67 0000  .r.i.ovSrnlong..
+00002d60: 0001 0000 000b 0053 0054 0041 0047 0041  .......S.T.A.G.A
+00002d70: 0054 0045 005f 0070 0079 0047 6277 7370  .T.E._.p.y.Gbwsp
+00002d80: 626c 6f62 0000 00b8 6270 6c69 7374 3030  blob....bplist00
+00002d90: d601 0203 0405 0607 0807 080b 085d 5368  .............]Sh
+00002da0: 6f77 5374 6174 7573 4261 725b 5368 6f77  owStatusBar[Show
+00002db0: 546f 6f6c 6261 725b 5368 6f77 5461 6256  Toolbar[ShowTabV
+00002dc0: 6965 775f 1014 436f 6e74 6169 6e65 7253  iew_..ContainerS
+00002dd0: 686f 7753 6964 6562 6172 5c57 696e 646f  howSidebar\Windo
+00002de0: 7742 6f75 6e64 735b 5368 6f77 5369 6465  wBounds[ShowSide
+00002df0: 6261 7208 0908 095f 1018 7b7b 3139 302c  bar...._..{{190,
+00002e00: 2031 3630 7d2c 207b 3932 302c 2034 3336   160}, {920, 436
+00002e10: 7d7d 0908 1523 2f3b 525f 6b6c 6d6e 6f8a  }}...#/;R_klmno.
+00002e20: 0000 0000 0000 0101 0000 0000 0000 000d  ................
+00002e30: 0000 0000 0000 0000 0000 0000 0000 008b  ................
+00002e40: 0000 000b 0053 0054 0041 0047 0041 0054  .....S.T.A.G.A.T
+00002e50: 0045 005f 0070 0079 0047 7653 726e 6c6f  .E._.p.y.GvSrnlo
+00002e60: 6e67 0000 0001 0000 0005 0075 0074 0069  ng.........u.t.i
+00002e70: 006c 0073 496c 6f63 626c 6f62 0000 0010  .l.sIlocblob....
+00002e80: 0000 0267 0000 002e ffff ffff ffff 0000  ...g............
+00002e90: 0000 0003 0076 0069 0061 496c 6f63 626c  .....v.i.aIlocbl
+00002ea0: 6f62 0000 0010 0000 00af 0000 009e ffff  ob..............
+00002eb0: ffff ffff 0000 0000 0003 0076 0069 0061  ...........v.i.a
+00002ec0: 6277 7370 626c 6f62 0000 00b8 6270 6c69  bwspblob....bpli
+00002ed0: 7374 3030 d601 0203 0405 0607 0807 080b  st00............
+00002ee0: 085d 5368 6f77 5374 6174 7573 4261 725b  .]ShowStatusBar[
+00002ef0: 5368 6f77 546f 6f6c 6261 725b 5368 6f77  ShowToolbar[Show
+00002f00: 5461 6256 6965 775f 1014 436f 6e74 6169  TabView_..Contai
+00002f10: 6e65 7253 686f 7753 6964 6562 6172 5c57  nerShowSidebar\W
+00002f20: 696e 646f 7742 6f75 6e64 735b 5368 6f77  indowBounds[Show
+00002f30: 5369 6465 6261 7208 0908 095f 1018 7b7b  Sidebar...._..{{
+00002f40: 3531 302c 2031 3834 7d2c 207b 3932 302c  510, 184}, {920,
+00002f50: 2034 3336 7d7d 0908 1523 2f3b 525f 6b6c   436}}...#/;R_kl
+00002f60: 6d6e 6f8a 0000 0000 0000 0101 0000 0000  mno.............
+00002f70: 0000 000d 0000 0000 0000 0000 0000 0000  ................
+00002f80: 0000 008b 0000 0003 0076 0069 0061 7653  .........v.i.avS
+00002f90: 726e 6c6f 6e67 0000 0001 0000 0000 0000  rnlong..........
 00002fa0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fb0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fc0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fd0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002fe0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00002ff0: 0000 0000 0000 0000 0000 0000 0000 0000  ................
 00003000: 0000 0000 0000 0005 0000 0000 0000 300b  ..............0.
```

### Comparing `omicverse-1.5.8/omicverse/CEFCON/.DS_Store` & `omicverse-1.5.9/omicverse/CEFCON/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/CEFCON.py` & `omicverse-1.5.9/omicverse/CEFCON/CEFCON.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/__init__.py` & `omicverse-1.5.9/omicverse/CEFCON/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/cefcon_result_object.py` & `omicverse-1.5.9/omicverse/CEFCON/cefcon_result_object.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/cell_lineage_GRN.py` & `omicverse-1.5.9/omicverse/CEFCON/cell_lineage_GRN.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/datasets.py` & `omicverse-1.5.9/omicverse/CEFCON/datasets.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/driver_regulators.py` & `omicverse-1.5.9/omicverse/CEFCON/driver_regulators.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/eval_utils.py` & `omicverse-1.5.9/omicverse/CEFCON/eval_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/resources/__init__.py` & `omicverse-1.5.9/omicverse/CEFCON/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/resources/hs_hgnc_tfs_animaltfdb4.txt` & `omicverse-1.5.9/omicverse/CEFCON/resources/hs_hgnc_tfs_animaltfdb4.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/resources/hs_hgnc_tfs_lambert2018.txt` & `omicverse-1.5.9/omicverse/CEFCON/resources/hs_hgnc_tfs_lambert2018.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/resources/mm_mgi_tfs.txt` & `omicverse-1.5.9/omicverse/CEFCON/resources/mm_mgi_tfs.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/resources/mm_mgi_tfs_animaltfdb4.txt` & `omicverse-1.5.9/omicverse/CEFCON/resources/mm_mgi_tfs_animaltfdb4.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/CEFCON/utils.py` & `omicverse-1.5.9/omicverse/CEFCON/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/Rscripts/chromVAR.R` & `omicverse-1.5.9/omicverse/SEACells/Rscripts/chromVAR.R`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/accessibility.py` & `omicverse-1.5.9/omicverse/SEACells/accessibility.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/build_graph.py` & `omicverse-1.5.9/omicverse/SEACells/build_graph.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/core.py` & `omicverse-1.5.9/omicverse/SEACells/core.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/cpu.py` & `omicverse-1.5.9/omicverse/SEACells/cpu.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/cpu_dense.py` & `omicverse-1.5.9/omicverse/SEACells/cpu_dense.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/domainadapt.py` & `omicverse-1.5.9/omicverse/SEACells/domainadapt.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/evaluate.py` & `omicverse-1.5.9/omicverse/SEACells/evaluate.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/genescores.py` & `omicverse-1.5.9/omicverse/SEACells/genescores.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/gpu.py` & `omicverse-1.5.9/omicverse/SEACells/gpu.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/plot.py` & `omicverse-1.5.9/omicverse/SEACells/plot.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/tfactivity.py` & `omicverse-1.5.9/omicverse/SEACells/tfactivity.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/SEACells/utils.py` & `omicverse-1.5.9/omicverse/SEACells/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAGATE_pyG/STAGATE.py` & `omicverse-1.5.9/omicverse/STAGATE_pyG/STAGATE.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAGATE_pyG/Train_STAGATE.py` & `omicverse-1.5.9/omicverse/STAGATE_pyG/Train_STAGATE.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAGATE_pyG/gat_conv.py` & `omicverse-1.5.9/omicverse/STAGATE_pyG/gat_conv.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAGATE_pyG/utils.py` & `omicverse-1.5.9/omicverse/STAGATE_pyG/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAligner/STALIGNER.py` & `omicverse-1.5.9/omicverse/STAligner/STALIGNER.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAligner/ST_utils.py` & `omicverse-1.5.9/omicverse/STAligner/ST_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAligner/gat_conv.py` & `omicverse-1.5.9/omicverse/STAligner/gat_conv.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAligner/mnn_utils.py` & `omicverse-1.5.9/omicverse/STAligner/mnn_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/STAligner/train_STAligner.py` & `omicverse-1.5.9/omicverse/STAligner/train_STAligner.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/__init__.py` & `omicverse-1.5.9/omicverse/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 try:
     from importlib.metadata import version
 except ModuleNotFoundError:
     from pkg_resources import get_distribution
     version = lambda name: get_distribution(name).version
 
-from . import bulk,single,mofapy2,utils,bulk2single,pp,space,pl
+from . import bulk,single,mofapy2,utils,bulk2single,pp,space,pl,spatrio
 #usually
 from .utils._data import read
 from .utils._plot import palette,ov_plot_set,plot_set
 
 name = "omicverse"
 __version__ = version(name)
 omics="""
@@ -21,8 +21,8 @@
  / / / / __ `__ \/ / ___/ | / / _ \/ ___/ ___/ _ \ 
 / /_/ / / / / / / / /__ | |/ /  __/ /  (__  )  __/ 
 \____/_/ /_/ /_/_/\___/ |___/\___/_/  /____/\___/                                              
 """
 print(omics)
 print(f'Version: {__version__}, Tutorials: https://omicverse.readthedocs.io/')
 
-
+from ._settings import settings
```

### Comparing `omicverse-1.5.8/omicverse/bulk/.DS_Store` & `omicverse-1.5.9/omicverse/bulk/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_Deseq2.py` & `omicverse-1.5.9/omicverse/bulk/_Deseq2.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_Enrichment.py` & `omicverse-1.5.9/omicverse/bulk/_Enrichment.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_Gene_module.py` & `omicverse-1.5.9/omicverse/bulk/_Gene_module.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/__init__.py` & `omicverse-1.5.9/omicverse/bulk/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_chm13.py` & `omicverse-1.5.9/omicverse/bulk/_chm13.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_df_apply.py` & `omicverse-1.5.9/omicverse/bulk/_df_apply.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_dynamicTree.py` & `omicverse-1.5.9/omicverse/bulk/_dynamicTree.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_network.py` & `omicverse-1.5.9/omicverse/bulk/_network.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk/_tcga.py` & `omicverse-1.5.9/omicverse/bulk/_tcga.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_bulk2single.py` & `omicverse-1.5.9/omicverse/bulk2single/_bulk2single.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_bulkdeconvolve.py` & `omicverse-1.5.9/omicverse/bulk2single/_bulkdeconvolve.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_bulktrajblend.py` & `omicverse-1.5.9/omicverse/bulk2single/_bulktrajblend.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_map_utils.py` & `omicverse-1.5.9/omicverse/bulk2single/_map_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_map_utils1.py` & `omicverse-1.5.9/omicverse/bulk2single/_map_utils1.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_single2spatial.py` & `omicverse-1.5.9/omicverse/bulk2single/_single2spatial.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_utils.py` & `omicverse-1.5.9/omicverse/bulk2single/_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/bulk2single/_vae.py` & `omicverse-1.5.9/omicverse/bulk2single/_vae.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/cylib/fast_utils.py` & `omicverse-1.5.9/omicverse/cylib/fast_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/README.md` & `omicverse-1.5.9/omicverse/data_files/README.md`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/apoptosis_human.gmt` & `omicverse-1.5.9/omicverse/data_files/apoptosis_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/apoptosis_mouse.gmt` & `omicverse-1.5.9/omicverse/data_files/apoptosis_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt` & `omicverse-1.5.9/omicverse/data_files/c2.cp.v7.5.1.symbols.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/cell_cycle_human.gmt` & `omicverse-1.5.9/omicverse/data_files/cell_cycle_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/cell_cycle_mouse.gmt` & `omicverse-1.5.9/omicverse/data_files/cell_cycle_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/h.all.v7.5.1.symbols.gmt` & `omicverse-1.5.9/omicverse/data_files/h.all.v7.5.1.symbols.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/human_lung.gmt` & `omicverse-1.5.9/omicverse/data_files/human_lung.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/human_t_cell_markers.gmt` & `omicverse-1.5.9/omicverse/data_files/human_t_cell_markers.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/mitochondrial_genes_human.gmt` & `omicverse-1.5.9/omicverse/data_files/mitochondrial_genes_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/mitochondrial_genes_mouse.gmt` & `omicverse-1.5.9/omicverse/data_files/mitochondrial_genes_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/mouse_brain.gmt` & `omicverse-1.5.9/omicverse/data_files/mouse_brain.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/mouse_liver.gmt` & `omicverse-1.5.9/omicverse/data_files/mouse_liver.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/mouse_lung.gmt` & `omicverse-1.5.9/omicverse/data_files/mouse_lung.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/ribosomal_genes_human.gmt` & `omicverse-1.5.9/omicverse/data_files/ribosomal_genes_human.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/data_files/ribosomal_genes_mouse.gmt` & `omicverse-1.5.9/omicverse/data_files/ribosomal_genes_mouse.gmt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/build_model/build_model.py` & `omicverse-1.5.9/omicverse/mofapy2/build_model/build_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/build_model/init_model.py` & `omicverse-1.5.9/omicverse/mofapy2/build_model/init_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/build_model/save_model.py` & `omicverse-1.5.9/omicverse/mofapy2/build_model/save_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/build_model/train_model.py` & `omicverse-1.5.9/omicverse/mofapy2/build_model/train_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/build_model/utils.py` & `omicverse-1.5.9/omicverse/mofapy2/build_model/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/BayesNet.py` & `omicverse-1.5.9/omicverse/mofapy2/core/BayesNet.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/basic_distributions.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/basic_distributions.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/bernoulli.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/bernoulli.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/bernoulli_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/beta.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/beta.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/binomial.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/binomial.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/gamma.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/gamma.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/multi_task_GP.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/multi_task_GP.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/multivariate_gaussian.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/multivariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/poisson.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/poisson.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/distributions/univariate_gaussian.py` & `omicverse-1.5.9/omicverse/mofapy2/core/distributions/univariate_gaussian.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/gp_utils.py` & `omicverse-1.5.9/omicverse/mofapy2/core/gp_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/gpu_utils.py` & `omicverse-1.5.9/omicverse/mofapy2/core/gpu_utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Alpha_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Alpha_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Kc_node.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Kc_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Kg_node.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Kg_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Sigma_node.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Sigma_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Tau_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Tau_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Theta_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Theta_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/U_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/U_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/W_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/W_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Y_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Y_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes_GP.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes_GP.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/Z_nodes_GP_mv.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/ZgU_node.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/ZgU_node.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/__init__.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/basic_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/basic_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/multiview_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/multiview_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/nongaussian_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/nongaussian_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/nodes/variational_nodes.py` & `omicverse-1.5.9/omicverse/mofapy2/core/nodes/variational_nodes.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/core/utils.py` & `omicverse-1.5.9/omicverse/mofapy2/core/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/entry_point.py` & `omicverse-1.5.9/omicverse/mofapy2/run/entry_point.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_0.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_0.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_1.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_1.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/view_2.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/view_2.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_0.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_0.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_1.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_1.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/run/test_data/with_nas/500_2.txt` & `omicverse-1.5.9/omicverse/mofapy2/run/test_data/with_nas/500_2.txt`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/mofapy2/simulate/simulate_mofa.py` & `omicverse-1.5.9/omicverse/mofapy2/simulate/simulate_mofa.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/generate-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/sampler-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/train-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/data.py` & `omicverse-1.5.9/omicverse/nocd/data.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/generate.py` & `omicverse-1.5.9/omicverse/nocd/generate.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/metrics/.ipynb_checkpoints/supervised-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/metrics/.ipynb_checkpoints/unsupervised-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/metrics/supervised.py` & `omicverse-1.5.9/omicverse/nocd/metrics/supervised.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/metrics/unsupervised.py` & `omicverse-1.5.9/omicverse/nocd/metrics/unsupervised.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/decoder-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/gcn-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py` & `omicverse-1.5.9/omicverse/nocd/nn/.ipynb_checkpoints/imrpoved_gcn-checkpoint.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/decoder.py` & `omicverse-1.5.9/omicverse/nocd/nn/decoder.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/gcn.py` & `omicverse-1.5.9/omicverse/nocd/nn/gcn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/nn/imrpoved_gcn.py` & `omicverse-1.5.9/omicverse/nocd/nn/imrpoved_gcn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/sampler.py` & `omicverse-1.5.9/omicverse/nocd/sampler.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/train.py` & `omicverse-1.5.9/omicverse/nocd/train.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/nocd/utils.py` & `omicverse-1.5.9/omicverse/nocd/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/core.py` & `omicverse-1.5.9/omicverse/palantir/core.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/io.py` & `omicverse-1.5.9/omicverse/palantir/io.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/plot.py` & `omicverse-1.5.9/omicverse/palantir/plot.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/preprocess.py` & `omicverse-1.5.9/omicverse/palantir/preprocess.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/presults.py` & `omicverse-1.5.9/omicverse/palantir/presults.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/utils.py` & `omicverse-1.5.9/omicverse/palantir/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/palantir/validation.py` & `omicverse-1.5.9/omicverse/palantir/validation.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pl/_bulk.py` & `omicverse-1.5.9/omicverse/pl/_bulk.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pl/_heatmap.py` & `omicverse-1.5.9/omicverse/pl/_heatmap.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pl/_multi.py` & `omicverse-1.5.9/omicverse/pl/_multi.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pl/_palette.py` & `omicverse-1.5.9/omicverse/pl/_palette.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pl/_single.py` & `omicverse-1.5.9/omicverse/pl/_single.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/pp/__init__.py` & `omicverse-1.5.9/omicverse/pp/__init__.py`

 * *Files 25% similar despite different names*

```diff
@@ -6,10 +6,11 @@
                           preprocess,
                           normalize_pearson_residuals,
                           highly_variable_genes,
                           scale,
                           regress,
                           regress_and_scale,
                           neighbors,
-                          pca,score_genes_cell_cycle)
+                          pca,score_genes_cell_cycle,
+                          leiden,umap,louvain,anndata_to_GPU,anndata_to_CPU,)
 
 from ._qc import quantity_control,qc,filter_cells,filter_genes
```

### Comparing `omicverse-1.5.8/omicverse/pp/_preprocess.py` & `omicverse-1.5.9/omicverse/pp/_preprocess.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,17 +6,19 @@
 
 import anndata
 import numpy as np
 import pandas as pd
 from typing import Union, Tuple, Optional, Sequence, List, Dict
 import skmisc.loess as sl
 import scanpy as sc
+import time 
 
 from scipy.sparse import issparse, csr_matrix
 from ..utils import load_signatures_from_file,predefined_signatures
+from .._settings import settings
 
 def identify_robust_genes(data: anndata.AnnData, percent_cells: float = 0.05) -> None:
     """ 
     Identify robust genes as candidates for HVG selection and remove genes that are not expressed in any cells.
 
     Arguments:
         data: Use current selected modality in data, which should contain one RNA expression matrix.
@@ -333,14 +335,25 @@
         f'{np.sum(max_corr > corr_threshold)} cell cycle correlated genes will be removed...'
     )
     # Update 
     adata.var['highly_variable_features'] = adata.var_names.isin(HVGs_no_cc)
 
 from sklearn.cluster import KMeans  
 
+def anndata_to_GPU(adata,**kwargs):
+    import rapids_singlecell as rsc
+    rsc.get.anndata_to_GPU(adata,**kwargs)
+    print('Data has been moved to GPU')
+    print('Don`t forget to move it back to CPU after analysis is done')
+    print('Use `ov.pp.anndata_to_CPU(adata)`')
+
+def anndata_to_CPU(adata,layer=None, convert_all=True, copy=False):
+    import rapids_singlecell as rsc
+    rsc.get.anndata_to_CPU(adata,layers=layer, convert_all=convert_all, copy=copy)
+
 
 def preprocess(adata, mode='shiftlog|pearson', target_sum=50*1e4, n_HVGs=2000,
     organism='human', no_cc=False,batch_key=None,):
     """
     Preprocesses the AnnData object adata using either a scanpy or a pearson residuals workflow for size normalization
     and highly variable genes (HVGs) selection, and calculates signature scores if necessary. 
 
@@ -364,47 +377,78 @@
     print('Begin robust gene identification')
     identify_robust_genes(adata, percent_cells=0.05)
     adata = adata[:, adata.var['robust']]
     print(f'End of robust gene identification.')
     method_list = mode.split('|')
     print(f'Begin size normalization: {method_list[0]} and HVGs selection {method_list[1]}')
     
+    if settings.mode == 'cpu':
+        data_load_start = time.time()
+        if method_list[0] == 'shiftlog': # Size normalization + scanpy batch aware HVGs selection
+            sc.pp.normalize_total(
+                adata, 
+                target_sum=target_sum,
+                exclude_highly_expressed=True,
+                max_fraction=0.2,
+            )
+            sc.pp.log1p(adata)
+        elif method_list[0] == 'pearson':
+            # Perason residuals workflow
+            sc.experimental.pp.normalize_pearson_residuals(adata)
+
+        if method_list[1] == 'pearson': # Size normalization + scanpy batch aware HVGs selection
+            sc.experimental.pp.highly_variable_genes(
+                adata, 
+                flavor="pearson_residuals",
+                layer='counts',
+                n_top_genes=n_HVGs,
+                batch_key=batch_key,
+            )
+            if no_cc:
+                remove_cc_genes(adata, organism=organism, corr_threshold=0.1)
+        elif method_list[1] == 'seurat':
+            sc.pp.highly_variable_genes(
+                adata,
+                flavor="seurat_v3",
+                layer='counts',
+                n_top_genes=n_HVGs,
+                batch_key=batch_key,
+            )
+            if no_cc:
+                remove_cc_genes(adata, organism=organism, corr_threshold=0.1)
+        data_load_end = time.time()
+        print(f'Time to analyze data in cpu: {data_load_end - data_load_start} seconds.')
+    else:
+        import rapids_singlecell as rsc
+        data_load_start = time.time()
+        if method_list[0] == 'shiftlog': # Size normalization + scanpy batch aware HVGs selection
+            rsc.pp.normalize_total(adata, target_sum=target_sum)
+            rsc.pp.log1p(adata)
+        elif method_list[0] == 'pearson':
+            # Perason residuals workflow
+            rsc.pp.normalize_pearson_residuals(adata)
+        if method_list[1] == 'pearson': # Size normalization + scanpy batch aware HVGs selection
+            rsc.pp.highly_variable_genes(
+                adata, 
+                flavor="pearson_residuals",
+                layer='counts',
+                n_top_genes=n_HVGs,
+                batch_key=batch_key,
+            )
+        elif method_list[1] == 'seurat':
+            rsc.pp.highly_variable_genes(
+                adata,
+                flavor="seurat_v3",
+                layer='counts',
+                n_top_genes=n_HVGs,
+                batch_key=batch_key,
+            )
+        data_load_end = time.time()
+        print(f'Time to analyze data in gpu: {data_load_end - data_load_start} seconds.')
 
-    if method_list[0] == 'shiftlog': # Size normalization + scanpy batch aware HVGs selection
-        sc.pp.normalize_total(
-            adata, 
-            target_sum=target_sum,
-            exclude_highly_expressed=True,
-            max_fraction=0.2,
-        )
-        sc.pp.log1p(adata)
-    elif method_list[0] == 'pearson':
-        # Perason residuals workflow
-        sc.experimental.pp.normalize_pearson_residuals(adata)
-
-    if method_list[1] == 'pearson': # Size normalization + scanpy batch aware HVGs selection
-        sc.experimental.pp.highly_variable_genes(
-            adata, 
-            flavor="pearson_residuals",
-            layer='counts',
-            n_top_genes=n_HVGs,
-            batch_key=batch_key,
-        )
-        if no_cc:
-            remove_cc_genes(adata, organism=organism, corr_threshold=0.1)
-    elif method_list[1] == 'seurat':
-        sc.pp.highly_variable_genes(
-            adata,
-            flavor="seurat_v3",
-            layer='counts',
-            n_top_genes=n_HVGs,
-            batch_key=batch_key,
-        )
-        if no_cc:
-            remove_cc_genes(adata, organism=organism, corr_threshold=0.1)
 
     adata.var = adata.var.drop(columns=['highly_variable_features'])
     adata.var['highly_variable_features'] = adata.var['highly_variable']
     adata.var = adata.var.drop(columns=['highly_variable'])
     adata.var = adata.var.rename(columns={'means':'mean', 'variances':'var'})
     print(f'End of size normalization: {method_list[0]} and HVGs selection {method_list[1]}')
    
@@ -426,34 +470,42 @@
         adata : Annotated data matrix with n_obs x n_vars shape.
 
     Returns:
         adata : Annotated data matrix with n_obs x n_vars shape. Adds a new layer called 'scaled' that stores
             the expression matrix that has been scaled to unit variance and zero mean.
 
     """
-    adata_mock = sc.pp.scale(adata, copy=True,max_value=max_value)
-    adata.layers[layers_add] = adata_mock.X.copy()
-    del adata_mock
+    if settings.mode == 'cpu':
+        adata_mock = sc.pp.scale(adata, copy=True,max_value=max_value)
+        adata.layers[layers_add] = adata_mock.X.copy()
+        del adata_mock
+    else:
+        import rapids_singlecell as rsc
+        adata.layers['scaled']=rsc.pp.scale(adata, max_value=max_value,inplace=False)
 
 def regress(adata):
     """
     Regress out covariates from the input AnnData object.
 
     Arguments:
         adata : Annotated data matrix with n_obs x n_vars shape. Should contain columns 'mito_perc' and 'nUMIs'
             that represent the percentage of mitochondrial genes and the total number of UMI counts, respectively.
 
     Returns:
         adata : Annotated data matrix with n_obs x n_vars shape. Adds a new layer called 'regressed' that stores
             the expression matrix with covariates regressed out.
 
     """
-    adata_mock = sc.pp.regress_out(adata, ['mito_perc', 'nUMIs'], n_jobs=8, copy=True)
-    adata.layers['regressed'] = adata_mock.X
-    return adata
+    if settings.mode == 'cpu':
+        adata_mock = sc.pp.regress_out(adata, ['mito_perc', 'nUMIs'], n_jobs=8, copy=True)
+        adata.layers['regressed'] = adata_mock.X.copy()
+        del adata_mock
+    else:
+        import rapids_singlecell as rsc
+        adata.layers['regressed']=rsc.pp.regress_out(adata, ['mito_perc', 'nUMIs'], inplace=False)
 
 def regress_and_scale(adata):
     """
     Regress out covariates from the input AnnData object and scale the resulting expression matrix.
 
     Arguments:
         adata : Annotated data matrix with n_obs x n_vars shape. Should contain a layer called 'regressed'
@@ -514,32 +566,41 @@
         layer : The name of the layer in `adata` where the data to be analyzed is stored. Defaults to the 'scaled' layer,
             and falls back to 'lognorm' if that layer does not exist. Raises a KeyError if the specified layer is not present.
 
     Returns:
         adata : The original AnnData object with the calculated PCA embeddings and other information stored in its `obsm`, `varm`,
             and `uns` fields.
     """
+    
     if 'lognorm' not in adata.layers:
         adata.layers['lognorm'] = adata.X
     if layer in adata.layers: 
         X = adata.layers[layer]
         key = f'{layer}|original'
     else:
         raise KeyError(f'Selected layer {layer} is not present. Compute it first!')
-
-    model = my_PCA()
-    model.calculate_PCA(X, n_components=n_pcs)
-    adata.obsm[key + '|X_pca'] = model.embs
-    adata.varm[key + '|pca_loadings'] = model.loads
-    adata.uns[key + '|pca_var_ratios'] = model.var_ratios
-    adata.uns[key + '|cum_sum_eigenvalues'] = np.cumsum(model.var_ratios)
-    if inplace:
-        return None
+    
+    if settings.mode == 'cpu':
+        model = my_PCA()
+        model.calculate_PCA(X, n_components=n_pcs)
+        adata.obsm[key + '|X_pca'] = model.embs
+        adata.varm[key + '|pca_loadings'] = model.loads
+        adata.uns[key + '|pca_var_ratios'] = model.var_ratios
+        adata.uns[key + '|cum_sum_eigenvalues'] = np.cumsum(model.var_ratios)
+        if inplace:
+            return None
+        else:
+            return adata  
     else:
-        return adata  
+        import rapids_singlecell as rsc
+        rsc.pp.pca(adata, layer=layer,n_comps=n_pcs)
+        adata.obsm[key + '|X_pca'] = adata.obsm['X_pca']
+        adata.varm[key + '|pca_loadings'] = adata.varm['PCs']
+        adata.uns[key + '|pca_var_ratios'] = adata.uns['pca']['variance_ratio']
+        adata.uns[key + '|cum_sum_eigenvalues'] = adata.uns['pca']['variance']
 
 def red(adata):
     """
     Reduce the input AnnData object to highly variable features and store the resulting expression matrices.
 
     Arguments:
         adata : Annotated data matrix with n_obs x n_vars shape. Should contain a variable 'highly_variable_features'
@@ -680,19 +741,47 @@
     Notes
     -----
     If `method='umap'`, it's highly recommended to install pynndescent ``pip install pynndescent``.
     Installing `pynndescent` can significantly increase performance,
     and in later versions it will become a hard dependency.
     
     """
-    return sc.pp.neighbors(adata,n_neighbors,
-                           n_pcs,use_rep,knn,random_state,
-                           method,metric,metric_kwds,key_added) if copy else None
+    if settings.mode =='cpu':
+        sc.pp.neighbors(adata,use_rep=use_rep,n_neighbors=n_neighbors, n_pcs=n_pcs,
+                         random_state=random_state,method=method,metric=metric,metric_kwds=metric_kwds,
+                         key_added=key_added,copy=copy)
+    else:
+        import rapids_singlecell as rsc
+        rsc.pp.neighbors(adata,use_rep=use_rep,n_neighbors=n_neighbors, n_pcs=n_pcs,
+                         random_state=random_state,algorithm=method,metric=metric,metric_kwds=metric_kwds,
+                         key_added=key_added,copy=copy)
+
+
+def umap(adata, **kwargs):
+    if settings.mode =='cpu':
+        sc.tl.umap(adata, **kwargs)
+    else:
+        import rapids_singlecell as rsc
+
+        rsc.tl.umap(adata, **kwargs)
 
 
+def louvain(adata, **kwargs):
+    if settings.mode =='cpu':
+        sc.tl.louvain(adata, **kwargs)
+    else:
+        import rapids_singlecell as rsc
+        rsc.tl.louvain(adata, **kwargs)
+
+def leiden(adata, **kwargs):
+    if settings.mode =='cpu':
+        sc.tl.leiden(adata, **kwargs)
+    else:
+        import rapids_singlecell as rsc
+        rsc.tl.leiden(adata, **kwargs)
 
 
 def score_genes_cell_cycle(adata,s_genes=None, g2m_genes=None):
     if s_genes==None:
         s_genes=['MCM5', 'PCNA', 'TYMS', 'FEN1', 'MCM2', 'MCM4', 'RRM1', 'UNG', 'GINS2', 'MCM6', 'CDCA7', 'DTL', 'PRIM1', 'UHRF1', 'MLF1IP', 'HELLS', 'RFC2', 'RPA2', 'NASP', 'RAD51AP1', 'GMNN', 'WDR76', 'SLBP', 'CCNE2', 'UBR7', 'POLD3', 'MSH2', 'ATAD2', 'RAD51', 'RRM2', 'CDC45', 'CDC6', 'EXO1', 'TIPIN', 'DSCC1', 'BLM', 'CASP8AP2', 'USP1', 'CLSPN', 'POLA1', 'CHAF1B', 'BRIP1', 'E2F8']
     if g2m_genes==None:
         g2m_genes=['HMGB2', 'CDK1', 'NUSAP1', 'UBE2C', 'BIRC5', 'TPX2', 'TOP2A', 'NDC80', 'CKS2', 'NUF2', 'CKS1B', 'MKI67', 'TMPO', 'CENPF', 'TACC3', 'FAM64A', 'SMC4', 'CCNB2', 'CKAP2L', 'CKAP2', 'AURKB', 'BUB1', 'KIF11', 'ANP32E', 'TUBB4B', 'GTSE1', 'KIF20B', 'HJURP', 'CDCA3', 'HN1', 'CDC20', 'TTK', 'CDC25C', 'KIF2C', 'RANGAP1', 'NCAPD2', 'DLGAP5', 'CDCA2', 'CDCA8', 'ECT2', 'KIF23', 'HMMR', 'AURKA', 'PSRC1', 'ANLN', 'LBR', 'CKAP5', 'CENPE', 'CTCF', 'NEK2', 'G2E3', 'GAS2L3', 'CBX5', 'CENPA']
```

### Comparing `omicverse-1.5.8/omicverse/pp/_qc.py` & `omicverse-1.5.9/omicverse/pp/_qc.py`

 * *Files 16% similar despite different names*

```diff
@@ -15,14 +15,16 @@
 import matplotlib.pyplot as plt 
 from matplotlib.backends.backend_pdf import PdfPages 
 from matplotlib import rcParams
 import seaborn as sns
 from typing import Union, Optional, Sequence, Tuple, List, Dict
 from scipy.sparse import issparse
 
+from .._settings import settings
+
 
 def mads(meta, cov, nmads=5, lt=None): 
     """
     Given a certain array, it calculate its Median Absolute Deviation (MAD).
     """
     x = meta[cov]
     mad = np.median(np.absolute(x - np.median(x)))
@@ -169,15 +171,23 @@
     # Last gene and cell filter
     sc.pp.filter_cells(adata, min_genes=min_genes)
     sc.pp.filter_genes(adata, min_cells=min_cells)
 
     return adata, removed_cells
 
 
-def qc(adata:anndata.AnnData, mode='seurat', 
+def qc(adata,**kwargs):
+    if settings.mode == 'gpu':
+        print('GPU mode activated')
+        return qc_gpu(adata,**kwargs)
+    else:
+        print('CPU mode activated')
+        return qc_cpu(adata,**kwargs)
+
+def qc_cpu(adata:anndata.AnnData, mode='seurat', 
        min_cells=3, min_genes=200, nmads=5, 
        max_cells_ratio=1,max_genes_ratio=1,
        batch_key=None,doublets=True,
        path_viz=None, tresh=None,mt_startswith='MT-',mt_genes=None):
     """
     Perform quality control on a dictionary of AnnData objects.
     
@@ -224,15 +234,15 @@
     
     if issparse(adata.X):
         adata.obs['nUMIs'] = np.array(adata.X.sum(axis=1)).reshape(-1)
         adata.obs['mito_perc'] = np.array(adata[:, adata.var["mt"]].X.sum(axis=1)).reshape(-1) / adata.obs['nUMIs'].values
         adata.obs['detected_genes'] = adata.X.getnnz(axis=1)
     else:
         adata.obs['nUMIs'] = adata.X.sum(axis=1)  
-        adata.obs['mito_perc'] = adata[:, adata.var["mt"]].X.sum(axis=1) / adata.obs['nUMIs'].values
+        adata.obs['mito_perc'] = adata[:, adata.var["mt"]==True].X.sum(axis=1) / adata.obs['nUMIs'].values
         adata.obs['detected_genes'] = np.count_nonzero(adata.X, axis=1)
     adata.obs['cell_complexity'] = adata.obs['detected_genes'] / adata.obs['nUMIs']
     print(f'End calculation of QC metrics.')
 
     # Original QC plot
     n0 = adata.shape[0]
     print(f'Original cell number: {n0}')
@@ -291,14 +301,108 @@
     sc.pp.filter_cells(adata, min_genes=min_genes)
     sc.pp.filter_genes(adata, min_cells=min_cells)
     sc.pp.filter_cells(adata, max_genes=max_genes_ratio*adata.shape[1])
     sc.pp.filter_genes(adata, max_cells=max_cells_ratio*adata.shape[0])
 
     return adata
 
+
+def qc_gpu(adata, mode='seurat', 
+       min_cells=3, min_genes=200, nmads=5, 
+       max_cells_ratio=1,max_genes_ratio=1,
+       batch_key=None,doublets=True,
+       path_viz=None, tresh=None,mt_startswith='MT-',mt_genes=None):
+    import rapids_singlecell as rsc
+     # Logging 
+    if tresh is None:
+        tresh={'mito_perc': 0.15, 'nUMIs': 500, 'detected_genes': 250}
+    
+    # For each adata, produce a figure
+    # with PdfPages(path_viz + 'original_QC_by_sample.pdf') as pdf: 
+    removed_cells = []
+    rsc.get.anndata_to_GPU(adata)
+    # QC metrics
+    print('Calculate QC metrics')
+    adata.var_names_make_unique()
+    if mt_genes is not None:
+        adata.var['mt']=False
+        adata.var.loc[list(set(adata.var_names) & set(mt_genes)),'mt']=True
+    else:
+        rsc.pp.flag_gene_family(adata, gene_family_name="mt", gene_family_prefix=mt_startswith)
+    rsc.pp.calculate_qc_metrics(adata, qc_vars=["mt"])
+    adata.obs['nUMIs'] = adata.obs['total_counts']
+    adata.obs['mito_perc'] = adata.obs['pct_counts_mt']/100
+    adata.obs['detected_genes'] = adata.obs['n_genes_by_counts']
+    adata.obs['cell_complexity'] = adata.obs['detected_genes'] / adata.obs['nUMIs']
+    print(f'End calculation of QC metrics.')
+
+    # Original QC plot
+    n0 = adata.shape[0]
+    print(f'Original cell number: {n0}')
+
+    if doublets==True:
+        # Post doublets removal QC plot
+        print('Begin of post doublets removal and QC plot')
+        rsc.pp.scrublet(adata, random_state=1234,batch_key=batch_key)
+        adata_remove = adata[adata.obs['predicted_doublet'], :]
+        removed_cells.extend(list(adata_remove.obs_names))
+        adata = adata[~adata.obs['predicted_doublet'], :]
+        n1 = adata.shape[0]
+        print(f'Cells retained after scrublet: {n1}, {n0-n1} removed.')
+        print(f'End of post doublets removal and QC plots.')
+
+    # Filters
+    print('Filters application (seurat or mads)')
+    if mode == 'seurat':
+        adata.obs['passing_mt'] = adata.obs['mito_perc'] < tresh['mito_perc']
+        adata.obs['passing_nUMIs'] = adata.obs['nUMIs'] > tresh['nUMIs']
+        adata.obs['passing_ngenes'] = adata.obs['detected_genes'] > tresh['detected_genes']
+    elif mode == 'mads':
+        adata.obs['passing_mt'] = adata.obs['mito_perc'] < tresh['mito_perc']
+        adata.obs['passing_nUMIs'] = mads_test(adata.obs, 'nUMIs', nmads=nmads, lt=tresh)
+        adata.obs['passing_ngenes'] = mads_test(adata.obs, 'detected_genes', nmads=nmads, lt=tresh) 
+
+    
+
+    # Report 
+    if mode == 'seurat':
+        print(f'Lower treshold, nUMIs: {tresh["nUMIs"]}; filtered-out-cells: {n1-np.sum(adata.obs["passing_nUMIs"])}')
+        print(f'Lower treshold, n genes: {tresh["detected_genes"]}; filtered-out-cells: {n1-np.sum(adata.obs["passing_ngenes"])}')
+        print(f'Lower treshold, mito %: {tresh["mito_perc"]}; filtered-out-cells: {n1-np.sum(adata.obs["passing_mt"])}')
+    elif mode == 'mads':
+        nUMIs_t = mads(adata.obs, 'nUMIs', nmads=nmads, lt=tresh)
+        n_genes_t = mads(adata.obs, 'detected_genes', nmads=nmads, lt=tresh)
+        print(f'Tresholds used, nUMIs: ({nUMIs_t[0]}, {nUMIs_t[1]}); filtered-out-cells: {n1-np.sum(adata.obs["passing_nUMIs"])}')
+        print(f'Tresholds used, n genes: ({n_genes_t[0]}, {n_genes_t[1]}); filtered-out-cells: {n1-np.sum(adata.obs["passing_ngenes"])}')
+        print(f'Lower treshold, mito %: {tresh["mito_perc"]}; filtered-out-cells: {n1-np.sum(adata.obs["passing_mt"])}')
+    print(f'Filters applicated.')
+
+    # QC plot
+    QC_test = (adata.obs['passing_mt']) & (adata.obs['passing_nUMIs']) & (adata.obs['passing_ngenes'])
+    removed = QC_test.loc[lambda x : x == False]
+    removed_cells.extend(list(removed.index.values))
+    print(f'Total cell filtered out with this last --mode {mode} QC (and its chosen options): {n1-np.sum(QC_test)}')
+    adata = adata[QC_test, :]
+    n2 = adata.shape[0]
+        
+
+
+    # Store cleaned adata
+    print(f'Cells retained after scrublet and {mode} filtering: {n2}, {n0-n2} removed.')
+
+    # Last gene and cell filter
+    rsc.pp.filter_cells(adata,qc_var='detected_genes', min_count=min_genes, max_count=max_genes_ratio*adata.shape[1])
+    rsc.pp.filter_genes(adata, min_count=min_cells, max_count=max_cells_ratio*adata.shape[0])
+
+
+    return adata
+
+
+
+
 def filter_cells(adata: anndata.AnnData,
     min_counts: Optional[int] = None,
     min_genes: Optional[int] = None,
     max_counts: Optional[int] = None,
     max_genes: Optional[int] = None,
     inplace: bool = True,):
     """
```

### Comparing `omicverse-1.5.8/omicverse/single/.DS_Store` & `omicverse-1.5.9/omicverse/single/.DS_Store`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/README.md` & `omicverse-1.5.9/omicverse/single/README.md`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_SCSA.py` & `omicverse-1.5.9/omicverse/single/_SCSA.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/__init__.py` & `omicverse-1.5.9/omicverse/single/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,8 +16,9 @@
 from ._batch import batch_correction
 from ._cellfategenie import cellfategenie,gene_trends
 from ._ltnn import scLTNN,plot_origin_tesmination,find_related_gene
 from ._traj import TrajInfer
 from ._cefcon import pyCEFCON,convert_human_to_mouse_network,load_human_prior_interaction_network,mouse_hsc_nestorowa16
 from ._aucell import aucell
 from ._metacell import MetaCell,plot_metacells,get_obs_value
-from ._mdic3 import pyMDIC3
+from ._mdic3 import pyMDIC3
+from ._cnmf import *
```

### Comparing `omicverse-1.5.8/omicverse/single/_anno.py` & `omicverse-1.5.9/omicverse/single/_anno.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_atac.py` & `omicverse-1.5.9/omicverse/single/_atac.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_aucell.py` & `omicverse-1.5.9/omicverse/single/_aucell.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_batch.py` & `omicverse-1.5.9/omicverse/single/_batch.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_cefcon.py` & `omicverse-1.5.9/omicverse/single/_cefcon.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_cellfategenie.py` & `omicverse-1.5.9/omicverse/single/_cellfategenie.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_cosg.py` & `omicverse-1.5.9/omicverse/single/_cosg.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_cpdb.py` & `omicverse-1.5.9/omicverse/single/_cpdb.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_ltnn.py` & `omicverse-1.5.9/omicverse/single/_ltnn.py`

 * *Files 0% similar despite different names*

```diff
@@ -578,14 +578,15 @@
         
 class RadioModel(nn.Module):
     def __init__(self, input_dim):
         super(RadioModel, self).__init__()
         self.fc1 = nn.Linear(input_dim, 512)
         self.fc2 = nn.Linear(512, 512)
         self.fc3 = nn.Linear(512, 512)
+        #self.fc3 = nn.Linear(512, 50)
         self.fc4 = nn.Linear(512, 1)
     
     def forward(self, x):
 
         x=self.fc1(x)
         x=F.relu(x)
         x=self.fc2(x)
```

### Comparing `omicverse-1.5.8/omicverse/single/_mdic3.py` & `omicverse-1.5.9/omicverse/single/_mdic3.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_metacell.py` & `omicverse-1.5.9/omicverse/single/_metacell.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_mofa.py` & `omicverse-1.5.9/omicverse/single/_mofa.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_nocd.py` & `omicverse-1.5.9/omicverse/single/_nocd.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_scannorl.py` & `omicverse-1.5.9/omicverse/single/_scannorl.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_scdrug.py` & `omicverse-1.5.9/omicverse/single/_scdrug.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_scgsea.py` & `omicverse-1.5.9/omicverse/single/_scgsea.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_simba.py` & `omicverse-1.5.9/omicverse/single/_simba.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_tosica.py` & `omicverse-1.5.9/omicverse/single/_tosica.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/single/_traj.py` & `omicverse-1.5.9/omicverse/single/_traj.py`

 * *Files 10% similar despite different names*

```diff
@@ -76,14 +76,28 @@
             sc.tl.diffmap(self.adata)
             sc.pp.neighbors(self.adata, n_neighbors=self.n_neighbors, use_rep='X_diffmap')
             sc.tl.draw_graph(self.adata)
             self.adata.uns['iroot'] = np.flatnonzero(self.adata.obs[self.groupby]  == self.origin)[0]
             sc.tl.dpt(self.adata)
             sc.pp.neighbors(self.adata, n_neighbors=self.n_neighbors, n_pcs=self.n_comps,
                use_rep=self.use_rep)
+        elif method=='slingshot':
+            #sc.pp.neighbors(self.adata, n_neighbors=self.n_neighbors, n_pcs=self.n_comps,
+            #   use_rep=self.use_rep)
+            #sc.tl.umap(self.adata)
+            from ._pyslingshot import Slingshot
+            slingshot = Slingshot(self.adata, 
+                      celltype_key=self.groupby, 
+                      obsm_key=self.basis, 
+                      start_node=self.origin,
+                      end_nodes=self.terminal,
+                      debug_level='verbose')
+            slingshot.fit(**kwargs)
+            pseudotime = slingshot.unified_pseudotime
+            self.adata.obs['slingshot_pseudotime']=pseudotime
         else:
             print('Please input the correct method name, such as `palantir` or `diffusion_map`')
             return
         
     def palantir_plot_pseudotime(self,**kwargs):
 
         plot_palantir_results(self.adata,**kwargs)
```

### Comparing `omicverse-1.5.8/omicverse/single/_via.py` & `omicverse-1.5.9/omicverse/single/_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/space/_cluster.py` & `omicverse-1.5.9/omicverse/space/_cluster.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/space/_integrate.py` & `omicverse-1.5.9/omicverse/space/_integrate.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/space/_spaceflow.py` & `omicverse-1.5.9/omicverse/space/_spaceflow.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/space/_tangram.py` & `omicverse-1.5.9/omicverse/space/_tangram.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/spaceflow/_SpaceFlow.py` & `omicverse-1.5.9/omicverse/spaceflow/_SpaceFlow.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tape/deconvolution.py` & `omicverse-1.5.9/omicverse/tape/deconvolution.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tape/model.py` & `omicverse-1.5.9/omicverse/tape/model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tape/simulation.py` & `omicverse-1.5.9/omicverse/tape/simulation.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tape/train.py` & `omicverse-1.5.9/omicverse/tape/train.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tape/utils.py` & `omicverse-1.5.9/omicverse/tape/utils.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tosica/TOSICA_model.py` & `omicverse-1.5.9/omicverse/tosica/TOSICA_model.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tosica/customized_linear.py` & `omicverse-1.5.9/omicverse/tosica/customized_linear.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tosica/pre.py` & `omicverse-1.5.9/omicverse/tosica/pre.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/tosica/train.py` & `omicverse-1.5.9/omicverse/tosica/train.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/__init__.py` & `omicverse-1.5.9/omicverse/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_cluster.py` & `omicverse-1.5.9/omicverse/utils/_cluster.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_data.py` & `omicverse-1.5.9/omicverse/utils/_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -590,7 +590,17 @@
 class easter_egg(object):
 
     def __init__(self,):
         print('Easter egg is ready to be hatched!')
 
     def O(self):
         print('尊嘟假嘟')
+
+def save(file,path):
+    import pickle
+    with open(path, 'wb') as f:
+        pickle.dump(file, f)
+
+def load(path):
+    import pickle
+    with open(path, 'rb') as f:
+        return pickle.load(f)
```

### Comparing `omicverse-1.5.8/omicverse/utils/_enum.py` & `omicverse-1.5.9/omicverse/utils/_enum.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_genomics.py` & `omicverse-1.5.9/omicverse/utils/_genomics.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_heatmap.py` & `omicverse-1.5.9/omicverse/utils/_heatmap.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_knn.py` & `omicverse-1.5.9/omicverse/utils/_knn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_mde.py` & `omicverse-1.5.9/omicverse/utils/_mde.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_paga.py` & `omicverse-1.5.9/omicverse/utils/_paga.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_plot.py` & `omicverse-1.5.9/omicverse/utils/_plot.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_roe.py` & `omicverse-1.5.9/omicverse/utils/_roe.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_scatterplot.py` & `omicverse-1.5.9/omicverse/utils/_scatterplot.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_syn.py` & `omicverse-1.5.9/omicverse/utils/_syn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/utils/_venn.py` & `omicverse-1.5.9/omicverse/utils/_venn.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/core.py` & `omicverse-1.5.9/omicverse/via/core.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/datasets_via.py` & `omicverse-1.5.9/omicverse/via/datasets_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/examples.py` & `omicverse-1.5.9/omicverse/via/examples.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/plotting_via.py` & `omicverse-1.5.9/omicverse/via/plotting_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/utils_via.py` & `omicverse-1.5.9/omicverse/via/utils_via.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/omicverse/via/windmap.py` & `omicverse-1.5.9/omicverse/via/windmap.py`

 * *Files identical despite different names*

### Comparing `omicverse-1.5.8/pyproject.toml` & `omicverse-1.5.9/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools", "wheel", "flit_core >=3.4,<4","Cython"]
 build-backend = "flit_core.buildapi"
 
 
 
 [project]
 name = "omicverse"
-version = "1.5.8"
+version = "1.5.9"
 description = "OmicVerse: A single pipeline for exploring the entire transcriptome universe"
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [
     {name = "Zehua Zeng", email = "starlitnightly@163.com"},
 ]
@@ -30,15 +30,15 @@
     'hnswlib>=0.7',
     'ERgene>=1.2',
     'numpy>=1.22, <1.24',
     'scanpy>=1.9',
     'pandas>=1.0.3, <=1.5.3',
     'matplotlib<3.7',
     'scikit-learn>=1.2',
-    'scipy>=1.8',
+    'scipy>=1.8, <1.12',
     'networkx>=2.8',
     'multiprocess>=0.70',
     'seaborn>=0.11',
     'datetime>=4.5',
     'statsmodels>=0.13',
     'gseapy==0.10.8',
     'ipywidgets>=8.0',
@@ -54,15 +54,15 @@
     'gdown>=4.6',
     'igraph>=0.10',
     'leidenalg>=0.9',
     'graphtools>=1.5',
     'datashader>=0.14',
     'phate>=1.0',
     'tqdm>=4.64',
-    'pydeseq2>=0.3',
+    'pydeseq2>=0.3, <=0.4.0',
     'mofax>=0.3',
     'adjustText>=0.8',
     'scikit-misc>=0.1',
     'metatime>=1.3.0',
     'einops>=0.6',
     'tensorboard>=2.6',
     'scrublet >=0.2',
```

### Comparing `omicverse-1.5.8/PKG-INFO` & `omicverse-1.5.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: omicverse
-Version: 1.5.8
+Version: 1.5.9
 Summary: OmicVerse: A single pipeline for exploring the entire transcriptome universe
 Keywords: bioinformatics,deep-learning,scRNA-seq,RNA-seq
 Author-email: Zehua Zeng <starlitnightly@163.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
@@ -18,15 +18,15 @@
 Requires-Dist: hnswlib>=0.7
 Requires-Dist: ERgene>=1.2
 Requires-Dist: numpy>=1.22, <1.24
 Requires-Dist: scanpy>=1.9
 Requires-Dist: pandas>=1.0.3, <=1.5.3
 Requires-Dist: matplotlib<3.7
 Requires-Dist: scikit-learn>=1.2
-Requires-Dist: scipy>=1.8
+Requires-Dist: scipy>=1.8, <1.12
 Requires-Dist: networkx>=2.8
 Requires-Dist: multiprocess>=0.70
 Requires-Dist: seaborn>=0.11
 Requires-Dist: datetime>=4.5
 Requires-Dist: statsmodels>=0.13
 Requires-Dist: gseapy==0.10.8
 Requires-Dist: ipywidgets>=8.0
@@ -42,15 +42,15 @@
 Requires-Dist: gdown>=4.6
 Requires-Dist: igraph>=0.10
 Requires-Dist: leidenalg>=0.9
 Requires-Dist: graphtools>=1.5
 Requires-Dist: datashader>=0.14
 Requires-Dist: phate>=1.0
 Requires-Dist: tqdm>=4.64
-Requires-Dist: pydeseq2>=0.3
+Requires-Dist: pydeseq2>=0.3, <=0.4.0
 Requires-Dist: mofax>=0.3
 Requires-Dist: adjustText>=0.8
 Requires-Dist: scikit-misc>=0.1
 Requires-Dist: metatime>=1.3.0
 Requires-Dist: einops>=0.6
 Requires-Dist: tensorboard>=2.6
 Requires-Dist: scrublet >=0.2
@@ -61,14 +61,18 @@
 <img src="https://raw.githubusercontent.com/Starlitnightly/omicverse/master/README.assets/logo.png" width="400">
 </h1><br>
 
 [![pypi-badge](https://img.shields.io/pypi/v/omicverse)](https://pypi.org/project/omicverse) [![Documentation Status](https://readthedocs.org/projects/omicverse/badge/?version=latest)](https://omicverse.readthedocs.io/en/latest/?badge=latest) [![pypiDownloads](https://static.pepy.tech/badge/omicverse)](https://pepy.tech/project/omicverse) [![condaDownloads](https://img.shields.io/conda/dn/conda-forge/omicverse?logo=Anaconda)](https://anaconda.org/conda-forge/omicverse) [![License:GPL](https://img.shields.io/badge/license-GNU-blue)](https://img.shields.io/apm/l/vim-mode) [![scverse](https://img.shields.io/badge/scverse-ecosystem-blue.svg?labelColor=yellow)](https://scverse.org/) [![Pytest](https://github.com/Starlitnightly/omicverse/workflows/py38|py39/badge.svg)](https://github.com/Starlitnightly/omicverse/) 
 
 OmicVerse is the fundamental package for multi omics included bulk and single cell analysis with Python. For more information, please read our paper: [OmicVerse: A single pipeline for exploring the entire transcriptome universe](https://www.biorxiv.org/content/10.1101/2023.06.06.543913v2)
 
+If you like **OmicVerse** and want to support our mission, please consider making a [donation](https://afdian.net/a/starlitnightly) to support our efforts.
+
+## Introduction
+
 The original name of the omicverse was [Pyomic](https://pypi.org/project/Pyomic/), but we wanted to address a whole universe of transcriptomics, so we changed the name to OmicVerse, it aimed to solve all task in RNA-seq.
 
 BulkTrajBlend algorithm in OmicVerse that combines Beta-Variational AutoEncoder for deconvolution and graph neural networks for overlapping community discovery to effectively interpolate and restore the continuity of “interrupted” cells in the original scRNA-seq data.
 
 ![omicverse-light](omicverse_guide/docs/img/omicverse.png#gh-light-mode-only)
 ![omicverse-dark](omicverse_guide/docs/img/omicverse_dark.png#gh-dark-mode-only)
 
@@ -134,14 +138,15 @@
 - [29] [CEFCON](https://github.com/WPZgithub/CEFCON) was originally published in [*Nature Communications*](https://www.nature.com/articles/s41467-023-44103-3)
 - [30] [PyComplexHeatmap](https://github.com/DingWB/PyComplexHeatmap) was originally published in [*iMeta*](https://doi.org/10.1002/imt2.115)
 
 ## Included Package not published or preprint
 
 - [1] [Cellula](https://github.com/andrecossa5/Cellula/) is to provide a toolkit for the exploration of scRNA-seq. These tools perform common single-cell analysis tasks
 - [2] [pegasus](https://github.com/lilab-bcb/pegasus/) is a tool for analyzing transcriptomes of millions of single cells. It is a command line tool, a python package and a base for Cloud-based analysis workflows.
+- [3] [cNMF](https://github.com/dylkot/cNMF) is an analysis pipeline for inferring gene expression programs from single-cell RNA-Seq (scRNA-Seq) data.
 
 ## Contact
 
 - Zehua Zeng ([starlitnightly@163.com](mailto:starlitnightly@163.com) or [zehuazeng@xs.ustb.edu.cn](mailto:zehuazeng@xs.ustb.edu.cn))
 - Lei Hu ([hulei@westlake.edu.cn](mailto:hulei@westlake.edu.cn))
 
 ## Developer Guild
@@ -152,10 +157,12 @@
 
 We would like to thank the following WeChat Official Accounts for promoting Omicverse.
 
 <p align="left"> <a href="http://www.biotrainee.com/" target="_blank" rel="noreferrer"> <img src="README.assets/image-20230701163953794.png" alt="linux" width="50" height="50"/> </a> <a href="https://zhuanlan.zhihu.com/c_1257815636945915904?page=3" target="_blank" rel="noreferrer"> <img src="README.assets/WechatIMG688.png" alt="linux" width="50" height="50"/> </a> </p>
 
 ## Other
 
+If you would like to sponsor the development of our project, you can go to the afdian website (https://afdian.net/a/starlitnightly) and sponsor us.
+
 <div>Logo made by <a href="https://www.designevo.com/" title="Free Online Logo Maker">DesignEvo free logo creator</a></div>
```

