# Comparing `tmp/PowerGenome-0.6.1a0.tar.gz` & `tmp/powergenome-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PowerGenome-0.6.1a0.tar", last modified: Thu Jun  8 05:26:42 2023, max compression
+gzip compressed data, last modified: Sun Feb  2 00:00:00 2020, max compression
```

## Comparing `PowerGenome-0.6.1a0.tar` & `powergenome-0.6.2.tar`

### file list

```diff
@@ -1,51 +1,83 @@
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.260635 PowerGenome-0.6.1a0/
--rw-r--r--   0 gs5183     (501) staff       (20)     1070 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/LICENSE.md
--rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.260376 PowerGenome-0.6.1a0/PKG-INFO
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249740 PowerGenome-0.6.1a0/PowerGenome.egg-info/
--rw-r--r--   0 gs5183     (501) staff       (20)    16941 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/PKG-INFO
--rw-r--r--   0 gs5183     (501) staff       (20)     1308 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/SOURCES.txt
--rw-r--r--   0 gs5183     (501) staff       (20)        1 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/dependency_links.txt
--rw-r--r--   0 gs5183     (501) staff       (20)       99 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/entry_points.txt
--rw-r--r--   0 gs5183     (501) staff       (20)      232 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/requires.txt
--rw-r--r--   0 gs5183     (501) staff       (20)       17 2023-06-08 05:26:42.000000 PowerGenome-0.6.1a0/PowerGenome.egg-info/top_level.txt
--rw-r--r--   0 gs5183     (501) staff       (20)    16060 2023-06-08 05:16:33.000000 PowerGenome-0.6.1a0/README.md
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.249896 PowerGenome-0.6.1a0/data/
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255083 PowerGenome-0.6.1a0/data/additional_technologies/
--rw-r--r--   0 gs5183     (501) staff       (20)     1083 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      823 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2030.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      822 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2045.csv
--rw-r--r--   0 gs5183     (501) staff       (20)      625 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/additional_technologies/sample_additional_tech.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255232 PowerGenome-0.6.1a0/data/coal_fgd/
--rw-r--r--   0 gs5183     (501) staff       (20)    15123 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/coal_fgd/fgd_output.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255548 PowerGenome-0.6.1a0/data/cost_multipliers/
--rw-r--r--   0 gs5183     (501) staff       (20)     6226 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
--rw-r--r--   0 gs5183     (501) staff       (20)     1844 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/cost_multipliers/EIA regional cost multipliers.csv
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.255706 PowerGenome-0.6.1a0/data/cpi_data/
--rw-r--r--   0 gs5183     (501) staff       (20)      694 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/data/cpi_data/cpi_data.csv
--rw-r--r--   0 gs5183     (501) staff       (20)  7754322 2023-06-05 17:55:42.000000 PowerGenome-0.6.1a0/data/ipm_regions_simple.geojson
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259538 PowerGenome-0.6.1a0/powergenome/
--rw-r--r--   0 gs5183     (501) staff       (20)    44811 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/GenX.py
--rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 02:26:41.000000 PowerGenome-0.6.1a0/powergenome/__init__.py
-drwxr-xr-x   0 gs5183     (501) staff       (20)        0 2023-06-08 05:26:42.259894 PowerGenome-0.6.1a0/powergenome/cluster/
--rw-r--r--   0 gs5183     (501) staff       (20)    20651 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster/renewables.py
--rw-r--r--   0 gs5183     (501) staff       (20)     6669 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/cluster_method.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7980 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py
--rw-r--r--   0 gs5183     (501) staff       (20)     9047 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/distributed_gen.py
--rw-r--r--   0 gs5183     (501) staff       (20)    19178 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/eia_opendata.py
--rw-r--r--   0 gs5183     (501) staff       (20)    21119 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/external_data.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7656 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py
--rw-r--r--   0 gs5183     (501) staff       (20)     4856 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/fuels.py
--rw-r--r--   0 gs5183     (501) staff       (20)   135331 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/generators.py
--rw-r--r--   0 gs5183     (501) staff       (20)    11145 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/load_construction.py
--rw-r--r--   0 gs5183     (501) staff       (20)    33579 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/load_profiles.py
--rw-r--r--   0 gs5183     (501) staff       (20)    63909 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/nrelatb.py
--rw-r--r--   0 gs5183     (501) staff       (20)     2381 2023-06-08 03:45:29.000000 PowerGenome-0.6.1a0/powergenome/params.py
--rw-r--r--   0 gs5183     (501) staff       (20)     7516 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/price_adjustment.py
--rw-r--r--   0 gs5183     (501) staff       (20)    45619 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/resource_clusters.py
--rw-r--r--   0 gs5183     (501) staff       (20)    17869 2023-06-08 03:49:06.000000 PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py
--rw-r--r--   0 gs5183     (501) staff       (20)    14981 2023-06-07 04:30:00.000000 PowerGenome-0.6.1a0/powergenome/time_reduction.py
--rw-r--r--   0 gs5183     (501) staff       (20)    11110 2023-06-07 04:30:01.000000 PowerGenome-0.6.1a0/powergenome/transmission.py
--rw-r--r--   0 gs5183     (501) staff       (20)    36496 2023-06-08 03:59:24.000000 PowerGenome-0.6.1a0/powergenome/util.py
--rw-r--r--   0 gs5183     (501) staff       (20)       23 2023-06-08 01:52:09.000000 PowerGenome-0.6.1a0/powergenome/version.py
--rw-r--r--   0 gs5183     (501) staff       (20)     1730 2023-06-08 03:23:37.000000 PowerGenome-0.6.1a0/pyproject.toml
--rw-r--r--   0 gs5183     (501) staff       (20)       38 2023-06-08 05:26:42.260707 PowerGenome-0.6.1a0/setup.cfg
+-rw-r--r--   0        0        0      154 2020-02-02 00:00:00.000000 powergenome-0.6.2/.codecov.yml
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 powergenome-0.6.2/.git-blame-ignore-revs
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 powergenome-0.6.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     1827 2020-02-02 00:00:00.000000 powergenome-0.6.2/.travis.yml
+-rw-r--r--   0        0        0     1409 2020-02-02 00:00:00.000000 powergenome-0.6.2/.zenodo.json
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 powergenome-0.6.2/environment.yml
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 powergenome-0.6.2/requirements.txt
+-rw-r--r--   0        0        0  7754322 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/ipm_regions_simple.geojson
+-rw-r--r--   0        0        0     1083 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech.csv
+-rw-r--r--   0        0        0      823 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2030.csv
+-rw-r--r--   0        0        0      822 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2045.csv
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/additional tech documentation.md
+-rw-r--r--   0        0        0      625 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/additional_technologies/sample_additional_tech.csv
+-rw-r--r--   0        0        0    15123 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/coal_fgd/fgd_output.csv
+-rw-r--r--   0        0        0     6226 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv
+-rw-r--r--   0        0        0     1844 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cost_multipliers/EIA regional cost multipliers.csv
+-rw-r--r--   0        0        0      710 2020-02-02 00:00:00.000000 powergenome-0.6.2/data/cpi_data/cpi_data.csv
+-rw-r--r--   0        0        0    12734 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/issue_settings.yaml
+-rw-r--r--   0        0        0    49625 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/log.txt
+-rw-r--r--   0        0        0    77755 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/2030/p1_2030_Full_timeseries/Inputs/Fuels_data.csv
+-rw-r--r--   0        0        0   462368 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/2030/p1_2030_Full_timeseries/extra_outputs/existing_gen_units.csv
+-rw-r--r--   0        0        0    77755 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/Fuels_data.csv
+-rw-r--r--   0        0        0    75207 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
+-rw-r--r--   0        0        0     2407 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0    23159 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_OffShoreWind_Class3_Moderate_fixed_1_site_cluster_assignments.csv
+-rw-r--r--   0        0        0   401505 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/ERCOT_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0   288788 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0    97421 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0     2263 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
+-rw-r--r--   0        0        0    86283 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0    10591 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_OffShoreWind_Class3_Moderate_fixed_1_site_cluster_assignments.csv
+-rw-r--r--   0        0        0  1881138 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Eastern_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0   140067 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_LandbasedWind_Class3_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0    51701 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class12_Moderate_floating_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0     4144 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class12_Moderate_floating_1_site_cluster_assignments.csv
+-rw-r--r--   0        0        0      808 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_OffShoreWind_Class3_Moderate_fixed_0_site_cluster_assignments.csv
+-rw-r--r--   0        0        0   861463 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/Western_UtilityPV_Class1_Moderate__site_cluster_assignments.csv
+-rw-r--r--   0        0        0   479171 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/p1/Inputs/Inputs_p1/extra_outputs/existing_gen_units.csv
+-rw-r--r--   0        0        0     2424 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/demand.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/distributed_gen.yml
+-rw-r--r--   0        0        0       89 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/env.yml
+-rw-r--r--   0        0        0      749 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/extra_inputs.yml
+-rw-r--r--   0        0        0     2511 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/flexible_load.yml
+-rw-r--r--   0        0        0     3644 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/fuels.yml
+-rw-r--r--   0        0        0     4562 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/model_definition.yml
+-rw-r--r--   0        0        0     7367 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/resource_tags.yml
+-rw-r--r--   0        0        0    15057 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/resources.yml
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/scenario_management.yml
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/startup_costs.yml
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/time_clustering.yml
+-rw-r--r--   0        0        0      638 2020-02-02 00:00:00.000000 powergenome-0.6.2/debug/pg_settings/transmission.yml
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/.coveragerc
+-rw-r--r--   0        0        0    46651 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/GenX.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/__init__.py
+-rw-r--r--   0        0        0     6669 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/cluster_method.py
+-rw-r--r--   0        0        0     9078 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/co2_pipeline_cost.py
+-rw-r--r--   0        0        0     3571 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/debug.py
+-rw-r--r--   0        0        0     9471 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/distributed_gen.py
+-rw-r--r--   0        0        0    19170 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/eia_opendata.py
+-rw-r--r--   0        0        0    22359 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/external_data.py
+-rw-r--r--   0        0        0     7657 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/extract_pudl_data.py
+-rw-r--r--   0        0        0    13023 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/financials.py
+-rw-r--r--   0        0        0    10640 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/fuels.py
+-rw-r--r--   0        0        0   149932 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/generators.py
+-rw-r--r--   0        0        0    11200 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/load_construction.py
+-rw-r--r--   0        0        0    33914 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/load_profiles.py
+-rw-r--r--   0        0        0    67403 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/nrelatb.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/params.py
+-rw-r--r--   0        0        0     1869 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/price_adjustment.py
+-rw-r--r--   0        0        0    46177 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/resource_clusters.py
+-rw-r--r--   0        0        0    22404 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/run_powergenome_multiple_outputs_cli.py
+-rw-r--r--   0        0        0    18819 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/time_reduction.py
+-rw-r--r--   0        0        0    11195 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/transmission.py
+-rw-r--r--   0        0        0    49513 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/util.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/version.py
+-rw-r--r--   0        0        0    26970 2020-02-02 00:00:00.000000 powergenome-0.6.2/powergenome/cluster/renewables.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 powergenome-0.6.2/.gitignore
+-rw-r--r--   0        0        0     1070 2020-02-02 00:00:00.000000 powergenome-0.6.2/LICENSE.md
+-rw-r--r--   0        0        0    17355 2020-02-02 00:00:00.000000 powergenome-0.6.2/README.md
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 powergenome-0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    18797 2020-02-02 00:00:00.000000 powergenome-0.6.2/PKG-INFO
```

### Comparing `PowerGenome-0.6.1a0/LICENSE.md` & `powergenome-0.6.2/LICENSE.md`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/PKG-INFO` & `powergenome-0.6.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,56 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: PowerGenome
-Version: 0.6.1a0
+Version: 0.6.2
 Summary: Create power system inputs for capacity expansion models
+Project-URL: Source, https://github.com/PowerGenome/PowerGenome
 Author-email: Greg Schivley <greg.schivley@princeton.edu>
 Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
 License: MIT
-Project-URL: Source, https://github.com/PowerGenome/PowerGenome
-Keywords: power system data,capacity expansion,two
+License-File: LICENSE.md
+Keywords: capacity expansion,power system data,two
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.8
-Description-Content-Type: text/markdown
+Requires-Dist: beautifulsoup4>=4.8.13
+Requires-Dist: catalystcoop-pudl<=2022.11.30,>=0.6.0
+Requires-Dist: flatten-dict
+Requires-Dist: frozendict
+Requires-Dist: geopandas>=0.11
+Requires-Dist: openpyxl>=3.0
+Requires-Dist: python-dotenv
+Requires-Dist: pyyaml
+Requires-Dist: ruamel-yaml
+Requires-Dist: statsmodels>=0.12.2
 Provides-Extra: dev
-License-File: LICENSE.md
+Requires-Dist: black[jupyter]==24.3.0; extra == 'dev'
+Requires-Dist: build; extra == 'dev'
+Requires-Dist: isort; extra == 'dev'
+Requires-Dist: pre-commit; extra == 'dev'
+Requires-Dist: pytest; extra == 'dev'
+Requires-Dist: twine; extra == 'dev'
+Description-Content-Type: text/markdown
 
 # PowerGenome
 
 [![The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4426097.svg)](https://doi.org/10.5281/zenodo.4426096)
 [![pytest](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml/badge.svg)](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/PowerGenome/PowerGenome/branch/master/graph/badge.svg?token=7KJYLE3jOW)](https://codecov.io/gh/PowerGenome/PowerGenome)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/PowerGenome/PowerGenome/master.svg)](https://results.pre-commit.ci/latest/github/PowerGenome/PowerGenome/master)
 
-**Note:** The code and data for PowerGenome are under active development and some changes may break existing functions. Keep up to date with major code and data releases by joining [PowerGenome on groups.io](https://groups.io/g/powergenome). And **check out the growing documentation on the [Wiki](https://github.com/PowerGenome/PowerGenome/wiki)** for helpful background information.
+The code and data for PowerGenome are under active development and some changes may break existing functions. Keep up to date with major code and data releases by joining [PowerGenome on groups.io](https://groups.io/g/powergenome). And **check out the growing documentation on the [Wiki](https://github.com/PowerGenome/PowerGenome/wiki)** for helpful background information.
 
 Power system optimization models can be used to explore the cost and emission implications of different regulations in future energy systems. One of the most difficult parts of running these models is assembling all the data. A typical model will define several regions, each of which need data such as:
 
 - All existing generating units (perhaps grouped into a few discrete clusters within each region)
 - Transmission constraints between regions
 - Hourly load profiles (including new loads from vehicle and building electrification)
 - Hourly generation profiles for wind & solar
@@ -41,25 +58,19 @@
 
 Because computational complexity and run times increase as the number of regions and generating unit clusters increases, a user might want only want to disaggregate regions and generating units close to the primary region of interest. For example, a study focused on clean electricity regulations in New Mexico might combine several states in the Pacific Northwest into a single region while also splitting Arizona combined cycle units into multiple clusters.
 
 The goal of PowerGenome is to let a user make all of these choices in a settings file and then run a single script that generates input files for the power system model. PowerGenome currently generates input files for [GenX](https://energy.mit.edu/wp-content/uploads/2017/10/Enhanced-Decision-Support-for-a-Changing-Electricity-Landscape.pdf), and we hope to expand to other models in the near future.
 
 ## Data
 
-PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files.
-
-1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below).
-2. A [second sqlite database (pg_misc_efs)](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
-3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios ([efs_files_utc](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=share_link)).
+PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files. All data files [are available here](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing).
 
-There are also a few data files stored in this repository:
-
-- Regional cost multipliers for individual technologies developed by EIA (`data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`).
-- A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
-- Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
+1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below). This file is available at the link above or you can download it from the Zenodo repository.
+2. A second sqlite database (`pg_misc_tables_efs_2023_2.sqlite`) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
+3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios (`efs_files_utc`).
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
 `catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
@@ -83,41 +94,53 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
+5. Download the PUDL database [from Zenodo](https://doi.org/10.5281/zenodo.3653158) or the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
-6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
+6. Download the additional PowerGenome database from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). It includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
+7. Download the appropriate renewable resource data files from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). There is a single set of generation profiles and resource group folders specific to different regional aggregations. Read through the [included README](https://docs.google.com/document/d/1p_zDk6ng4tvgL1v1ZAXkvY9b34FmaLqdWFlJmUHP1Eo/edit?usp=share_link) for more background. This folder contains:
 
 - `generation_profiles` can be saved in a single place and used across multiple studies.
-- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the PowerGenome [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
+8. Download data files derived from NREL's EFS from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). These provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps and are used to both build up demand profiles in the future and create flexible demand resources that can shift their load.
 
-9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
+9. Download distributed generation profiles from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing) compiled from NREL Cambium 2022 scenarios.
 
-9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
+10. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
 - `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
 - `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
 - OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
 
 Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
 
-## Installation a packaged version (pip/conda-forge)
+## Installation with a packaged version (pip/conda-forge)
+
+Installing Powergenome with pip has only been tested within a conda environment but it should work in other environment management systems. Make sure that you have an updated version of pip installed. If you hit dependency errors I suggest trying to install them using mamba or conda. PowerGenome has `catalystcoop.pudl` as a dependency, which has a large number of its own dependencies. I have not (yet) had to install `catalystcoop.pudl` using mamba but doing so may help clear up errors.
 
-If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
+Depending on your operating system you might also have issues installing some other packages from pip. The example code below is what works for me on a Mac, where python-snappy fails to build wheels.
+
+```sh
+(base) conda create -n powergenome python=3.10 pip python-snappy=0.6.1
+(base) conda activate powergenome
+(powergenome) pip install powergenome
+```
+
+PowerGenome has been submitted to conda-forge but is not yet available.
+
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env_params.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
 
@@ -141,14 +164,20 @@
 
 Functions from each module can be imported and used in an interactive environment (e.g. JupyterLab). Examples of how to load data in this way are included in `PowerGenome/notebooks`. To run from the command line, navigate to a project folder that contains a settings file and extra inputs (e.g. `myproject/powergenome`), activate the  `powergenome` conda environment, and use the command `run_powergenome_multiple` with flags for the settings file name and where the results should be saved. Since the `powergenome` package is installed in the `powergenome` conda environment, you can run the command line function from anywhere on your computer (not just within the cloned `PowerGenome` folder).
 
 ```sh
 run_powergenome_multiple --settings_file settings --results_folder test_system
 ```
 
+Or to set up files for multi-period runs in GenX
+
+```sh
+run_powergenome_multiple --settings_file settings --results_folder test_system --multi-period
+```
+
 The command line arguments `--settings_file` and `--results_folder` can be shortened to `-sf` and `-rf` respectively. For all options, run:
 
 ```sh
 run_powergenome_multiple --help
 ```
 
 A folder with extra user inputs is required when using the `run_powergenome_multiple` command. The name of this folder is defined in the settings YAML file with the `input_folder` parameter. Look at the files in each example system for test cases to follow.
```

### Comparing `PowerGenome-0.6.1a0/PowerGenome.egg-info/PKG-INFO` & `powergenome-0.6.2/README.md`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,17 @@
-Metadata-Version: 2.1
-Name: PowerGenome
-Version: 0.6.1a0
-Summary: Create power system inputs for capacity expansion models
-Author-email: Greg Schivley <greg.schivley@princeton.edu>
-Maintainer-email: Greg Schivley <greg.schivley@princeton.edu>
-License: MIT
-Project-URL: Source, https://github.com/PowerGenome/PowerGenome
-Keywords: power system data,capacity expansion,two
-Classifier: Development Status :: 4 - Beta
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Science/Research
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Natural Language :: English
-Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3
-Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-Provides-Extra: dev
-License-File: LICENSE.md
-
 # PowerGenome
 
 [![The project has reached a stable, usable state and is being actively developed.](https://www.repostatus.org/badges/latest/active.svg)](https://www.repostatus.org/#active)
 [![code style black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![DOI](https://zenodo.org/badge/DOI/10.5281/zenodo.4426097.svg)](https://doi.org/10.5281/zenodo.4426096)
 [![pytest](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml/badge.svg)](https://github.com/PowerGenome/PowerGenome/actions/workflows/pytest.yml)
 [![codecov](https://codecov.io/gh/PowerGenome/PowerGenome/branch/master/graph/badge.svg?token=7KJYLE3jOW)](https://codecov.io/gh/PowerGenome/PowerGenome)
+[![pre-commit.ci status](https://results.pre-commit.ci/badge/github/PowerGenome/PowerGenome/master.svg)](https://results.pre-commit.ci/latest/github/PowerGenome/PowerGenome/master)
 
-**Note:** The code and data for PowerGenome are under active development and some changes may break existing functions. Keep up to date with major code and data releases by joining [PowerGenome on groups.io](https://groups.io/g/powergenome). And **check out the growing documentation on the [Wiki](https://github.com/PowerGenome/PowerGenome/wiki)** for helpful background information.
+The code and data for PowerGenome are under active development and some changes may break existing functions. Keep up to date with major code and data releases by joining [PowerGenome on groups.io](https://groups.io/g/powergenome). And **check out the growing documentation on the [Wiki](https://github.com/PowerGenome/PowerGenome/wiki)** for helpful background information.
 
 Power system optimization models can be used to explore the cost and emission implications of different regulations in future energy systems. One of the most difficult parts of running these models is assembling all the data. A typical model will define several regions, each of which need data such as:
 
 - All existing generating units (perhaps grouped into a few discrete clusters within each region)
 - Transmission constraints between regions
 - Hourly load profiles (including new loads from vehicle and building electrification)
 - Hourly generation profiles for wind & solar
@@ -41,25 +19,19 @@
 
 Because computational complexity and run times increase as the number of regions and generating unit clusters increases, a user might want only want to disaggregate regions and generating units close to the primary region of interest. For example, a study focused on clean electricity regulations in New Mexico might combine several states in the Pacific Northwest into a single region while also splitting Arizona combined cycle units into multiple clusters.
 
 The goal of PowerGenome is to let a user make all of these choices in a settings file and then run a single script that generates input files for the power system model. PowerGenome currently generates input files for [GenX](https://energy.mit.edu/wp-content/uploads/2017/10/Enhanced-Decision-Support-for-a-Changing-Electricity-Landscape.pdf), and we hope to expand to other models in the near future.
 
 ## Data
 
-PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files.
-
-1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below).
-2. A [second sqlite database (pg_misc_efs)](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
-3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios ([efs_files_utc](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=share_link)).
+PowerGenome uses data from a number of different sources, including EIA, NREL, and EPA. The data are accessed through a combination of sqlite databases, CSV files, and parquet data files. All data files [are available here](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing).
 
-There are also a few data files stored in this repository:
-
-- Regional cost multipliers for individual technologies developed by EIA (`data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`).
-- A simplified geojson version of EPA's shapefile for IPM regions (`data/ipm_regions_simple.geojson`).
-- Information on user-defined technologies, which can be included in outputs. This can be used to define a custom cost case (e.g. $500/kW PV) or a new technology such as natural gas with 100% carbon capture. The CSV files are stored in the `extra_inputs` subfolders of each example system. A documentation file in that folder describes what to include in the file.
+1. EIA data on existing generating units are already compiled into a [single sqlite database (PUDL)](https://doi.org/10.5281/zenodo.3653158) (see instructions for using it below). This file is available at the link above or you can download it from the Zenodo repository.
+2. A second sqlite database (`pg_misc_tables_efs_2023_2.sqlite`) has tables with new resource costs from NREL ATB, transmission constraints between IPM regions from EIA, and hourly demand within each IPM region derived from NREL or FERC data.
+3. The hourly incremental demand for different flexible demand technologies, and stock values across a range of projection scenarios (`efs_files_utc`).
 
 ## PUDL Dependency
 
 This project pulls data from [PUDL](https://github.com/catalyst-cooperative/pudl). As such, it requires installation of PUDL to access a normalized sqlite database and some of the convienience PUDL functions.
 
 `catalystcoop.pudl` is included in the `environment.yml` file and will be installed automatically in the conda environment (see instructions below). Catalyst Cooperative will be creating versioned data releases of PUDL, which can be [accessed on Zenodo](https://doi.org/10.5281/zenodo.3653158). Download the zip file from Zenodo, unzip it, and find the sqlite database under `pudl_data/sqlite/pudl.sqlite`. Note that the version of `catalystcoop.pudl` software may change based on the database version you use. Look on the right-hand side of the zenodo archive to see what software version was used to compile the data. If the version in your conda environment does not match the version used to compile the data, you can change it in the `environment.yml` file or install a [different version](https://docs.conda.io/projects/conda/en/latest/user-guide/tasks/manage-pkgs.html#installing-packages) using `mamba install catalystcoop.pudl=<your_version>`.
 
@@ -83,41 +55,53 @@
 
 4. pip-install an editable version of this project
 
 ```sh
 pip install -e .
 ```
 
-5. Download [the PUDL database](https://doi.org/10.5281/zenodo.3653158), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
+5. Download the PUDL database [from Zenodo](https://doi.org/10.5281/zenodo.3653158) or the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing), unzip it, and copy the `/pudl_data/sqlite/pudl.sqlite` to wherever you would like to store PowerGenome data on your computer. The zip file contains other data sets that aren't needed for PowerGenome and can be deleted.  Note that as of May 2023 the most recent version of this database (v2022.11.30) is compatible with `catalystcoop.pudl` version v2022.11.30 and may not work if an earlier software version is included in your conda environment.
 
-6. Download [additional PowerGenome data](https://drive.google.com/file/d/1LCB0uwnx6VHrmHQDPH2huLHU6fKXb7kG/view?usp=sharing) that includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
+6. Download the additional PowerGenome database from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). It includes NREL ATB cost data, transmission constraints between IPM regions, and hourly demand for each IPM region. Hourly demand is based on a 2012 weather year and was constructed either directly from FERC 714 data (`load_curves_ferc`) or from NREL EFS data (`load_curves_nrel_efs`) that also sources back to FERC 714. The NREL load curves, which separate hourly demand by sector and subsector, are now the default source for load curves in PowerGenome. See [the wiki](https://github.com/PowerGenome/PowerGenome/wiki/Settings-files#demand) for more information. These files will eventually be provided through a data repository with citation information.
 
-7. Download the appropriate [renewable resource data files](https://drive.google.com/drive/folders/1G9IHtY1RMZHUEXAmYQEb-mvzzhqun-Kb?usp=sharing). Read through the README for more background. This folder contains:
+7. Download the appropriate renewable resource data files from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). There is a single set of generation profiles and resource group folders specific to different regional aggregations. Read through the [included README](https://docs.google.com/document/d/1p_zDk6ng4tvgL1v1ZAXkvY9b34FmaLqdWFlJmUHP1Eo/edit?usp=share_link) for more background. This folder contains:
 
 - `generation_profiles` can be saved in a single place and used across multiple studies.
-- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
+- Each of the folders under `resource_groups` has CSV files that tell PowerGenome the metro that each potential wind/solar site will deliver power to based on a set of regional aggregations. Use the corresponding regional aggregations in your settings file. You can request new resource group files for different regional aggregations on the PowerGenome [repository discussion page](https://github.com/PowerGenome/PowerGenome/discussions)
 
-8. Download and unzip [data files derived from NREL's EFS](https://drive.google.com/file/d/1bS-5LycImdp1AYoS_0uK7tXRHo8TWKCD/view?usp=sharing) that provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps.
+8. Download data files derived from NREL's EFS from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing). These provide hourly demand profiles for growing electrification technologies like electric vehicles and heat pumps and are used to both build up demand profiles in the future and create flexible demand resources that can shift their load.
 
-9. Download and unzip [distributed generation profiles](https://drive.google.com/file/d/1kqBQle2CLET_BMZd0Y91o6AjfgunQKf4/view?usp=share_link) compiled from NREL Cambium 2022 scenarios.
+9. Download distributed generation profiles from the [PowerGenome data repository](https://drive.google.com/drive/folders/1K5GWF5lbe-mKSTUSuJxnFdYGCdyDJ7iE?usp=sharing) compiled from NREL Cambium 2022 scenarios.
 
-9. Create the file `PowerGenome/powergenome/.env`. In this file, add:
+10. Create the file `PowerGenome/powergenome/.env`. In this file, add:
 
 - `PUDL_DB=YOUR_PATH_HERE` (your path to the PUDL database downloaded in step 5)
 - `PG_DB=YOUR_PATH_HERE` (your path to the additional PowerGenome data downloaded in step 6)
 - `RESOURCE_GROUP_PROFILES=YOUR_PATH_HERE` (your path to the folder with hourly wind/solar generation parquet files)
 - `EFS_DATA=YOUR_PATH_HERE` (your path to the folder with EFS derived data files)
 - `DISTRIBUTED_GEN_DATA=YOUR_PATH_HERE` (your path to the folder with distributed generation profiles)
 - OPTIONAL: `RESOURCE_GROUPS=YOUR_PATH_HERE` (your path to the resource groups data for a project -- **this can be included in your settings file instead of the .env file**)
 
 Quotation marks are only needed if your values contain spaces. The `.env` file is included in `.gitignore` and will not be synced with the repository.
 
-## Installation a packaged version (pip/conda-forge)
+## Installation with a packaged version (pip/conda-forge)
+
+Installing Powergenome with pip has only been tested within a conda environment but it should work in other environment management systems. Make sure that you have an updated version of pip installed. If you hit dependency errors I suggest trying to install them using mamba or conda. PowerGenome has `catalystcoop.pudl` as a dependency, which has a large number of its own dependencies. I have not (yet) had to install `catalystcoop.pudl` using mamba but doing so may help clear up errors.
 
-If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
+Depending on your operating system you might also have issues installing some other packages from pip. The example code below is what works for me on a Mac, where python-snappy fails to build wheels.
+
+```sh
+(base) conda create -n powergenome python=3.10 pip python-snappy=0.6.1
+(base) conda activate powergenome
+(powergenome) pip install powergenome
+```
+
+PowerGenome has been submitted to conda-forge but is not yet available.
+
+If you are installing a packaged version of PowerGenome you won't be able to easily use a .env file. Instead, add the environment parameters (`PUDL_DB`, `PG_DB`, etc) to a YAML file in the same folder as the rest of your settings. It doesn't really matter which file these parameters are included in but creating a new file such as `env_params.yml` will help keep them separate from other settings parameters that might be shared with other PowerGenome users.
 
 ## Running code
 
 ### Suggested folder structure
 
 It is best practice to set up project folders outside of the cloned repository so that git doesn't track any new/changed files within the upper-level `PowerGenome` folder. Try copying one of the example systems (settings file and extra inputs) and modifying it. Copy the `notebooks` folder into your project folder, change the path to the settings file as needed, and run code in the notebooks. This can also be a good way to learn how data are created in PowerGenome and debug problem.
 
@@ -141,14 +125,20 @@
 
 Functions from each module can be imported and used in an interactive environment (e.g. JupyterLab). Examples of how to load data in this way are included in `PowerGenome/notebooks`. To run from the command line, navigate to a project folder that contains a settings file and extra inputs (e.g. `myproject/powergenome`), activate the  `powergenome` conda environment, and use the command `run_powergenome_multiple` with flags for the settings file name and where the results should be saved. Since the `powergenome` package is installed in the `powergenome` conda environment, you can run the command line function from anywhere on your computer (not just within the cloned `PowerGenome` folder).
 
 ```sh
 run_powergenome_multiple --settings_file settings --results_folder test_system
 ```
 
+Or to set up files for multi-period runs in GenX
+
+```sh
+run_powergenome_multiple --settings_file settings --results_folder test_system --multi-period
+```
+
 The command line arguments `--settings_file` and `--results_folder` can be shortened to `-sf` and `-rf` respectively. For all options, run:
 
 ```sh
 run_powergenome_multiple --help
 ```
 
 A folder with extra user inputs is required when using the `run_powergenome_multiple` command. The name of this folder is defined in the settings YAML file with the `input_folder` parameter. Look at the files in each example system for test cases to follow.
```

### Comparing `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech.csv` & `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2030.csv` & `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2030.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/additional_technologies/AZ_additional_tech_2045.csv` & `powergenome-0.6.2/data/additional_technologies/AZ_additional_tech_2045.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/additional_technologies/sample_additional_tech.csv` & `powergenome-0.6.2/data/additional_technologies/sample_additional_tech.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/coal_fgd/fgd_output.csv` & `powergenome-0.6.2/data/coal_fgd/fgd_output.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv` & `powergenome-0.6.2/data/cost_multipliers/AEO_2020_regional_cost_corrections.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/cost_multipliers/EIA regional cost multipliers.csv` & `powergenome-0.6.2/data/cost_multipliers/EIA regional cost multipliers.csv`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/data/cpi_data/cpi_data.csv` & `powergenome-0.6.2/data/cpi_data/cpi_data.csv`

 * *Files 8% similar despite different names*

```diff
@@ -38,7 +38,8 @@
 2016,12,240.007
 2017,12,245.12
 2018,12,251.107
 2019,12,255.657
 2020,12,258.811
 2021,12,270.97
 2022,12,292.655
+2023,12,304.702
```

### Comparing `PowerGenome-0.6.1a0/data/ipm_regions_simple.geojson` & `powergenome-0.6.2/data/ipm_regions_simple.geojson`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/powergenome/GenX.py` & `powergenome-0.6.2/powergenome/GenX.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,21 +6,19 @@
 from typing import Dict, List
 
 import pandas as pd
 
 from powergenome.external_data import (
     load_demand_segments,
     load_policy_scenarios,
-    load_user_genx_settings,
     make_generator_variability,
 )
-from powergenome.load_profiles import make_distributed_gen_profiles
-from powergenome.nrelatb import investment_cost_calculator
+from powergenome.financials import investment_cost_calculator
 from powergenome.time_reduction import kmeans_time_clustering
-from powergenome.util import find_region_col, load_settings, snake_case_col
+from powergenome.util import find_region_col, snake_case_col, snake_case_str
 
 logger = logging.getLogger(__name__)
 
 INT_COLS = [
     "Inv_Cost_per_MWyr",
     "Fixed_OM_Cost_per_MWyr",
     "Inv_Cost_per_MWhyr",
@@ -103,17 +101,17 @@
                     zone_df.loc[0, col] = value
             else:
                 zone_df.loc[:, col] = value
     else:
         for region, col in product(
             year_case_policy["region"].unique(), year_case_policy[policy_cols].columns
         ):
-            zone_df.loc[
-                zone_df["Region_description"] == region, col
-            ] = year_case_policy.loc[year_case_policy.region == region, col].values[0]
+            zone_df.loc[zone_df["Region_description"] == region, col] = (
+                year_case_policy.loc[year_case_policy.region == region, col].values[0]
+            )
 
     # zone_df = zone_df.drop(columns="region")
 
     return zone_df
 
 
 def create_regional_cap_res(settings: dict) -> pd.DataFrame:
@@ -182,17 +180,17 @@
         within the constraint. Values of 0 mean it connects two regions that are both
         within or outside the constraint.
     """
     cap_res_list = []
     for name in path_names:
         s_r = name.split("_to_")[0]
         e_r = name.split("_to_")[-1]
-        if (s_r in dest_regions) and not (e_r in dest_regions):
+        if (s_r in dest_regions) and e_r not in dest_regions:
             cap_res_list.append(1)
-        elif (e_r in dest_regions) and not (s_r in dest_regions):
+        elif (e_r in dest_regions) and s_r not in dest_regions:
             cap_res_list.append(-1)
         else:
             cap_res_list.append(0)
 
     assert len(cap_res_list) == len(path_names)
 
     return cap_res_list
@@ -222,18 +220,14 @@
     if (
         "Transmission Path Name" in tx_df.columns
         and "transmission_path_name" not in tx_df.columns
     ):
         tx_df["transmission_path_name"] = tx_df["Transmission Path Name"]
     original_cols = tx_df.columns.to_list()
 
-    zones = settings["model_regions"]
-    zone_num_map = {
-        zone: f"z{number + 1}" for zone, number in zip(zones, range(len(zones)))
-    }
     path_names = tx_df["transmission_path_name"].to_list()
     policy_nums = []
 
     # Loop through capacity reserve constraints (CapRes_*) and determine network
     # parameters for each
     for cap_res in settings.get("regional_capacity_reserves", {}) or {}:
         cap_res_num = int(cap_res.split("_")[-1])  # the number of the capres constraint
@@ -313,17 +307,17 @@
                     zone_df.loc[0, col] = value
             else:
                 zone_df.loc[:, col] = value
     else:
         for region, col in product(
             year_case_policy["region"].unique(), year_case_policy.columns
         ):
-            zone_df.loc[
-                zone_df["Region description"] == region, col
-            ] = year_case_policy.loc[year_case_policy.region == region, col].values[0]
+            zone_df.loc[zone_df["Region description"] == region, col] = (
+                year_case_policy.loc[year_case_policy.region == region, col].values[0]
+            )
 
     zone_df = zone_df.drop(columns="region")
 
     network_df = pd.concat([zone_df, transmission_df], axis=1)
 
     return network_df
 
@@ -357,30 +351,31 @@
 
     context = f"Assigning misc generator values from the user-supplied file {path}."
     try:
         region_col = find_region_col(misc_values.columns, context)
     except ValueError:
         region_col = "region"
         misc_values["region"] = "all"
-    regions = [r for r in misc_values[region_col].unique() if r.lower() != "all"]
+    regions = [
+        r for r in misc_values[region_col].fillna("all").unique() if r.lower() != "all"
+    ]
     wrong_regions = [r for r in regions if r not in settings["model_regions"]]
     if wrong_regions:
         raise ValueError(
             f"The `misc_gen_inputs_fn` CSV has regions {wrong_regions}, which are not "
             f"valid model regions. Valid model regions are {settings['model_regions']}."
         )
 
     for region in settings["model_regions"]:
         _df = misc_values.loc[misc_values[region_col].str.lower() == "all", :]
         _df.loc[:, "region"] = region
         misc_values = misc_values.append(_df)
 
     misc_values = misc_values.loc[misc_values[region_col].str.lower() != "all", :]
 
-    resource_len = 0
     for tech, _df in misc_values.groupby(resource_col):
         num_tech_regions = len(
             gen_clusters.loc[
                 gen_clusters[resource_col].str.contains(tech, case=False)
             ].drop_duplicates(subset=["region"])
         )
         num_values = len(_df)
@@ -388,18 +383,18 @@
             logger.warning(
                 f"The `misc_gen_inputs_fn` CSV has {num_values} region(s) for the resource "
                 f"'{tech}', but the resource is in {num_tech_regions} regions. Check "
                 "your input file to ensure values are provided for all appropriate regions."
             )
     generic_resources = []
     for gen_resource in gen_clusters[resource_col].unique():
-        for r in settings["model_regions"]:
+        for r in sorted(settings["model_regions"])[::-1]:
             if r in gen_resource:
                 gen_resource = gen_resource.replace(r + "_", "")
-                generic_resources.append(gen_resource)
+                generic_resources.append(snake_case_str(gen_resource))
                 continue
     generic_resources = set(generic_resources)
     missing_resources = []
     for resource in generic_resources:
         match = False
         for misc_resource in misc_values[resource_col].unique():
             if misc_resource in resource.lower():
@@ -419,15 +414,19 @@
         col for col in misc_values.columns if col not in [region_col, resource_col]
     ]
 
     for idx, row in misc_values.iterrows():
         row_cols = row[value_cols].dropna().index
         gen_clusters.loc[
             (gen_clusters["region"] == row[region_col])
-            & (gen_clusters[resource_col].str.contains(row[resource_col], case=False)),
+            & (
+                snake_case_col(gen_clusters[resource_col]).str.contains(
+                    row[resource_col], case=False
+                )
+            ),
             row_cols,
         ] = row[row_cols].values
     return gen_clusters
 
 
 def reduce_time_domain(
     resource_profiles, load_profiles, settings, variable_resources_only=True
@@ -444,14 +443,15 @@
             resource_profiles=resource_profiles,
             load_profiles=load_profiles,
             days_in_group=days,
             num_clusters=time_periods,
             include_peak_day=include_peak_day,
             load_weight=load_weight,
             variable_resources_only=variable_resources_only,
+            n_init=settings.get("tdr_n_init", 100),
         )
 
         reduced_resource_profile = results["resource_profiles"]
         reduced_resource_profile.index.name = "Resource"
         reduced_resource_profile.index = range(1, len(reduced_resource_profile) + 1)
         reduced_load_profile = results["load_profiles"]
         time_series_mapping = results["time_series_mapping"]
@@ -480,15 +480,15 @@
             reduced_load_output,
             time_series_mapping,
             representative_point,
         )
 
     else:
         time_index = pd.Series(data=range(1, len(load_profiles) + 1), name="Time_Index")
-        sub_weights = pd.Series(data=[1], name="Sub_Weights")
+        sub_weights = pd.Series(data=[8760], name="Sub_Weights")
         hours_per_period = pd.Series(
             data=[len(load_profiles)], name="Timesteps_per_Rep_Period"
         )
         subperiods = pd.Series(data=[1], name="Rep_Periods")
 
         # Not actually reduced
         load_output = pd.concat(
@@ -528,15 +528,15 @@
         )
     loss_per_100_miles = settings["tx_line_loss_100_miles"]
     if "distance_mile" in transmission.columns:
         distance_col = "distance_mile"
     elif "distance_km" in transmission.columns:
         distance_col = "distance_km"
         loss_per_100_miles *= 0.62137
-        logger.info("Line loss per 100 miles was converted to km.")
+        logger.debug("Line loss per 100 miles was converted to km.")
     else:
         raise KeyError("No distance column is available in the transmission dataframe")
 
     transmission["Line_Loss_Percentage"] = (
         transmission[distance_col] / 100 * loss_per_100_miles
     )
 
@@ -603,15 +603,20 @@
     if not line_inv_period:
         raise KeyError(
             "No value for the transmission investment period is included in the settings."
             "This numeric value is included under transmission_investment_costs.tx."
             "investment_years. See the `test_settings.yml` file for an example."
         )
     line_inv_cost = (
-        investment_cost_calculator(line_capex, line_wacc, line_inv_period)
+        investment_cost_calculator(
+            line_capex,
+            line_wacc,
+            line_inv_period,
+            settings.get("interest_compound_method", "discrete"),
+        )
         * transmission["distance_mile"]
     )
 
     transmission["Line_Reinforcement_Cost_per_MWyr"] = line_inv_cost.round(0)
 
     return transmission
 
@@ -929,15 +934,15 @@
     resource_df = resource_df.reset_index(drop=True)
     resource_df.loc[:, "unadjusted_min_power"] = resource_df.loc[:, min_power_col]
     _gen_profile = gen_profile_df.copy(deep=True)
     _gen_profile
     gen_profile_min = _gen_profile.min().reset_index(drop=True)
     mask = (resource_df[min_power_col].fillna(0) > gen_profile_min).values
 
-    logger.info(
+    logger.debug(
         f"{sum(mask)} resources have {min_power_col} larger than hourly generation."
     )
 
     resource_df.loc[mask, min_power_col] = gen_profile_min[mask].round(3)
 
     return resource_df
 
@@ -1154,17 +1159,17 @@
 
     for region, factor in (regional_factors or {}).items():
         region_mask = df["region"] == region
         if region_mask.any():
             avg_inflow = (
                 make_generator_variability(df).mean().reset_index(drop=True) * factor
             ).loc[hydro_mask & region_mask]
-            df.loc[
-                (df["HYDRO"] == 1) & region_mask, "Hydro_Energy_to_Power_Ratio"
-            ] = avg_inflow.where(avg_inflow > 1, 1)
+            df.loc[(df["HYDRO"] == 1) & region_mask, "Hydro_Energy_to_Power_Ratio"] = (
+                avg_inflow.where(avg_inflow > 1, 1)
+            )
     df["Hydro_Energy_to_Power_Ratio"] = df["Hydro_Energy_to_Power_Ratio"].fillna(0)
     return df
 
 
 def rename_gen_cols(
     df: pd.DataFrame, rename_cols: Dict[str, str] = None
 ) -> pd.DataFrame:
@@ -1210,16 +1215,67 @@
     Returns
     -------
     pd.DataFrame
         Modified version of original df with CO2 pipeline annuity/O&M added to plant
         costs
     """
     if "co2_cost_mwh" in df.columns:
-        df["Var_OM_Cost_per_MWh"] += df["co2_cost_mwh"]
+        df["Var_OM_Cost_per_MWh"] += df["co2_cost_mwh"].fillna(0)
     if "co2_pipeline_annuity_mw" in df.columns:
-        df["Inv_Cost_per_MWyr"] += df["co2_pipeline_annuity_mw"]
+        df["Inv_Cost_per_MWyr"] += df["co2_pipeline_annuity_mw"].fillna(0)
     if "co2_o_m_mw" in df.columns:
-        df["Fixed_OM_Cost_per_MWyr"] += df["co2_o_m_mw"]
+        df["Fixed_OM_Cost_per_MWyr"] += df["co2_o_m_mw"].fillna(0)
     if "co2_pipeline_capex_mw" in df.columns:
-        df["capex_mw"] += df["co2_pipeline_capex_mw"]
+        df["capex_mw"] += df["co2_pipeline_capex_mw"].fillna(0)
 
     return df
+
+
+def cap_retire_within_period(
+    gens: pd.DataFrame, first_year: int, last_year: int, capacity_col: str
+) -> pd.Series:
+    retired_cap = (
+        gens.query("retirement_year <= @last_year and retirement_year >= @first_year")
+        .groupby("Resource", as_index=False)[[capacity_col, "capacity_mwh"]]
+        .sum()
+    ).rename(
+        columns={
+            capacity_col: "Min_Retired_Cap_MW",
+            "capacity_mwh": "Min_Retired_Energy_Cap_MW",
+        }
+    )
+    retired_cap["Min_Retired_Charge_Cap_MW"] = 0
+
+    return retired_cap
+
+
+def check_vre_profiles(
+    gen_df: pd.DataFrame,
+    gen_var_df: pd.DataFrame,
+    vre_cols: List[str] = ["VRE", "HYDRO"],
+):
+    """Check generation profiles of VRE resources to ensure they are variable. Alert the
+    user with a logger warning if any are not.
+
+    Parameters
+    ----------
+    gen_df : pd.DataFrame
+        Dataframe of generators. Must have column "Resource".
+    gen_var_df : pd.DataFrame
+        Dataframe of hourly generation for each resource. Column names are from the
+        "Resource" column of `gen_df`.
+    vre_cols : List[str]
+        List of boolean columns indicating inclusion in the group of variable resources.
+        By default, ["VRE", "HYDRO"].
+    """
+    var_gen_names = []
+    vre_cols = [c for c in vre_cols if c in gen_df.columns]
+    if vre_cols:
+        for c in vre_cols:
+            var_gen_names.extend(gen_df.loc[gen_df[c] == 1, "Resource"].to_list())
+
+        vre_std = gen_var_df[var_gen_names].std()
+        if (vre_std == 0).any():
+            non_variable = vre_std.loc[vre_std == 0].index.to_list()
+            logger.warning(
+                f"The variable resources {non_variable} have non-variable generation profiles."
+            )
```

### Comparing `PowerGenome-0.6.1a0/powergenome/cluster/renewables.py` & `powergenome-0.6.2/powergenome/cluster/renewables.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,32 @@
 """
 Flexible methods to cluster/aggregate renewable projects
 """
+
 import logging
+import operator
 from functools import lru_cache
 from pathlib import Path
 from typing import Any, Dict, List, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow.parquet as pq
-from sklearn.cluster import AgglomerativeClustering
+from sklearn.cluster import AgglomerativeClustering, KMeans
+from sklearn.preprocessing import StandardScaler
 
 from powergenome.resource_clusters import MERGE
 from powergenome.util import deep_freeze_args, snake_case_str
 
 logger = logging.getLogger(__name__)
 
 
 def load_site_profiles(path: Path, site_ids: List[str]) -> pd.DataFrame:
     suffix = path.suffix
+    site_ids = [s.replace(".0", "") for s in site_ids]
     if suffix == ".parquet":
         df = pq.read_table(path, columns=site_ids).to_pandas()
     elif suffix == ".csv":
         df = pd.read_csv(path, usecols=site_ids)
     return df
 
 
@@ -118,15 +122,15 @@
         labels = np.ones_like(s)
 
     return labels
 
 
 @deep_freeze_args
 @lru_cache()
-def agg_cluster_profile(s: pd.Series, n_clusters: int) -> pd.DataFrame:
+def agg_cluster_profile(s: pd.Series, n_clusters: int, **kwargs) -> np.ndarray:
     if len(s) == 0:
         return []
     if len(s) == 1:
         return np.array([0])
     if n_clusters <= 0:
         logger.warning(
             f"You have entered a n_clusters parameter that is less than or equal to 0 "
@@ -147,15 +151,15 @@
     )
     labels = clust.labels_
     return labels
 
 
 @deep_freeze_args
 @lru_cache()
-def agg_cluster_other(s: pd.Series, n_clusters: int) -> pd.DataFrame:
+def agg_cluster_other(s: pd.Series, n_clusters: int, **kwargs) -> np.ndarray:
     if len(s) == 0:
         return []
     if len(s) == 1:
         return np.array([0])
     if n_clusters <= 0:
         logger.warning(
             f"You have entered a n_clusters parameter that is less than or equal to 0 "
@@ -173,77 +177,130 @@
     clust = AgglomerativeClustering(n_clusters=n_clusters).fit(
         np.array(s).reshape(-1, 1)
     )
     labels = clust.labels_
     return labels
 
 
-def agglomerative_cluster_binned(
+def kmeans_cluster_other(df: pd.DataFrame, n_clusters: int, **kwargs) -> np.ndarray:
+    if len(df) == 0 or df.empty:
+        return []
+    if len(df) == 1:
+        return np.array([0])
+    if n_clusters <= 0:
+        logger.warning(
+            f"You have entered a n_clusters parameter that is less than or equal to 0 "
+            "in the settings parameter renewables_clusters. n_clusters must be >= 1. "
+            "Manually setting n_clusters to 1 in this case."
+        )
+        n_clusters = 1
+    if n_clusters > len(df):
+        logger.warning(
+            f"You have entered a n_clusters parameter that is greater than the number of "
+            "renewable sites for one grouping in the settings parameter renewables_clusters."
+            "Manually assiging each site to its own cluster."
+        )
+        return np.arange(0, len(df))
+
+    clust = KMeans(n_clusters=n_clusters, random_state=42, **kwargs).fit(
+        StandardScaler().fit_transform(df)
+    )
+    labels = clust.labels_
+    return labels
+
+
+def cluster_sites_binned(
     data: pd.DataFrame,
     by: Union[str, List[str]],
-    feature: str,
+    method: str,
+    feature: Union[str, List[str]],
     n_clusters: Union[int, pd.Series, dict],
     **kwargs,
 ) -> pd.DataFrame:
     if data.empty:
         data["cluster"] = []
         return data
 
     if feature == "profile":
+        if method not in ["agglomerative", "agg", "hierarchical"]:
+            logger.warning(
+                f"The renewables clustering method {method} cannot be used with the "
+                "'profile' feature. Using agglomerative clustering instead."
+            )
         func = agg_cluster_profile
     else:
-        func = agg_cluster_other
+        func = CLUSTER_METHOD_FUNCS[method]
 
     grouped = data.groupby(by)
     df_list = []
     first_label = 0
     if isinstance(n_clusters, int):
         _n_clusters = n_clusters
     for _, _df in grouped:
         if not _df.empty:
             if not isinstance(n_clusters, int):
                 _n_clusters = n_clusters[_]
-            labels = func(_df[feature], min(_n_clusters, len(_df)))
+            labels = func(_df[feature], min(_n_clusters, len(_df)), **kwargs)
             labels += first_label
             first_label = max(labels) + 1
             _df["cluster"] = labels
             df_list.append(_df)
+        else:
+            _df = pd.DataFrame(columns=list(data.columns) + ["cluster"])
+            df_list.append(_df)
     df = pd.concat(df_list)
 
     return df
 
 
-def agglomerative_cluster_no_bin(
-    data: pd.DataFrame, feature: str, n_clusters: int, **kwargs
+def cluster_sites_no_bin(
+    data: pd.DataFrame,
+    method: str,
+    feature: Union[str, List[str]],
+    n_clusters: int,
+    **kwargs,
 ) -> pd.DataFrame:
     if data.empty:
         data["cluster"] = []
         return data
     _data = data.copy()
     if feature == "profile":
+        if method not in ["agglomerative", "agg", "hierarchical"]:
+            logger.warning(
+                f"The renewables clustering method {method} cannot be used with the "
+                "'profile' feature. Using agglomerative clustering instead."
+            )
         func = agg_cluster_profile
     else:
-        func = agg_cluster_other
+        func = CLUSTER_METHOD_FUNCS[method]
 
     if len(_data) == 1:
         labels = 1
         _data["cluster"] = labels
     else:
-        labels = func(_data[feature], min(n_clusters, len(_data)))
+        labels = func(_data[feature], min(n_clusters, len(_data)), **kwargs)
         _data["cluster"] = labels
 
     return _data
 
 
-def agglomerative_cluster(binned: bool, data: pd.DataFrame, **kwargs) -> pd.DataFrame:
-    kwargs.pop("method")
+CLUSTER_METHOD_FUNCS = {
+    "agglomerative": agg_cluster_other,
+    "agg": agg_cluster_other,
+    "hierarchical": agg_cluster_other,
+    "kmeans": kmeans_cluster_other,
+}
+
+
+def cluster_sites(binned: bool, data: pd.DataFrame, **kwargs) -> pd.DataFrame:
+    # kwargs.pop("method")
     if binned:
-        return agglomerative_cluster_binned(data, **kwargs)
+        return cluster_sites_binned(data, **kwargs)
     else:
-        return agglomerative_cluster_no_bin(data, **kwargs)
+        return cluster_sites_no_bin(data, **kwargs)
 
 
 def value_filter(
     data: pd.DataFrame, feature: str, max_value: float = None, min_value: float = None
 ) -> pd.DataFrame:
     df = data.copy()
     if max_value:
@@ -277,14 +334,15 @@
     mask[mask] = temp
 
     return _df.loc[mask, :]
 
 
 def calc_cluster_values(
     df: pd.DataFrame,
+    group: List[str] = None,
     sums: List[str] = MERGE["sums"],
     means: List[str] = MERGE["means"],
     weight: str = MERGE["weight"],
 ) -> pd.DataFrame:
     sums = [s for s in sums if s in df.columns]
     means = [m for m in means if m in df.columns]
     assert weight in df.columns
@@ -302,22 +360,26 @@
     for row in df.loc[1:, :].itertuples():
         profile += row.profile * row.weight
 
     profile /= df["weight"].sum()
 
     _df["profile"] = [profile]
     _df["cluster"] = df["cluster"].values[0]
+    for g in group or []:
+        _df["cluster"] = (
+            str(_df["cluster"][0]) + f"_{g}_" + str(df[snake_case_str(g)].iloc[0])
+        )
 
     return _df
 
 
 CLUSTER_FUNCS = {
-    "agglomerative": agglomerative_cluster,
-    "agg": agglomerative_cluster,
-    "hierarchical": agglomerative_cluster,
+    "agglomerative": cluster_sites,
+    "agg": cluster_sites,
+    "hierarchical": cluster_sites,
 }
 
 
 def assign_site_cluster(
     renew_data: pd.DataFrame,
     profile_path: Path,
     regions: List[str],
@@ -407,36 +469,43 @@
           - state
         cluster:
           - feature: profile
             method: agglomerative
             n_clusters: 2
     """
     data = renew_data.loc[renew_data["region"].isin(regions), :]
+    group = [snake_case_str(g) for g in group or []]
+    if group:
+        data[group] = data[group].convert_dtypes()
 
+    # Filter sites
     for filt in filter or []:
         data = value_filter(
             data=data,
             feature=snake_case_str(filt["feature"]),
             max_value=filt.get("max"),
             min_value=filt.get("min"),
         )
     if data.empty:
         data["cluster"] = []
         return data
+
+    # Only keep X MW least cost capacity
     if min_capacity:
         data = min_capacity_mw(data, min_cap=min_capacity)
     if site_map is not None:
-        site_ids = [str(site_map.loc[i]) for i in data["cpa_id"]]
+        site_ids = [site_map.loc[i] for i in data["cpa_id"]]
     else:
-        site_ids = [str(i) for i in data["cpa_id"]]
+        site_ids = [str(int(i)) for i in data["cpa_id"]]
     if profile_path is not None:
         cpa_profiles = load_site_profiles(profile_path, site_ids=list(set(site_ids)))
         profiles = [np.roll(cpa_profiles[site].values, utc_offset) for site in site_ids]
         data["profile"] = profiles
 
+    # Split sites into bins using numeric features
     bin_features = []
     for b in bin or []:
         feature = snake_case_str(b.get("feature"))
         if not feature:
             raise KeyError(
                 "One of your renewables_clusters uses the 'bin' option but doesn't include "
                 "the 'feature' argument. You must specify a numeric feature (column) to "
@@ -485,36 +554,42 @@
                 )
                 df_list.append(_df)
             data = pd.concat(df_list, ignore_index=True)
         bin_features.append(f"{feature}_bin")
 
     group_by = bin_features + ([snake_case_str(g) for g in group or []])
     prev_feature_cluster_col = None
+
+    # Using a clustering method (agglomerative or kmeans)
     for clust in cluster or []:
-        clust["feature"] = snake_case_str(clust["feature"])
+        if isinstance(clust["feature"], str):
+            clust["feature"] = snake_case_str(clust["feature"])
+        else:
+            clust["feature"] = [snake_case_str(f) for f in clust["feature"]]
         if "mw_per_cluster" in clust:
             if clust.get("n_clusters") is not None:
                 logger.warning("Overwriting 'n_clusters' based on mw_cluster_size")
             if not group_by:
                 clust["n_clusters"] = max(
                     int(data["mw"].sum() / clust["mw_per_cluster"]), 1
                 )
             else:
                 n_clusters = (
                     data.groupby(group_by)["mw"].sum() / clust["mw_per_cluster"]
                 ).astype(int)
                 clust["n_clusters"] = n_clusters.where(n_clusters > 0, 1)
+            del clust["mw_per_cluster"]
 
         if "cluster" in data.columns and prev_feature_cluster_col:
             data = data.rename(columns={"cluster": prev_feature_cluster_col})
         if group_by:
             clust["by"] = group_by
-            data = CLUSTER_FUNCS[clust["method"]](True, data, **clust)
+            data = cluster_sites(True, data, **clust)
         else:
-            data = CLUSTER_FUNCS[clust["method"]](False, data, **clust)
+            data = cluster_sites(False, data, **clust)
 
         group_by.append(f"{clust['feature']}_clust")
         prev_feature_cluster_col = f"{clust['feature']}_clust"
 
     if "cluster" not in data.columns:
         if group_by:
             i = 1
@@ -560,7 +635,89 @@
     elif "mw_per_q" in b:
         if b.get("q") is not None:
             logger.warning("Overwriting 'q' based on mw_per_q")
         b["q"] = max(int(data["mw"].sum() / b["mw_per_q"]), 1)
         del b["mw_per_q"]
 
     return b
+
+
+def modify_renewable_group(
+    df: pd.DataFrame, group_modifiers: List[Dict[str, Union[float, str, list]]] = None
+) -> pd.DataFrame:
+    """Modify values (e.g. cost) of a rewnewables cluster based on group membership.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Clustered renewable sites with averaged parameters like cost and profile. Must
+        have column "cluster".
+    group_modifiers : List[Dict[str, Union[float, str, list]]], optional
+        List of dicts. Each must have keys "group" and "group_value". Any other keys should
+         correspond to a column in `df` such as "capex_mw", "Inv_Cost_per_MW", etc. The
+         values for these keys should either be a 2-item list with an operator and a value
+         or a single numeric value.
+
+         Rows of `df` are identified by string matching f"{group}:{group_value}" on the
+         "cluster" column.
+
+         By default None
+
+    Returns
+    -------
+    pd.DataFrame
+        Modified version of input df. No change in columns.
+
+    Raises
+    ------
+    KeyError
+        One dictionary in group_modifiers is missing either "group" or "group_value" keys
+    ValueError
+        The operator list is not a 2-item list. Must be 2 items (operator and value)
+    ValueError
+        The operator is not in the valid list (["add", "mul", "truediv", "sub"])
+    """
+    allowed_operators = ["add", "mul", "truediv", "sub"]
+    for _group_mod in group_modifiers or []:
+        group_mod = _group_mod.copy()
+        missing_keys = [
+            k for k in ["group", "group_value"] if k not in group_mod.keys()
+        ]
+        if missing_keys:
+            raise KeyError(
+                f"One of your 'renewables_clusters' has a 'group_modifiers' key but is "
+                f"missing the key(s) {missing_keys}. These are required to modify values "
+                "of a renewables cluster. Add these keys or remove the 'group_modifiers' "
+                "section."
+            )
+
+        group = group_mod.pop("group")
+        group_value = group_mod.pop("group_value")
+        group_id = f"{group}_{group_value}"
+        # for group, mod in (group_modifiers or {}).items():
+        for key, op_list in group_mod.items():
+            if isinstance(op_list, float) | isinstance(op_list, int):
+                df.loc[df["cluster"].str.contains(group_id, case=False), key] = op_list
+            else:
+                if len(op_list) != 2:
+                    raise ValueError(
+                        "Either a single numeric value or a list of two values - an operator "
+                        "and a numeric value - are needed in the parameter "
+                        f"'{key}' whenever 'group_modifiers' are used in 'renewables_clusters'. "
+                        f"One of your 'group_modifiers' has {op_list} instead."
+                    )
+                op, op_value = op_list
+                if op not in allowed_operators:
+                    raise ValueError(
+                        f"One of the 'group_modifiers' in your 'renewables_clusters' with key "
+                        f"{key} has {op} as the mathmatical operator. Only {allowed_operators} "
+                        "in the format [<operator>, <value>] can be used to modify the "
+                        "properties of a renewable cluster.\n"
+                    )
+                f = operator.attrgetter(op)
+                df.loc[df["cluster"].str.contains(group_id, case=False), key] = f(
+                    operator
+                )(
+                    df.loc[df["cluster"].str.contains(group_id, case=False), key],
+                    op_value,
+                )
+    return df
```

### Comparing `PowerGenome-0.6.1a0/powergenome/cluster_method.py` & `powergenome-0.6.2/powergenome/cluster_method.py`

 * *Files identical despite different names*

### Comparing `PowerGenome-0.6.1a0/powergenome/co2_pipeline_cost.py` & `powergenome-0.6.2/powergenome/co2_pipeline_cost.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,27 +2,27 @@
 
 import logging
 from pathlib import Path
 from typing import Dict, List
 
 import pandas as pd
 
-from powergenome.params import DATA_PATHS
 from powergenome.price_adjustment import inflation_price_adjustment
-from powergenome.util import snake_case_col, snake_case_str
+from powergenome.util import snake_case_str
 
 logger = logging.getLogger(__name__)
 
 
 def merge_co2_pipeline_costs(
     df: pd.DataFrame,
     co2_data_path: Path,
     co2_pipeline_filters: List[dict],
     region_aggregations: Dict[str, List[str]] = None,
     fuel_emission_factors: Dict[str, float] = None,
+    extra_ccs_cost_tonne: float = None,
     target_usd_year: int = None,
 ) -> pd.DataFrame:
     """Merge columns with CO2 pipeline costs to a dataframe.
 
     Data come from an external file. Filters from the settings are used to select the
     data that will be merged.
 
@@ -44,33 +44,37 @@
         Path to the file with CO2 pipeline cost data
     co2_pipeline_filters : List[dict]
         Filters to apply to the CO2 cost data file
     region_aggregations : Dict[str, List[str]], optional
         Aggregations of multiple base regions to model regions, by default None
     fuel_emission_factors : Dict[str, float], optional
         CO2 emissions per unit of energy for different fuel types, by default None
+    extra_ccs_cost_tonne: float
+        An extra cost (positive or negative) assigned per tonne of CO2. Converted to
+        cost per MWh.
     target_usd_year : int, optional
         The target year for cost inflation adjustment, by default None
 
     Returns
     -------
     pd.DataFrame
         The input dataframe (one row per resource) plus columns with cost data for CO2
         pipeline constuction/operation and CO2 disposal
     """
+    logger.info("Adding CCS pipeline costs")
     co2_df = pd.read_csv(co2_data_path)
     co2_df = co2_df.loc[co2_df["parameter"] != "capacity_mw", :]
     if target_usd_year:
         for dollar_year in co2_df["dollar_year"].unique():
-            co2_df.loc[
-                (co2_df["dollar_year"] == dollar_year), "parameter_value"
-            ] = inflation_price_adjustment(
-                co2_df.loc[co2_df["dollar_year"] == dollar_year, "parameter_value"],
-                dollar_year,
-                target_usd_year,
+            co2_df.loc[(co2_df["dollar_year"] == dollar_year), "parameter_value"] = (
+                inflation_price_adjustment(
+                    co2_df.loc[co2_df["dollar_year"] == dollar_year, "parameter_value"],
+                    dollar_year,
+                    target_usd_year,
+                )
             )
     for k, v in (region_aggregations or {}).items():
         co2_df.loc[co2_df["region"].isin(v), "region"] = k
 
     # When regions are aggregated, use the lowest-cost ipm region
     co2_df = co2_df.sort_values("parameter_value").drop_duplicates(
         [
@@ -121,32 +125,52 @@
             index=["region", "technology"],
             columns="parameter",
             values="parameter_value",
         ).reset_index()
         co2_costs_wide["capture_rate"] = filt.get("capture_rate", 90)
         df_list.append(co2_costs_wide)
 
-    df_co2_costs = pd.merge(df, pd.concat(df_list), how="left")
+    full_co2_costs_wide = pd.concat(df_list)
+    full_co2_costs_wide["extra_ccs_cost_tonne"] = extra_ccs_cost_tonne or 0
+    # Split incoming df into techs with and without pipeline cost. Remove pipeline cost
+    # columns from the "with" techs to avoid duplicates, merge in co2 costs, then concat
+    # with the "without" techs
+    df = df.reset_index()
+    drop_cols = [
+        c for c in full_co2_costs_wide.columns if c not in ["region", "technology"]
+    ]
+    df_co2_techs = df.loc[df["technology"].isin(co2_resources.values()), :]
+    df_co2_techs = df_co2_techs.drop(columns=drop_cols, errors="ignore")
+    df_co2_techs = pd.merge(
+        df_co2_techs, full_co2_costs_wide, on=["region", "technology"], how="left"
+    )
+    df_non_co2_techs = df.loc[~df["technology"].isin(co2_resources.values()), :]
+
+    df_co2_costs = (
+        pd.concat([df_co2_techs, df_non_co2_techs]).set_index("index").sort_index()
+    )
 
     drop_idx = df_co2_costs.loc[
         (df_co2_costs["technology"].isin(co2_resources.values()))
         & (df_co2_costs[co2_costs_wide.columns].isna().any(axis=1))
     ].index
 
     if not drop_idx.empty:
         for tech, _df in df_co2_costs.loc[drop_idx, :].groupby("technology"):
             regs = _df["region"].to_list()
-            f"The CCS resource {tech} is being removed from regions {regs} because cost "
-            "data was not included in your CO2 pipeline cost file."
+            logger.warning(
+                f"The CCS resource {tech} is being removed from regions {regs} because cost "
+                "data was not included in your CO2 pipeline cost file."
+            )
     df_co2_costs = df_co2_costs.drop(index=drop_idx)
     df_co2_costs.loc[:, co2_costs_wide.columns] = df_co2_costs[
         co2_costs_wide.columns
     ].fillna(0)
 
-    mass_cols = [c for c in co2_costs_wide.columns if "tonne" in c]
+    mass_cols = [c for c in full_co2_costs_wide.columns if "tonne" in c]
     if mass_cols and fuel_emission_factors:
         df_co2_costs = mass_to_energy_costs(
             df_co2_costs, mass_cols, fuel_emission_factors
         )
 
     return df_co2_costs
```

### Comparing `PowerGenome-0.6.1a0/powergenome/distributed_gen.py` & `powergenome-0.6.2/powergenome/distributed_gen.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
 from typing import Dict, List
 
+import numpy as np
 import pandas as pd
 import pyarrow.parquet as pq
 
 from powergenome.load_construction import us_state_abbrev
 from powergenome.params import SETTINGS
 from powergenome.util import deep_freeze_args, snake_case_col
 
@@ -66,14 +67,15 @@
 def distributed_gen_profiles(
     profile_fn: str,
     year: int,
     scenario: str,
     regions: List[str],
     path_in: Path,
     region_aggregations: Dict[str, str] = None,
+    tz_offset: int = None,
 ) -> pd.DataFrame:
     """Build distributed generation profiles for each region
 
     Parameters
     ----------
     profile_fn : str
         Name of the data file with distributed generation profiles
@@ -86,14 +88,17 @@
         not the regions in the data file.
     path_in : Path
         Folder where the distributed generation data file and population weight file are
         found.
     region_aggregations : Dict[str, str]
         Mapping of region aggregations from base regions to model regions (where used),
         by default None
+    tz_offset: int
+        Number of hours offset from the original data, by default None. If None, the
+        original data will not be modified.
 
     Returns
     -------
     pd.DataFrame
         Wide dataframe with hourly distributed generation from each model region
 
     Raises
@@ -231,8 +236,14 @@
         )
     else:
         region_scenario_profile = scenario_profile.groupby(
             ["time_index", "region"], as_index=True
         )["region_distpv_mwh"].sum()
         region_scenario_profile = region_scenario_profile.unstack()
 
+    # Adjust for timezone
+    if tz_offset is not None:
+        for col in region_scenario_profile.columns:
+            region_scenario_profile[col] = np.roll(
+                region_scenario_profile[col], tz_offset
+            )
     return region_scenario_profile.reset_index(drop=True)
```

### Comparing `PowerGenome-0.6.1a0/powergenome/eia_opendata.py` & `powergenome-0.6.2/powergenome/eia_opendata.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,17 +5,16 @@
 import logging
 import operator
 import zipfile
 from itertools import product
 from typing import Union
 
 import pandas as pd
-import requests
 
-from powergenome.params import DATA_PATHS, SETTINGS
+from powergenome.params import DATA_PATHS
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.util import download_save, reverse_dict_of_lists
 
 logger = logging.getLogger(__name__)
 
 numeric = Union[int, float]
 
@@ -459,20 +458,20 @@
             fuel_data["region"].extend([""] * len(years))
             fuel_data["scenario"].extend(["user"] * len(years))
             fuel_data["full_fuel_name"].extend([fuel] * len(years))
 
     user_fuel_price = pd.DataFrame(fuel_data)
     if settings.get("target_usd_year"):
         for fuel, year in (settings.get("user_fuel_usd_year", {}) or {}).items():
-            user_fuel_price.loc[
-                user_fuel_price["fuel"] == fuel, "price"
-            ] = inflation_price_adjustment(
-                user_fuel_price.loc[user_fuel_price["fuel"] == fuel, "price"],
-                year,
-                settings["target_usd_year"],
+            user_fuel_price.loc[user_fuel_price["fuel"] == fuel, "price"] = (
+                inflation_price_adjustment(
+                    user_fuel_price.loc[user_fuel_price["fuel"] == fuel, "price"],
+                    year,
+                    settings["target_usd_year"],
+                )
             )
     if df is not None:
         user_fuel_price = pd.concat([df, user_fuel_price])
     return user_fuel_price
 
 
 def get_aeo_load(
```

### Comparing `PowerGenome-0.6.1a0/powergenome/external_data.py` & `powergenome-0.6.2/powergenome/external_data.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from pathlib import Path
 from typing import Any, List
 
 import numpy as np
 import pandas as pd
 
 from powergenome.price_adjustment import inflation_price_adjustment
-from powergenome.util import remove_feb_29, snake_case_col
+from powergenome.util import remove_feb_29
 
 logger = logging.getLogger(__name__)
 
 
 def make_demand_response_profiles(
     path: Path, resource_name: str, year: int, scenario: str
 ) -> pd.DataFrame:
@@ -126,17 +126,27 @@
         capacity_col: -1,
         "interconnect_annuity": 0,
         "interconnect_capex_mw": 0,
     }
     # Prepare file
     path = Path(settings["input_folder"]) / settings["capacity_limit_spur_fn"]
     df = pd.read_csv(path)
-    for col in "region", "technology":
-        if col not in df:
-            raise KeyError(f"The max capacity/spur file must have column {col}")
+    if "technology" not in df.columns:
+        raise KeyError("The max capacity/spur file must have column 'technology'")
+
+    # Let users omit the "region" column or set a value of "all"
+    if "region" not in df.columns:
+        df["region"] = "all"
+    for region in settings["model_regions"]:
+        _df = df.loc[df["region"].str.lower() == "all", :]
+        _df.loc[:, "region"] = region
+        df = df.append(_df)
+
+    df = df.loc[df["region"].str.lower() != "all", :]
+
     for key, value in defaults.items():
         df[key] = df[key].fillna(value) if key in df else value
         new_resource_df[key] = (
             new_resource_df[key].fillna(value) if key in new_resource_df else value
         )
     # Update resources
     grouped_df = df.groupby(["region", "technology"])
@@ -271,14 +281,34 @@
 
     # Update the policies. The column `copy_case_id` can be used to copy values from
     # another policy to reduce human copy/paste errors.
     if "copy_case_id" in policies.columns:
         policies = copy_case_values(policies, match_cols=["case_id", "year", "region"])
         policies = policies.drop(columns="copy_case_id", errors="ignore")
 
+    if "case_id" not in policies.columns:
+        policies["case_id"] = settings["case_id"]
+
+    warned = False
+    if policies.duplicated(subset=["case_id", "year", "region"]).any():
+        logger.warning(
+            "Your emissions policies file has repeated values of 'case_id' and 'year'. "
+            "This duplication of emission policies across multiple years may cause erors."
+        )
+        warned = True
+    policies.loc[policies["case_id"].astype(str).str.lower() == "all", "case_id"] = (
+        settings["case_id"]
+    )
+    if policies.duplicated(subset=["case_id", "year", "region"]).any() and not warned:
+        logger.warning(
+            f"After replacing values of 'all' with {settings['case_id']}, your emissions "
+            "policies file has repeated values of 'case_id' and 'year'. "
+            "This duplication of emission policies across multiple years may cause erors."
+        )
+
     policies = policies.set_index(["case_id", "year"])
 
     return policies
 
 
 def copy_case_values(df, match_cols):
     """Copy values for one case to others in an external data file. Must have column
@@ -551,20 +581,20 @@
     unused_lines = []
     for row in user_costs.itertuples():
         line_row = tx_df.loc[(tx_df[row.zone_1] != 0) & (tx_df[row.zone_2] != 0), :]
         assert not len(line_row) > 1
 
         if line_row.empty:
             unused_lines.append(row)
-        tx_df.loc[
-            line_row.index, "Line_Reinforcement_Cost_per_MWyr"
-        ] = row.total_interconnect_annuity_mw
-        tx_df.loc[
-            line_row.index, "Line_Reinforcement_Cost_per_MW"
-        ] = row.total_interconnect_cost_mw
+        tx_df.loc[line_row.index, "Line_Reinforcement_Cost_per_MWyr"] = (
+            row.total_interconnect_annuity_mw
+        )
+        tx_df.loc[line_row.index, "Line_Reinforcement_Cost_per_MW"] = (
+            row.total_interconnect_cost_mw
+        )
         tx_df.loc[line_row.index, "Line_Loss_Percentage"] = row.total_line_loss_frac
 
     unused_line_df = pd.DataFrame(unused_lines)
     unused_line_df = unused_line_df.rename(
         columns={
             "total_interconnect_annuity_mw": "Line_Reinforcement_Cost_per_MWyr",
             "total_interconnect_cost_mw": "Line_Reinforcement_Cost_per_MW",
@@ -573,17 +603,17 @@
     )
 
     zone_cols = [c for c in tx_df.columns if c[0] == "z"]
     unused_line_df[zone_cols] = 0
     for idx, row in unused_line_df.iterrows():
         unused_line_df.loc[idx, row["zone_1"]] = 1
         unused_line_df.loc[idx, row["zone_2"]] = -1
-        unused_line_df.loc[
-            idx, "transmission_path_name"
-        ] = f"{row.start_region}_to_{row.dest_region}"
+        unused_line_df.loc[idx, "transmission_path_name"] = (
+            f"{row.start_region}_to_{row.dest_region}"
+        )
 
     cols = [c for c in tx_df.columns if c in unused_line_df.columns]
     tx_df = pd.concat([tx_df, unused_line_df[cols]], ignore_index=True)
     tx_df["Network_Lines"] = range(1, len(tx_df) + 1)
     tx_df["Line_Max_Flow_MW"] = tx_df["Line_Max_Flow_MW"].fillna(0)
     tx_df["Line_Min_Flow_MW"] = tx_df["Line_Max_Flow_MW"].fillna(0)
```

### Comparing `PowerGenome-0.6.1a0/powergenome/extract_pudl_data.py` & `powergenome-0.6.2/powergenome/extract_pudl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,15 @@
         fuels["fuel_indices"] = range(1, len(fuels) + 1)
         fuels = remove_fuel_scenario_name(fuels, settings)
 
     logger.info(f"Write GenX input files to {args.results_folder}")
     if args.gens:
         gen_clusters.to_csv(
             out_folder / f"generator_clusters_{args.results_folder}.csv",
-            index=False
+            index=False,
             # float_format="%.3f",
         )
         # if args.all_units is True:
         # gc.all_units.to_csv(out_folder / f"all_units_{args.results_folder}.csv")
 
     if args.load:
         load.astype(int).to_csv(out_folder / f"load_curves_{args.results_folder}.csv")
```

### Comparing `PowerGenome-0.6.1a0/powergenome/generators.py` & `powergenome-0.6.2/powergenome/generators.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,62 +1,62 @@
 import collections
 import logging
+import os
 import re
 from numbers import Number
 from pathlib import Path
 from typing import Dict, List, Union
 from zipfile import BadZipFile
 
+os.environ["USE_PYGEOS"] = "0"
+
 import geopandas as gpd
 import numpy as np
 import pandas as pd
 import pudl
 import requests
 import sqlalchemy
 from bs4 import BeautifulSoup
 from flatten_dict import flatten
 from scipy.stats import iqr
 from sklearn import cluster, preprocessing
 from xlrd import XLRDError
 
-from powergenome.cluster_method import (
-    cluster_by_owner,
-    cluster_kmeans,
-    weighted_ownership_by_unit,
-)
+from powergenome.cluster_method import cluster_by_owner
 from powergenome.co2_pipeline_cost import merge_co2_pipeline_costs
 from powergenome.eia_opendata import fetch_fuel_prices, modify_fuel_prices
 from powergenome.external_data import (
     add_resource_max_cap_spur,
     demand_response_resource_capacity,
     make_demand_response_profiles,
 )
-from powergenome.GenX import rename_gen_cols
+from powergenome.financials import investment_cost_calculator
+from powergenome.GenX import cap_retire_within_period, rename_gen_cols
 from powergenome.load_profiles import make_distributed_gen_profiles
 from powergenome.nrelatb import (
     atb_fixed_var_om_existing,
     atb_new_generators,
     fetch_atb_costs,
     fetch_atb_heat_rates,
     fetch_atb_offshore_spur_costs,
-    investment_cost_calculator,
 )
-from powergenome.params import DATA_PATHS, IPM_GEOJSON_PATH, build_resource_clusters
+from powergenome.params import DATA_PATHS, build_resource_clusters
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.resource_clusters import map_eia_technology
 from powergenome.util import (
     download_save,
     find_region_col,
     load_ipm_shapefile,
     map_agg_region_names,
     regions_to_keep,
     remove_leading_zero,
     reverse_dict_of_lists,
     snake_case_col,
     snake_case_str,
+    sort_nested_dict,
 )
 
 logger = logging.getLogger(__name__)
 
 
 planned_col_map = {
     "Entity ID": "utility_id_eia",
@@ -238,35 +238,35 @@
         etc.
 
     Returns
     -------
     DataFrame
         Modified df with new column "Start_Cost_per_MW"
     """
-    logger.info("Adding non-fuel startup costs")
+    logger.debug("Adding non-fuel startup costs")
     target_usd_year = settings.get("target_usd_year")
 
     vom_costs = settings.get("startup_vom_costs_mw", {})
     vom_usd_year = settings.get("startup_vom_costs_usd_year")
 
     if target_usd_year and vom_usd_year:
-        logger.info(
+        logger.debug(
             f"Changing non-fuel VOM costs from {vom_usd_year} to " f"{target_usd_year}"
         )
         for key, cost in vom_costs.items():
             vom_costs[key] = inflation_price_adjustment(
                 price=cost, base_year=vom_usd_year, target_year=target_usd_year
             )
 
     startup_type = settings.get("startup_costs_type")
     startup_costs = settings.get(startup_type, {})
     startup_costs_usd_year = settings.get("startup_costs_per_cold_start_usd_year")
 
     if target_usd_year and startup_costs_usd_year:
-        logger.info(
+        logger.debug(
             f"Changing non-fuel startup costs from {vom_usd_year} to {target_usd_year}"
         )
         for key, cost in startup_costs.items():
             startup_costs[key] = inflation_price_adjustment(
                 price=cost,
                 base_year=startup_costs_usd_year,
                 target_year=target_usd_year,
@@ -281,17 +281,17 @@
         df.loc[
             df["technology"].str.contains(existing_tech, case=False),
             "Start_Cost_per_MW",
         ] = total_startup_costs
 
     for new_tech, cost_tech in settings.get("new_build_startup_costs", {}).items():
         total_startup_costs = vom_costs[cost_tech] + startup_costs[cost_tech]
-        df.loc[
-            df["technology"].str.contains(new_tech), "Start_Cost_per_MW"
-        ] = total_startup_costs
+        df.loc[df["technology"].str.contains(new_tech), "Start_Cost_per_MW"] = (
+            total_startup_costs
+        )
     df.loc[:, "Start_Cost_per_MW"] = df.loc[:, "Start_Cost_per_MW"]
 
     # df.loc[df["technology"].str.contains("Nuclear"), "Start_Cost_per_MW"] = "FILL VALUE"
 
     return df
 
 
@@ -367,15 +367,17 @@
         gens_860["technology_description"] == "Conventional Hydroelectric"
     ].merge(plant_entity[["plant_id_eia", "latitude", "longitude"]], on="plant_id_eia")
 
     no_lat_lon = model_hydro.loc[
         (model_hydro["latitude"].isnull()) | (model_hydro["longitude"].isnull()), :
     ]
     if not no_lat_lon.empty:
-        print(no_lat_lon["summer_capacity_mw"].sum(), " MW without lat/lon")
+        logger.debug(
+            f"{no_lat_lon['summer_capacity_mw'].sum().round(1)}, MW without lat/lon"
+        )
     model_hydro = model_hydro.dropna(subset=["latitude", "longitude"])
 
     # Convert the lon/lat values to geo points. Need to add an initial CRS and then
     # change it to align with the IPM regions
     model_hydro_gdf = gpd.GeoDataFrame(
         model_hydro,
         geometry=gpd.points_from_xy(model_hydro.longitude, model_hydro.latitude),
@@ -450,15 +452,15 @@
         settings["model_regions"], settings.get("region_aggregations")
     )
 
     # Create a new column "model_region" with labels that we're using for aggregated regions
 
     model_region_map_df = region_map_df.loc[
         region_map_df.region.isin(keep_regions), :
-    ].drop(columns="id")
+    ].drop(columns="id", errors="ignore")
 
     model_region_map_df = map_agg_region_names(
         df=model_region_map_df,
         region_agg_map=region_agg_map,
         original_col_name="region",
         new_col_name="model_region",
     )
@@ -526,20 +528,20 @@
             ~df["planned_retirement_date"].isnull(), "planned_retirement_date"
         ].dt.year
     except KeyError:
         pass
 
     # Add additonal retirements from settings file
     if settings.get("additional_retirements") and add_additional_retirements:
-        logger.info("Changing retirement dates based on settings file")
+        logger.debug("Changing retirement dates based on settings file")
         model_year = settings["model_year"]
         start_ret_cap = df.loc[
             df["retirement_year"] <= model_year, settings["capacity_col"]
         ].sum()
-        logger.info(f"Starting retirement capacity is {start_ret_cap} MW")
+        logger.debug(f"Starting retirement capacity is {start_ret_cap} MW")
         i = 0
         ret_cap = 0
         for record in settings["additional_retirements"]:
             plant_id, gen_id, ret_year = record
             # gen ids are strings, not integers
             gen_id = str(gen_id)
 
@@ -553,30 +555,30 @@
                 (df["plant_id_eia"] == plant_id) & (df["generator_id"] == gen_id),
                 settings["capacity_col"],
             ].sum()
 
         end_ret_cap = df.loc[
             df["retirement_year"] <= model_year, settings["capacity_col"]
         ].sum()
-        logger.info(f"Ending retirement capacity is {end_ret_cap} MW")
+        logger.debug(f"Ending retirement capacity is {end_ret_cap} MW")
         if not end_ret_cap > start_ret_cap:
             logger.debug(
                 "Adding retirements from settings didn't change the retiring capacity."
             )
         if end_ret_cap - start_ret_cap != ret_cap:
             logger.debug(
                 f"Retirement diff is {end_ret_cap - start_ret_cap}, adding retirements "
                 f"yields {ret_cap} MW"
             )
-        logger.info(
+        logger.debug(
             f"The retirement year for {i} plants, totaling {ret_cap} MW, was changed "
             "based on settings file parameters"
         )
     else:
-        logger.info("No retirement dates changed based on the settings file")
+        logger.debug("No retirement dates changed based on the settings file")
 
     end_len = len(df)
 
     assert start_len == end_len
 
     return df
 
@@ -612,15 +614,15 @@
         x
         for x in settings["model_regions"] + list(region_agg_map)
         if x in settings["small_hydro_regions"]
     ]
     start_len = len(df)
     size_cap = settings["small_hydro_mw"]
     cap_col = settings.get("capacity_col")
-    if not cap_col in df:
+    if cap_col not in df:
         cap_col = "capacity_mw"
 
     start_hydro_capacity = df.query(
         "technology_description=='Conventional Hydroelectric'"
     )[cap_col].sum()
 
     plant_capacity = (
@@ -833,21 +835,25 @@
             ]
 
     merged_capacity = gens_860_model.groupby("technology_description")[
         settings["capacity_col"]
     ].sum()
     if not np.allclose(initial_capacity.sum(), merged_capacity.sum()):
         for i_idx, i_row in initial_capacity.iteritems():
+            if abs(i_row - merged_capacity[i_idx]) / i_row > 0.05:
+                logger.info(
+                    "When adding plant entity/boiler info to generators and filling missing"
+                    " seasonal capacity values, "
+                    f"{i_idx} changed capacity from {i_row} to {merged_capacity[i_idx]}"
+                )
             if not np.allclose(i_row, merged_capacity[i_idx]):
-                logger.warning(
-                    "********************************\n"
+                logger.debug(
                     "When adding plant entity/boiler info to generators and filling missing"
-                    " seasonal capacity values, technology"
+                    " seasonal capacity values, "
                     f"{i_idx} changed capacity from {i_row} to {merged_capacity[i_idx]}"
-                    "\n********************************"
                 )
 
     return gens_860_model
 
 
 def create_plant_gen_id(df):
     """Combine the plant id and generator id to form a unique combination
@@ -927,14 +933,75 @@
 
     if not retired.empty:
         assert len(df) == len(retired) + len(not_retired_df)
 
     return not_retired_df.reset_index(drop=True)
 
 
+def update_planned_retirement_date_860m(
+    df: pd.DataFrame, operating_860m: pd.DataFrame
+) -> pd.DataFrame:
+    """Update the planned retirement date in the main dataframe using the planned
+    retirement year column from 860m existing generators.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        Main dataframe of generators from EIA 860. Must have columns "plant_id_eia",
+        "generator_id", and "planned_retirement_date", which should be in a datatime format.
+    operating_860m : pd.DataFrame
+        Dataframe of operating generators from EIA 860m. Must have columns "plant_id_eia",
+        "generator_id", and "planned_retirement_year"
+
+    Returns
+    -------
+    pd.DataFrame
+        Modified version of "df" dataframe, with updated values in column
+        "planned_retirement_date" based on EIA-860m.
+    """
+    if "planned_retirement_date" not in df.columns:
+        logger.warning(
+            "The main generators dataframe from EIA 860 does not have a column "
+            "'planned_retirement_date'. If this column is missing all retirement dates "
+            "will be based on plant age."
+        )
+        return df
+    if "planned_retirement_year" not in operating_860m.columns:
+        logger.warning(
+            "The EIA-860m existing dataframe does not have a column 'planned_retirement_year'."
+            "Check the 860m file to see if it has been renamed. No values from the original "
+            "860 data will be changed."
+        )
+        return df
+    if df.empty or operating_860m.empty:
+        return df
+    _df = df.set_index(["plant_id_eia", "generator_id"])
+    _operating_860m = operating_860m.set_index(["plant_id_eia", "generator_id"])
+    _operating_860m["planned_retirement_date_860m"] = pd.to_datetime(
+        _operating_860m["planned_retirement_year"], format="%Y"
+    )
+    update_df = pd.merge(
+        _df,
+        _operating_860m[["planned_retirement_date_860m"]],
+        how="inner",
+        left_index=True,
+        right_index=True,
+    )
+    mask = update_df.loc[
+        update_df["planned_retirement_date"].dt.year.fillna(9999)
+        != update_df["planned_retirement_date_860m"].dt.year.fillna(9999),
+        :,
+    ].index
+    _df.loc[mask, "planned_retirement_date"] = update_df.loc[
+        mask, "planned_retirement_date_860m"
+    ]
+
+    return _df.reset_index()
+
+
 def remove_future_retirements_860m(df, retired_860m):
     """Remove generators that 860m shows as having been retired
 
     Parameters
     ----------
     df : dataframe
         All of the EIA 860 generators
@@ -1307,15 +1374,15 @@
     grouped_units = grouped_units.replace([np.inf, -np.inf], np.nan)
     grouped_units = grouped_units.fillna(grouped_units.mean())
 
     return grouped_units
 
 
 def calc_unit_cluster_values(
-    df: pd.DataFrame, capacity_col: str, technology: str = None
+    df: pd.DataFrame, capacity_col: str, technology: str = None, clustered: bool = True
 ):
     """
     Calculate the total capacity, minimum load, weighted heat rate, and number of
     units/generators in a technology cluster.
 
     Parameters
     ----------
@@ -1323,34 +1390,46 @@
         A dataframe with units/generators of a single technology. One column should be
         'cluster', to label units as belonging to a specific cluster grouping.
     capacity_col: str
         Name of the column with capacity values (e.g. capacity_mw, summer_capacity_mw or
         winter_capacity_mw).
     technology : str, optional
         Name of the generating technology, by default None
+    clustered : bool, optional
+        If units are clustered or only a single unit is being passed, by default True
 
     Returns
     -------
     dataframe
         Aggragate values for generators in a technology cluster
     """
     # if not clustering units no need to calulate cluster average values
-    if df["cluster"].max() == len(df):
+    if len(df) == 1:
+        clustered = False
+    elif df["cluster"].nunique() == len(df):
+        clustered = False
+
+    if not clustered:
         df["Min_Power"] = df["minimum_load_mw"] / df[capacity_col]
         df["num_units"] = 1
         if technology:
             df["technology"] = technology
 
-        return df.reset_index()
+        return df.reset_index().replace(np.inf, 0)
 
     # Define a function to compute the weighted mean.
     # The issue here is that the df name needs to be used in the function.
     # So this will need to be within a function that takes df as an input
     def wm(x):
-        return np.average(x, weights=df.loc[x.index, capacity_col])
+        try:
+            return np.average(
+                x, weights=df.loc[x.index, capacity_col].replace(np.nan, 0)
+            )
+        except ZeroDivisionError:
+            return x.mean()
 
     if df["heat_rate_mmbtu_mwh"].isnull().values.any():
         # mean =
         # df["heat_rate_mmbtu_mwh"] = df["heat_rate_mmbtu_mwh"].fillna(
         #     df["heat_rate_mmbtu_mwh"].median()
         # )
         start_cap = df[capacity_col].sum()
@@ -1381,71 +1460,118 @@
     )
     df_values["fixed_o_m_mw_std"] = df.groupby("cluster").agg(
         {"Fixed_OM_Cost_per_MWyr": "std"}
     )
 
     df_values["Min_Power"] = df_values["minimum_load_mw"] / df_values[capacity_col]
 
-    df_values["num_units"] = df.groupby("cluster")["cluster"].count()
+    df_values["num_units"] = (
+        df.dropna(subset=capacity_col).groupby("cluster")["cluster"].count()
+    )
 
     if technology:
         df_values["technology"] = technology
 
     return df_values
 
 
-def add_genx_model_tags(df, settings):
-    """
+def add_resource_tags(
+    df: pd.DataFrame,
+    model_tag_values: Dict[str, Dict[str, int]],
+    regional_tag_values: Dict[str, Dict[str, Dict[str, int]]] = None,
+    model_tag_names: List[str] = None,
+    default_model_tag: Union[int, float, str] = 0,
+) -> pd.DataFrame:
+    """Add columns to the dataframe of resources and assign values based on technology
+    names. Can be boolean-type integers, floats, or strings. Different values can be
+    assigned by region.
+
     Each generator type needs to have certain tags for use by the GenX model. Each tag
     is a column, e.g. THERM for thermal generators. These columns and tag values are
-    defined in the settings file and applied here. Tags are (usually?) boolean 0/1
-    values.
+    defined in the settings file and applied here.
+
+    Keys representing technology names are sorted by length so that shorter names are
+    applied first. This prevents short or generic names like "nuclear" from overriding
+    more specific names like "nuclear_nuclear".
 
     Parameters
     ----------
-    df : dataframe
-        Clusters of generators. The index should have a column 'technology', which
-        is used to map tag values.
-    settings : dict
-        User-defined settings loaded from a YAML file.
+    df : pd.DataFrame
+        Each row represents one resource. Should have the column "technology",
+        and the column "region" if `regional_tag_values` is used.
+    model_tag_values : Dict[str, Dict[str, int]]
+        Mapping of values to technology names that will be assigned to a new column using
+        the key as the column name.
+    regional_tag_values : Dict[str, Dict[str, Dict[str, int]]]
+        Mapping of values to technology names within a given region that will be assigned
+        to a new column using the key as the column name.
+    model_tag_names : List[str], optional
+        List of tag names to either assign specific values or the default value, by default
+        None. Only necessary if a column is required but not specified within
+        `model_tag_values` or `regional_tag_values`.
+    default_model_tag : Union[int, float, str], optional
+        The default value used to fill within a column before assigning specific values to
+        each technology, by default 0
 
     Returns
     -------
-    dataframe
-        The original generator cluster results with new columns for each model tag.
+    pd.DataFrame
+        Modified version of the input df with new columns from the dictionary keys.
     """
+    if "technology" not in df.columns:
+        raise KeyError(
+            "The column 'techology' is required when adding model tag values."
+        )
+    if regional_tag_values is not None and "region" not in df.columns:
+        raise KeyError(
+            "When assigning regional model tags, the column 'region' is required."
+        )
+    _df = df.copy()
+    if model_tag_names is None:
+        model_tag_names = []
     ignored = r"_"
-    technology = df["technology"].str.replace(ignored, "")
-    # Create a new dataframe with the same index
-    default = settings.get("default_model_tag", 0)
-    for tag_col in settings.get("model_tag_names", []):
-        df[tag_col] = default
-        if tag_col not in settings.get("generator_columns", []) and isinstance(
-            settings.get("generator_columns"), list
-        ):
-            settings["generator_columns"].append(tag_col)
+    technology = _df["technology"].str.replace(ignored, "")
+
+    global_keys = list((model_tag_values or {}).keys())
+    regional_keys = []
+    for region, regional_tags in (regional_tag_values or {}).items():
+        regional_keys.extend(list(regional_tags.keys()))
 
+    # global_keys = list(set(global_keys + regional_keys))
+    # Create a new dataframe with the same index
+    tags_no_value = set(model_tag_names) - set(global_keys + regional_keys)
+    if tags_no_value:
+        logger.warning(
+            f"The model resource tags {tags_no_value} are listed in the settings parameter "
+            "'model_tags_name' but are not assigned values for any resources"
+        )
+    for tag_col in set(model_tag_names + global_keys + regional_keys):
+        _df.loc[:, tag_col] = default_model_tag
+    for tag_col in global_keys:
         try:
-            for tech, tag_value in settings["model_tag_values"][tag_col].items():
+            for tech, tag_value in sorted(
+                model_tag_values[tag_col].items(),
+                key=lambda item: len(str(item[0])),
+            ):
                 tech = re.sub(ignored, "", tech)
                 mask = technology.str.contains(rf"^{tech}", case=False)
-                df.loc[mask, tag_col] = tag_value
+                _df.loc[mask, tag_col] = tag_value
         except (KeyError, AttributeError) as e:
             logger.warning(f"No model tag values found for {tag_col} ({e})")
 
     # Change tags with specific regional values for a technology
-    flat_regional_tags = flatten(settings.get("regional_tag_values", {}) or {})
+    flat_regional_tags = flatten(sort_nested_dict(regional_tag_values or {}))
 
     for tag_tuple, tag_value in flat_regional_tags.items():
         region, tag_col, tech = tag_tuple
         tech = re.sub(ignored, "", tech)
         mask = technology.str.contains(rf"^{tech}", case=False)
-        df.loc[(df["region"] == region) & mask, tag_col] = tag_value
+        _df.loc[(_df["region"] == region) & mask, tag_col] = tag_value
 
-    return df
+    return _df
 
 
 def download_860m(settings: dict) -> pd.ExcelFile:
     """Load the entire 860m file into memory as an ExcelFile object.
 
     Parameters
     ----------
@@ -1456,15 +1582,18 @@
     Returns
     -------
     pd.ExcelFile
         The ExcelFile object with all sheets from 860m.
     """
     fn = settings.get("eia_860m_fn")
     if not fn:
-        logger.info("Trying to determine the most recent EIA860m file...")
+        logger.info(
+            "Trying to determine the most recent EIA860m file. For reproducible results "
+            "use the settings parameter 'eia_860m_fn'."
+        )
         fn = find_newest_860m()
 
     engine = None
     ext = fn.split(".")[-1]
     if ext == "xlsx":
         engine = "openpyxl"
     elif ext == "xls":
@@ -1472,23 +1601,25 @@
 
     # Only the most recent file will not have archive in the url
     url = f"https://www.eia.gov/electricity/data/eia860m/xls/{fn}"
     archive_url = f"https://www.eia.gov/electricity/data/eia860m/archive/xls/{fn}"
 
     local_file = DATA_PATHS["eia_860m"] / fn
     if local_file.exists():
-        logger.info(f"Reading a local copy of the EIA860m file {fn}")
+        logger.debug(f"Reading a local copy of the EIA860m file {fn}")
         eia_860m = pd.ExcelFile(local_file)
     else:
-        logger.info(f"Downloading the EIA860m file {fn}")
+        logger.debug(f"Downloading the EIA860m file {fn}")
         try:
             download_save(url, local_file)
             eia_860m = pd.ExcelFile(local_file, engine=engine)
-        except (XLRDError, ValueError, BadZipFile):
-            logger.warning("A more recent version of EIA-860m is available")
+        except (XLRDError, ValueError, BadZipFile) as e:
+            logger.warning(
+                f"There was an error when downloading the EIA-860m file. Trying again {e}"
+            )
             download_save(archive_url, local_file)
             eia_860m = pd.ExcelFile(local_file, engine=engine)
         # write the file to disk
 
     return eia_860m
 
 
@@ -1561,18 +1692,14 @@
     df["plant_id_eia"] = df["plant_id_eia"].astype("Int64")
 
     if sheet_name in ["Operating", "Planned"]:
         df.loc[:, "operational_status_code"] = df.loc[:, "operational_status"].map(
             op_status_map
         )
 
-    if sheet_name == "Planned":
-        df = df.loc[
-            df["operational_status_code"].isin(settings["proposed_status_included"]), :
-        ]
     df.columns = snake_case_col(df.columns)
 
     return df
 
 
 def load_860m(settings: dict) -> Dict[str, pd.DataFrame]:
     """Load the planned, canceled, and retired sheets from an EIA 860m file.
@@ -1603,27 +1730,75 @@
 
     data_dict = {}
     eia_860m_excelfile = None
     for name, sheet in sheet_map.items():
         pkl_path = DATA_PATHS["eia_860m"] / f"{fn_name}_{name}.pkl"
         if pkl_path.exists():
             data_dict[name] = pd.read_pickle(pkl_path)
+            if sheet == "Planned":
+                data_dict[name] = filter_op_status_codes(
+                    data_dict[name], settings.get("proposed_status_included")
+                )
             data_dict[name]["plant_id_eia"] = data_dict[name]["plant_id_eia"].astype(
                 "Int64"
             )
             data_dict[name].columns = snake_case_col(data_dict[name].columns)
         else:
             if eia_860m_excelfile is None:
                 eia_860m_excelfile = download_860m(settings)
             data_dict[name] = clean_860m_sheet(eia_860m_excelfile, sheet, settings)
+            if sheet == "planned":
+                data_dict[name] = filter_op_status_codes(
+                    data_dict[name], settings.get("proposed_status_included")
+                )
             data_dict[name].to_pickle(pkl_path)
 
     return data_dict
 
 
+def filter_op_status_codes(
+    df: pd.DataFrame, proposed_status_included: Union[List[str], None]
+) -> pd.DataFrame:
+    """Filter a planned 860m sheet to only include desired operational status codes.
+    Used to filter out projects that are still early in the pipeline and might not be built.
+
+    If proposed_status_included is None, included all proposed plants. Will warn user
+    in logs if invalid codes are included.
+
+    Parameters
+    ----------
+    df : pd.DataFrame
+        EIA860m planned generators. Includes the column "operational_status_code".
+    proposed_status_included : Union[List[str], None]
+        List of status codes for proposed generators that should be included in the model.
+        Examples include "V" (Under construction, more than 50 percent complete),
+        "TS" (Construction complete, but not yet in commercial operation), "U", (Under
+        construction, less than or equal to 50 percent complete), etc.
+
+    Returns
+    -------
+    pd.DataFrame
+        Filtered input dataframe.
+    """
+    if proposed_status_included is None:
+        return df
+
+    valid_status_codes = df["operational_status_code"].unique()
+    invalid_user_codes = [
+        c for c in proposed_status_included if c not in valid_status_codes
+    ]
+    if invalid_user_codes:
+        logger.warning(
+            f"The operational status codes {invalid_user_codes} included in the "
+            "settings parameter 'proposed_status_included' do not appear in EIA 860m.\n"
+            f"Valid status codes from 'operational_status_code' are {valid_status_codes}"
+        )
+    return df.loc[df["operational_status_code"].isin(proposed_status_included), :]
+
+
 def label_gen_region(
     df: pd.DataFrame, settings: dict, model_regions_gdf: gpd.GeoDataFrame
 ) -> pd.DataFrame:
     """Label the region that generators in a dataframe belong to based on their
     geographic location. This is done via geospaital join and may not always be accurate
     based on actual utility connections.
 
@@ -1655,15 +1830,14 @@
             f"\n{no_lat_lon['balancing_authority_code'].tolist()}"
         )
 
     df = df.dropna(subset=["latitude", "longitude"])
 
     # Convert the lon/lat values to geo points. Need to add an initial CRS and then
     # change it to align with the IPM regions
-    print("Creating gdf")
     gdf = gpd.GeoDataFrame(
         df.copy(),
         geometry=gpd.points_from_xy(df.longitude.copy(), df.latitude.copy()),
         crs="EPSG:4326",
     )
     if gdf.crs != model_regions_gdf.crs:
         gdf = gdf.to_crs(model_regions_gdf.crs)
@@ -1760,28 +1934,30 @@
             .to_numpy()
         )
         plant_capacity = new_operating.loc[
             new_operating["technology_description"].isnull(),
             settings.get("capacity_col", "capacity_mw"),
         ].sum()
 
-        logger.warning(
+        logger.debug(
             f"The EIA860 file has {len(plant_ids)} operating generator(s) without a technology "
             f"description. The plant IDs are {plant_ids}, and they have a combined "
             f"capcity of {plant_capacity} MW."
         )
 
     if settings.get("group_technologies"):
         new_operating = group_technologies(
             new_operating,
             settings["group_technologies"],
             settings.get("tech_groups", {}) or {},
             settings.get("regional_no_grouping", {}) or {},
         )
-        print(new_operating["technology_description"].unique().tolist())
+        logger.debug(
+            f"Existing technology groups are {new_operating['technology_description'].unique().tolist()}"
+        )
 
     keep_cols = [
         "model_region",
         "technology_description",
         "generator_id",
         settings.get("capacity_col", "capacity_mw"),
         "capacity_mwh",
@@ -1844,14 +2020,15 @@
     #     crs="EPSG:4326",
     # )
     # if planned_gdf.crs != model_regions_gdf.crs:
     #     planned_gdf = planned_gdf.to_crs(model_regions_gdf.crs)
 
     # planned_gdf = gpd.sjoin(model_regions_gdf.drop(columns="IPM_Region"), planned_gdf)
     _planned = planned.copy()
+    _planned["generator_id"] = _planned["generator_id"].fillna("no_gen_id")
     _planned["generator_id"] = _planned["generator_id"].apply(remove_leading_zero)
     planned_gdf = label_gen_region(_planned, settings, model_regions_gdf)
     planned_gdf = planned_gdf.drop_duplicates(subset=["plant_id_eia", "generator_id"])
 
     # Add planned additions from the settings file
     additional_planned = settings.get("additional_planned") or []
     for record in additional_planned:
@@ -1860,15 +2037,15 @@
             (planned["plant_id_eia"] == plant_id) & (planned["generator_id"] == gen_id),
             :,
         ]
         plant_record["model_region"] = model_region
 
         planned_gdf = planned_gdf.append(plant_record, sort=False)
 
-    logger.info(
+    logger.debug(
         f"{len(additional_planned)} generators were added to the planned list based on settings"
     )
 
     planned_gdf.loc[:, "heat_rate_mmbtu_mwh"] = planned_gdf.loc[
         :, "technology_description"
     ].map(settings["proposed_gen_heat_rates"])
 
@@ -1899,15 +2076,15 @@
             .index.get_level_values("plant_id_eia")
             .to_numpy()
         )
         plant_capacity = planned_gdf.loc[
             planned_gdf["technology_description"].isnull(), settings["capacity_col"]
         ].sum()
 
-        logger.warning(
+        logger.debug(
             f"The EIA860 file has {len(plant_ids)} proposed generator(s) without a technology "
             f"description. The plant IDs are {plant_ids}, and they have a combined "
             f"capcity of {plant_capacity} MW."
         )
 
     # Add a retirement year based on the planned start year
     label_retirement_year(
@@ -1920,15 +2097,17 @@
     if settings.get("group_technologies"):
         planned_gdf = group_technologies(
             planned_gdf,
             settings["group_technologies"],
             settings.get("tech_groups", {}) or {},
             settings.get("regional_no_grouping", {}) or {},
         )
-        print(planned_gdf["technology_description"].unique().tolist())
+        logger.debug(
+            f"Grouped planned technologies are {planned_gdf['technology_description'].unique().tolist()}"
+        )
 
     keep_cols = [
         "model_region",
         "technology_description",
         "generator_id",
         settings["capacity_col"],
         "minimum_load_mw",
@@ -1963,15 +2142,17 @@
         The dictionary of settings with a dictionary of region aggregations
 
     Returns
     -------
     DataFrame
         A dataframe with the capacity factor of every selected technology
     """
-    data_years = [str(y) for y in settings["eia_data_years"]]
+    data_years = settings[
+        "eia_data_years"
+    ].copy()  # [str(y) for y in settings["eia_data_years"]]
     data_years.extend(settings.get("capacity_factor_default_year_filter", []))
 
     cap_col = settings["capacity_col"]
 
     # Include standby (SB) generators since they are in our capacity totals
     sql = f"""
         SELECT
@@ -1993,15 +2174,18 @@
             G.technology_description,
             G.fuel_type_code_pudl,
             G.generator_id
         ORDER by G.plant_id_eia, G.report_date
     """
 
     plant_gen_tech_cap = pd.read_sql_query(
-        sql, pudl_engine, params=data_years, parse_dates=["report_date"]
+        sql,
+        pudl_engine,
+        params=[str(y) for y in data_years],
+        parse_dates=["report_date"],
     )
     plant_gen_tech_cap = plant_gen_tech_cap.loc[
         plant_gen_tech_cap["plant_id_eia"].isin(plant_region_map["plant_id_eia"]), :
     ]
 
     plant_gen_tech_cap = fill_missing_tech_descriptions(plant_gen_tech_cap)
     plant_tech_cap = group_generators_at_plant(
@@ -2411,15 +2595,18 @@
                 f"{SETTING}.{ttype}.capex_mw_mile should be numeric or a dictionary"
                 f" of <region>: <capex>, not {params['capex_mw_mile']}"
             )
         resource_df[f"{ttype}_capex"] = (
             capex_mw_mile.fillna(0) * resource_df[f"{ttype}_miles"]
         )
         resource_df[f"{ttype}_inv_mwyr"] = investment_cost_calculator(
-            resource_df[f"{ttype}_capex"], params["wacc"], params["investment_years"]
+            resource_df[f"{ttype}_capex"],
+            params["wacc"],
+            params["investment_years"],
+            settings.get("interest_compound_method", "discrete"),
         )
     return resource_df
 
 
 def add_transmission_inv_cost(
     resource_df: pd.DataFrame, settings: dict
 ) -> pd.DataFrame:
@@ -2556,27 +2743,28 @@
             (df[tech_col].isin(storage_techs)) & ~(df[energy_col] > 0),
             tech_col,
         ].unique()
     )
     missing_techs = [t for t in partial_storage if t not in energy_storage_duration]
     if missing_techs:
         logger.warning(
-            "\n\n**************************\n"
             f"The storage technology(ies) {missing_techs} have some existing generators "
             "with energy capacity (MWh) values and some where the energy capacity is "
             "missing. You have not included these technologies in the settings parameter "
             "'energy_storage_duration', which is used to fill missing energy capacity "
             "data.\n\nNOTE: This is not a comprehensive list of technologies that *should* "
             "be included in 'energy_storage_duration'. Technologies without any existing "
-            "energy capacity data might also be missing.\n"
-            "**************************\n"
+            "energy capacity data might also be missing."
         )
     for tech, val in energy_storage_duration.items():
         if isinstance(val, dict):
             tech_regions = val.keys()
+            df.loc[df[tech_col].isna(), "technology_description"] = (
+                "missing_tech_description"
+            )
             model_tech_regions = df.loc[
                 snake_case_col(df[tech_col]).str.contains(snake_case_str(tech)),
                 region_col,
             ].to_list()
             if not all(r in tech_regions for r in model_tech_regions):
                 missing_regions = [
                     r for r in model_tech_regions if r not in tech_regions
@@ -2759,14 +2947,16 @@
         pg_engine,
         settings,
         current_gens=True,
         supplement_with_860m=True,
         sort_gens=False,
         plant_region_map_table="plant_region_map_epaipm",
         settings_agg_key="region_aggregations",
+        multi_period=False,
+        include_retired_cap=False,
     ):
         """
 
         Parameters
         ----------
         pudl_engine : sqlalchemy.Engine
             A sqlalchemy connection for use by pandas
@@ -2776,20 +2966,25 @@
             The dictionary of settings with a dictionary of region aggregations
         """
         self.pudl_engine = pudl_engine
         self.pudl_out = pudl_out
         self.pg_engine = pg_engine
         self.settings = settings
         self.current_gens = current_gens
+        if self.settings.get("num_clusters") is None:
+            self.current_gens = False
         self.sort_gens = sort_gens
         self.model_regions_gdf = load_ipm_shapefile(self.settings)
         self.weighted_unit_hr = None
         self.supplement_with_860m = supplement_with_860m
+        self.multi_period = multi_period
+        self.include_retired_cap = include_retired_cap
         self.cluster_builder = build_resource_clusters(
-            self.settings.get("RESOURCE_GROUPS")
+            self.settings.get("RESOURCE_GROUPS"),
+            self.settings.get("RESOURCE_GROUP_PROFILES"),
         )
 
         if self.current_gens:
             self.data_years = self.settings.get("eia_data_years") or []
 
             self.gens_860 = load_generator_860_data(self.pudl_engine, self.data_years)
             self.gens_entity = pd.read_sql_table(
@@ -2797,15 +2992,15 @@
             )
 
             bga = self.pudl_out.bga_eia860()
             self.bga = bga.loc[
                 bga.report_date.dt.year.isin(self.data_years), :
             ].drop_duplicates(["plant_id_eia", "generator_id"])
 
-            logger.info("Loading map of plants to IPM regions")
+            logger.debug("Loading map of plants to IPM regions")
             self.plant_region_map = load_plant_region_map(
                 self.gens_860,
                 self.pudl_engine,
                 self.pg_engine,
                 self.settings,
                 self.model_regions_gdf,
                 table=plant_region_map_table,
@@ -2861,15 +3056,15 @@
         else:
             return s
         # median_hr = df["heat_rate_mmbtu_mwh"].median()
         # df["heat_rate_mmbtu_mwh"].fillna(median_hr, inplace=True)
 
         # return df
 
-    def remove_860_duplicates(self, df_860: pd.DataFrame()) -> pd.DataFrame():
+    def remove_860_duplicates(self, df_860: pd.DataFrame) -> pd.DataFrame:
         """
         Remove rows from an EIA 860 DF that contain a duplicate plant-generator pairing.
         """
         df = df_860.copy(deep=True)
         df = df.set_index(["plant_id_eia", "generator_id"])
         df = df.loc[~df.index.duplicated(), :].reset_index()
         return df
@@ -2879,14 +3074,15 @@
         generators file.
 
         Returns
         -------
         DataFrame
             One row for each region/DSM resource with values in all columns filled.
         """
+        logger.info("Creating flexible demand resources")
         year = self.settings["model_year"]
         df_list = []
         self.demand_response_profiles = {}
 
         if not self.settings.get("flexible_demand_resources"):
             logger.warning(
                 "A demand response file is included in extra inputs but the parameter "
@@ -2898,20 +3094,20 @@
             logger.warning(
                 f"The model year {year} is not included in your 'flexible_demand_resources' "
                 "parameter. No flexible demand resources will be included for this "
                 "planning period."
             )
         if self.settings["flexible_demand_resources"][year] is None:
             logger.warning(
-                f"Your 'flexible_demand_resources' settings parameter has the value 'None' "
+                "Your 'flexible_demand_resources' settings parameter has the value 'None' "
                 "for this planning period. No flexible demand resources will be included."
             )
         for resource, parameters in (
-            self.settings["flexible_demand_resources"].get(year, {}).items()
-        ):
+            self.settings["flexible_demand_resources"].get(year, {}) or {}
+        ).items():
             _df = pd.DataFrame(
                 index=self.settings["model_regions"],
                 columns=list(self.settings["generator_columns"]) + ["profile"],
             )
             _df = _df.drop(columns="Resource")
             _df["technology"] = resource
             _df["region"] = self.settings["model_regions"]
@@ -3007,26 +3203,28 @@
             False
 
         Returns
         -------
         dataframe
 
         """
+        logger.info("Compiling existing generators and their attributes")
         if self.gens_860.technology_description.isna().any():
             self.gens_860 = fill_missing_tech_descriptions(self.gens_860)
         self.gens_860_model = (
             self.gens_860.pipe(
                 supplement_generator_860_data,
                 self.gens_entity,
                 self.bga,
                 self.plant_region_map,
                 self.settings,
             )
             .pipe(remove_canceled_860m, self.canceled_860m)
             .pipe(remove_retired_860m, self.retired_860m)
+            .pipe(update_planned_retirement_date_860m, self.operating_860m.copy())
             .pipe(update_operating_date_860m, self.operating_860m.copy())
             .pipe(label_retirement_year, self.settings, add_additional_retirements=True)
             .pipe(
                 label_retirement_year,
                 self.settings,
                 age_col="original_planned_operating_date",
             )
@@ -3046,43 +3244,43 @@
         self.annual_gen_hr_923 = (
             self.gen_923.pipe(modify_cc_prime_mover_code, self.gens_860_model)
             .pipe(group_gen_by_year_fuel_primemover)
             .pipe(add_923_heat_rate)
         )
 
         # Add heat rates to the data we already have from 860
-        logger.info("Loading heat rate data for units and generator/fuel combinations")
+        logger.debug("Loading heat rate data for units and generator/fuel combinations")
         self.prime_mover_hr_map = plant_pm_heat_rates(self.annual_gen_hr_923)
         if self.weighted_unit_hr is None:
             self.weighted_unit_hr = unit_generator_heat_rates(
                 self.pudl_out, self.data_years
             )
         else:
-            logger.info("Using unit heat rates from previous round.")
+            logger.debug("Using unit heat rates from previous round.")
         self.weighted_unit_hr["unit_id_pg"] = self.weighted_unit_hr[
             "unit_id_pudl"
         ].astype("object")
 
         # Merge the PUDL calculated heat rate data and set the index for easy
         # mapping using plant/prime mover heat rates from 923
         hr_cols = ["plant_id_eia", "unit_id_pg", "heat_rate_mmbtu_mwh"]
         idx = ["plant_id_eia", "prime_mover_code", "energy_source_code_1"]
         self.units_model = self.gens_860_model.merge(
             self.weighted_unit_hr[hr_cols],
             on=["plant_id_eia", "unit_id_pg"],
             how="left",
         ).set_index(idx)
 
-        logger.info(
+        logger.debug(
             f"Units model technologies are "
             f"{self.units_model.technology_description.unique().tolist()}"
         )
         # print(units_model.head())
 
-        logger.info(
+        logger.debug(
             "Assigning technology/fuel heat rates where unit heat rates are not "
             "available"
         )
         self.units_model.loc[
             self.units_model.heat_rate_mmbtu_mwh.isnull(), "heat_rate_mmbtu_mwh"
         ] = self.units_model.loc[
             self.units_model.heat_rate_mmbtu_mwh.isnull()
@@ -3123,20 +3321,20 @@
             )
         # assert (
         #     self.units_model["heat_rate_mmbtu_mwh"].isnull().any() is False
         # ), "There are still some null heat rate values"
         # from IPython import embed
 
         # embed()
-        logger.info(
+        logger.debug(
             f"Units model technologies are "
             f"{self.units_model.technology_description.unique().tolist()}"
         )
         if self.supplement_with_860m:
-            logger.info(
+            logger.debug(
                 f"Before adding proposed generators, {len(self.units_model)} units with "
                 f"{self.units_model[self.settings['capacity_col']].sum()} MW capacity"
             )
             self.proposed_gens = import_proposed_generators(
                 planned=self.planned_860m,
                 settings=self.settings,
                 model_regions_gdf=self.model_regions_gdf,
@@ -3156,19 +3354,19 @@
                     ].drop_duplicates(),
                     self.new_860m_gens.reset_index()[
                         ["plant_id_eia", "model_region"]
                     ].drop_duplicates(),
                 ]
             ).drop_duplicates(subset=["plant_id_eia", "model_region"])
             # embed()
-            logger.info(
+            logger.debug(
                 f"Proposed gen technologies are "
                 f"{self.proposed_gens.technology_description.unique().tolist()}"
             )
-            logger.info(
+            logger.debug(
                 f"{self.proposed_gens[self.settings['capacity_col']].sum()} MW proposed"
             )
             self.units_model = pd.concat(
                 [self.proposed_gens, self.units_model, self.new_860m_gens], sort=False
             )
 
         # Create a pudl unit id based on plant and generator id where one doesn't exist.
@@ -3214,15 +3412,15 @@
             + "_"
             + self.units_model.loc[
                 self.units_model.unit_id_pg.isnull(), "generator_id"
             ].astype(str)
         ).values
         self.units_model.set_index(idx, inplace=True)
 
-        logger.info("Calculating plant O&M costs")
+        logger.debug("Calculating plant O&M costs")
         techs = self.settings["num_clusters"].keys()
         self.units_model = (
             self.units_model.rename(columns={"technology_description": "technology"})
             .query("technology.isin(@techs).values")
             .pipe(
                 atb_fixed_var_om_existing,
                 self.atb_hr,
@@ -3232,15 +3430,15 @@
             )
         )
 
         # logger.info(
         #     f"After adding proposed, units model technologies are "
         #     f"{self.units_model.technology_description.unique().tolist()}"
         # )
-        logger.info(
+        logger.debug(
             f"After adding proposed generators, {len(self.units_model)} units with "
             f"{self.units_model[self.settings['capacity_col']].sum()} MW capacity"
         )
 
         techs = list(self.settings["num_clusters"])
 
         num_clusters = {}
@@ -3250,23 +3448,58 @@
         if self.settings.get("alt_num_clusters"):
             for region in self.settings["alt_num_clusters"]:
                 for tech, cluster_size in self.settings["alt_num_clusters"][
                     region
                 ].items():
                     num_clusters[region][tech] = cluster_size
 
-        region_tech_grouped = self.units_model.loc[
-            (self.units_model.technology.isin(techs))
-            & ~(self.units_model.retirement_year <= self.settings["model_year"]),
-            :,
-        ].groupby(["model_region", "technology"])
-
         self.retired = self.units_model.loc[
             ~(self.units_model.retirement_year > self.settings["model_year"]), :
         ]
+        self.period_retired = self.units_model.loc[
+            ~(self.units_model.retirement_year > self.settings["model_year"])
+            & (
+                self.units_model.retirement_year
+                >= self.settings["model_first_planning_year"]
+            ),
+            :,
+        ]
+        self.retired_index = self.retired.set_index(
+            ["plant_id_eia", "unit_id_pg"]
+        ).index
+        if (
+            self.multi_period
+            and self.settings.get("cluster_with_retired_gens", True) is True
+        ):
+            logger.info(
+                "Age-retired gens are included for clustering to keep consistent "
+                "cluster assignments across periods. "
+            )
+            region_tech_grouped = self.units_model.loc[
+                self.units_model.technology.isin(techs), :
+            ].groupby(["model_region", "technology"])
+        elif self.settings.get("cluster_with_retired_gens", False) is True:
+            logger.info(
+                "Age-retired gens are included for clustering to keep consistent "
+                "cluster assignments across periods."
+            )
+            region_tech_grouped = self.units_model.loc[
+                self.units_model.technology.isin(techs), :
+            ].groupby(["model_region", "technology"])
+        else:
+            logger.info(
+                "Age-retired gens are NOT included for clustering. This may lead to "
+                "inconsistent cluster assignments across periods. If you want to change "
+                "this behavior, add 'cluster_with_retired_gens: true' to your settings."
+            )
+            region_tech_grouped = self.units_model.loc[
+                (self.units_model.technology.isin(techs))
+                & ~(self.units_model.retirement_year <= self.settings["model_year"]),
+                :,
+            ].groupby(["model_region", "technology"])
 
         # gens_860 lost the ownership code... refactor this!
         # self.all_gens_860 = load_generator_860_data(self.pudl_engine, self.data_years)
         # Getting weighted ownership for each unit, which will be used below.
         # self.weighted_ownership = weighted_ownership_by_unit(
         #     self.units_model, self.all_gens_860, self.ownership, self.settings
         # )
@@ -3277,59 +3510,77 @@
         unit_list = []
         self.cluster_list = []
         alt_cluster_method = self.settings.get("alt_cluster_method") or {}
 
         for _, df in region_tech_grouped:
             region, tech = _
             grouped = group_units(df, self.settings)
+            grouped["technology"] = tech
 
             # This is bad. Should be setting up a dictionary of objects that picks the
             # correct clustering method. Can't keep doing if statements as the number of
             # methods grows. CHANGE LATER.
             if not alt_cluster_method:
-                # Allow users to set value as None and not cluster units.
-                if num_clusters[region][tech] is None:
+                # Allow users to set value as None and not cluster units, or when the
+                # num clusters is equal to the number of units.
+                if num_clusters[region][tech] is None or num_clusters[region][
+                    tech
+                ] == len(grouped):
+                    if self.multi_period:
+                        grouped.loc[
+                            grouped.index.isin(self.retired_index),
+                            [
+                                self.settings["capacity_col"],
+                                "minimum_load_mw",
+                                "capacity_mwh",
+                            ],
+                        ] = np.nan
+                    else:
+                        grouped = grouped.loc[
+                            ~grouped.index.isin(self.retired_index), :
+                        ]
+
                     grouped["cluster"] = np.arange(len(grouped)) + 1
                     unit_list.append(grouped)
-                    _df = calc_unit_cluster_values(
-                        grouped, self.settings["capacity_col"], tech
-                    )
-                    _df["region"] = region
+                    if not grouped.empty:
+                        _df = calc_unit_cluster_values(
+                            grouped, self.settings["capacity_col"], tech
+                        )
+                        _df["region"] = region
 
-                    self.cluster_list.append(_df)
-                    continue
-                if num_clusters[region][tech] > 0:
+                        self.cluster_list.append(_df)
+                        continue
+                elif num_clusters[region][tech] > 0:
                     cluster_cols = [
                         "Fixed_OM_Cost_per_MWyr",
                         # "Var_OM_Cost_per_MWh",
                         # "minimum_load_mw",
                         "heat_rate_mmbtu_mwh",
                     ]
                     if len(grouped) < num_clusters[region][tech]:
                         s = f"""
-    *****************************
     The technology {tech} in region {region} has only {len(grouped)} operating units,
     which is less than the {num_clusters[region][tech]} clusters you specified.
     The number of clusters has been set equal to the number of units.
-    *****************************
                             """
                         logger.info(s)
                         num_clusters[region][tech] = len(grouped)
                     clusters = cluster.KMeans(
                         n_clusters=num_clusters[region][tech], random_state=6
                     ).fit(
                         preprocessing.StandardScaler().fit_transform(
                             grouped[cluster_cols]
                         )
                     )
 
                     grouped["cluster"] = (
                         clusters.labels_ + 1
                     )  # Change to 1-index for julia
-
+                else:
+                    continue
             else:
                 if (
                     region in alt_cluster_method
                     and tech in alt_cluster_method[region]["technology_description"]
                 ):
                     grouped = cluster_by_owner(
                         df,
@@ -3345,49 +3596,70 @@
                     clusters = cluster.KMeans(
                         n_clusters=num_clusters[region][tech], random_state=6
                     ).fit(preprocessing.StandardScaler().fit_transform(grouped))
 
                     grouped["cluster"] = (
                         clusters.labels_ + 1
                     )  # Change to 1-index for julia
+                else:
+                    continue
 
             # Saving individual unit data for later analysis (if needed)
             unit_list.append(grouped)
 
             # Don't add technologies with specified 0 clusters
             if num_clusters[region][tech] != 0:
-                _df = calc_unit_cluster_values(
-                    grouped, self.settings["capacity_col"], tech
-                )
-                _df["region"] = region
-                _df["plant_id_eia"] = (
-                    grouped.reset_index().groupby("cluster")["plant_id_eia"].apply(list)
-                )
-                _df["unit_id_pg"] = (
-                    grouped.reset_index().groupby("cluster")["unit_id_pg"].apply(list)
-                )
+                # Remove retired units before calculating cluster operating values
+                if self.multi_period:
+                    grouped.loc[
+                        grouped.index.isin(self.retired_index),
+                        [
+                            self.settings["capacity_col"],
+                            "minimum_load_mw",
+                            "capacity_mwh",
+                        ],
+                    ] = np.nan
+                else:
+                    grouped = grouped.loc[~grouped.index.isin(self.retired_index), :]
+                if not grouped.empty:
+                    _df = calc_unit_cluster_values(
+                        grouped, self.settings["capacity_col"], tech
+                    )
+                    _df["region"] = region
+                    _df["plant_id_eia"] = (
+                        grouped.reset_index()
+                        .groupby("cluster")["plant_id_eia"]
+                        .apply(list)
+                    )
+                    _df["unit_id_pg"] = (
+                        grouped.reset_index()
+                        .groupby("cluster")["unit_id_pg"]
+                        .apply(list)
+                    )
 
-                self.cluster_list.append(_df)
+                    self.cluster_list.append(_df)
 
         # Save some data about individual units for easy access
         self.all_units = pd.concat(unit_list, sort=False)
         self.all_units = pd.merge(
             self.units_model,  # .reset_index(),
-            self.all_units.reset_index()[["plant_id_eia", "unit_id_pg", "cluster"]],
-            on=["plant_id_eia", "unit_id_pg"],
+            self.all_units.reset_index()[
+                ["plant_id_eia", "unit_id_pg", "cluster", "technology"]
+            ],
+            on=["plant_id_eia", "unit_id_pg", "technology"],
             how="inner",
         ).merge(
             self.plants_860[["plant_id_eia", "utility_id_eia"]],
             on=["plant_id_eia"],
             how="left",
         )
 
-        logger.info("Finalizing generation clusters")
+        # logger.info("Finalizing generation clusters")
         self.results = pd.concat(self.cluster_list)
-        logger.info(
+        logger.debug(
             f"Results technologies are {self.results.technology.unique().tolist()}"
         )
 
         # if self.settings.get("region_wind_pv_cap_fn"):
         #     from powergenome.external_data import overwrite_wind_pv_capacity
 
         #     logger.info("Setting existing wind/pv using external file")
@@ -3443,44 +3715,48 @@
                     "unmodified_cap_size",
                 ]
                 * self.results.loc[
                     self.results["technology"].isin(derate_techs), "capacity_factor"
                 ]
             )
 
+        self.all_units = self.all_units.rename(columns={"model_region": "region"})
+        self.all_units["Resource"] = (
+            self.all_units["region"]
+            + "_"
+            + snake_case_col(self.all_units["technology"])
+            + "_"
+            + self.all_units["cluster"].astype(int).astype(str)
+        )
+
         if self.settings.get("extra_outputs"):
-            self.all_units = self.all_units.rename(columns={"model_region": "region"})
-            self.all_units["Resource"] = (
-                self.all_units["region"]
-                + "_"
-                + snake_case_col(self.all_units["technology"])
-                + "_"
-                + self.all_units["cluster"].astype(str)
-            )
             self.all_units.to_csv(
                 Path(self.settings["extra_outputs"]) / "existing_gen_units.csv",
                 index=False,
             )
         # Round Cap_size to prevent GenX error.
         self.results = self.results.round(3)
         self.results["Cap_Size"] = self.results["Cap_Size"]
         self.results["Existing_Cap_MW"] = self.results.Cap_Size * self.results.num_units
+
+        # A cap size of 0 causes issues in GenX with thermal commitment.
+        self.results["Cap_Size"] = self.results["Cap_Size"].fillna(1).replace(0, 1)
         if self.settings.get("derate_capacity"):
             self.results["unmodified_existing_cap_mw"] = (
                 self.results["unmodified_cap_size"] * self.results["num_units"]
             )
 
         if self.settings.get("region_wind_pv_cap_fn"):
             from powergenome.external_data import overwrite_wind_pv_capacity
 
-            logger.info("Setting existing wind/pv using external file")
+            logger.debug("Setting existing wind/pv using external file")
             self.results = overwrite_wind_pv_capacity(self.results, self.settings)
 
         if self.settings.get("dg_as_resource"):
-            logger.info(
+            logger.debug(
                 "\n **************** \nDistributed generation is being added as generating"
                 " resources. The capacity of DG in each region is increased by "
                 f"{self.settings.get('avg_distribution_loss', 0):%} to account for no "
                 "distribution losses.\n"
             )
             self.results = add_dg_resources(
                 self.pg_engine, self.settings, self.results.reset_index()
@@ -3494,29 +3770,73 @@
             # .pipe(
             #     atb_fixed_var_om_existing, self.atb_costs, self.atb_hr, self.settings
             # )
             # .pipe(atb_new_generators, self.atb_costs, self.atb_hr, self.settings)
             .pipe(startup_fuel, self.settings)
             .pipe(add_fuel_labels, self.fuel_prices, self.settings)
             .pipe(startup_nonfuel_costs, self.settings)
-            .pipe(add_genx_model_tags, self.settings)
+            .pipe(
+                add_resource_tags,
+                model_tag_values=self.settings.get("model_tag_values", {}),
+                regional_tag_values=self.settings.get("regional_tag_values", {}),
+                model_tag_names=self.settings.get("model_tag_names", []),
+                default_model_tag=self.settings.get("default_model_tag", {}),
+            )
         )
 
         if self.sort_gens:
-            logger.info("Sorting new resources alphabetically.")
+            logger.debug("Sorting new resources alphabetically.")
             self.results = self.results.sort_values(["region", "technology"])
 
         # self.results = self.results.rename(columns={"technology": "Resource"})
         self.results["Resource"] = (
             self.results["region"]
             + "_"
             + snake_case_col(self.results["technology"])
             + "_"
             + self.results["cluster"].astype(str)
         )
+        if self.results["Resource"].nunique() != len(self.results):
+            dup_resources = (
+                self.results[self.results["Resource"].duplicated()]
+                .drop_duplicates()
+                .to_list()
+            )
+            raise ValueError(
+                f"The generator resource names {dup_resources} have duplicates. These "
+                "names should be unique. You'll probably need to file an issue for this "
+                "at https://github.com/PowerGenome/PowerGenome/issues."
+            )
+
+        if self.multi_period:
+            retire_cols = [
+                "Min_Retired_Cap_MW",
+                "Min_Retired_Energy_Cap_MW",
+                "Min_Retired_Charge_Cap_MW",
+            ]
+            for col in retire_cols:
+                if col not in self.settings.get("generator_columns", []) and isinstance(
+                    self.settings.get("generator_columns"), list
+                ):
+                    self.settings["generator_columns"].append(col)
+
+            if self.include_retired_cap:
+                # Add mimimum retirement amounts
+                cap_retired = cap_retire_within_period(
+                    self.all_units,
+                    self.settings["model_first_planning_year"],
+                    self.settings["model_year"],
+                    self.settings.get("capacity_col", "capacity_mw"),
+                )
+                self.results = pd.merge(
+                    self.results, cap_retired, on="Resource", how="left", validate="1:1"
+                )
+                self.results[retire_cols].fillna(0, inplace=True)
+            else:
+                self.results[retire_cols] = 0
 
         # Add variable resource profiles
         self.results = self.results.reset_index(drop=True)
         for i, row in enumerate(self.results.itertuples()):
             params = map_eia_technology(row.technology)
             if not params:
                 # EIA technology not supported
@@ -3525,15 +3845,15 @@
             groups = self.cluster_builder.find_groups(**params)
             if not groups:
                 # No matching resource groups
                 continue
             if len(groups) > 1:
                 # Multiple matching resource groups
                 raise ValueError(
-                    f"Multiple existing resource groups match EIA technology"
+                    "Multiple existing resource groups match EIA technology"
                     + row.technology
                 )
             group = groups[0]
             if group.profiles is None:
                 # Resource group has no profiles
                 continue
             if row.region in (self.settings.get("region_aggregations", {}) or {}):
@@ -3549,17 +3869,23 @@
                 max_clusters=1,
                 utc_offset=self.settings.get("utc_offset", 0),
             )
             self.results["profile"][i] = clusters["profile"][0]
 
         self.results = rename_gen_cols(self.results)
 
+        # Drop old index cols from df
+        self.results.drop(columns=["level_0", "index"], errors="ignore", inplace=True)
+
+        logger.info("Finished creating existing generator clusters")
+
         return self.results
 
     def create_new_generators(self):
+        logger.info("Starting to build new generation resources")
         self.offshore_spur_costs = fetch_atb_offshore_spur_costs(
             self.pg_engine, self.settings
         )
         self.atb_costs = fetch_atb_costs(
             self.pg_engine, self.settings, self.offshore_spur_costs
         )
 
@@ -3571,15 +3897,15 @@
             self.new_generators = (
                 self.new_generators.pipe(startup_fuel, self.settings)
                 .pipe(add_fuel_labels, self.fuel_prices, self.settings)
                 .pipe(startup_nonfuel_costs, self.settings)
             )
 
             if self.sort_gens:
-                logger.info("Sorting new resources alphabetically.")
+                logger.debug("Sorting new resources alphabetically.")
                 self.new_generators = self.new_generators.sort_values(
                     ["region", "technology"]
                 )
 
             if self.settings.get("capacity_limit_spur_fn"):
                 self.new_generators = self.new_generators.pipe(
                     add_resource_max_cap_spur, self.settings
@@ -3593,26 +3919,36 @@
         if self.settings.get("demand_response_fn") or self.settings.get(
             "electrification_stock_fn"
         ):
             dr_rows = self.create_demand_response_gen_rows()
             self.new_generators = pd.concat(
                 [self.new_generators, dr_rows], sort=False, ignore_index=True
             )
-        self.new_generators = add_genx_model_tags(self.new_generators, self.settings)
+        self.new_generators = add_resource_tags(
+            self.new_generators,
+            model_tag_values=self.settings.get("model_tag_values", {}),
+            regional_tag_values=self.settings.get("regional_tag_values", {}),
+            model_tag_names=self.settings.get("model_tag_names", []),
+            default_model_tag=self.settings.get("default_model_tag", {}),
+        )
         if "cluster" not in self.new_generators.columns:
             self.new_generators["cluster"] = 1
-        self.new_generators["cluster"] = self.new_generators["cluster"].astype("Int64")
+        self.new_generators["cluster"] = self.new_generators["cluster"].astype(
+            "Int64", errors="ignore"
+        )
         self.new_generators["Resource"] = (
             self.new_generators["region"]
             + "_"
             + snake_case_col(self.new_generators["technology"])
             + "_"
             + self.new_generators["cluster"].astype(str)
         )
 
+        logger.info("Finished creating new generation resources")
+
         return self.new_generators
 
     def create_all_generators(self):
         if self.current_gens:
             self.existing_resources = self.create_region_technology_clusters()
 
         self.new_resources = self.create_new_generators()
@@ -3629,14 +3965,15 @@
                 df=self.all_resources,
                 co2_data_path=self.settings["input_folder"]
                 / self.settings.get("co2_pipeline_cost_fn"),
                 co2_pipeline_filters=self.settings["co2_pipeline_filters"],
                 region_aggregations=self.settings.get("region_aggregations"),
                 fuel_emission_factors=self.settings["fuel_emission_factors"],
                 target_usd_year=self.settings.get("target_usd_year"),
+                extra_ccs_cost_tonne=self.settings.get("ccs_disposal_cost"),
             )
 
         self.all_resources = self.all_resources.round(3)
         self.all_resources["Cap_Size"] = self.all_resources["Cap_Size"]
         self.all_resources["Heat_Rate_MMBTU_per_MWh"] = self.all_resources[
             "Heat_Rate_MMBTU_per_MWh"
         ]
@@ -3650,12 +3987,12 @@
         # Set Min_Power of wind/solar to 0
         if "VRE" in self.all_resources.columns:
             self.all_resources.loc[self.all_resources["VRE"] == 1, "Min_Power"] = 0
 
         self.all_resources["R_ID"] = np.arange(len(self.all_resources)) + 1
 
         if self.current_gens:
-            logger.info(
+            logger.debug(
                 f"Capacity of {self.all_resources['Existing_Cap_MW'].sum()} MW in final clusters"
             )
 
         return self.all_resources
```

### Comparing `PowerGenome-0.6.1a0/powergenome/load_construction.py` & `powergenome-0.6.2/powergenome/load_construction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 import logging
 import os
 from functools import lru_cache
 from pathlib import Path
-from typing import Dict, List, Union
+from typing import List
 
 import numpy as np
 import pandas as pd
 
-from powergenome.params import DATA_PATHS, SETTINGS
+from powergenome.params import SETTINGS
 from powergenome.util import deep_freeze_args, find_region_col, snake_case_col
 
 logger = logging.getLogger(__name__)
 
 
 us_state_abbrev = {
     "Alabama": "AL",
@@ -172,15 +172,15 @@
     stock_temp = scenario_stock.loc[
         (scenario_stock["sector"] == sector)
         & (scenario_stock["subsector"] == subsector),
         ["state", "year", "agg_stock_type1", "agg_stock_type2"],
     ]
 
     factor_years = timeseries["year"].unique()
-    if not year in factor_years:
+    if year not in factor_years:
         diff = np.array(factor_years - year)
         index = diff[np.where(diff <= 0)].argmax()
         year_approx = factor_years[index]
         timeseries = timeseries.loc[timeseries["year"] == year_approx, :]
         timeseries["year"] = year
         logger.warning(
             f"No incremental factor available for {sector}/{subsector} "
@@ -286,14 +286,15 @@
         No "EFS_DATA" key is included in the .env file.
     FileNotFoundError
         The "EFS_DATA" or "path_in" folder does not exist.
     ValueError
         The "electrificication_scenario" parameter does not match scenarios in the stock
         file.
     """
+    logger.info("Building demand profiles of electrified end-use technologies")
     if not path_in:
         try:
             path_in = Path(SETTINGS["EFS_DATA"])
         except TypeError:
             raise KeyError("The variable 'EFS_DATA' is not included in your .env file.")
     if not path_in.is_dir():
         raise FileNotFoundError(
```

### Comparing `PowerGenome-0.6.1a0/powergenome/load_profiles.py` & `powergenome-0.6.2/powergenome/load_profiles.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 """
 Hourly demand profiles
 """
 
 import logging
+from functools import lru_cache
 from inspect import signature
 from pathlib import Path
 from typing import Dict, List, Tuple
 
 import numpy as np
 import pandas as pd
 import sqlalchemy as sa
 
 from powergenome.distributed_gen import distributed_gen_profiles
 from powergenome.eia_opendata import get_aeo_load
 from powergenome.external_data import make_demand_response_profiles
 from powergenome.load_construction import electrification_profiles
 from powergenome.util import (
+    deep_freeze_args,
     find_region_col,
     map_agg_region_names,
     regions_to_keep,
     remove_feb_29,
     reverse_dict_of_lists,
 )
 
@@ -78,14 +80,48 @@
             return load_profile
 
         return wrapper
 
     return decorator
 
 
+@deep_freeze_args
+@lru_cache
+def read_subsector_demand(
+    pg_engine_str: str, keep_regions: List[str], pg_table: str, region_col: str
+) -> pd.DataFrame:
+    pg_engine = sa.create_engine(pg_engine_str)
+    # This is a default list of sector/subsectors that are considered "base" demand
+    # and are not affected by stock levels of electric technologies (e.g. EVs and heat pumps)
+    # NOTE: This should be parameratized so it can be changed by the user, especially
+    # if load data is from a source other than NREL EFS
+    base_sector_subsectors = [
+        ("commercial", "other"),
+        ("residential", "other"),
+        ("residential", "clothes and dish washing/drying"),
+        ("industrial", "machine drives"),
+        ("industrial", "process heat"),
+        ("industrial", "other"),
+    ]
+    s = f"""
+            SELECT year, {region_col} as region, time_index, sector, sum(load_mw) as load_mw
+            FROM {pg_table}
+            WHERE {region_col} in ({','.join(['?']*len(keep_regions))})
+            AND
+            ({' OR '.join(["(sector=? and subsector=?)"]*len(base_sector_subsectors))})
+            GROUP BY year, region, sector, time_index
+            """
+    params = list(keep_regions) + [
+        item for sublist in base_sector_subsectors for item in sublist
+    ]
+    load_curves = pd.read_sql_query(sql=s, con=pg_engine, params=params)
+
+    return load_curves
+
+
 def make_load_curves(
     pg_engine: sa.engine.base.Engine,
     settings: dict,
     pg_table: str = "load_curves_nrel_efs",
 ) -> pd.DataFrame:
     """Read base load profiles from database and grow the load to a future year.
 
@@ -116,52 +152,34 @@
     # dataframe
     keep_regions, region_agg_map = regions_to_keep(
         settings["model_regions"], settings.get("region_aggregations")
     )
 
     # I'd rather use a sql query and only pull the regions of interest but
     # sqlalchemy doesn't allow table names to be parameterized.
-    logger.info("Loading load curves from PUDL")
+    logger.debug("Loading demand profiles from the database")
     inst = sa.inspect(pg_engine)
     if not inst.has_table(pg_table):
         raise KeyError(
             f"There is no load curves table with the name {pg_table} in the 'PG_DB' "
             "database specified in your .env file."
         )
     table_cols = [c["name"] for c in inst.get_columns(pg_table)]
     context = f"Load curves table ({pg_table} in database {pg_engine}."
     region_col = find_region_col(table_cols, context)
     if "sector" in table_cols or "subsector" in table_cols:
         if settings.get("electrification_stock_fn") and settings.get(
             "electrification_scenario"
         ):
-            # This is a default list of sector/subsectors that are considered "base" demand
-            # and are not affected by stock levels of electric technologies (e.g. EVs and heat pumps)
-            # NOTE: This should be parameratized so it can be changed by the user, especially
-            # if load data is from a source other than NREL EFS
-            base_sector_subsectors = [
-                ("commercial", "other"),
-                ("residential", "other"),
-                ("residential", "clothes and dish washing/drying"),
-                ("industrial", "machine drives"),
-                ("industrial", "process heat"),
-                ("industrial", "other"),
-            ]
-            s = f"""
-                    SELECT year, {region_col} as region, time_index, sector, sum(load_mw) as load_mw
-                    FROM {pg_table}
-                    WHERE {region_col} in ({','.join(['?']*len(keep_regions))})
-                    AND
-                    ({' OR '.join(["(sector=? and subsector=?)"]*len(base_sector_subsectors))})
-                    GROUP BY year, region, sector, time_index
-                    """
-            params = keep_regions + [
-                item for sublist in base_sector_subsectors for item in sublist
-            ]
-            load_curves = pd.read_sql_query(sql=s, con=pg_engine, params=params)
+            load_curves = read_subsector_demand(
+                pg_engine_str=str(pg_engine)[7:-1],
+                keep_regions=keep_regions,
+                pg_table=pg_table,
+                region_col=region_col,
+            )
         else:
             s = f"""
                     SELECT year, {region_col} as region, time_index, sector, sum(load_mw) as load_mw
                     FROM {pg_table}
                     WHERE {region_col} in ({','.join(['?']*len(keep_regions))})
                     GROUP BY year, region, sector, time_index
                     """
@@ -176,19 +194,19 @@
             """
         params = keep_regions
         load_curves = pd.read_sql_query(sql=s, con=pg_engine, params=params)
 
     # Increase demand to account for load growth
     load_curves = add_load_growth(load_curves, settings)
 
-    load_curves.loc[
-        load_curves.region.isin(region_agg_map), "region"
-    ] = load_curves.region.map(region_agg_map)
+    load_curves.loc[load_curves.region.isin(region_agg_map), "region"] = (
+        load_curves.region.map(region_agg_map)
+    )
 
-    logger.info("Aggregating load curves in grouped regions")
+    logger.debug("Aggregating load curves in grouped regions")
     load_curves_agg = load_curves.groupby(["region", "time_index"])["load_mw"].sum()
 
     lc_wide = load_curves_agg.unstack(level=0)
     if lc_wide.columns.nlevels > 1:
         lc_wide.columns = lc_wide.columns.droplevel()
 
     if len(lc_wide) == 8784:
@@ -579,15 +597,15 @@
                     f"user-supplied load curves file {regional_load_fn}."
                 )
             hourly_load_profiles = hourly_load_profiles.reindex(columns=cols)
 
         return hourly_load_profiles
 
     else:
-        logger.info("User supplied load profile not found.")
+        logger.warning("User supplied load profile not found.")
         return None
 
 
 def make_final_load_curves(
     pg_engine: sa.engine.base.Engine,
     settings: dict,
 ):
@@ -611,34 +629,30 @@
 
     Raises
     ------
     ValueError
         When all load curves are null.
     """
 
-    logger.info("Loading load curves")
+    logger.info("Creating hourly demand profiles")
     user_load_curves = load_usr_demand_profiles(settings)
 
     if user_load_curves is not None and all(
         [r in user_load_curves.columns for r in settings["model_regions"]]
     ):
         load_curves_before_dr = user_load_curves
 
     else:
         load_sources = settings.get("load_source_table_name")
         if load_sources is None:
-            s = """
-            *****************************
-            Regional load data sources have not been specified. Defaulting to EFS load data.
-            Check your settings file, and please specify the preferred source for load data
-            (FERC, EFS, USER) either for each region or for the entire system with the setting
-            "regional_load_source".
-            *****************************
-            """
-            logger.warning(s)
+            s = (
+                "Regional load data sources have not been specified. Defaulting to EFS load data. "
+                "See documentation of the parameter 'regional_load_source' to use other data."
+            )
+            logger.info(s)
             load_sources = {"EFS": "load_curves_nrel_efs"}
 
         # `filter_load_by_region` is a decorator factory that generates a decorator
         # when given the parameter `load_source`. This decorator creates a wrapper
         # for the function `make_load_curves`, which is passed the args from the final
         # parentheses.
         load_curves_before_dr = [
@@ -748,39 +762,42 @@
         need to be accounted for.
 
     Raises
     ------
     KeyError
         If the calculation method specified in settings is not 'capacity' or 'fraction_load'
     """
-
+    logger.info("Creating distributed generation profiles")
     year = settings["model_year"]
 
     if settings.get("distributed_gen_fn"):
         scenario = settings.get("distributed_gen_scenario")
-        path_in = settings.get("")
         if settings.get("region_aggregations"):
             regions = [
                 r
                 for r in settings["model_regions"]
                 if r not in settings["region_aggregations"].keys()
             ]
             regions.extend(
                 list(reverse_dict_of_lists(settings["region_aggregations"]).keys())
             )
+            regions = [
+                r for r in regions if r not in settings["region_aggregations"].keys()
+            ]
         else:
             regions = settings["model_regions"]
 
         dg_profiles = distributed_gen_profiles(
             settings.get("distributed_gen_fn"),
             settings["model_year"],
             scenario,
             regions,
             settings.get("DISTRIBUTED_GEN_DATA"),
             settings.get("region_aggregations"),
+            settings.get("utc_offset"),
         )
         return dg_profiles
 
     dg_profiles_path = (
         Path(settings["input_folder"]) / settings["distributed_gen_profiles_fn"]
     )
 
@@ -788,15 +805,15 @@
     profile_regions = hourly_norm_profiles.columns
 
     dg_calc_methods = settings["distributed_gen_method"]
     dg_calc_values = settings["distributed_gen_values"]
 
     assert (
         year in dg_calc_values
-    ), f"The years in settings parameter 'distributed_gen_values' do not match the model years."
+    ), "The years in settings parameter 'distributed_gen_values' do not match the model years."
 
     for region in dg_calc_values[year]:
         assert region in set(profile_regions), (
             "The profile regions in settings parameter 'distributed_gen_values' do not\n"
             f"match the regions in {settings['distributed_gen_profiles_fn']} for year {year}"
         )
```

### Comparing `PowerGenome-0.6.1a0/powergenome/nrelatb.py` & `powergenome-0.6.2/powergenome/nrelatb.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,29 +10,35 @@
 from typing import Dict, List, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import sqlalchemy
 from joblib import Parallel, delayed
 
-from powergenome.cluster.renewables import assign_site_cluster, calc_cluster_values
+from powergenome.cluster.renewables import (
+    assign_site_cluster,
+    calc_cluster_values,
+    modify_renewable_group,
+)
+from powergenome.financials import investment_cost_calculator
 from powergenome.params import DATA_PATHS, SETTINGS, build_resource_clusters
 from powergenome.price_adjustment import inflation_price_adjustment
 from powergenome.resource_clusters import (
     ClusterBuilder,
     ResourceGroup,
     Table,
     map_nrel_atb_technology,
 )
 from powergenome.util import (
+    add_row_to_csv,
     apply_all_tag_to_regions,
+    hash_string_sha256,
     remove_leading_zero,
     reverse_dict_of_lists,
     snake_case_col,
-    snake_case_str,
 )
 
 idx = pd.IndexSlice
 logger = logging.getLogger(__name__)
 
 
 def fetch_atb_costs(
@@ -63,15 +69,15 @@
     -------
     pd.DataFrame
         Power plant cost data with columns:
         ['technology', 'cap_recovery_years', 'cost_case', 'financial_case',
        'basis_year', 'tech_detail', 'fixed_o_m_mw', 'variable_o_m_mwh', 'capex', 'cf',
        'fuel', 'lcoe', 'wacc_real']
     """
-    logger.info("Loading NREL ATB data")
+    logger.debug("Loading NREL ATB data")
 
     col_names = [
         "technology",
         "tech_detail",
         "cost_case",
         "parameter",
         "basis_year",
@@ -169,15 +175,15 @@
                 for year in range(2017, 2051)
             ]
             wacc_rows.extend(battery_wacc_rows)
         elif battery_wacc_standin in atb_techs:
             # if battery_wacc_standin in tech_list:
             #     pass
             # else:
-            logger.info(
+            logger.debug(
                 f"Using {battery_wacc_standin} {fin_case} WACC for Battery storage."
             )
             for cost_case in ["Mid", "Moderate"]:
                 wacc_s = f"""
                 select technology, cost_case, basis_year, parameter_value
                 from technology_costs_nrelatb
                 where
@@ -254,15 +260,15 @@
     if any("PV" in tech for tech in tech_list) and atb_year == 2019:
         print("Inflating ATB 2019 PV costs from DC to AC")
         atb_costs.loc[
             atb_costs["technology"].str.contains("PV"),
             ["capex_mw", "fixed_o_m_mw", "variable_o_m_mwh"],
         ] *= settings.get("pv_ac_dc_ratio", 1.3)
     elif atb_year > 2019:
-        logger.info("PV costs are already in AC units, not inflating the cost.")
+        logger.debug("PV costs are already in AC units, not inflating the cost.")
 
     if offshore_spur_costs is not None and "OffShoreWind" in atb_costs["technology"]:
         idx_cols = ["technology", "tech_detail", "cost_case", "basis_year"]
         offshore_spur_costs = offshore_spur_costs.set_index(idx_cols)
         atb_costs = atb_costs.set_index(idx_cols)
 
         atb_costs.loc[idx["OffShoreWind", :, :, :], "capex_mw"] = (
@@ -407,23 +413,97 @@
 
     Returns
     -------
     DataFrame
         Same as incoming "results" dataframe but with new columns
         "Fixed_OM_Cost_per_MWyr" and "Var_OM_Cost_per_MWh"
     """
-    logger.info("Adding fixed and variable O&M for existing plants")
+    logger.debug("Adding fixed and variable O&M for existing plants")
 
     existing_year = settings["atb_existing_year"]
 
     techs = {}
+    missing_techs = []
     for eia, atb in settings["eia_atb_tech_map"].items():
         if not isinstance(atb, list):
             atb = [atb]
-        techs[eia] = atb[0].split("_")
+        missing = True
+        for tech_detail in atb:
+            tech, detail = tech_detail.split("_")
+            if not atb_hr_df.query(
+                "technology == @tech and tech_detail == @detail"
+            ).empty:
+                techs[eia] = [tech, detail]
+                missing = False
+                break
+        if missing is True and eia in results["technology"].unique():
+            missing_techs.append(eia)
+
+        # techs[eia] = atb[0].split("_")
+    if missing_techs:
+        s = (
+            f"The EIA technologies {missing_techs} do not have an ATB counterpart with a "
+            "valid heat rate. Not all ATB technologies *should* have a valid heat rate "
+            "(e.g. wind, solar, and hydro). Check the 'eia_atb_tech_map' parameter in your "
+            "settings file(s) if you think one of these technologies should be mapped to "
+            "an ATB technology with a valid heat rate."
+        )
+        logger.info(s)
+
+    # Find valid ATB tech/tech_details with O&M costs where heat rate was missing.
+    s = """
+            SELECT
+            technology,
+            tech_detail
+        FROM
+            technology_costs_nrelatb
+        WHERE
+            basis_year == ?
+            AND financial_case == "Market"
+            AND cost_case in("Mid", "Moderate")
+            AND atb_year == ?
+            AND parameter in("variable_o_m_mwh", "fixed_o_m_mw")
+    """
+    params = [existing_year, settings["atb_data_year"]]
+    atb_om_names = pd.read_sql_query(
+        s,
+        pg_engine,
+        params=params,
+    ).drop_duplicates()
+    _missing_techs = missing_techs.copy()
+    for eia_tech in missing_techs:
+        atb = settings["eia_atb_tech_map"][eia_tech]
+        if not isinstance(atb, list):
+            atb = [atb]
+        missing = True
+        for tech_detail in atb:
+            tech, detail = tech_detail.split("_")
+            if (
+                not atb_om_names.query(
+                    "technology == @tech and tech_detail == @detail"
+                ).empty
+                and missing is True
+            ):
+                techs[eia_tech] = [tech, detail]
+                missing = False
+                # break
+        if missing is False:
+            _missing_techs.remove(eia_tech)
+        elif missing is True and eia_tech in results["technology"].unique():
+            techs[eia_tech] = atb[0].split("_")
+        # else:
+        #     techs[eia_tech] = atb[0].split("_")
+    if _missing_techs:
+        s = (
+            f"The EIA technologies {_missing_techs} do not have an ATB counterpart with "
+            "valid fixed or variable O&M costs. All ATB technologies *should* have valid "
+            "fixed/variable O&M costs. Check the 'eia_atb_tech_map' parameter in your "
+            "settings file(s)."
+        )
+        logger.info(s)
 
     target_usd_year = settings["target_usd_year"]
     simple_o_m = {
         "Natural Gas Steam Turbine": {
             "variable_o_m_mwh": inflation_price_adjustment(1.0, 2017, target_usd_year)
         },
         "Coal": {
@@ -509,17 +589,17 @@
 
     mod_results = pd.concat(df_list, ignore_index=True)
 
     # Fill na FOM values, first by technology and then across all techs
     if not mod_results.loc[mod_results["Fixed_OM_Cost_per_MWyr"].isna()].empty:
         df_list = []
         for tech, _df in mod_results.groupby("technology"):
-            _df.loc[
-                _df["Fixed_OM_Cost_per_MWyr"].isna(), "Fixed_OM_Cost_per_MWyr"
-            ] = _df["Fixed_OM_Cost_per_MWyr"].mean()
+            _df.loc[_df["Fixed_OM_Cost_per_MWyr"].isna(), "Fixed_OM_Cost_per_MWyr"] = (
+                _df["Fixed_OM_Cost_per_MWyr"].mean()
+            )
             df_list.append(_df)
         mod_results = pd.concat(df_list, ignore_index=True)
         mod_results.loc[
             mod_results["Fixed_OM_Cost_per_MWyr"].isna(), "Fixed_OM_Cost_per_MWyr"
         ] = mod_results["Fixed_OM_Cost_per_MWyr"].mean()
     mod_results.loc[:, "Fixed_OM_Cost_per_MWyr"] = mod_results.loc[
         :, "Fixed_OM_Cost_per_MWyr"
@@ -614,15 +694,15 @@
                 f"should be a single value but is {new_build_hr}. This could cause "
                 f"issues with your variable O&M costs for {eia_tech}. Please report "
                 "this as an issue on the PowerGenome repository.\n"
             )
     except (ValueError, TypeError, KeyError):
         # Not all technologies have a heat rate. If they don't, just set both values
         # to 10.34 (33% efficiency)
-        df["heat_rate_mmbtu_mwh"] = 10.34
+        df.loc[df["heat_rate_mmbtu_mwh"].isna(), "heat_rate_mmbtu_mwh"] = 10.34
         new_build_hr = 10.34
 
     try:
         atb_var_om_mwh = atb_om_df.loc[
             (atb_tech, tech_detail, "variable_o_m_mwh"), "parameter_value"
         ]
     except KeyError:
@@ -644,15 +724,15 @@
             # Change CC and CT O&M to EIA NEMS values, which are much higher for CCs and
             # lower for CTs than a heat rate & linear mulitpler correction to the ATB
             # values.
             # Add natural gas steam turbine O&M.
             # Also using the new values for coal plants, assuming 40-50 yr age and half
             # FGD
             # https://www.eia.gov/analysis/studies/powerplants/generationcost/pdf/full_report.pdf
-            # logger.info(f"Using NEMS values for {eia_tech} fixed/variable O&M")
+            # logger.debug(f"Using NEMS values for {eia_tech} fixed/variable O&M")
 
             if "Combined Cycle" in eia_tech:
                 # https://www.eia.gov/analysis/studies/powerplants/generationcost/pdf/full_report.pdf
                 assert not _df[settings["capacity_col"]].isnull().all()
                 plant_capacity = _df[settings["capacity_col"]].sum()
                 if plant_capacity < 500:
                     fixed = 15.62 * 1000
@@ -798,17 +878,17 @@
                     # fixed[age >= 30] *= (27+37) * 1000
 
                 _df["Fixed_OM_Cost_per_MWyr"] = inflation_price_adjustment(
                     fixed, 2015, target_usd_year
                 )
 
                 # If nuclear heat rates are NaN, set them to new build value
-                _df.loc[
-                    _df["heat_rate_mmbtu_mwh"].isna(), "heat_rate_mmbtu_mwh"
-                ] = new_build_hr
+                _df.loc[_df["heat_rate_mmbtu_mwh"].isna(), "heat_rate_mmbtu_mwh"] = (
+                    new_build_hr
+                )
                 _df["Var_OM_Cost_per_MWh"] = atb_var_om_mwh * (
                     _df["heat_rate_mmbtu_mwh"].mean() / new_build_hr
                 )
 
             df_list.append(_df)
 
         return pd.concat(df_list, ignore_index=True)
@@ -891,31 +971,14 @@
     row = pd.DataFrame([technology, cost_case, tech_detail] + s.to_list(), index=cols).T
 
     row["Cap_Size"] = size_mw
 
     return row
 
 
-def investment_cost_calculator(capex, wacc, cap_rec_years):
-    capex = np.asarray(capex, dtype=float)
-    wacc = np.asarray(wacc, dtype=float)
-
-    for variable in capex, wacc, cap_rec_years:
-        if np.isnan(variable).any():
-            raise ValueError(f"Investment costs contains nan values")
-
-    inv_cost = capex * (
-        np.exp(wacc * cap_rec_years)
-        * (np.exp(wacc) - 1)
-        / (np.exp(wacc * cap_rec_years) - 1)
-    )
-
-    return inv_cost
-
-
 def regional_capex_multiplier(
     df: pd.DataFrame,
     region: str,
     region_map: Dict[str, str],
     tech_map: Dict[str, str],
     regional_multipliers: pd.DataFrame,
 ) -> pd.DataFrame:
@@ -1051,15 +1114,15 @@
     DataFrame
         New generating resources in every region. Contains the columns:
         ['technology', 'basis_year', 'Fixed_OM_Cost_per_MWyr',
        'Fixed_OM_Cost_per_MWhyr', 'Var_OM_Cost_per_MWh', 'capex', 'capex_mwh',
        'Inv_Cost_per_MWyr', 'Inv_Cost_per_MWhyr', 'Heat_Rate_MMBTU_per_MWh',
        'Cap_Size', 'region']
     """
-    logger.info("Creating new resources for each region.")
+    logger.debug("Creating new resources for each region.")
     new_gen_types = settings["atb_new_gen"]
     model_year = settings["model_year"]
     try:
         first_planning_year = settings["model_first_planning_year"]
         model_year_range = range(first_planning_year, model_year + 1)
     except KeyError:
         model_year_range = list(range(model_year + 1))
@@ -1190,20 +1253,22 @@
                 "cap_recovery_years",
             ] = years
 
         new_gen_df["Inv_Cost_per_MWyr"] = investment_cost_calculator(
             capex=new_gen_df["capex_mw"],
             wacc=new_gen_df["wacc_real"],
             cap_rec_years=new_gen_df["cap_recovery_years"],
+            compound_method=settings.get("interest_compound_method", "discrete"),
         )
 
         new_gen_df["Inv_Cost_per_MWhyr"] = investment_cost_calculator(
             capex=new_gen_df["capex_mwh"],
             wacc=new_gen_df["wacc_real"],
             cap_rec_years=new_gen_df["cap_recovery_years"],
+            compound_method=settings.get("interest_compound_method", "discrete"),
         )
 
         # Set no capacity limit on new resources that aren't renewables.
         new_gen_df["Max_Cap_MW"] = -1
         new_gen_df["Max_Cap_MWh"] = -1
         regional_cost_multipliers = pd.read_csv(
             DATA_PATHS["cost_multipliers"]
@@ -1247,15 +1312,15 @@
         results = pd.concat(df_list, ignore_index=True, sort=False)
 
         int_cols = [
             "Fixed_OM_Cost_per_MWyr",
             "Fixed_OM_Cost_per_MWhyr",
             "Inv_Cost_per_MWyr",
             "Inv_Cost_per_MWhyr",
-            "cluster",
+            # "cluster",
         ]
         int_cols = [c for c in int_cols if c in results.columns]
         results = results.fillna(0)
         results[int_cols] = results[int_cols].astype(int)
         results["Var_OM_Cost_per_MWh"] = results["Var_OM_Cost_per_MWh"].astype(float)
 
     return results
@@ -1339,16 +1404,19 @@
     data = rg.metadata.read(cache=cache)
     data.columns = snake_case_col(data.columns)
     if "metro_region" in data.columns and "region" not in data.columns:
         data["region"] = data.loc[:, "metro_region"]
     if "cpa_mw" in data.columns and "mw" not in data.columns:
         data["mw"] = data.loc[:, "cpa_mw"]
     data = data.loc[data["mw"] > 0, :]
-    profile_path = Path(rg.group["profiles"])
-    if rg.group.get("site_map"):
+    if rg.group.get("profiles"):
+        profile_path = Path(rg.group["profiles"])
+    else:
+        profile_path = None
+    if rg.group.get("site_map") and profile_path is not None:
         table = Table(profile_path.parent / rg.group["site_map"])
         cols = table.columns
         df = table.read().set_index(cols[0])
         site_map = df[df.columns[0]]
     else:
         site_map = None
 
@@ -1423,15 +1491,17 @@
         NREL ATB technologies are not unique.
     ValueError
         Renewables clusters do not match NREL ATB technologies.
     ValueError
         Renewables clusters match multiple NREL ATB technologies.
     """
     if not cluster_builder:
-        cluster_builder = build_resource_clusters(settings.get("RESOURCE_GROUPS"))
+        cluster_builder = build_resource_clusters(
+            settings.get("RESOURCE_GROUPS"), settings.get("RESOURCE_GROUP_PROFILES")
+        )
     if not df["technology"].is_unique:
         raise ValueError(
             f"NREL ATB technologies are not unique: {df['technology'].to_list()}"
         )
     atb_map = {
         x: map_nrel_atb_technology(x.split("_")[0], x.split("_")[1])
         for x in df["technology"]
@@ -1492,33 +1562,50 @@
                     "technology",
                     "max_clusters",
                     "min_capacity",
                     "filter",
                     "bin",
                     "group",
                     "cluster",
+                    "group_modifiers",
                 ]
             ]
         )
-        detail_suffix = flatten_cluster_def(_scenario, "_")
-        cache_cluster_fn = f"{region}_{technology}_{detail_suffix}_cluster_data.parquet"
-        cache_site_assn_fn = f"{region}_{technology}_{detail_suffix}_site_assn.parquet"
-        sub_folder = SETTINGS.get("RESOURCE_GROUPS") or settings["RESOURCE_GROUPS"]
+        detail_suffix = flatten_cluster_def(
+            {k: v for (k, v) in _scenario.items() if k != "group_modifiers"}, "_"
+        )
+        unique_hash = hash_string_sha256(f"{region}_{technology}_{detail_suffix}")
+        cache_cluster_fn = unique_hash + "_cluster_data.parquet"
+        cache_site_assn_fn = unique_hash + "_site_assn.parquet"
+
+        sub_folder = settings.get("RESOURCE_GROUPS") or SETTINGS.get("RESOURCE_GROUPS")
         sub_folder = str(sub_folder).replace("/", "_").replace("\\", "_")
         cache_folder = Path(
             settings["input_folder"] / "cluster_assignments" / sub_folder
         )
+        add_row_to_csv(
+            cache_folder / "hash_map.csv",
+            headers=["name", "hash"],
+            new_row=[f"{region}_{technology}_{detail_suffix}", unique_hash],
+        )
         cache_cluster_fpath = cache_folder / cache_cluster_fn
         cache_site_assn_fpath = cache_folder / cache_site_assn_fn
         if precluster is False:
             if cache_cluster_fpath.exists() and cache_site_assn_fpath.exists():
                 clusters = pd.read_parquet(cache_cluster_fpath)
                 data = pd.read_parquet(cache_site_assn_fpath)
             else:
-                drop_keys = ["min_capacity", "filter", "bin", "group", "cluster"]
+                drop_keys = [
+                    "min_capacity",
+                    "filter",
+                    "bin",
+                    "group",
+                    "cluster",
+                    "group_modifiers",
+                ]
                 group_kwargs = dict(
                     [(k, v) for k, v in _scenario.items() if k not in drop_keys]
                 )
                 resource_groups = cluster_builder.find_groups(
                     existing=False,
                     **group_kwargs,
                 )
@@ -1542,15 +1629,15 @@
                     utc_offset=settings.get("utc_offset", 0),
                     **_scenario,
                 )
                 if data.empty:
                     continue
                 clusters = (
                     data.groupby("cluster", as_index=False)
-                    .apply(calc_cluster_values)
+                    .apply(calc_cluster_values, _scenario.get("group"))
                     .rename(columns={"mw": "Max_Cap_MW"})
                     .assign(technology=technology, region=region)
                 )
 
                 cache_folder.mkdir(parents=True, exist_ok=True)
                 if not cache_cluster_fpath.exists():
                     clusters.to_parquet(cache_cluster_fpath)
@@ -1581,30 +1668,34 @@
                     .assign(technology=technology, region=region)
                 )
                 clusters["cluster"] = range(1, 1 + len(clusters))
                 data = None
         cache_folder.mkdir(parents=True, exist_ok=True)
         if not cache_cluster_fpath.exists():
             clusters.to_parquet(cache_cluster_fpath)
-        if not cache_site_assn_fpath.exists() and not data is None:
+        if not cache_site_assn_fpath.exists() and data is not None:
             cols = ["cpa_id", "cluster"]
             data[cols].to_parquet(cache_site_assn_fpath)
         if _scenario.get("min_capacity"):
             # Warn if total capacity less than expected
             capacity = clusters["Max_Cap_MW"].sum()
-            if capacity < scenario["min_capacity"]:
+            if capacity < _scenario["min_capacity"]:
                 logger.warning(
                     f"Selected technology {_scenario['technology']} capacity"
                     + f" in region {region}"
                     + f" less than minimum ({capacity} < {_scenario['min_capacity']} MW)"
                 )
         row = df[df["technology"] == technology].to_dict("records")[0]
         clusters["technology"] = clusters["technology"] + new_tech_suffix
         kwargs = {k: v for k, v in row.items() if k not in clusters}
-        cdfs.append(clusters.assign(**kwargs))
+        cdfs.append(
+            clusters.assign(**kwargs).pipe(
+                modify_renewable_group, _scenario.get("group_modifiers")
+            )
+        )
     return pd.concat([df[~mask]] + cdfs, sort=False)
 
 
 def load_user_defined_techs(settings: dict) -> pd.DataFrame:
     """Load user-defined technologies from a CSV file. Returns cost columns and heat
     rate.
```

### Comparing `PowerGenome-0.6.1a0/powergenome/params.py` & `powergenome-0.6.2/powergenome/params.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 """
 Parameters and settings
 """
+
 import os
 from pathlib import Path
 from typing import Union
 
-from dotenv import find_dotenv, load_dotenv
+from dotenv import load_dotenv
 
 from powergenome import __file__
 from powergenome.resource_clusters import ClusterBuilder
 from powergenome.util import sqlalchemy_prefix
 
 # Not convinced this is the best way to set folder paths but it works!
 powergenome_path = Path(__file__).parent
@@ -44,17 +45,23 @@
 SETTINGS["PG_DB"] = sqlalchemy_prefix(os.environ.get("PG_DB"))
 SETTINGS["EFS_DATA"] = os.environ.get("EFS_DATA")
 SETTINGS["RESOURCE_GROUPS"] = os.environ.get("RESOURCE_GROUPS")
 SETTINGS["DISTRIBUTED_GEN_DATA"] = os.environ.get("DISTRIBUTED_GEN_DATA")
 SETTINGS["RESOURCE_GROUP_PROFILES"] = os.environ.get("RESOURCE_GROUP_PROFILES")
 
 
-def build_resource_clusters(group_path: Union[str, Path] = None):
+def build_resource_clusters(
+    group_path: Union[str, Path] = None, profile_path: Union[str, Path] = None
+) -> ClusterBuilder:
     if not group_path:
         group_path = SETTINGS.get("RESOURCE_GROUPS")
+    if not profile_path:
+        profile_path = SETTINGS.get("RESOURCE_GROUP_PROFILES")
+    if profile_path is not None:
+        profile_path = Path(profile_path)
     if not group_path:
         cluster_builder = ClusterBuilder([])
     else:
         cluster_builder = ClusterBuilder.from_json(
-            Path(group_path, ".").glob("**/*.json")
+            Path(group_path, ".").glob("**/*.json"), profile_path
         )
     return cluster_builder
```

### Comparing `PowerGenome-0.6.1a0/powergenome/resource_clusters.py` & `powergenome-0.6.2/powergenome/resource_clusters.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import copy
-import glob
 import json
 import os
 import re
 from pathlib import Path
-from typing import Any, Callable, Dict, Iterable, List, Mapping, Optional, Union
+from typing import Any, Dict, Iterable, List, Mapping, Optional, Union
 
 import numpy as np
 import pandas as pd
 import pyarrow
 import pyarrow.parquet as pq
 import scipy.cluster.hierarchy
 
@@ -267,15 +266,15 @@
                 raise ValueError("Dataframe columns are not all strings")
         self.format = None
         self._dataset = None
         self._columns = None
         if path is not None:
             try:
                 self._dataset = pq.ParquetDataset(path)
-                self._columns = self._dataset.schema.names
+                self._columns = pq.read_schema(path).names
                 self.format = "parquet"
             except pyarrow.lib.ArrowInvalid:
                 # Assume CSV file
                 self.format = "csv"
         if path is None and df is None:
             raise ValueError("Mising either path to tabular data or a pandas DataFrame")
 
@@ -434,25 +433,31 @@
 
     def __init__(
         self,
         group: Dict[str, Any],
         metadata: pd.DataFrame = None,
         profiles: pd.DataFrame = None,
         path: str = ".",
+        profile_path: str = None,
     ) -> None:
         from powergenome.params import SETTINGS
 
         self.group = {"existing": False, "tree": None, **group.copy()}
 
         # Convert relative paths (relative to group file) to absolute paths
         # Profiles may be stored in a single location and reused across resource groups
         if self.group.get("metadata"):
             self.group["metadata"] = Path(path) / self.group["metadata"]
         if self.group.get("profiles"):
-            if (
+            # Check for location passed as an arg (probably from settings file),
+            # then the SETTINGS (from .env file), then assume they are in the same folder
+            # as the JSON file
+            if profile_path and (profile_path / self.group["profiles"]).exists():
+                self.group["profiles"] = Path(profile_path) / self.group["profiles"]
+            elif (
                 SETTINGS.get("RESOURCE_GROUP_PROFILES")
                 and (
                     Path(SETTINGS["RESOURCE_GROUP_PROFILES"]) / self.group["profiles"]
                 ).exists()
             ):
                 self.group["profiles"] = (
                     Path(SETTINGS["RESOURCE_GROUP_PROFILES"]) / self.group["profiles"]
@@ -469,26 +474,28 @@
             )
         self.metadata = Table(df=metadata, path=self.group.get("metadata"))
         self.profiles = None
         if profiles is not None or self.group.get("profiles"):
             self.profiles = Table(df=profiles, path=self.group.get("profiles"))
 
     @classmethod
-    def from_json(cls, path: Union[str, os.PathLike]) -> "ResourceGroup":
+    def from_json(
+        cls, path: Union[str, os.PathLike], profile_path: Union[str, os.PathLike] = None
+    ) -> "ResourceGroup":
         """
         Build from JSON file.
 
         Parameters
         ----------
         path
             Path to JSON file.
         """
         with open(path, mode="r") as fp:
             group = json.load(fp)
-        return cls(group, path=os.path.dirname(path))
+        return cls(group, path=os.path.dirname(path), profile_path=profile_path)
 
     def test_metadata(self) -> None:
         """
         Test that `:attr:metadata` is valid.
 
         Raises
         ------
@@ -517,19 +524,19 @@
         if self.profiles is None:
             return None
         # Cast identifiers to string to match profile columns
         ids = self.metadata.read(columns=["id"])["id"].astype(str)
         columns = self.profiles.columns
         if not set(columns) == set(ids):
             raise ValueError(
-                f"Resource profiles column names do not match resource identifiers"
+                "Resource profiles column names do not match resource identifiers"
             )
         df = self.profiles.read(columns=columns[0])
         if len(df) not in [8760, 8784]:
-            raise ValueError(f"Resource profiles are not either 8760 or 8784 elements")
+            raise ValueError("Resource profiles are not either 8760 or 8784 elements")
 
     def get_clusters(
         self,
         ipm_regions: Iterable[str] = None,
         min_capacity: float = None,
         max_clusters: int = None,
         max_lcoe: float = None,
@@ -615,15 +622,15 @@
             temp = (df.loc[mask, CAPACITY].cumsum() < min_capacity).values
             temp[temp.argmin()] = True
             mask[mask] = temp
         if max_lcoe and "lcoe" in df:
             # Select clusters with LCOE below the cutoff
             mask[mask] = df.loc[mask, "lcoe"] <= max_lcoe
         if not mask.any():
-            raise ValueError(f"No resources found or selected")
+            raise ValueError("No resources found or selected")
         if tree:
             # Only keep trees with one ore more base resources
             if isinstance(tree, list):
                 df["tree"] = ""
                 for t in tree:
                     df["tree"] += df[t].astype(str)
             else:
@@ -705,15 +712,19 @@
     ValueError: No resources found or selected
     """
 
     def __init__(self, groups: Iterable[ResourceGroup]) -> None:
         self.groups = groups
 
     @classmethod
-    def from_json(cls, paths: Iterable[Union[str, os.PathLike]]) -> "ClusterBuilder":
+    def from_json(
+        cls,
+        paths: Iterable[Union[str, os.PathLike]],
+        profile_path: Union[str, os.PathLike] = None,
+    ) -> "ClusterBuilder":
         """
         Load resources from resource group JSON files.
 
         Parameters
         ----------
         paths
             Paths to resource group JSON files.
@@ -722,15 +733,15 @@
         ------
         ValueError
             No resource groups specified.
         """
         paths = list(paths)
         if not paths:
             raise ValueError(f"No resource groups specified {paths}")
-        return cls([ResourceGroup.from_json(path) for path in paths])
+        return cls([ResourceGroup.from_json(path, profile_path) for path in paths])
 
     def find_groups(self, **kwargs: Any) -> List[ResourceGroup]:
         """
         Return the resource groups matching the specified arguments.
 
         Parameters
         ----------
```

### Comparing `PowerGenome-0.6.1a0/powergenome/run_powergenome_multiple_outputs_cli.py` & `powergenome-0.6.2/powergenome/run_powergenome_multiple_outputs_cli.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import argparse
-import copy
 import logging
 import shutil
 import sys
 from datetime import datetime as dt
 from pathlib import Path
 
 import pandas as pd
@@ -11,25 +10,21 @@
 import powergenome
 from powergenome.external_data import (
     insert_user_tx_costs,
     load_user_tx_costs,
     make_generator_variability,
 )
 from powergenome.fuels import fuel_cost_table
-from powergenome.generators import (
-    GeneratorClusters,
-    add_fuel_labels,
-    add_genx_model_tags,
-)
+from powergenome.generators import GeneratorClusters
 from powergenome.GenX import (
     add_cap_res_network,
     add_co2_costs_to_o_m,
     add_misc_gen_values,
-    calculate_partial_CES_values,
     check_resource_tags,
+    check_vre_profiles,
     create_policy_req,
     create_regional_cap_res,
     fix_min_power_values,
     hydro_energy_to_power,
     max_cap_req,
     min_cap_req,
     network_line_loss,
@@ -37,28 +32,26 @@
     network_reinforcement_cost,
     reduce_time_domain,
     round_col_values,
     set_int_cols,
     set_must_run_generation,
 )
 from powergenome.load_profiles import make_final_load_curves
-from powergenome.nrelatb import atb_fixed_var_om_existing
 from powergenome.transmission import (
     agg_transmission_constraints,
     transmission_line_distance,
 )
 from powergenome.util import (
     build_scenario_settings,
     check_settings,
     init_pudl_connection,
     load_ipm_shapefile,
     load_settings,
     remove_fuel_gen_scenario_name,
     remove_fuel_scenario_name,
-    update_dictionary,
     write_case_settings_file,
     write_results_file,
 )
 
 if not sys.warnoptions:
     import warnings
 
@@ -128,55 +121,86 @@
         dest="sort_gens",
         action="store_true",
         help=(
             "Sort generators alphabetically within region. Existing resources will "
             "still be separate from new resources."
         ),
     )
+    parser.add_argument(
+        "-c",
+        "--case-id",
+        dest="case_id",
+        nargs="*",
+        help=(
+            "One or more case IDs to select from the scenario inputs file. Only these "
+            "cases will be used."
+        ),
+    )
+    parser.add_argument(
+        "-mp",
+        "--multi-period",
+        dest="multi_period",
+        action="store_true",
+        help=("Use multi-period output format."),
+    )
     arguments = parser.parse_args(argv[1:])
     return arguments
 
 
 def main(**kwargs):
     args = parse_command_line(sys.argv)
     args.__dict__.update(kwargs)
     cwd = Path.cwd()
 
     out_folder = cwd / args.results_folder
     out_folder.mkdir(exist_ok=True)
 
     # Create a logger to output any messages we might have...
     logger = logging.getLogger(powergenome.__name__)
-    logger.setLevel(logging.INFO)
+    logger.setLevel(logging.DEBUG)
     handler = logging.StreamHandler()
-    formatter = logging.Formatter(
+    stream_formatter = logging.Formatter(
         # More extensive test-like formatter...
         "%(asctime)s [%(levelname)8s] %(name)s:%(lineno)s %(message)s",
         # This is the datetime format string.
-        "%Y-%m-%d %H:%M:%S",
+        "%H:%M:%S",
     )
-    handler.setFormatter(formatter)
+    handler.setFormatter(stream_formatter)
+    handler.setLevel(logging.INFO)
     logger.addHandler(handler)
 
+    file_formatter = logging.Formatter(
+        # More extensive test-like formatter...
+        "%(asctime)s [%(levelname)8s] %(name)s:%(lineno)s %(message)s",
+        # This is the datetime format string.
+        "%Y-%m-%d %H:%M:%S",
+    )
     filehandler = logging.FileHandler(out_folder / "log.txt")
-    filehandler.setFormatter(formatter)
+    filehandler.setLevel(logging.DEBUG)
+    filehandler.setFormatter(file_formatter)
     logger.addHandler(filehandler)
 
+    if not args.multi_period:
+        logger.info(
+            "As of version 0.6.2 the --multi-period/-mp flag can be used to format inputs "
+            "for multi-stage modeling in GenX."
+        )
+
     logger.info("Reading settings file")
     settings = load_settings(path=args.settings_file)
 
     # Copy the settings file to results folder
     if Path(args.settings_file).is_file():
         shutil.copy(args.settings_file, out_folder)
     else:
         shutil.copytree(
             args.settings_file, out_folder / "pg_settings", dirs_exist_ok=True
         )
 
-    logger.info("Initiating PUDL connections")
+    logger.debug("Initiating PUDL connections")
 
     pudl_engine, pudl_out, pg_engine = init_pudl_connection(
         freq="AS",
         start_year=min(settings.get("eia_data_years")),
         end_year=max(settings.get("eia_data_years")),
         pudl_db=settings.get("PUDL_DB"),
         pg_db=settings.get("PG_DB"),
@@ -200,113 +224,171 @@
             "One or more model regions is not valid. Check to make sure all regions "
             "are either in IPM or region_aggregations in the settings YAML file."
         )
 
     # Sort zones in the settings to make sure they are correctly sorted everywhere.
     settings["model_regions"] = sorted(settings["model_regions"])
     zones = settings["model_regions"]
-    logger.info(f"Sorted zones are {', '.join(zones)}")
+    logger.info(f"Sorted model regions are {', '.join(zones)}")
     zone_num_map = {
         zone: f"{number + 1}" for zone, number in zip(zones, range(len(zones)))
     }
 
-    input_folder = Path(args.settings_file).parent / settings["input_folder"]
+    input_folder = Path(args.settings_file).parent / Path(settings["input_folder"]).name
     settings["input_folder"] = input_folder
 
     scenario_definitions = pd.read_csv(
         input_folder / settings["scenario_definitions_fn"]
     )
 
+    if args.case_id:
+        missing_case_ids = set(args.case_id) - set(scenario_definitions["case_id"])
+        if missing_case_ids:
+            raise ValueError(
+                f"The requested case IDs {missing_case_ids} are not in your scenario "
+                "inputs file."
+            )
+        scenario_definitions = scenario_definitions.loc[
+            scenario_definitions["case_id"].isin(args.case_id), :
+        ]
+
     if set(scenario_definitions["year"]) != set(settings["model_year"]):
         logger.warning(
             f"The years included the secenario definitions file ({set(scenario_definitions['year'])}) "
             f"does not match the settings parameter `model_year` ({settings['model_year']})"
         )
     assert len(settings["model_year"]) == len(
         settings["model_first_planning_year"]
     ), "The number of years in the settings parameter 'model_year' must be the same as 'model_first_planning_year'"
 
     # Build a dictionary of settings for every planning year and case_id
     scenario_settings = build_scenario_settings(settings, scenario_definitions)
+    period_map = {}
+    for case, _df in scenario_definitions.groupby(["case_id"]):
+        period_map[case] = {}
+        for idx, year in enumerate(_df["year"].sort_values()):
+            period_map[case][year] = idx + 1
 
-    i = 0
     model_regions_gdf = None
+    first_year = True
     for year in scenario_settings:
         for case_id, _settings in scenario_settings[year].items():
-            case_folder = (
-                out_folder / f"{year}" / f"{case_id}_{year}_{_settings['case_name']}"
-            )
+            if not args.multi_period:
+                if settings.get("case_name"):
+                    case_folder = (
+                        out_folder
+                        / f"{year}"
+                        / f"{case_id}_{year}_{_settings['case_name']}"
+                    )
+                else:
+                    case_folder = out_folder / f"{year}" / f"{case_id}_{year}"
+            else:
+                if settings.get("case_name"):
+                    case_folder = (
+                        out_folder
+                        / f"{case_id}_{_settings['case_name']}"
+                        / "Inputs"
+                        / f"Inputs_p{period_map[case_id][year]}"
+                    )
+                else:
+                    case_folder = (
+                        out_folder
+                        / f"{case_id}"
+                        / "Inputs"
+                        / f"Inputs_p{period_map[case_id][year]}"
+                    )
             _settings["extra_outputs"] = case_folder / "extra_outputs"
             _settings["extra_outputs"].mkdir(parents=True, exist_ok=True)
-            logger.info(f"Starting year {year} scenario {case_id}\n")
+            logger.info(f"\n\nStarting year {year} scenario {case_id}\n\n")
             if args.gens:
                 gc = GeneratorClusters(
                     pudl_engine=pudl_engine,
                     pudl_out=pudl_out,
                     pg_engine=pg_engine,
                     settings=_settings,
                     current_gens=args.current_gens,
                     sort_gens=args.sort_gens,
+                    multi_period=args.multi_period,
+                    include_retired_cap=first_year is False,
                 )
                 gen_clusters = gc.create_all_generators()
                 if args.fuel and args.gens:
                     fuels = fuel_cost_table(
                         fuel_costs=gc.fuel_prices,
                         generators=gc.all_resources,
                         settings=_settings,
                     )
                     fuels.index.name = "Time_Index"
                     write_results_file(
                         df=remove_fuel_scenario_name(fuels, _settings),
                         folder=case_folder,
                         file_name="Fuels_data.csv",
                         include_index=True,
+                        multi_period=args.multi_period,
                     )
 
                 gen_clusters["Zone"] = gen_clusters["region"].map(zone_num_map)
                 gen_clusters = add_misc_gen_values(gen_clusters, _settings)
                 gen_clusters = hydro_energy_to_power(
                     gen_clusters,
                     _settings.get("hydro_factor"),
                     _settings.get("regional_hydro_factor", {}),
                 )
 
-                # Save existing resources that aren't demand response for use in
-                # other cases
-                existing_gens = gc.existing_resources.copy()
-
                 gen_variability = make_generator_variability(gen_clusters)
                 gen_variability.index.name = "Time_Index"
                 gen_variability.columns = gen_clusters["Resource"]
                 if "MUST_RUN" in gen_clusters.columns:
                     gen_variability = set_must_run_generation(
                         gen_variability,
                         gen_clusters.loc[
                             gen_clusters["MUST_RUN"] == 1, "Resource"
                         ].to_list(),
                     )
                 gens = fix_min_power_values(gen_clusters, gen_variability).pipe(
                     add_co2_costs_to_o_m
                 )
+                check_vre_profiles(gens, gen_variability)
                 for col in _settings["generator_columns"]:
                     if col not in gens.columns:
                         gens[col] = 0
-                cols = [c for c in _settings["generator_columns"] if c in gens]
 
+                # Some extra fixes for multi-period
+                gens = gens.rename(
+                    columns={
+                        "cap_recovery_years": "Capital_Recovery_Period",
+                        "wacc_real": "WACC",
+                    }
+                )
+                gens["Lifetime"] = gens["Capital_Recovery_Period"]
+                gens.loc[
+                    (gens["Lifetime"] == 0) | (gens["Lifetime"].isna()), "Lifetime"
+                ] = 50
+                cols = [c for c in _settings["generator_columns"] if c in gens]
+                cols.extend(["Capital_Recovery_Period", "WACC", "Lifetime"])
                 write_results_file(
                     df=remove_fuel_gen_scenario_name(gens[cols].fillna(0), _settings)
                     .pipe(set_int_cols)
                     .pipe(round_col_values)
                     .pipe(check_resource_tags),
                     folder=case_folder,
                     file_name="Generators_data.csv",
                     include_index=False,
+                    multi_period=args.multi_period,
                 )
+                if not args.load:
+                    write_results_file(
+                        df=gen_variability,
+                        folder=case_folder,
+                        file_name="Generators_variability.csv",
+                        include_index=True,
+                        float_format="%.3f",
+                        multi_period=args.multi_period,
+                    )
 
-                i += 1
             if args.transmission:
                 if args.gens is False:
                     model_regions_gdf = load_ipm_shapefile(_settings)
 
             if args.load:
                 load = make_final_load_curves(pg_engine=pg_engine, settings=_settings)
                 load.columns = "Load_MW_z" + load.columns.map(zone_num_map)
@@ -319,51 +401,55 @@
                 ) = reduce_time_domain(gen_variability, load, _settings)
                 reduced_resource_profile.index.name = "Time_Index"
                 write_results_file(
                     df=reduced_load_profile,
                     folder=case_folder,
                     file_name="Load_data.csv",
                     include_index=False,
+                    multi_period=args.multi_period,
                 )
 
                 write_results_file(
                     df=reduced_resource_profile,
                     folder=case_folder,
                     file_name="Generators_variability.csv",
                     include_index=True,
                     float_format="%.3f",
+                    multi_period=args.multi_period,
                 )
                 if time_series_mapping is not None:
                     write_results_file(
                         df=time_series_mapping,
                         folder=case_folder,
                         file_name="Period_map.csv",
                         include_index=False,
+                        multi_period=args.multi_period,
                     )
                 if representative_point is not None:
                     write_results_file(
                         df=representative_point,
                         folder=case_folder,
                         file_name="Representative_Period.csv",
                         include_index=False,
+                        multi_period=args.multi_period,
                     )
 
             if args.transmission:
-                model_regions_gdf = gc.model_regions_gdf
                 if _settings.get("user_transmission_costs"):
                     user_tx_costs = load_user_tx_costs(
                         _settings["input_folder"]
                         / _settings["user_transmission_costs"],
                         _settings["model_regions"],
                         _settings.get("target_usd_year"),
                     )
                     transmission = agg_transmission_constraints(
                         pg_engine=pg_engine, settings=_settings
                     ).pipe(insert_user_tx_costs, user_costs=user_tx_costs)
                 else:
+                    model_regions_gdf = gc.model_regions_gdf
                     transmission = (
                         agg_transmission_constraints(
                             pg_engine=pg_engine, settings=_settings
                         )
                         .pipe(
                             transmission_line_distance,
                             ipm_shapefile=model_regions_gdf,
@@ -391,56 +477,72 @@
                     energy_share_req = None
                     co2_cap = None
                 min_cap = min_cap_req(_settings)
                 max_cap = max_cap_req(_settings)
 
                 cap_res = create_regional_cap_res(_settings)
 
+                if args.multi_period:
+                    for line in network["Network_Lines"].dropna():
+                        network.loc[
+                            network["Network_Lines"] == line,
+                            "Line_Max_Flow_Possible_MW",
+                        ] = 1e6
+                        network.loc[
+                            network["Network_Lines"] == line, "Capital_Recovery_Period"
+                        ] = 60
+                        network.loc[network["Network_Lines"] == line, "WACC"] = 0.044
                 write_results_file(
                     df=network,
                     folder=case_folder,
                     file_name="Network.csv",
                     include_index=False,
+                    multi_period=args.multi_period,
                 )
                 if energy_share_req is not None:
                     write_results_file(
                         df=energy_share_req,
                         folder=case_folder,
                         file_name="Energy_share_requirement.csv",
                         include_index=False,
+                        multi_period=args.multi_period,
                     )
                 if cap_res is not None:
                     write_results_file(
                         df=cap_res,
                         folder=case_folder,
                         file_name="Capacity_reserve_margin.csv",
                         include_index=True,
+                        multi_period=args.multi_period,
                     )
                 if co2_cap is not None:
                     co2_cap = co2_cap.set_index("Region_description")
                     co2_cap.index.name = None
                     write_results_file(
                         df=co2_cap,
                         folder=case_folder,
                         file_name="CO2_cap.csv",
                         include_index=True,
+                        multi_period=args.multi_period,
                     )
                 if min_cap is not None:
                     write_results_file(
                         df=min_cap,
                         folder=case_folder,
                         file_name="Minimum_capacity_requirement.csv",
                         include_index=False,
+                        multi_period=args.multi_period,
                     )
                 if max_cap is not None:
                     write_results_file(
                         df=max_cap,
                         folder=case_folder,
-                        file_name="Maximum_capacity_limit.csv",
+                        file_name="Maximum_capacity_requirement.csv",
                         include_index=False,
+                        multi_period=args.multi_period,
                     )
 
             if args.fuel and args.gens:
                 fuels = fuel_cost_table(
                     fuel_costs=gc.fuel_prices,
                     generators=gc.all_resources,
                     settings=_settings,
@@ -450,14 +552,15 @@
                 write_results_file(
                     df=remove_fuel_scenario_name(fuels, _settings)
                     .pipe(set_int_cols)
                     .pipe(round_col_values),
                     folder=case_folder,
                     file_name="Fuels_data.csv",
                     include_index=True,
+                    multi_period=args.multi_period,
                 )
             if _settings.get("reserves_fn"):
                 shutil.copy(
                     _settings["input_folder"] / _settings["reserves_fn"],
                     case_folder / "Inputs",
                 )
 
@@ -471,11 +574,12 @@
                     shutil.copy(f, genx_settings_folder)
 
             write_case_settings_file(
                 settings=_settings,
                 folder=case_folder,
                 file_name="powergenome_case_settings.yml",
             )
+            first_year = False
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `PowerGenome-0.6.1a0/powergenome/time_reduction.py` & `powergenome-0.6.2/powergenome/time_reduction.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,86 @@
 "Functions to cluster or otherwise reduce the number of hours in generation and load profiles"
 
 import datetime
+import logging
+from typing import List, Tuple
 
 import numpy as np
 import pandas as pd
 from sklearn.cluster import KMeans
 from sklearn.preprocessing import minmax_scale
 
+logger = logging.getLogger(__name__)
+
+
+def max_rep_periods(
+    resource_profiles: pd.DataFrame,
+    load_profiles: pd.DataFrame,
+    days_in_group: int,
+    num_clusters: int,
+) -> Tuple[pd.DataFrame, pd.DataFrame, List[int], pd.DataFrame, pd.DataFrame]:
+    """Shortcut clustering when every representative period is assigned once (e.g. 52 rep
+    weeks in a year).
+
+    Parameters
+    ----------
+    resource_profiles : pd.DataFrame
+        Hourly profiles of all resources
+    load_profiles : pd.DataFrame
+        Hourly demand profile in each region
+    days_in_group : int
+        Number of days in each period
+    num_clusters : int
+        Numer of representative periods
+
+    Returns
+    -------
+    Tuple[pd.DataFrame, pd.DataFrame, List[int], pd.DataFrame, pd.DataFrame]
+        Load and resource profile dataframes with first N hours, where N is
+        num_clusters * days_in_group * 24, the cluster weights (all values are 1),
+        a mapping of each period to the representative period and the month,
+        and the order of representative periods.
+    """
+    num_hours = num_clusters * days_in_group * 24
+    cluster_weights = [1] * num_clusters
+    time_series_mapping = pd.DataFrame(
+        data={
+            "Period_Index": range(1, 1 + num_clusters),
+            "Rep_Period_Index": range(1, 1 + num_clusters),
+            "Month": 0,
+        }
+    )
+    for Period_Index in time_series_mapping["Period_Index"]:
+        dayOfYear = days_in_group * Period_Index
+        d = datetime.datetime.strptime("{} {}".format(dayOfYear, 2011), "%j %Y")
+        time_series_mapping["Month"][Period_Index - 1] = d.month
+    rep_point = [f"p{i}" for i in range(1, 1 + num_clusters)]
+    rep_point_df = pd.DataFrame(data=rep_point, columns=["slot"])
+
+    reduced_load_profiles = load_profiles.iloc[:num_hours, :].reset_index(drop=True)
+    reduced_resouce_profiles = resource_profiles.iloc[:num_hours, :]
+
+    return (
+        reduced_load_profiles,
+        reduced_resouce_profiles,
+        cluster_weights,
+        time_series_mapping,
+        rep_point_df,
+    )
+
 
 def kmeans_time_clustering(
     resource_profiles,
     load_profiles,
     days_in_group,
     num_clusters,
     include_peak_day=True,
     load_weight=1,
     variable_resources_only=True,
+    n_init=100,
 ):
     """Reduce the number of hours in load and resource variability timeseries using
     kmeans clustering.
 
     This script is adapted from work originally created by Dharik Mallapragada. For more
     information see:
     - Mallapragada, D. S., Papageorgiou, D. J., Venkatesh, A., Lara, C. L., & Grossmann,
@@ -48,27 +109,65 @@
         If the days with system peak demand should be included in outputs, by default
         True
     load_weight : int, optional
         A weighting factor for load profiles during clustering, by default 1
     variable_resources_only : bool, optional
         If clustering should only consider resources with variable (non-zero standard
         deviation) profiles, by default True
+    n_init : int, optional
+        Parameter for k-means clustering.
 
     Returns
     -------
     (dict, list, list)
         This function returns multiple items. The dict has keys ['load_profiles',
         'resource_profiles', 'ClusterWeights', 'AnnualGenScaleFactor', 'RMSE', and
         'AnnualProfile']
 
         The first list has strings with the order of periods selected e.g. ['p42','p26',
         'p3', 'p13', 'p32', 'p8'].
 
         The second list has integer weights of each cluster.
     """
+    logger.info("Reducing time domain from 8760 hours to representative periods")
+    # In cases where each cluster is selected exactly once, skip the clustering entirely
+    total_cluster_hours = days_in_group * num_clusters * 24
+    if len(load_profiles) - total_cluster_hours < days_in_group * 24:
+        (
+            load_df,
+            resource_df,
+            EachClusterWeight,
+            time_series_mapping,
+            EachClusterRepPoint,
+        ) = max_rep_periods(
+            resource_profiles=resource_profiles,
+            load_profiles=load_profiles,
+            days_in_group=days_in_group,
+            num_clusters=num_clusters,
+        )
+        rep_period_map = {
+            i + 1: int(p[1:]) for i, p in enumerate(EachClusterRepPoint["slot"])
+        }
+        time_series_mapping["Rep_Period"] = time_series_mapping["Rep_Period_Index"].map(
+            rep_period_map
+        )
+        return (
+            {
+                "load_profiles": load_df,  # Scaled Output Load and Renewables profiles for the sampled representative groupings
+                "resource_profiles": resource_df,
+                "ClusterWeights": EachClusterWeight,  # Weight of each for the representative groupings
+                "AnnualGenScaleFactor": 1,  # Scale factor used to adjust load output to match annual generation of original data
+                "RMSE": None,  # Root mean square error between full year data and modeled full year data (duration curves)
+                "AnnualProfile": None,
+                "time_series_mapping": time_series_mapping,
+            },
+            EachClusterRepPoint,
+            EachClusterWeight,
+        )
+
     resource_col_names = resource_profiles.columns
     if variable_resources_only:
         input_std = resource_profiles.describe().loc["std", :]
         var_col_names = input_std[input_std > 0].index.to_list()
         resource_profiles = resource_profiles.loc[:, var_col_names]
 
     # Initialize dataframes to store final and intermediate data in
@@ -99,15 +198,17 @@
     # and 1
     norm_tseries = pd.DataFrame(
         data=minmax_scale(input_data), columns=input_data.columns
     )
     norm_tseries.loc[:, load_col_names] *= load_weight
 
     # Identify hour with maximum system wide load
-    hr_maxSysLoad = input_data.loc[:, load_col_names].sum(axis=1).idxmax()
+    hr_maxSysLoad = (
+        input_data.loc[: total_cluster_hours - 1, load_col_names].sum(axis=1).idxmax()
+    )
     ################################ pre-processing data to create concatenated column
     # of load, pv and wind data
 
     # Number of such samples in a year - by avoiding division by float we are excluding
     # a few days in each sample set
     # Hence annual generation for each zone will not exactly match up with raw data
     # num_data_points = round(hours_per_year / 24 / days_in_group)
@@ -154,15 +255,15 @@
     # number of replications =100, squared euclidean distance
 
     if include_peak_day:  # If peak day in cluster, generate one less cluster
         num_clusters = num_clusters - 1
 
     # K-means clutering with 100 trials with randomly selected starting values
     model = KMeans(
-        n_clusters=num_clusters, n_init=100, init="k-means++", random_state=42
+        n_clusters=num_clusters, n_init=n_init, init="k-means++", random_state=42
     )
     model.fit(ClusteringInputDF.values.transpose())
 
     # Store clustered data
     # Create an empty list storing weight of each cluster
     EachClusterWeight = [None] * num_clusters
 
@@ -319,19 +420,15 @@
     }
 
     load_df = final_output_data.loc[:, load_col_names]
     # if variable_only:
     resource_df = pd.DataFrame(
         columns=resource_col_names, index=final_output_data.index
     )
-    for col in resource_col_names:
-        try:
-            resource_df[col] = final_output_data.loc[:, col].values
-        except KeyError:
-            pass
+    resource_df.loc[:, var_col_names] = final_output_data.loc[:, var_col_names]
     resource_df = resource_df.fillna(value=1)
 
     # load_df["Sub_Weights"] = np.nan
     # load_df.loc[: len(EachClusterWeight) - 1, "Sub_Weights"] = (
     #     np.array(EachClusterWeight) * NumGrpDays * 24
     # )
     # load_df.to_csv("load_time_reduced.csv", index=False)
```

### Comparing `PowerGenome-0.6.1a0/powergenome/transmission.py` & `powergenome-0.6.2/powergenome/transmission.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
     zone_num_map = {
         zone: f"z{number + 1}" for zone, number in zip(zones, range(len(zones)))
     }
 
     combos = list(itertools.combinations(zones, 2))
     reverse_combos = [(combo[-1], combo[0]) for combo in combos]
 
-    logger.info("Loading transmission constraints from PUDL")
+    logger.debug("Loading transmission constraints from the database")
     transmission_constraints_table = pd.read_sql_table(pg_table, con=pg_engine)
 
     if tx_value_col not in transmission_constraints_table.columns:
         raise KeyError(
             f"There is no column {tx_value_col} in the transmission capacity table '{pg_table}'"
         )
     if transmission_constraints_table.duplicated(
@@ -96,14 +96,15 @@
         ]
 
         raise KeyError(
             "The transmission table has duplicate lines. This table should only have unique lines.\n",
             dup_lines,
         )
     if settings.get("user_transmission_constraints_fn"):
+        logger.debug("Adding user-supplied transmission constraint data")
         user_tx_constraints = pd.read_csv(
             Path(settings["input_folder"])
             / settings["user_transmission_constraints_fn"]
         )
         if tx_value_col not in user_tx_constraints.columns:
             raise KeyError(
                 f"There is no column {tx_value_col} in the user supplied transmission capacity table"
@@ -130,16 +131,16 @@
             ]
         )
 
         if transmission_constraints_table.duplicated(
             subset=["region_from", "region_to"]
         ).any():
             logger.warning(
-                "The user transmission capacity table duplicates values from the "
-                "database. Database values will be discarded in favor of user values."
+                "The user transmission capacity table duplicates some values from the "
+                "database. Database values will be discarded in these cases."
             )
 
         transmission_constraints_table = transmission_constraints_table.drop_duplicates(
             keep="last"
         )
 
     # Settings has a dictionary of lists for regional aggregations. Need
@@ -158,15 +159,15 @@
     # we're using for aggregated regions
     transmission_constraints_table = transmission_constraints_table.loc[
         (transmission_constraints_table.region_from.isin(keep_regions))
         & (transmission_constraints_table.region_to.isin(keep_regions)),
         :,
     ].drop(columns="id", errors="ignore")
 
-    logger.info("Map and aggregate region names for transmission constraints")
+    logger.debug("Map and aggregate region names for transmission constraints")
     for col in ["region_from", "region_to"]:
         model_col = "model_" + col
 
         transmission_constraints_table = map_agg_region_names(
             df=transmission_constraints_table,
             region_agg_map=region_agg_map,
             original_col_name=col,
@@ -179,26 +180,26 @@
     ]
     transmission_constraints_table.drop(columns=drop_cols, inplace=True)
     transmission_constraints_table = transmission_constraints_table.groupby(
         ["model_region_from", "model_region_to"]
     ).sum()
 
     # Build the final output dataframe
-    logger.info(
+    logger.debug(
         "Build a new transmission constraints dataframe with a single line between "
         "regions"
     )
     tc_joined = pd.DataFrame(
         columns=["Network_Lines"] + zones + ["Line_Max_Flow_MW", "Line_Min_Flow_MW"],
         index=transmission_constraints_table.reindex(combos).dropna().index,
         data=0,
     )
 
     if tc_joined.empty:
-        logger.info(f"No transmission lines exist between model regions {combos}")
+        logger.warning(f"No transmission lines exist between model regions {combos}")
         tc_joined["transmission_path_name"] = None
         tc_joined.rename(columns=zone_num_map, inplace=True)
         return tc_joined.reset_index(drop=True)
 
     tc_joined["Network_Lines"] = range(1, len(tc_joined) + 1)
     tc_joined["Line_Max_Flow_MW"] = transmission_constraints_table.reindex(
         combos
@@ -279,15 +280,15 @@
 
     return distance
 
 
 def transmission_line_distance(
     trans_constraints_df, ipm_shapefile, settings, units="mile"
 ):
-    logger.info("Calculating transmission line distance")
+    logger.debug("Calculating transmission line distance")
     ipm_shapefile["geometry"] = ipm_shapefile.buffer(0.01)
     model_polygons = ipm_shapefile.dissolve(by="model_region")
     model_polygons = model_polygons.to_crs(epsg=4326)
     region_centroids = find_centroid(model_polygons)
 
     distances = [
         single_line_distance(line_name, region_centroids, units=units)
```

### Comparing `PowerGenome-0.6.1a0/powergenome/util.py` & `powergenome-0.6.2/powergenome/util.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import collections
+import csv
+import hashlib
 import itertools
 import logging
 import os
 import re
 import subprocess
 from collections.abc import Iterable
 from copy import deepcopy
 from pathlib import Path
-from typing import Dict, List, Tuple, Union
+from typing import Any, Dict, List, Tuple, Union
+
+os.environ["USE_PYGEOS"] = "0"
 
 import geopandas as gpd
 import pandas as pd
 import pudl
 import requests
 import sqlalchemy as sa
 import yaml
@@ -52,42 +56,137 @@
         raise FileNotFoundError(
             "Path is not recognized. Check that your path is valid."
         )
 
     if settings.get("input_folder"):
         settings["input_folder"] = path.parent / settings["input_folder"]
 
+    if settings.get("generator_columns"):
+        settings["generator_columns"] = add_model_tags_to_gen_columns(
+            model_tag_values=settings.get("model_tag_values", {}),
+            regional_tag_values=settings.get("regional_tag_values", {}),
+            generator_columns=settings["generator_columns"],
+        )
+
     settings = apply_all_tag_to_regions(settings)
+    settings = sort_nested_dict(settings)
 
     for key in ["PUDL_DB", "PG_DB"]:
         # Add correct connection string prefix if it isn't there
         if settings.get(key):
             settings[key] = sqlalchemy_prefix(settings[key])
 
+    for key in [
+        "EFS_DATA",
+        "RESOURCE_GROUPS",
+        "DISTRIBUTED_GEN_DATA",
+        "RESOURCE_GROUP_PROFILES",
+    ]:
+        if settings.get(key):
+            settings[key] = Path(settings[key])
+
     return fix_param_names(settings)
 
 
+def add_model_tags_to_gen_columns(
+    model_tag_values: Dict[str, Dict[str, int]],
+    regional_tag_values: Dict[str, Dict[str, Dict[str, int]]],
+    generator_columns: List[str],
+) -> List[str]:
+    """Add model resource tag keys to the list of columns that will be included in
+    generator outputs.
+
+    Parameters
+    ----------
+    model_tag_values : Dict[str, Dict[str, int]]
+        Tags applied to resources in all regions. Top level is the tag name, which will
+        become a column in the generators output. The next level is technology names
+        and the value for each technology.
+    regional_tag_values : Dict[str, Dict[str, Dict[str, int]]]
+        Regional values applied to technologies. Top level is the region, then the tag
+        name, then the technology name and value.
+    generator_columns : List[str]
+        List of columns to include in generator outputs from the settings.
+
+    Returns
+    -------
+    List[str]
+        Updated list of column names, now including any resource tags/columns.
+
+    Example
+    -------
+    >>> model_tag_values = {'cost': {'solar': 100, 'wind': 150}}
+    >>> regional_tag_values = {'NA': {'other_tag': {'solar': 20, 'wind': 25}}}
+    >>> generator_columns = ['capacity', 'output']
+    >>> add_model_tags_to_gen_columns(model_tag_values, regional_tag_values, generator_columns)
+    ['capacity', 'output', 'cost', 'other_tag']
+
+    """
+
+    if not isinstance(generator_columns, list):
+        logger.warning(
+            "There is a parameter 'generator_columns' in your settings but it is not a "
+            "list. This parameter will not have any effect in it's current form."
+        )
+        return generator_columns
+
+    tag_keys = list((model_tag_values or {}).keys())
+    regional_keys = []
+    for region, regional_tags in (regional_tag_values or {}).items():
+        regional_keys.extend(list(regional_tags.keys()))
+
+    tag_keys = set(tag_keys + regional_keys)
+    for tag in tag_keys:
+        if tag not in generator_columns:
+            generator_columns.append(tag)
+
+    return generator_columns
+
+
+def sort_nested_dict(d: Dict[str, Any]) -> Dict[str, Any]:
+    """
+    Given a nested dictionary, iterate through all levels to sort keys by length.
+    Dictionary values can be more nested dictionaries, strings, numbers, or lists.
+
+    Parameters
+    ----------
+    d : Dict[str, Any]
+        The nested dictionary to be sorted.
+
+    Returns
+    -------
+    Dict[str, Any]
+        The sorted dictionary where keys are sorted by length at each level.
+
+    """
+    sorted_dict = dict()
+
+    for key, value in sorted(d.items(), key=lambda x: len(str(x[0]))):
+        if isinstance(value, dict):
+            sorted_dict[key] = sort_nested_dict(value)
+        else:
+            sorted_dict[key] = value
+
+    return sorted_dict
+
+
 def sqlalchemy_prefix(db_path: str) -> str:
     """Check the database path and add sqlite prefix if needed
 
     Parameters
     ----------
     db_path : str
         Path to the sqlite database. May or may not include sqlite://// (OS specific)
 
     Returns
     -------
     str
         SqlAlchemy connection string
     """
-    if os.name == "nt":
-        # if user is using a windows system
-        sql_prefix = "sqlite:///"
-    else:
-        sql_prefix = "sqlite:////"
+    sql_prefix = "sqlite:///"
 
     if not db_path:
         return None
     if sql_prefix in db_path:
         return db_path
     else:
         return sql_prefix + str(Path(db_path))
@@ -425,14 +524,22 @@
             logger.warning(
                 "The settings EIA demand growth scenario (growth_scenario) key "
                 f"value is {growth_scenario}, which does not match the aeo data year "
                 f"{load_aeo_year}. It has been changed to REF{load_aeo_year}."
             )
             settings["growth_scenario"] = f"REF{load_aeo_year}"
 
+    if not settings.get("interest_compound_method"):
+        logger.info(
+            "The default interest compounding method for calculating annuities has "
+            "changed from continuous to discrete. This method can be set with the parameter "
+            "'interest_compound_method', using values `discrete` or `continuous`.\n"
+            "This message will be removed after version 0.7.0."
+        )
+
 
 def init_pudl_connection(
     freq: str = "AS",
     start_year: int = None,
     end_year: int = None,
     pudl_db: str = None,
     pg_db: str = None,
@@ -612,27 +719,43 @@
     save_path.parent.mkdir(parents=True, exist_ok=True)
     save_path.write_bytes(r.content)
 
 
 def update_dictionary(d: dict, u: dict) -> dict:
     """
     Update keys in an existing dictionary (d) with values from u
+    Sort keys in updated dictionary by their lengths from shortest to longest
+
+    Parameters
+    ----------
+    d : dict
+        The existing dictionary to be updated.
+    u : dict
+        The dictionary containing the new values to update the existing dictionary.
 
-    https://stackoverflow.com/a/32357112
+    Returns
+    -------
+    dict
+        The updated dictionary with keys sorted by length.
     """
-    for k, v in u.items():
+    if not (isinstance(d, collections.abc.Mapping) or d is None) or not isinstance(
+        u, collections.abc.Mapping
+    ):
+        raise TypeError("Inputs must be dictionaries")
+
+    for k, v in sorted(u.items(), key=lambda item: len(str(item[0]))):
         if isinstance(d, collections.abc.Mapping):
             if isinstance(v, collections.abc.Mapping):
                 r = update_dictionary(d.get(k, {}), v)
                 d[k] = r
             else:
                 d[k] = u[k]
         else:
             d = {k: u[k]}
-    return d
+    return dict(sorted(d.items(), key=lambda item: len(str(item[0]))))
 
 
 def remove_fuel_scenario_name(df, settings):
     _df = df.copy()
     scenarios = settings["eia_series_scenario_names"].keys()
     for s in scenarios:
         _df.columns = _df.columns.str.replace(f"_{s}", "")
@@ -651,14 +774,15 @@
 
 def write_results_file(
     df: pd.DataFrame,
     folder: Path,
     file_name: str,
     include_index: bool = False,
     float_format: str = None,
+    multi_period: bool = True,
 ):
     """Write a finalized dataframe to one of the results csv files.
 
     Parameters
     ----------
     df : DataFrame
         Data for a single results file
@@ -666,19 +790,23 @@
         A Path object representing the folder for a single case/scenario
     file_name : str
         Name of the file.
     include_index : bool, optional
         If pandas should include the index when writing to csv, by default False
     float_format: str
         Parameter passed to pandas .to_csv
+    multi_period : bool, optional
+        If results should be formatted for multi-period, by default True
     """
-    sub_folder = folder / "Inputs"
-    sub_folder.mkdir(exist_ok=True, parents=True)
+    if not multi_period:
+        folder = folder / "Inputs"
 
-    path_out = sub_folder / file_name
+    folder.mkdir(exist_ok=True, parents=True)
+
+    path_out = folder / file_name
     df.to_csv(path_out, index=include_index, float_format=float_format)
 
 
 def write_case_settings_file(settings, folder, file_name):
     """Write a finalized dictionary to YAML file.
 
     Parameters
@@ -799,14 +927,149 @@
     ).squeeze("columns")
     case_id_name_df = case_id_name_df.str.replace(" ", "_")
     case_id_name_map = case_id_name_df.to_dict()
 
     return case_id_name_map
 
 
+def make_iterable(item: Union[int, str, Iterable]) -> Iterable:
+    """Return an iterable version of the one or more items passed.
+
+    Parameters
+    ----------
+    item : Union[int, str, Iterable]
+       Item that may or may not already be iterable
+
+    Returns
+    -------
+    Iterable
+        An iterable version of the item
+    """
+    if isinstance(item, str):
+        i = iter([item])
+    else:
+        try:
+            # check if it's iterable
+            i = iter(item)
+        except TypeError:
+            i = iter([item])
+    return i
+
+
+def assign_model_planning_years(_settings: dict, year: int) -> dict:
+    """Make sure "model_year" and "model_first_planning_year" appear as scalars.
+
+    These can originally be set in any of these forms, in either the default
+    settings or in the settings_management dictionary:
+
+    model_year: 2040 and model_first_planning_year: 2031
+    model_year: [2040, 2050] and model_first_planning_year: [2031, 2041]
+    model_periods: (2031, 2040)
+    model_periods: [(2031, 2040), (2041, 2050)]
+
+    This function looks up the right values for the current year and assigns
+    them as scalars (the first form above).
+
+    Parameters
+    ----------
+    _settings : dict
+        Model settings dictionary. Must have either "model_periods", "model_year"
+        AND "model_first_planning_year", or "model_first_planning_year" as keys.
+    year : int
+        Model year.
+
+    Returns
+    -------
+    dict
+        Modified settings with scaler versions of "model_year" and "model_first_planning_year".
+
+    Raises
+    ------
+    ValueError
+        model_periods is not a series of tuples
+    ValueError
+        model_periods tuples are not all length 2
+    ValueError
+        model_year and model_first_planning_year must all be integer
+    KeyError
+        None of the required keys found
+    ValueError
+        The model year from scenario definitions is not in the settings
+    """
+    if "model_periods" in _settings:
+        model_periods = make_iterable(_settings["model_periods"])
+        if not all([isinstance(t, tuple) for t in model_periods]):
+            raise ValueError(
+                "The settings parameter 'model_periods' must be a list of tuples. It is "
+                f"currently {_settings['model_periods']}"
+            )
+        if not all(len(t) == 2 for t in model_periods):
+            raise ValueError(
+                "The tuples in settings parameter 'model_periods' must all be 2 years. "
+                f"The values found are {_settings['model_periods']}"
+            )
+        model_planning_period_dict = {
+            year: (start_year, year)
+            for (start_year, year) in make_iterable(_settings["model_periods"])
+        }
+    elif "model_year" in _settings and "model_first_planning_year" in _settings:
+        model_year = make_iterable(_settings["model_year"])
+        first_planning_year = make_iterable(_settings["model_first_planning_year"])
+        if not all(isinstance(y, int) for y in model_year) and all(
+            isinstance(y, int) for y in first_planning_year
+        ):
+            raise ValueError(
+                "Both 'model_year' and 'model_first_planning_year' parameters must be "
+                f"integers or lists of integers. The values found are {model_periods} and "
+                f"{first_planning_year}."
+            )
+        model_planning_period_dict = {
+            year: (start_year, year)
+            for year, start_year in zip(
+                make_iterable(_settings["model_year"]),
+                make_iterable(_settings["model_first_planning_year"]),
+            )
+        }
+    elif "model_first_planning_year" in _settings:
+        # we also allow leaving out the model_year tag and just specifying
+        # model_first_planning_year
+        model_planning_period_dict = {
+            year: (
+                _settings["model_first_planning_year"],
+                _settings["model_first_planning_year"],
+            )
+        }
+    else:
+        raise KeyError(
+            "To build a dictionary of scenario settings your settings file should include "
+            "either the key 'model_periods' (a list of 2-element lists) or the keys "
+            "'model_year' and 'model_first_planning_year' (each a list of years)."
+        )
+
+    # remove any model period data already there
+    for key in ["model_periods", "model_year", "model_first_planning_year"]:
+        try:
+            del _settings[key]
+        except KeyError:
+            pass
+
+    if year not in model_planning_period_dict:
+        raise ValueError(
+            f"The year {year} is in your scenario definition file for case {_settings.get('case_id')} "
+            "but was not found in the 'model_year' or 'model_periods' settings parameters. "
+            "Either it is missing in the main settings file or was removed in the "
+            "'settings_management' section."
+        )
+    # assign the scalar values
+    _settings["model_first_planning_year"] = model_planning_period_dict[year][0]
+    _settings["model_year"] = model_planning_period_dict[year][1]
+
+    return _settings
+
+
 def build_scenario_settings(
     settings: dict, scenario_definitions: pd.DataFrame
 ) -> Dict[int, Dict[Union[int, str], dict]]:
     """Build a nested dictionary of settings for each planning year/scenario
 
     Parameters
     ----------
@@ -821,110 +1084,124 @@
 
     Returns
     -------
     dict
         A nested dictionary. The first set of keys are the planning years, the second
         set of keys are the case ID values associated with each case.
     """
-    if settings.get("model_periods"):
-        model_planning_period_dict = {
-            year: (start_year, year) for (start_year, year) in settings["model_periods"]
-        }
-    elif isinstance(settings.get("model_year"), list) and isinstance(
-        settings.get("model_first_planning_year"), list
-    ):
-        model_planning_period_dict = {
-            year: (start_year, year)
-            for year, start_year in zip(
-                settings["model_year"], settings["model_first_planning_year"]
-            )
-        }
-    else:
-        raise KeyError(
-            "To build a dictionary of scenario settings your settings file should include "
-            "either the key 'model_periods' (a list of 2-element lists) or the keys "
-            "'model_year' and 'model_first_planning_year' (each a list of years)."
+
+    # don't allow duplicate rows in the scenario definitions table, since they
+    # could give unexpected results
+    dups = scenario_definitions[["case_id", "year"]].duplicated()
+    if dups.sum() > 0:
+        raise ValueError(
+            "The following cases and years are repeated in your scenario definitions file:\n\n"
+            + scenario_definitions[dups].to_string(index=False)
         )
 
-    case_id_name_map = build_case_id_name_map(settings)
+    if settings.get("case_id_description_fn"):
+        case_id_name_map = build_case_id_name_map(settings)
+    else:
+        case_id_name_map = None
 
+    all_category_levels = set()
+    active_category_levels = set()
     scenario_settings = {}
-    for year in model_planning_period_dict.keys():
-        scenario_settings[year] = {}
-        planning_year_settings_management = (
-            settings.get("settings_management", {}).get(year, {}) or {}
-        )
+    missing_flag = object()
+    for i, scenario_row in scenario_definitions.iterrows():
+        year, case_id = scenario_row[["year", "case_id"]]
 
-        # Create a dictionary with keys of things that change (e.g. ccs_capex) and
-        # values of nested dictionaries that give case_id: scenario name
-        planning_year_scenario_definitions_dict = (
-            scenario_definitions.loc[scenario_definitions.year == year]
-            .set_index("case_id")
-            .to_dict()
-        )
-        planning_year_scenario_definitions_dict.pop("year")
-        new_param_warn_list = []
-        for case_id in scenario_definitions.query("year==@year")["case_id"].unique():
-            _settings = deepcopy(settings)
-            _settings["case_id"] = case_id
+        _settings = deepcopy(settings)
+        _settings["case_id"] = case_id
+
+        # first apply any settings under "all_years", then any settings for this year
+        for settings_year in ["all_years", year]:
+
+            planning_year_settings_management = (
+                settings.get("settings_management", {}).get(settings_year) or {}
+            )
 
+            # update settings from all_cases entry if available (these settings
+            # are applied to all cases for this year, and don't use the category
+            # names or levels from the scenario definitions table)
             if "all_cases" in planning_year_settings_management:
                 new_parameter = planning_year_settings_management["all_cases"]
                 _settings = update_dictionary(_settings, new_parameter)
 
-            modified_settings = []
-            for (
-                category,
-                case_value_dict,
-            ) in planning_year_scenario_definitions_dict.items():
-                # key is the category e.g. ccs_capex, case_value_dict is p1: mid
-                try:
-                    case_value = case_value_dict[case_id]
-                    new_parameter = (
-                        planning_year_settings_management.get(category, {}).get(
-                            case_value, {}
-                        )
-                        or {}
-                    )
-                    if (
-                        not new_parameter
-                        and (category, case_value) not in new_param_warn_list
-                    ):
-                        new_param_warn_list.append((category, case_value))
-
-                        logger.warning(
-                            f"The parameter value '{case_value}' from column '{category}' "
-                            "in your scenario definitions file is not included in the "
-                            "'settings_management' dictionary. Settings for case id "
-                            f"'{case_id}' will not be modified to reflect this scenario."
-                        )
+            modified_settings = {}
+            for category, level in scenario_row.drop(["case_id", "year"]).items():
+                # category is a column from the scenario definitions table, e.g. ccs_capex
+                # level is the selection for this category for this case/year, e.g., "mid" or "none"
+
+                new_parameter = planning_year_settings_management.get(category, {}).get(
+                    level, missing_flag
+                )
+
+                # Remember category/levels that were selected and that actually
+                # had an effect.
+                all_category_levels.add((case_id, year, category, level))
+                if new_parameter is not missing_flag:
+                    # note: user could set None or {} as the setting, to indicate
+                    # this flag should use the default settings as-is
+                    active_category_levels.add((case_id, year, category, level))
+                if new_parameter in [missing_flag, None, {}]:
+                    continue
 
-                    try:
-                        settings_keys = list(flatten(new_parameter).keys())
-                    except AttributeError:
-                        settings_keys = {}
-
-                    for key in settings_keys:
-                        assert (
-                            key not in modified_settings
-                        ), f"The settings key {key} is modified twice in case id {case_id}"
-
-                        modified_settings.append(key)
-
-                    if new_parameter is not None:
-                        _settings = update_dictionary(_settings, new_parameter)
-                    # print(_settings[list(new_parameter.keys())[0]])
+                _settings = update_dictionary(_settings, new_parameter)
+
+                # report any conflicts between these settings and previous ones
+                for key in flatten(new_parameter).keys():
+                    if key in modified_settings:
+                        raise ValueError(
+                            f"The setting {key} is modified by both the "
+                            f"`{modified_settings[key]}` flag and the "
+                            f"`{category}={level}` flag in the scenario "
+                            f"definition for case {case_id}, {year}."
+                        )
+                    else:
+                        # remember this setting for later
+                        modified_settings[key] = f"{category}={level}"
 
-                except KeyError:
-                    pass
+        # make sure model year data appears in standard form
+        assign_model_planning_years(_settings, year)
 
-            _settings["model_first_planning_year"] = model_planning_period_dict[year][0]
-            _settings["model_year"] = model_planning_period_dict[year][1]
+        if case_id_name_map:
             _settings["case_name"] = case_id_name_map[case_id]
-            scenario_settings[year][case_id] = _settings
+
+        scenario_settings.setdefault(year, {})[case_id] = _settings
+        if _settings.get("generator_columns"):
+            _settings["generator_columns"] = add_model_tags_to_gen_columns(
+                model_tag_values=_settings.get("model_tag_values", {}),
+                regional_tag_values=_settings.get("regional_tag_values", {}),
+                generator_columns=_settings["generator_columns"],
+            )
+
+    # Report any settings in the scenario definitions that had no effect. Values
+    # can be changed via either the "all_years" key or a specific year, so we
+    # have to wait till the end to decide which tags had no effect.
+    missing_category_levels = all_category_levels - active_category_levels
+    if missing_category_levels:
+        missing = (
+            pd.DataFrame(
+                missing_category_levels,
+                columns=["case_id", "year", "category", "level"],
+            )
+            .pivot(index=["case_id", "year"], columns="category", values="level")
+            .fillna("")
+            .reset_index()
+        )
+        logger.warning(
+            "The following parameter value(s) in your scenario definitions file "
+            "are not included in the 'settings_management' dictionary for the "
+            "specified year(s). Settings will not be modified to reflect these "
+            "entries:\n\n"
+            + missing.to_string(index=False)
+            + "\n\nYou can place empty entries (~) for these in the "
+            "settings_management dictionary to avoid this message.\n"
+        )
 
     return scenario_settings
 
 
 def remove_feb_29(df: pd.DataFrame) -> pd.DataFrame:
     """Remove Feb 29 from a wide format leap-year dataseries
 
@@ -982,18 +1259,20 @@
 
     if settings.get("user_region_geodata_fn"):
         logger.info("Appending user regions to IPM Regions")
         user_regions = gpd.read_file(
             Path(settings["input_folder"]) / settings["user_region_geodata_fn"]
         )
         if "region" not in user_regions.columns:
-            raise KeyError(
+            region_col = [c for c in user_regions.columns if "region" in c.lower()][0]
+            user_regions = user_regions.rename(columns={region_col: "region"})
+            logger.warning(
                 "The user supplied region geodata file does not include the "
-                "property 'region' for any of the region polygons! User region "
-                "geodata can not be appropriately mapped to model regions."
+                "property 'region' for any of the region polygons! Automatically detecting "
+                "the correct column but this may cause errors."
             )
         user_regions = user_regions.to_crs(ipm_regions.crs)
         ipm_regions = ipm_regions.append(user_regions)
 
     model_regions_gdf = ipm_regions.loc[ipm_regions["region"].isin(keep_regions)]
     model_regions_gdf = map_agg_region_names(
         model_regions_gdf, region_agg_map, "region", "model_region"
@@ -1105,10 +1384,84 @@
     -------
     Union[str, int]
         Either the original ID (if integer or non-numeric string) or an integer version
         of the ID with leading zeros removed
     """
     if isinstance(id, int):
         return id
+    elif isinstance(id, float):
+        return int(id)
     elif id.isnumeric():
-        id = id.strip("0")
+        id = id.lstrip("0")
     return id
+
+
+def hash_string_sha256(input_string: str) -> str:
+    """Create a reproducible hash of an input string. Use for creating cache filenames.
+
+    Parameters
+    ----------
+    input_string : str
+        String representing the data to hash
+
+    Returns
+    -------
+    str
+        Hexdigest hash of the input string.
+    """
+    # For simplicity, require string inputs.
+    if not isinstance(input_string, str):
+        raise TypeError("The input value cannot be hashed if it is not a string.")
+    # Encode the string into bytes
+    input_bytes = input_string.encode("utf-8")
+
+    # Create a SHA-256 hash object
+    hasher = hashlib.sha256()
+
+    # Pass the bytes to the hasher
+    hasher.update(input_bytes)
+
+    # Generate the hexadecimal representation of the digest
+    hex_digest = hasher.hexdigest()
+
+    return hex_digest
+
+
+def add_row_to_csv(file: Path, new_row: List[str], headers: List[str] = None) -> None:
+    """Add a row of data to an existing CSV file. If the file does not exist, create it
+    with headers and the first row of data.
+
+    Parameters
+    ----------
+    file : Path
+        Path to the CSV file
+    new_row : List[str]
+        Data to add as a new row in the CSV
+    headers : List[str], optional
+        Header names, by default None. Required if the file does not exist.
+
+    Raises
+    ------
+    ValueError
+        The file does not exist and no headers were provided.
+    """
+    file = Path(file)
+    # Check if file exists
+    if not file.exists():
+        if headers is None:
+            raise ValueError(
+                f"No headers provided. The file {file} does not exist, so headers are "
+                "required to create the file."
+            )
+        file.parent.mkdir(parents=True, exist_ok=True)
+        with file.open("w", newline="") as f:
+            writer = csv.writer(f)
+            writer.writerow(headers)  # write headers first time only
+
+    with file.open("r") as f:
+        reader = csv.reader(f)
+        data = list(reader)  # this contains all the rows in your CSV file
+
+    if new_row not in data:  # check if row already exists in data
+        with file.open("a", newline="") as f:
+            writer = csv.writer(f)
+            writer.writerow(new_row)  # add the new row to the CSV file
```

### Comparing `PowerGenome-0.6.1a0/pyproject.toml` & `powergenome-0.6.2/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
-requires = ["setuptools>=66,<68", "wheel"] # , "setuptools_scm[toml]>=6.2"]
-build-backend = "setuptools.build_meta"
+requires = ["hatchling"]
+build-backend = "hatchling.build"
 
 [project]
 name = "PowerGenome"
-version = "0.6.1a"
+dynamic = ["version"]
 authors = [{ name = "Greg Schivley", email = "greg.schivley@princeton.edu" }]
 maintainers = [
     { name = "Greg Schivley", email = "greg.schivley@princeton.edu" },
 ]
 description = "Create power system inputs for capacity expansion models"
 readme = "README.md"
 requires-python = ">=3.8"
@@ -24,42 +24,50 @@
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
     "Topic :: Scientific/Engineering",
 ]
 dependencies = [
     "catalystcoop.pudl>=0.6.0, <=2022.11.30",
     "beautifulsoup4 >= 4.8.13",
-    "statsmodels>=0.13",
+    "statsmodels>=0.12.2",
     "python-dotenv",
     "flatten-dict",
     "ruamel.yaml",
     "pyyaml",
     "frozendict",
     "openpyxl>=3.0",
-    "geopandas>=0.12",
+    "geopandas>=0.11",
 ]
 
-[tool.setuptools]
-include-package-data = true
+[tool.hatch.version]
+path = "powergenome/version.py"
 
-[tool.setuptools.packages.find]
-include = ["powergenome*", "data*"]
-exclude = ["tests*", "docs*", "data/eia*"]
-
-[tool.setuptools.package-data]
-"*" = ["*.csv", "*.geojson"]
+[tool.hatch.build.targets.sdist]
+exclude = [
+    "/.github",
+    "/docs",
+    "/notebooks",
+    "/data/eia*",
+    "/tests",
+    "/bin",
+    "/example_systems",
+    "/wiki",
+]
 
 [project.optional-dependencies]
 dev = [
-    "black[jupyter] == 23.3.0",
+    "black[jupyter] == 24.3.0",
     "pre-commit",
     "pytest",
     "isort",
     "build",
     "twine",
 ]
 
 [project.scripts]
 run_powergenome_multiple = "powergenome.run_powergenome_multiple_outputs_cli:main"
 
 [project.urls]
 "Source" = "https://github.com/PowerGenome/PowerGenome"
+
+[tool.isort]
+profile = "black"
```

