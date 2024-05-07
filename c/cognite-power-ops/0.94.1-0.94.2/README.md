# Comparing `tmp/cognite_power_ops-0.94.1.tar.gz` & `tmp/cognite_power_ops-0.94.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognite_power_ops-0.94.1.tar", max compression
+gzip compressed data, was "cognite_power_ops-0.94.2.tar", max compression
```

## Comparing `cognite_power_ops-0.94.1.tar` & `cognite_power_ops-0.94.2.tar`

### file list

```diff
@@ -1,672 +1,672 @@
--rw-r--r--   0        0        0    10758 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/LICENSE
--rw-r--r--   0        0        0     3322 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/README.md
--rw-r--r--   0        0        0      150 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/__init__.py
--rw-r--r--   0        0        0       23 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/_version.py
--rw-r--r--   0        0        0     5273 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/cdf_labels.py
--rw-r--r--   0        0        0     8779 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/cli.py
--rw-r--r--   0        0        0       74 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/__init__.py
--rw-r--r--   0        0        0      105 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
--rw-r--r--   0        0        0    32135 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
--rw-r--r--   0        0        0    26235 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
--rw-r--r--   0        0        0     1492 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
--rw-r--r--   0        0        0    27110 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2041 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2039 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
--rw-r--r--   0        0        0    11759 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    16844 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1513 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    27874 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
--rw-r--r--   0        0        0     1971 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8302 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
--rw-r--r--   0        0        0    16131 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
--rw-r--r--   0        0        0    25401 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    25313 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    25313 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    25195 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    25692 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    25604 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1513 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    25330 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    25780 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    25692 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     9211 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api_client.py
--rw-r--r--   0        0        0     2654 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16179 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    19431 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0     8148 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    23764 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.455745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
--rw-r--r--   0        0        0     9015 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0      109 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/__init__.py
--rw-r--r--   0        0        0    32350 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/_core.py
--rw-r--r--   0        0        0    16860 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method.py
--rw-r--r--   0        0        0     1511 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
--rw-r--r--   0        0        0    26226 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator.py
--rw-r--r--   0        0        0    15705 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1625 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0    28005 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
--rw-r--r--   0        0        0     5828 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_query.py
--rw-r--r--   0        0        0    27596 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2197 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
--rw-r--r--   0        0        0    32967 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant.py
--rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
--rw-r--r--   0        0        0     1998 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_generators.py
--rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
--rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
--rw-r--r--   0        0        0    30438 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
--rw-r--r--   0        0        0    30100 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
--rw-r--r--   0        0        0    30100 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
--rw-r--r--   0        0        0     8084 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_query.py
--rw-r--r--   0        0        0    30394 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
--rw-r--r--   0        0        0    27060 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area.py
--rw-r--r--   0        0        0    27668 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
--rw-r--r--   0        0        0    27580 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
--rw-r--r--   0        0        0    27580 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
--rw-r--r--   0        0        0    27462 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
--rw-r--r--   0        0        0    27374 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
--rw-r--r--   0        0        0    27739 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
--rw-r--r--   0        0        0    27959 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27871 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     2011 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
--rw-r--r--   0        0        0    11709 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_query.py
--rw-r--r--   0        0        0    27597 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
--rw-r--r--   0        0        0    28047 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27959 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     2095 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
--rw-r--r--   0        0        0    20054 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir.py
--rw-r--r--   0        0        0     1510 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
--rw-r--r--   0        0        0    15561 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1615 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    22125 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse.py
--rw-r--r--   0        0        0     2026 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
--rw-r--r--   0        0        0    26508 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
--rw-r--r--   0        0        0     6635 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
--rw-r--r--   0        0        0    10150 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api_client.py
--rw-r--r--   0        0        0     4810 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/__init__.py
--rw-r--r--   0        0        0     8028 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_core.py
--rw-r--r--   0        0        0    19888 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator.py
--rw-r--r--   0        0        0     9775 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    32088 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_plant.py
--rw-r--r--   0        0        0    33431 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
--rw-r--r--   0        0        0    10116 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
--rw-r--r--   0        0        0     9645 2024-04-22 09:30:11.459745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    13820 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
--rw-r--r--   0        0        0      113 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
--rw-r--r--   0        0        0     8201 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/_core.py
--rw-r--r--   0        0        0    14521 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/case.py
--rw-r--r--   0        0        0     7486 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
--rw-r--r--   0        0        0     9780 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
--rw-r--r--   0        0        0    15960 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
--rw-r--r--   0        0        0    17869 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
--rw-r--r--   0        0        0    11367 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
--rw-r--r--   0        0        0    19744 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
--rw-r--r--   0        0        0    10871 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
--rw-r--r--   0        0        0     3003 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api_client.py
--rw-r--r--   0        0        0     2524 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
--rw-r--r--   0        0        0     4596 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
--rw-r--r--   0        0        0     2226 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
--rw-r--r--   0        0        0     5824 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
--rw-r--r--   0        0        0     2393 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
--rw-r--r--   0        0        0     4586 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
--rw-r--r--   0        0        0     5174 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
--rw-r--r--   0        0        0     2819 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
--rw-r--r--   0        0        0     6951 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
--rw-r--r--   0        0        0     2621 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
--rw-r--r--   0        0        0      118 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
--rw-r--r--   0        0        0    32598 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
--rw-r--r--   0        0        0    26333 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
--rw-r--r--   0        0        0     1497 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
--rw-r--r--   0        0        0    23471 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
--rw-r--r--   0        0        0     2115 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
--rw-r--r--   0        0        0     7177 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
--rw-r--r--   0        0        0    29138 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
--rw-r--r--   0        0        0     2059 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
--rw-r--r--   0        0        0     2106 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
--rw-r--r--   0        0        0    13622 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
--rw-r--r--   0        0        0    22831 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
--rw-r--r--   0        0        0     2032 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
--rw-r--r--   0        0        0     7128 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    16942 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
--rw-r--r--   0        0        0     1518 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
--rw-r--r--   0        0        0    24946 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
--rw-r--r--   0        0        0     2185 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
--rw-r--r--   0        0        0    10308 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
--rw-r--r--   0        0        0     2410 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
--rw-r--r--   0        0        0    19843 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
--rw-r--r--   0        0        0    25798 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
--rw-r--r--   0        0        0    25883 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
--rw-r--r--   0        0        0     2613 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
--rw-r--r--   0        0        0    20327 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
--rw-r--r--   0        0        0     2415 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
--rw-r--r--   0        0        0     4483 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
--rw-r--r--   0        0        0    18030 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
--rw-r--r--   0        0        0    24799 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
--rw-r--r--   0        0        0     1559 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
--rw-r--r--   0        0        0    15855 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
--rw-r--r--   0        0        0    24935 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
--rw-r--r--   0        0        0    25177 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
--rw-r--r--   0        0        0     2777 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
--rw-r--r--   0        0        0    18424 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
--rw-r--r--   0        0        0     1618 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
--rw-r--r--   0        0        0    11242 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
--rw-r--r--   0        0        0     7397 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
--rw-r--r--   0        0        0    16179 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
--rw-r--r--   0        0        0    14604 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
--rw-r--r--   0        0        0    24068 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
--rw-r--r--   0        0        0    14962 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0     8042 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
--rw-r--r--   0        0        0    22916 2024-04-22 09:30:11.463745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
--rw-r--r--   0        0        0    17010 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
--rw-r--r--   0        0        0    14696 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
--rw-r--r--   0        0        0    11922 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
--rw-r--r--   0        0        0     9353 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
--rw-r--r--   0        0        0    13242 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
--rw-r--r--   0        0        0     8909 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
--rw-r--r--   0        0        0      123 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/__init__.py
--rw-r--r--   0        0        0    41803 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/_core.py
--rw-r--r--   0        0        0    28392 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert.py
--rw-r--r--   0        0        0     1486 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert_query.py
--rw-r--r--   0        0        0    24852 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
--rw-r--r--   0        0        0     2445 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
--rw-r--r--   0        0        0     7859 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
--rw-r--r--   0        0        0    27557 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document.py
--rw-r--r--   0        0        0    29838 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
--rw-r--r--   0        0        0     2125 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
--rw-r--r--   0        0        0     2123 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
--rw-r--r--   0        0        0    11654 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
--rw-r--r--   0        0        0     2056 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
--rw-r--r--   0        0        0    31537 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
--rw-r--r--   0        0        0     2194 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
--rw-r--r--   0        0        0     2399 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
--rw-r--r--   0        0        0    13156 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
--rw-r--r--   0        0        0     6256 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
--rw-r--r--   0        0        0    16995 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
--rw-r--r--   0        0        0    20707 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
--rw-r--r--   0        0        0     2194 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2352 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     9120 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
--rw-r--r--   0        0        0     1507 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
--rw-r--r--   0        0        0    24990 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row.py
--rw-r--r--   0        0        0     1986 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
--rw-r--r--   0        0        0     8727 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
--rw-r--r--   0        0        0    23488 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input.py
--rw-r--r--   0        0        0     1527 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input_query.py
--rw-r--r--   0        0        0    26010 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output.py
--rw-r--r--   0        0        0     2098 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
--rw-r--r--   0        0        0     7530 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_query.py
--rw-r--r--   0        0        0    30503 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator.py
--rw-r--r--   0        0        0    29640 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
--rw-r--r--   0        0        0    14623 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
--rw-r--r--   0        0        0     1621 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
--rw-r--r--   0        0        0     5996 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_query.py
--rw-r--r--   0        0        0    29214 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
--rw-r--r--   0        0        0     2275 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
--rw-r--r--   0        0        0    30967 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration.py
--rw-r--r--   0        0        0     1557 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
--rw-r--r--   0        0        0    21738 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
--rw-r--r--   0        0        0     2719 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
--rw-r--r--   0        0        0    30364 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4187 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    31040 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2403 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0    10702 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    26004 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
--rw-r--r--   0        0        0     2305 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
--rw-r--r--   0        0        0     2463 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
--rw-r--r--   0        0        0    12658 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
--rw-r--r--   0        0        0    29102 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0     2502 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
--rw-r--r--   0        0        0     2660 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
--rw-r--r--   0        0        0     2676 2024-04-22 09:30:11.467745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
--rw-r--r--   0        0        0    16509 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
--rw-r--r--   0        0        0    21267 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant.py
--rw-r--r--   0        0        0    34870 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information.py
--rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2177 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
--rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
--rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
--rw-r--r--   0        0        0    31075 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
--rw-r--r--   0        0        0    31163 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
--rw-r--r--   0        0        0    31163 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
--rw-r--r--   0        0        0     6307 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
--rw-r--r--   0        0        0    31031 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
--rw-r--r--   0        0        0     1486 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_query.py
--rw-r--r--   0        0        0    35566 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
--rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
--rw-r--r--   0        0        0     2260 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
--rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
--rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
--rw-r--r--   0        0        0    31262 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
--rw-r--r--   0        0        0    31350 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
--rw-r--r--   0        0        0    31350 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
--rw-r--r--   0        0        0     6373 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
--rw-r--r--   0        0        0    31218 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
--rw-r--r--   0        0        0    21879 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset.py
--rw-r--r--   0        0        0     1512 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
--rw-r--r--   0        0        0    21768 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area.py
--rw-r--r--   0        0        0    23928 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
--rw-r--r--   0        0        0    27423 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
--rw-r--r--   0        0        0    27335 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
--rw-r--r--   0        0        0    27335 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
--rw-r--r--   0        0        0    27217 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
--rw-r--r--   0        0        0    27714 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    27626 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
--rw-r--r--   0        0        0     1528 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
--rw-r--r--   0        0        0    27352 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
--rw-r--r--   0        0        0    27802 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    27714 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
--rw-r--r--   0        0        0    24500 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
--rw-r--r--   0        0        0    27713 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
--rw-r--r--   0        0        0    27521 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
--rw-r--r--   0        0        0     2794 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
--rw-r--r--   0        0        0    26627 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information.py
--rw-r--r--   0        0        0    28169 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
--rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
--rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
--rw-r--r--   0        0        0    27963 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
--rw-r--r--   0        0        0    28081 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
--rw-r--r--   0        0        0    28460 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
--rw-r--r--   0        0        0    28372 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
--rw-r--r--   0        0        0    27889 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
--rw-r--r--   0        0        0     2851 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
--rw-r--r--   0        0        0    28098 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
--rw-r--r--   0        0        0    28548 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
--rw-r--r--   0        0        0    28460 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
--rw-r--r--   0        0        0     1507 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_query.py
--rw-r--r--   0        0        0    18930 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production.py
--rw-r--r--   0        0        0    25079 2024-04-22 09:30:11.471745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_price.py
--rw-r--r--   0        0        0    25321 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_production.py
--rw-r--r--   0        0        0     2623 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_query.py
--rw-r--r--   0        0        0    25220 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
--rw-r--r--   0        0        0     1601 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
--rw-r--r--   0        0        0    27660 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
--rw-r--r--   0        0        0    24151 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     3878 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    18438 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case.py
--rw-r--r--   0        0        0     6064 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
--rw-r--r--   0        0        0     2071 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
--rw-r--r--   0        0        0    17214 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands.py
--rw-r--r--   0        0        0     1521 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
--rw-r--r--   0        0        0    20249 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file.py
--rw-r--r--   0        0        0     1502 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
--rw-r--r--   0        0        0    23570 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model.py
--rw-r--r--   0        0        0     2279 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
--rw-r--r--   0        0        0     5631 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
--rw-r--r--   0        0        0    32763 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2608 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
--rw-r--r--   0        0        0     7877 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29852 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
--rw-r--r--   0        0        0     1548 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
--rw-r--r--   0        0        0    29105 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
--rw-r--r--   0        0        0     2688 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
--rw-r--r--   0        0        0    27944 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
--rw-r--r--   0        0        0     2223 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
--rw-r--r--   0        0        0     8858 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
--rw-r--r--   0        0        0    16377 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result.py
--rw-r--r--   0        0        0     2042 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
--rw-r--r--   0        0        0     2214 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
--rw-r--r--   0        0        0    11103 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
--rw-r--r--   0        0        0    22289 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
--rw-r--r--   0        0        0     2338 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
--rw-r--r--   0        0        0     8104 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
--rw-r--r--   0        0        0    23085 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
--rw-r--r--   0        0        0     4851 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
--rw-r--r--   0        0        0     2216 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
--rw-r--r--   0        0        0    21375 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
--rw-r--r--   0        0        0     1533 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
--rw-r--r--   0        0        0    26338 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
--rw-r--r--   0        0        0    27685 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
--rw-r--r--   0        0        0     3695 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
--rw-r--r--   0        0        0    27490 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
--rw-r--r--   0        0        0     2153 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
--rw-r--r--   0        0        0     8841 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
--rw-r--r--   0        0        0    27145 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
--rw-r--r--   0        0        0     2743 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
--rw-r--r--   0        0        0    27652 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
--rw-r--r--   0        0        0     2195 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
--rw-r--r--   0        0        0     2330 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
--rw-r--r--   0        0        0    11719 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
--rw-r--r--   0        0        0    30353 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     2477 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
--rw-r--r--   0        0        0     5956 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    29442 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     2375 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
--rw-r--r--   0        0        0     9141 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
--rw-r--r--   0        0        0    15615 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
--rw-r--r--   0        0        0     1611 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
--rw-r--r--   0        0        0    24038 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0     2906 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
--rw-r--r--   0        0        0    32573 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0     4476 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
--rw-r--r--   0        0        0    21933 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse.py
--rw-r--r--   0        0        0     1516 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
--rw-r--r--   0        0        0    44629 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api_client.py
--rw-r--r--   0        0        0    37530 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/__init__.py
--rw-r--r--   0        0        0    17724 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_alert.py
--rw-r--r--   0        0        0    19045 2024-04-22 09:30:11.475745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
--rw-r--r--   0        0        0    17003 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
--rw-r--r--   0        0        0    20325 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
--rw-r--r--   0        0        0    24038 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
--rw-r--r--   0        0        0     8689 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
--rw-r--r--   0        0        0    13311 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
--rw-r--r--   0        0        0    21939 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
--rw-r--r--   0        0        0    22919 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_core.py
--rw-r--r--   0        0        0    12436 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
--rw-r--r--   0        0        0    16494 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
--rw-r--r--   0        0        0    23071 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator.py
--rw-r--r--   0        0        0     9182 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
--rw-r--r--   0        0        0    16689 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
--rw-r--r--   0        0        0    13527 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
--rw-r--r--   0        0        0    21898 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    23503 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0    20874 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
--rw-r--r--   0        0        0    23363 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
--rw-r--r--   0        0        0    10500 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant.py
--rw-r--r--   0        0        0    26506 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
--rw-r--r--   0        0        0    29307 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
--rw-r--r--   0        0        0    11193 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
--rw-r--r--   0        0        0    10749 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
--rw-r--r--   0        0        0    23293 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
--rw-r--r--   0        0        0    17874 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
--rw-r--r--   0        0        0    27975 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
--rw-r--r--   0        0        0    13152 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
--rw-r--r--   0        0        0    15360 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
--rw-r--r--   0        0        0    16791 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    14456 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
--rw-r--r--   0        0        0     8881 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
--rw-r--r--   0        0        0    11080 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
--rw-r--r--   0        0        0    16536 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
--rw-r--r--   0        0        0    23998 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    18119 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
--rw-r--r--   0        0        0    17739 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
--rw-r--r--   0        0        0    18550 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
--rw-r--r--   0        0        0    16368 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
--rw-r--r--   0        0        0    16997 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
--rw-r--r--   0        0        0    13212 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
--rw-r--r--   0        0        0    12493 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
--rw-r--r--   0        0        0    19542 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
--rw-r--r--   0        0        0    18640 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
--rw-r--r--   0        0        0    17220 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
--rw-r--r--   0        0        0    18291 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
--rw-r--r--   0        0        0    20082 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    19880 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
--rw-r--r--   0        0        0     9657 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
--rw-r--r--   0        0        0    14420 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
--rw-r--r--   0        0        0    22515 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
--rw-r--r--   0        0        0    10848 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
--rw-r--r--   0        0        0     1301 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/_logger.py
--rw-r--r--   0        0        0      139 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/data_classes.py
--rw-r--r--   0        0        0     1322 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/data_set_api.py
--rw-r--r--   0        0        0     6750 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/powerops_client.py
--rw-r--r--   0        0        0       62 2024-04-22 09:30:11.479745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/__init__.py
--rw-r--r--   0        0        0      885 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/_api_client.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/__init__.py
--rw-r--r--   0        0        0     8367 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/dayahead_trigger_api.py
--rw-r--r--   0        0        0     4797 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_result_files_api.py
--rw-r--r--   0        0        0     4432 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_results_api.py
--rw-r--r--   0        0        0     9593 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_run_api.py
--rw-r--r--   0        0        0      600 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/__init__.py
--rw-r--r--   0        0        0     4114 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/case.py
--rw-r--r--   0        0        0     9057 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
--rw-r--r--   0        0        0     2720 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/helpers.py
--rw-r--r--   0        0        0      603 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/plotting.py
--rw-r--r--   0        0        0     6164 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_result_files.py
--rw-r--r--   0        0        0     6607 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results.py
--rw-r--r--   0        0        0    10210 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results_compare.py
--rw-r--r--   0        0        0     3021 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run.py
--rw-r--r--   0        0        0     3743 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run_event.py
--rw-r--r--   0        0        0     4374 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_case.py
--rw-r--r--   0        0        0     1101 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_file_reference.py
--rw-r--r--   0        0        0    13466 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run.py
--rw-r--r--   0        0        0    15419 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_api.py
--rw-r--r--   0        0        0     3885 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_filter.py
--rw-r--r--   0        0        0      563 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/client/shop/utils.py
--rw-r--r--   0        0        0      947 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/cognite_modules/_system.yaml
--rw-r--r--   0        0        0     1941 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/config.dev.yaml
--rw-r--r--   0        0        0      729 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1095 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
--rw-r--r--   0        0        0     1680 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      100 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
--rw-r--r--   0        0        0       92 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
--rw-r--r--   0        0        0      367 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
--rw-r--r--   0        0        0     2102 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
--rw-r--r--   0        0        0      750 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     1380 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
--rw-r--r--   0        0        0      857 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
--rw-r--r--   0        0        0     1038 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
--rw-r--r--   0        0        0      502 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
--rw-r--r--   0        0        0     1408 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
--rw-r--r--   0        0        0     2281 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
--rw-r--r--   0        0        0     2375 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
--rw-r--r--   0        0        0      556 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
--rw-r--r--   0        0        0      466 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
--rw-r--r--   0        0        0      767 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
--rw-r--r--   0        0        0      371 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
--rw-r--r--   0        0        0      532 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
--rw-r--r--   0        0        0      618 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
--rw-r--r--   0        0        0      416 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
--rw-r--r--   0        0        0      490 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
--rw-r--r--   0        0        0      113 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
--rw-r--r--   0        0        0      118 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
--rw-r--r--   0        0        0     1515 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      116 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
--rw-r--r--   0        0        0       81 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
--rw-r--r--   0        0        0     1379 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
--rw-r--r--   0        0        0      606 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
--rw-r--r--   0        0        0     3917 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
--rw-r--r--   0        0        0     2786 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
--rw-r--r--   0        0        0     2618 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
--rw-r--r--   0        0        0     1138 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
--rw-r--r--   0        0        0     5199 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
--rw-r--r--   0        0        0     5204 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
--rw-r--r--   0        0        0     1060 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
--rw-r--r--   0        0        0     1121 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
--rw-r--r--   0        0        0     1887 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
--rw-r--r--   0        0        0     2558 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
--rw-r--r--   0        0        0     2374 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
--rw-r--r--   0        0        0      858 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      579 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
--rw-r--r--   0        0        0     1945 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
--rw-r--r--   0        0        0     1845 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
--rw-r--r--   0        0        0      723 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
--rw-r--r--   0        0        0      700 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
--rw-r--r--   0        0        0      711 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
--rw-r--r--   0        0        0     1015 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
--rw-r--r--   0        0        0     1479 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
--rw-r--r--   0        0        0     1312 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
--rw-r--r--   0        0        0      666 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
--rw-r--r--   0        0        0     1230 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
--rw-r--r--   0        0        0      605 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
--rw-r--r--   0        0        0     4964 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
--rw-r--r--   0        0        0     6519 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
--rw-r--r--   0        0        0     2052 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
--rw-r--r--   0        0        0     3499 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2918 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
--rw-r--r--   0        0        0     2575 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
--rw-r--r--   0        0        0     2276 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
--rw-r--r--   0        0        0     2163 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
--rw-r--r--   0        0        0     1748 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
--rw-r--r--   0        0        0      814 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
--rw-r--r--   0        0        0     1292 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
--rw-r--r--   0        0        0      496 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
--rw-r--r--   0        0        0      771 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
--rw-r--r--   0        0        0     1659 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
--rw-r--r--   0        0        0      755 2024-04-22 09:30:11.483745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
--rw-r--r--   0        0        0     3521 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
--rw-r--r--   0        0        0     1038 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
--rw-r--r--   0        0        0     2082 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
--rw-r--r--   0        0        0      756 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0     2425 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
--rw-r--r--   0        0        0     1076 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
--rw-r--r--   0        0        0     1628 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
--rw-r--r--   0        0        0      689 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
--rw-r--r--   0        0        0      710 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
--rw-r--r--   0        0        0      504 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
--rw-r--r--   0        0        0     1074 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
--rw-r--r--   0        0        0     1106 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
--rw-r--r--   0        0        0     1462 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
--rw-r--r--   0        0        0      634 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
--rw-r--r--   0        0        0      464 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
--rw-r--r--   0        0        0     1128 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
--rw-r--r--   0        0        0     1446 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
--rw-r--r--   0        0        0      280 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
--rw-r--r--   0        0        0      978 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
--rw-r--r--   0        0        0      690 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
--rw-r--r--   0        0        0      869 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
--rw-r--r--   0        0        0     1789 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
--rw-r--r--   0        0        0     2661 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
--rw-r--r--   0        0        0      118 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
--rw-r--r--   0        0        0      104 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
--rw-r--r--   0        0        0     5275 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
--rw-r--r--   0        0        0      854 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
--rw-r--r--   0        0        0       91 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
--rw-r--r--   0        0        0     3704 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
--rw-r--r--   0        0        0     2834 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
--rw-r--r--   0        0        0     2983 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
--rw-r--r--   0        0        0      871 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
--rw-r--r--   0        0        0     1283 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
--rw-r--r--   0        0        0     2330 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
--rw-r--r--   0        0        0     1073 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0     1260 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
--rw-r--r--   0        0        0      535 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
--rw-r--r--   0        0        0      599 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
--rw-r--r--   0        0        0     4498 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
--rw-r--r--   0        0        0      512 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
--rw-r--r--   0        0        0     2932 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
--rw-r--r--   0        0        0     1659 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
--rw-r--r--   0        0        0      596 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
--rw-r--r--   0        0        0      543 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
--rw-r--r--   0        0        0     1476 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2264 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
--rw-r--r--   0        0        0     1059 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     1184 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
--rw-r--r--   0        0        0     2520 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
--rw-r--r--   0        0        0     1450 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
--rw-r--r--   0        0        0     1726 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
--rw-r--r--   0        0        0     1564 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
--rw-r--r--   0        0        0      701 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
--rw-r--r--   0        0        0     1225 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
--rw-r--r--   0        0        0     1349 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
--rw-r--r--   0        0        0      890 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
--rw-r--r--   0        0        0     2331 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
--rw-r--r--   0        0        0     1840 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
--rw-r--r--   0        0        0     1027 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
--rw-r--r--   0        0        0     1705 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
--rw-r--r--   0        0        0     2573 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
--rw-r--r--   0        0        0     1965 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
--rw-r--r--   0        0        0     1535 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
--rw-r--r--   0        0        0     1399 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
--rw-r--r--   0        0        0     1797 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1053 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
--rw-r--r--   0        0        0     1750 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1522 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
--rw-r--r--   0        0        0     1660 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
--rw-r--r--   0        0        0     1069 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
--rw-r--r--   0        0        0     1249 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
--rw-r--r--   0        0        0     1680 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     1336 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
--rw-r--r--   0        0        0     2119 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
--rw-r--r--   0        0        0      981 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
--rw-r--r--   0        0        0     1757 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1355 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
--rw-r--r--   0        0        0     1426 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
--rw-r--r--   0        0        0     1010 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
--rw-r--r--   0        0        0     1378 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
--rw-r--r--   0        0        0     1434 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
--rw-r--r--   0        0        0     1392 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
--rw-r--r--   0        0        0     2707 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
--rw-r--r--   0        0        0     1587 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
--rw-r--r--   0        0        0     1114 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/__init__.py
--rw-r--r--   0        0        0    34098 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/transformations.py
--rw-r--r--   0        0        0      278 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/__init__.py
--rw-r--r--   0        0        0     1792 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/__init__.py
--rw-r--r--   0        0        0    12764 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_main.py
--rw-r--r--   0        0        0      595 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_settings.py
--rw-r--r--   0        0        0    12408 2024-04-22 09:30:11.487745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/_shared.py
--rw-r--r--   0        0        0       75 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/__init__.py
--rw-r--r--   0        0        0      720 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/shop_file_config.py
--rw-r--r--   0        0        0      815 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/__init__.py
--rw-r--r--   0        0        0     5486 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/_core.py
--rw-r--r--   0        0        0     2106 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/benchmarking.py
--rw-r--r--   0        0        0     2105 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/dayahead.py
--rw-r--r--   0        0        0      961 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/market.py
--rw-r--r--   0        0        0    10827 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/rkom.py
--rw-r--r--   0        0        0      417 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/__init__.py
--rw-r--r--   0        0        0      830 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/connections.py
--rw-r--r--   0        0        0     1414 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/generator.py
--rw-r--r--   0        0        0     5675 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/plant.py
--rw-r--r--   0        0        0     2868 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/watercourse.py
--rw-r--r--   0        0        0      244 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/__init__.py
--rw-r--r--   0        0        0     9185 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/cdf.py
--rw-r--r--   0        0        0      442 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/echo.py
--rw-r--r--   0        0        0    27692 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/main.py
--rw-r--r--   0        0        0     2563 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/transform.py
--rw-r--r--   0        0        0     2161 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/core/validation.py
--rw-r--r--   0        0        0      474 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/__init__.py
--rw-r--r--   0        0        0     6774 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/core.py
--rw-r--r--   0        0        0    12631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/diff/data_classes.py
--rw-r--r--   0        0        0      424 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/__init__.py
--rw-r--r--   0        0        0       82 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
--rw-r--r--   0        0        0      811 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
--rw-r--r--   0        0        0    10495 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
--rw-r--r--   0        0        0     1143 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
--rw-r--r--   0        0        0     8337 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
--rw-r--r--   0        0        0      788 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/__init__.py
--rw-r--r--   0        0        0    11195 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_model.py
--rw-r--r--   0        0        0     9602 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_type.py
--rw-r--r--   0        0        0     5251 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/cdf_resources.py
--rw-r--r--   0        0        0    11641 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/data_model.py
--rw-r--r--   0        0        0     1896 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/dms_models.py
--rw-r--r--   0        0        0      592 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/graph_ql.py
--rw-r--r--   0        0        0      148 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/helpers.py
--rw-r--r--   0        0        0     6668 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/model.py
--rw-r--r--   0        0        0     1705 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/resource_type.py
--rw-r--r--   0        0        0     1302 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/__init__.py
--rw-r--r--   0        0        0     8141 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/cogshop.py
--rw-r--r--   0        0        0      243 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/__init__.py
--rw-r--r--   0        0        0     8940 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
--rw-r--r--   0        0        0    15631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
--rw-r--r--   0        0        0     9726 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
--rw-r--r--   0        0        0      491 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
--rw-r--r--   0        0        0      832 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
--rw-r--r--   0        0        0     3499 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/__init__.py
--rw-r--r--   0        0        0     1291 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/base.py
--rw-r--r--   0        0        0     3184 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/benchmark.py
--rw-r--r--   0        0        0     2405 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/dayahead.py
--rw-r--r--   0        0        0     2797 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/rkom.py
--rw-r--r--   0        0        0     7801 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/production.py
--rw-r--r--   0        0        0      395 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/__init__.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/__init__.py
--rw-r--r--   0        0        0     8873 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
--rw-r--r--   0        0        0    27181 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/powerops_models.py
--rw-r--r--   0        0        0     7631 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/production_dm.py
--rw-r--r--   0        0        0      150 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/__init__.py
--rw-r--r--   0        0        0     2149 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/mapping.py
--rw-r--r--   0        0        0     2456 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/static_mapping.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/__init__.py
--rw-r--r--   0        0        0      238 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/main.py
--rw-r--r--   0        0        0     7548 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/v2/shop_to_assets.py
--rw-r--r--   0        0        0     4524 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/resync/validation.py
--rw-r--r--   0        0        0        0 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/__init__.py
--rw-r--r--   0        0        0      160 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/__init__.py
--rw-r--r--   0        0        0     1389 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_cdf_auth.py
--rw-r--r--   0        0        0     3169 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_settings.py
--rw-r--r--   0        0        0     7517 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/calls.py
--rw-r--r--   0        0        0    10874 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/extraction_pipelines.py
--rw-r--r--   0        0        0      970 2024-04-22 09:30:11.491745 cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/resource_creation.py
--rw-r--r--   0        0        0     2540 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/lookup.py
--rw-r--r--   0        0        0     1097 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/navigation.py
--rw-r--r--   0        0        0      514 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/require.py
--rw-r--r--   0        0        0      227 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/retry/__init__.py
--rw-r--r--   0        0        0     5619 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/retry/api.py
--rw-r--r--   0        0        0     7828 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/serialization.py
--rw-r--r--   0        0        0     3667 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/cognite/powerops/utils/time.py
--rw-r--r--   0        0        0     3775 2024-04-22 09:30:11.495745 cognite_power_ops-0.94.1/pyproject.toml
--rw-r--r--   0        0        0     5516 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.1/PKG-INFO
+-rw-r--r--   0        0        0    10758 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/LICENSE
+-rw-r--r--   0        0        0     3322 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/README.md
+-rw-r--r--   0        0        0      150 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/__init__.py
+-rw-r--r--   0        0        0       23 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/_version.py
+-rw-r--r--   0        0        0     5273 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/cdf_labels.py
+-rw-r--r--   0        0        0     8779 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/cli.py
+-rw-r--r--   0        0        0       74 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/__init__.py
+-rw-r--r--   0        0        0      105 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32135 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/_core.py
+-rw-r--r--   0        0        0    26235 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/alert.py
+-rw-r--r--   0        0        0     1492 2024-05-07 07:54:21.408863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    27110 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2041 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2039 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py
+-rw-r--r--   0        0        0    11759 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16844 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1513 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    27874 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py
+-rw-r--r--   0        0        0     1971 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8302 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py
+-rw-r--r--   0        0        0    16131 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25401 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    25313 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    25313 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    25195 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    25692 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25604 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1513 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    25330 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    25780 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    25692 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     9211 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api_client.py
+-rw-r--r--   0        0        0     2654 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16231 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    19483 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0     8200 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    23816 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22916 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py
+-rw-r--r--   0        0        0     9041 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0      109 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/__init__.py
+-rw-r--r--   0        0        0    32350 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/_core.py
+-rw-r--r--   0        0        0    16860 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/bid_method.py
+-rw-r--r--   0        0        0     1511 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/bid_method_query.py
+-rw-r--r--   0        0        0    26226 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator.py
+-rw-r--r--   0        0        0    15705 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1625 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0    28005 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py
+-rw-r--r--   0        0        0     5828 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_query.py
+-rw-r--r--   0        0        0    27596 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2197 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py
+-rw-r--r--   0        0        0    32967 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant.py
+-rw-r--r--   0        0        0    30394 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     1998 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_generators.py
+-rw-r--r--   0        0        0    30394 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py
+-rw-r--r--   0        0        0    30394 2024-05-07 07:54:21.412863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py
+-rw-r--r--   0        0        0    30438 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py
+-rw-r--r--   0        0        0    30100 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py
+-rw-r--r--   0        0        0    30100 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py
+-rw-r--r--   0        0        0     8084 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_query.py
+-rw-r--r--   0        0        0    30394 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py
+-rw-r--r--   0        0        0    27060 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area.py
+-rw-r--r--   0        0        0    27668 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py
+-rw-r--r--   0        0        0    27580 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py
+-rw-r--r--   0        0        0    27580 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py
+-rw-r--r--   0        0        0    27462 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py
+-rw-r--r--   0        0        0    27374 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py
+-rw-r--r--   0        0        0    27739 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py
+-rw-r--r--   0        0        0    27959 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27871 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2011 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_plants.py
+-rw-r--r--   0        0        0    11709 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_query.py
+-rw-r--r--   0        0        0    27597 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py
+-rw-r--r--   0        0        0    28047 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27959 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     2095 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py
+-rw-r--r--   0        0        0    20054 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/reservoir.py
+-rw-r--r--   0        0        0     1510 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/reservoir_query.py
+-rw-r--r--   0        0        0    15561 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1615 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    22125 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse.py
+-rw-r--r--   0        0        0     2026 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py
+-rw-r--r--   0        0        0    26508 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py
+-rw-r--r--   0        0        0     6635 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_query.py
+-rw-r--r--   0        0        0    10150 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api_client.py
+-rw-r--r--   0        0        0     4810 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/__init__.py
+-rw-r--r--   0        0        0     8080 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_core.py
+-rw-r--r--   0        0        0    19940 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_generator.py
+-rw-r--r--   0        0        0     9827 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    32140 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_plant.py
+-rw-r--r--   0        0        0    33483 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_price_area.py
+-rw-r--r--   0        0        0    10168 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py
+-rw-r--r--   0        0        0     9697 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    13872 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py
+-rw-r--r--   0        0        0      113 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/__init__.py
+-rw-r--r--   0        0        0     8201 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/_core.py
+-rw-r--r--   0        0        0    14521 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/case.py
+-rw-r--r--   0        0        0     7486 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py
+-rw-r--r--   0        0        0     9780 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py
+-rw-r--r--   0        0        0    15960 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/mapping.py
+-rw-r--r--   0        0        0    17869 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/model_template.py
+-rw-r--r--   0        0        0    11367 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py
+-rw-r--r--   0        0        0    19744 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/scenario.py
+-rw-r--r--   0        0        0    10871 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/transformation.py
+-rw-r--r--   0        0        0     3003 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api_client.py
+-rw-r--r--   0        0        0     2524 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py
+-rw-r--r--   0        0        0     4596 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py
+-rw-r--r--   0        0        0     2226 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py
+-rw-r--r--   0        0        0     5824 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py
+-rw-r--r--   0        0        0     2393 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py
+-rw-r--r--   0        0        0     4586 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py
+-rw-r--r--   0        0        0     5174 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py
+-rw-r--r--   0        0        0     2819 2024-05-07 07:54:21.416863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py
+-rw-r--r--   0        0        0     6951 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py
+-rw-r--r--   0        0        0     2621 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py
+-rw-r--r--   0        0        0      118 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/__init__.py
+-rw-r--r--   0        0        0    32598 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py
+-rw-r--r--   0        0        0    26333 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py
+-rw-r--r--   0        0        0     1497 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py
+-rw-r--r--   0        0        0    23471 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py
+-rw-r--r--   0        0        0     2115 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7177 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py
+-rw-r--r--   0        0        0    29138 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py
+-rw-r--r--   0        0        0     2059 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0     2106 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py
+-rw-r--r--   0        0        0    13622 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py
+-rw-r--r--   0        0        0    22831 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py
+-rw-r--r--   0        0        0     2032 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py
+-rw-r--r--   0        0        0     7128 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    16942 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py
+-rw-r--r--   0        0        0     1518 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py
+-rw-r--r--   0        0        0    24946 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py
+-rw-r--r--   0        0        0     2185 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py
+-rw-r--r--   0        0        0    10308 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py
+-rw-r--r--   0        0        0     2410 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py
+-rw-r--r--   0        0        0    19843 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py
+-rw-r--r--   0        0        0    25798 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py
+-rw-r--r--   0        0        0    25883 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py
+-rw-r--r--   0        0        0     2613 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py
+-rw-r--r--   0        0        0    20327 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     2415 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py
+-rw-r--r--   0        0        0     4483 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py
+-rw-r--r--   0        0        0    18030 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py
+-rw-r--r--   0        0        0    24799 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py
+-rw-r--r--   0        0        0     1559 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py
+-rw-r--r--   0        0        0    15855 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py
+-rw-r--r--   0        0        0    24935 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py
+-rw-r--r--   0        0        0    25177 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py
+-rw-r--r--   0        0        0     2777 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py
+-rw-r--r--   0        0        0    18424 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py
+-rw-r--r--   0        0        0     1618 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py
+-rw-r--r--   0        0        0    11242 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py
+-rw-r--r--   0        0        0     7397 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py
+-rw-r--r--   0        0        0    16231 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py
+-rw-r--r--   0        0        0    14798 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py
+-rw-r--r--   0        0        0    24120 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    15156 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0     8094 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py
+-rw-r--r--   0        0        0    22916 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py
+-rw-r--r--   0        0        0    17204 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py
+-rw-r--r--   0        0        0    14748 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py
+-rw-r--r--   0        0        0    11974 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py
+-rw-r--r--   0        0        0     9405 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py
+-rw-r--r--   0        0        0    13294 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py
+-rw-r--r--   0        0        0     8961 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py
+-rw-r--r--   0        0        0      123 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/__init__.py
+-rw-r--r--   0        0        0    41803 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/_core.py
+-rw-r--r--   0        0        0    28392 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/alert.py
+-rw-r--r--   0        0        0     1486 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/alert_query.py
+-rw-r--r--   0        0        0    24852 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0     2445 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py
+-rw-r--r--   0        0        0     7859 2024-05-07 07:54:21.420863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py
+-rw-r--r--   0        0        0    27557 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document.py
+-rw-r--r--   0        0        0    29838 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py
+-rw-r--r--   0        0        0     2125 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py
+-rw-r--r--   0        0        0     2123 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py
+-rw-r--r--   0        0        0    11654 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py
+-rw-r--r--   0        0        0     2056 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py
+-rw-r--r--   0        0        0    31537 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py
+-rw-r--r--   0        0        0     2194 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py
+-rw-r--r--   0        0        0     2399 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py
+-rw-r--r--   0        0        0    13156 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py
+-rw-r--r--   0        0        0     6256 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_query.py
+-rw-r--r--   0        0        0    16995 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix.py
+-rw-r--r--   0        0        0    20707 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py
+-rw-r--r--   0        0        0     2194 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2352 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     9120 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py
+-rw-r--r--   0        0        0     1507 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py
+-rw-r--r--   0        0        0    24990 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row.py
+-rw-r--r--   0        0        0     1986 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py
+-rw-r--r--   0        0        0     8727 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row_query.py
+-rw-r--r--   0        0        0    23488 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_input.py
+-rw-r--r--   0        0        0     1527 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_input_query.py
+-rw-r--r--   0        0        0    26010 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output.py
+-rw-r--r--   0        0        0     2098 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py
+-rw-r--r--   0        0        0     7530 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output_query.py
+-rw-r--r--   0        0        0    30503 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator.py
+-rw-r--r--   0        0        0    29640 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py
+-rw-r--r--   0        0        0    14623 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py
+-rw-r--r--   0        0        0     1621 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py
+-rw-r--r--   0        0        0     5996 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_query.py
+-rw-r--r--   0        0        0    29214 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py
+-rw-r--r--   0        0        0     2275 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py
+-rw-r--r--   0        0        0    30967 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/market_configuration.py
+-rw-r--r--   0        0        0     1557 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py
+-rw-r--r--   0        0        0    21738 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py
+-rw-r--r--   0        0        0     2719 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    30364 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4187 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    31040 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2403 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0    10702 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    26004 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py
+-rw-r--r--   0        0        0     2305 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py
+-rw-r--r--   0        0        0     2463 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0    12658 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py
+-rw-r--r--   0        0        0    29102 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0     2502 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py
+-rw-r--r--   0        0        0     2660 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py
+-rw-r--r--   0        0        0     2676 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py
+-rw-r--r--   0        0        0    16509 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py
+-rw-r--r--   0        0        0    21267 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant.py
+-rw-r--r--   0        0        0    34870 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information.py
+-rw-r--r--   0        0        0    31031 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2177 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py
+-rw-r--r--   0        0        0    31031 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py
+-rw-r--r--   0        0        0    31031 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31075 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31163 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py
+-rw-r--r--   0        0        0    31163 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py
+-rw-r--r--   0        0        0     6307 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_query.py
+-rw-r--r--   0        0        0    31031 2024-05-07 07:54:21.424863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py
+-rw-r--r--   0        0        0     1486 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_query.py
+-rw-r--r--   0        0        0    35566 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py
+-rw-r--r--   0        0        0    31218 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py
+-rw-r--r--   0        0        0     2260 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py
+-rw-r--r--   0        0        0    31218 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py
+-rw-r--r--   0        0        0    31218 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py
+-rw-r--r--   0        0        0    31262 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py
+-rw-r--r--   0        0        0    31350 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py
+-rw-r--r--   0        0        0    31350 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py
+-rw-r--r--   0        0        0     6373 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py
+-rw-r--r--   0        0        0    31218 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py
+-rw-r--r--   0        0        0    21879 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/power_asset.py
+-rw-r--r--   0        0        0     1512 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/power_asset_query.py
+-rw-r--r--   0        0        0    21768 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area.py
+-rw-r--r--   0        0        0    23928 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py
+-rw-r--r--   0        0        0    27423 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py
+-rw-r--r--   0        0        0    27335 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py
+-rw-r--r--   0        0        0    27335 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py
+-rw-r--r--   0        0        0    27217 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py
+-rw-r--r--   0        0        0    27714 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27626 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1528 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py
+-rw-r--r--   0        0        0    27352 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py
+-rw-r--r--   0        0        0    27802 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    27714 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0    24500 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py
+-rw-r--r--   0        0        0    27713 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py
+-rw-r--r--   0        0        0    27521 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py
+-rw-r--r--   0        0        0     2794 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py
+-rw-r--r--   0        0        0    26627 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information.py
+-rw-r--r--   0        0        0    28169 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py
+-rw-r--r--   0        0        0    28081 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py
+-rw-r--r--   0        0        0    28081 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py
+-rw-r--r--   0        0        0    27963 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py
+-rw-r--r--   0        0        0    28081 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py
+-rw-r--r--   0        0        0    28460 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28372 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py
+-rw-r--r--   0        0        0    27889 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py
+-rw-r--r--   0        0        0     2851 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py
+-rw-r--r--   0        0        0    28098 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py
+-rw-r--r--   0        0        0    28548 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py
+-rw-r--r--   0        0        0    28460 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py
+-rw-r--r--   0        0        0     1507 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_query.py
+-rw-r--r--   0        0        0    18930 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production.py
+-rw-r--r--   0        0        0    25079 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_price.py
+-rw-r--r--   0        0        0    25321 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_production.py
+-rw-r--r--   0        0        0     2623 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_query.py
+-rw-r--r--   0        0        0    25220 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py
+-rw-r--r--   0        0        0     1601 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py
+-rw-r--r--   0        0        0    27660 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py
+-rw-r--r--   0        0        0    24151 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     3878 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    18438 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case.py
+-rw-r--r--   0        0        0     6064 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case_query.py
+-rw-r--r--   0        0        0     2071 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py
+-rw-r--r--   0        0        0    17214 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_commands.py
+-rw-r--r--   0        0        0     1521 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py
+-rw-r--r--   0        0        0    20249 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_file.py
+-rw-r--r--   0        0        0     1502 2024-05-07 07:54:21.428863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_file_query.py
+-rw-r--r--   0        0        0    23570 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model.py
+-rw-r--r--   0        0        0     2279 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py
+-rw-r--r--   0        0        0     5631 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model_query.py
+-rw-r--r--   0        0        0    32763 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2608 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py
+-rw-r--r--   0        0        0     7877 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29852 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py
+-rw-r--r--   0        0        0     1548 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py
+-rw-r--r--   0        0        0    29105 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py
+-rw-r--r--   0        0        0     2688 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py
+-rw-r--r--   0        0        0    27944 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py
+-rw-r--r--   0        0        0     2223 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py
+-rw-r--r--   0        0        0     8858 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py
+-rw-r--r--   0        0        0    16377 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result.py
+-rw-r--r--   0        0        0     2042 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py
+-rw-r--r--   0        0        0     2214 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py
+-rw-r--r--   0        0        0    11103 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_query.py
+-rw-r--r--   0        0        0    22289 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario.py
+-rw-r--r--   0        0        0     2338 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py
+-rw-r--r--   0        0        0     8104 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py
+-rw-r--r--   0        0        0    23085 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py
+-rw-r--r--   0        0        0     4851 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py
+-rw-r--r--   0        0        0     2216 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py
+-rw-r--r--   0        0        0    21375 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series.py
+-rw-r--r--   0        0        0     1533 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py
+-rw-r--r--   0        0        0    26338 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py
+-rw-r--r--   0        0        0    27685 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py
+-rw-r--r--   0        0        0     3695 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py
+-rw-r--r--   0        0        0    27490 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py
+-rw-r--r--   0        0        0     2153 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py
+-rw-r--r--   0        0        0     8841 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py
+-rw-r--r--   0        0        0    27145 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py
+-rw-r--r--   0        0        0     2743 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py
+-rw-r--r--   0        0        0    27652 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py
+-rw-r--r--   0        0        0     2195 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py
+-rw-r--r--   0        0        0     2330 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py
+-rw-r--r--   0        0        0    11719 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py
+-rw-r--r--   0        0        0    30353 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     2477 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py
+-rw-r--r--   0        0        0     5956 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    29442 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     2375 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py
+-rw-r--r--   0        0        0     9141 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py
+-rw-r--r--   0        0        0    15615 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py
+-rw-r--r--   0        0        0     1611 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py
+-rw-r--r--   0        0        0    24038 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0     2906 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py
+-rw-r--r--   0        0        0    32573 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0     4476 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py
+-rw-r--r--   0        0        0    21933 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/watercourse.py
+-rw-r--r--   0        0        0     1516 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/watercourse_query.py
+-rw-r--r--   0        0        0    44629 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api_client.py
+-rw-r--r--   0        0        0    37530 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/__init__.py
+-rw-r--r--   0        0        0    17776 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_alert.py
+-rw-r--r--   0        0        0    19097 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py
+-rw-r--r--   0        0        0    17055 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py
+-rw-r--r--   0        0        0    20377 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py
+-rw-r--r--   0        0        0    24090 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py
+-rw-r--r--   0        0        0     8899 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py
+-rw-r--r--   0        0        0    13521 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py
+-rw-r--r--   0        0        0    21991 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py
+-rw-r--r--   0        0        0    22919 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_core.py
+-rw-r--r--   0        0        0    12488 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_function_input.py
+-rw-r--r--   0        0        0    16546 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_function_output.py
+-rw-r--r--   0        0        0    23123 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_generator.py
+-rw-r--r--   0        0        0     9234 2024-05-07 07:54:21.432863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py
+-rw-r--r--   0        0        0    16741 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py
+-rw-r--r--   0        0        0    13579 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py
+-rw-r--r--   0        0        0    21950 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    23555 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0    21084 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py
+-rw-r--r--   0        0        0    23573 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py
+-rw-r--r--   0        0        0    10552 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant.py
+-rw-r--r--   0        0        0    26558 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py
+-rw-r--r--   0        0        0    29359 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py
+-rw-r--r--   0        0        0    11245 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py
+-rw-r--r--   0        0        0    10801 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area.py
+-rw-r--r--   0        0        0    23345 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py
+-rw-r--r--   0        0        0    17926 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py
+-rw-r--r--   0        0        0    28027 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py
+-rw-r--r--   0        0        0    13204 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_production.py
+-rw-r--r--   0        0        0    15412 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py
+-rw-r--r--   0        0        0    16843 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    14508 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py
+-rw-r--r--   0        0        0     8933 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py
+-rw-r--r--   0        0        0    11434 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py
+-rw-r--r--   0        0        0    16868 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py
+-rw-r--r--   0        0        0    24050 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    18171 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py
+-rw-r--r--   0        0        0    17791 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py
+-rw-r--r--   0        0        0    18602 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py
+-rw-r--r--   0        0        0    17342 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py
+-rw-r--r--   0        0        0    17049 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py
+-rw-r--r--   0        0        0    13264 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py
+-rw-r--r--   0        0        0    12545 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py
+-rw-r--r--   0        0        0    19594 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py
+-rw-r--r--   0        0        0    18692 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py
+-rw-r--r--   0        0        0    17272 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py
+-rw-r--r--   0        0        0    18343 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py
+-rw-r--r--   0        0        0    20134 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    19932 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py
+-rw-r--r--   0        0        0     9709 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py
+-rw-r--r--   0        0        0    14472 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py
+-rw-r--r--   0        0        0    22567 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py
+-rw-r--r--   0        0        0    10900 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py
+-rw-r--r--   0        0        0     1301 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/_logger.py
+-rw-r--r--   0        0        0      139 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/data_classes.py
+-rw-r--r--   0        0        0     1322 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/data_set_api.py
+-rw-r--r--   0        0        0     6750 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/powerops_client.py
+-rw-r--r--   0        0        0       62 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/__init__.py
+-rw-r--r--   0        0        0      885 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/_api_client.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/__init__.py
+-rw-r--r--   0        0        0     8367 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/dayahead_trigger_api.py
+-rw-r--r--   0        0        0     4797 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_result_files_api.py
+-rw-r--r--   0        0        0     4432 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_results_api.py
+-rw-r--r--   0        0        0     9593 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_run_api.py
+-rw-r--r--   0        0        0      600 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/__init__.py
+-rw-r--r--   0        0        0     4114 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/case.py
+-rw-r--r--   0        0        0     9057 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/dayahead_trigger.py
+-rw-r--r--   0        0        0     2720 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/helpers.py
+-rw-r--r--   0        0        0      603 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/plotting.py
+-rw-r--r--   0        0        0     6164 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_result_files.py
+-rw-r--r--   0        0        0     6607 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_results.py
+-rw-r--r--   0        0        0    10210 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_results_compare.py
+-rw-r--r--   0        0        0     3021 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_run.py
+-rw-r--r--   0        0        0     3743 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_run_event.py
+-rw-r--r--   0        0        0     4374 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_case.py
+-rw-r--r--   0        0        0     1101 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_file_reference.py
+-rw-r--r--   0        0        0    13466 2024-05-07 07:54:21.436863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run.py
+-rw-r--r--   0        0        0    15419 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run_api.py
+-rw-r--r--   0        0        0     3885 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run_filter.py
+-rw-r--r--   0        0        0      563 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/client/shop/utils.py
+-rw-r--r--   0        0        0      947 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/cognite_modules/_system.yaml
+-rw-r--r--   0        0        0     1941 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/config.dev.yaml
+-rw-r--r--   0        0        0      729 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1095 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml
+-rw-r--r--   0        0        0     1680 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      100 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/affr_space.space.yaml
+-rw-r--r--   0        0        0       92 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/asset.space.yaml
+-rw-r--r--   0        0        0      367 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidMethod.container.yaml
+-rw-r--r--   0        0        0     2102 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml
+-rw-r--r--   0        0        0      750 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     1380 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml
+-rw-r--r--   0        0        0      857 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml
+-rw-r--r--   0        0        0     1038 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml
+-rw-r--r--   0        0        0      502 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidMethod.container.yaml
+-rw-r--r--   0        0        0     1408 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml
+-rw-r--r--   0        0        0     2281 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml
+-rw-r--r--   0        0        0     2375 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml
+-rw-r--r--   0        0        0      556 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml
+-rw-r--r--   0        0        0      466 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidDocument.container.yaml
+-rw-r--r--   0        0        0      767 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml
+-rw-r--r--   0        0        0      371 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMethod.container.yaml
+-rw-r--r--   0        0        0      532 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml
+-rw-r--r--   0        0        0      618 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml
+-rw-r--r--   0        0        0      416 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenario.container.yaml
+-rw-r--r--   0        0        0      490 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPPriceScenarioResults.container.yaml
+-rw-r--r--   0        0        0      113 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/dayahead_space.space.yaml
+-rw-r--r--   0        0        0      118 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/instance.space.yaml
+-rw-r--r--   0        0        0     1515 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      116 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/shared.space.yaml
+-rw-r--r--   0        0        0       81 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/types.space.yaml
+-rw-r--r--   0        0        0     1379 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml
+-rw-r--r--   0        0        0      606 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml
+-rw-r--r--   0        0        0     3917 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml
+-rw-r--r--   0        0        0     2786 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml
+-rw-r--r--   0        0        0     2618 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml
+-rw-r--r--   0        0        0     1138 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml
+-rw-r--r--   0        0        0     5199 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml
+-rw-r--r--   0        0        0     5204 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1060 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml
+-rw-r--r--   0        0        0     1121 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml
+-rw-r--r--   0        0        0     1887 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml
+-rw-r--r--   0        0        0     2558 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml
+-rw-r--r--   0        0        0     2374 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0      858 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      579 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml
+-rw-r--r--   0        0        0     1945 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml
+-rw-r--r--   0        0        0     1845 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml
+-rw-r--r--   0        0        0      723 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml
+-rw-r--r--   0        0        0      700 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml
+-rw-r--r--   0        0        0      711 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml
+-rw-r--r--   0        0        0     1015 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml
+-rw-r--r--   0        0        0     1479 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml
+-rw-r--r--   0        0        0     1312 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml
+-rw-r--r--   0        0        0      666 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml
+-rw-r--r--   0        0        0     1230 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml
+-rw-r--r--   0        0        0      605 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml
+-rw-r--r--   0        0        0     4964 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     6519 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml
+-rw-r--r--   0        0        0     2052 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml
+-rw-r--r--   0        0        0     3499 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2918 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml
+-rw-r--r--   0        0        0     2575 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml
+-rw-r--r--   0        0        0     2276 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml
+-rw-r--r--   0        0        0     2163 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml
+-rw-r--r--   0        0        0     1748 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml
+-rw-r--r--   0        0        0      814 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml
+-rw-r--r--   0        0        0     1292 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml
+-rw-r--r--   0        0        0      496 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocumentDayAhead.container.yaml
+-rw-r--r--   0        0        0      771 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml
+-rw-r--r--   0        0        0     1659 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml
+-rw-r--r--   0        0        0      755 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml
+-rw-r--r--   0        0        0     3521 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml
+-rw-r--r--   0        0        0     1038 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml
+-rw-r--r--   0        0        0     2082 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml
+-rw-r--r--   0        0        0      756 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0     2425 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml
+-rw-r--r--   0        0        0     1076 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml
+-rw-r--r--   0        0        0     1628 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml
+-rw-r--r--   0        0        0      689 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml
+-rw-r--r--   0        0        0      710 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml
+-rw-r--r--   0        0        0      504 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPObjectiveValue.container.yaml
+-rw-r--r--   0        0        0     1074 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml
+-rw-r--r--   0        0        0     1106 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml
+-rw-r--r--   0        0        0     1462 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml
+-rw-r--r--   0        0        0      634 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml
+-rw-r--r--   0        0        0      464 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCommands.container.yaml
+-rw-r--r--   0        0        0     1128 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml
+-rw-r--r--   0        0        0     1446 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml
+-rw-r--r--   0        0        0      280 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopPartialBidConfiguration.container.yaml
+-rw-r--r--   0        0        0      978 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml
+-rw-r--r--   0        0        0      690 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml
+-rw-r--r--   0        0        0      869 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml
+-rw-r--r--   0        0        0     1789 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml
+-rw-r--r--   0        0        0     2661 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml
+-rw-r--r--   0        0        0      118 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/instance.space.yaml
+-rw-r--r--   0        0        0      104 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/models.space.yaml
+-rw-r--r--   0        0        0     5275 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml
+-rw-r--r--   0        0        0      854 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml
+-rw-r--r--   0        0        0       91 2024-05-07 07:54:21.440863 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/type.space.yaml
+-rw-r--r--   0        0        0     3704 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml
+-rw-r--r--   0        0        0     2834 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml
+-rw-r--r--   0        0        0     2983 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml
+-rw-r--r--   0        0        0      871 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml
+-rw-r--r--   0        0        0     1283 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml
+-rw-r--r--   0        0        0     2330 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml
+-rw-r--r--   0        0        0     1073 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0     1260 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml
+-rw-r--r--   0        0        0      535 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml
+-rw-r--r--   0        0        0      599 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml
+-rw-r--r--   0        0        0     4498 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml
+-rw-r--r--   0        0        0      512 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml
+-rw-r--r--   0        0        0     2932 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml
+-rw-r--r--   0        0        0     1659 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml
+-rw-r--r--   0        0        0      596 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml
+-rw-r--r--   0        0        0      543 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml
+-rw-r--r--   0        0        0     1476 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2264 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml
+-rw-r--r--   0        0        0     1059 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     1184 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml
+-rw-r--r--   0        0        0     2520 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml
+-rw-r--r--   0        0        0     1450 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml
+-rw-r--r--   0        0        0     1726 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml
+-rw-r--r--   0        0        0     1564 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml
+-rw-r--r--   0        0        0      701 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml
+-rw-r--r--   0        0        0     1225 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0     1349 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml
+-rw-r--r--   0        0        0      890 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml
+-rw-r--r--   0        0        0     2331 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml
+-rw-r--r--   0        0        0     1840 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml
+-rw-r--r--   0        0        0     1027 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml
+-rw-r--r--   0        0        0     1705 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml
+-rw-r--r--   0        0        0     2573 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml
+-rw-r--r--   0        0        0     1965 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml
+-rw-r--r--   0        0        0     1535 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml
+-rw-r--r--   0        0        0     1399 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml
+-rw-r--r--   0        0        0     1797 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1053 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml
+-rw-r--r--   0        0        0     1750 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1522 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml
+-rw-r--r--   0        0        0     1660 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml
+-rw-r--r--   0        0        0     1069 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml
+-rw-r--r--   0        0        0     1249 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml
+-rw-r--r--   0        0        0     1680 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     1336 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml
+-rw-r--r--   0        0        0     2119 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml
+-rw-r--r--   0        0        0      981 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml
+-rw-r--r--   0        0        0     1757 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1355 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml
+-rw-r--r--   0        0        0     1426 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml
+-rw-r--r--   0        0        0     1010 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml
+-rw-r--r--   0        0        0     1378 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml
+-rw-r--r--   0        0        0     1434 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml
+-rw-r--r--   0        0        0     1392 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml
+-rw-r--r--   0        0        0     2707 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml
+-rw-r--r--   0        0        0     1587 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml
+-rw-r--r--   0        0        0     1114 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/prerun_transformations/__init__.py
+-rw-r--r--   0        0        0    34098 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/prerun_transformations/transformations.py
+-rw-r--r--   0        0        0      278 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/resync/__init__.py
+-rw-r--r--   0        0        0     1792 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/__init__.py
+-rw-r--r--   0        0        0    12764 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/_main.py
+-rw-r--r--   0        0        0      595 2024-05-07 07:54:21.444862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/_settings.py
+-rw-r--r--   0        0        0    12408 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/_shared.py
+-rw-r--r--   0        0        0       75 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/cogshop/__init__.py
+-rw-r--r--   0        0        0      720 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/cogshop/shop_file_config.py
+-rw-r--r--   0        0        0      815 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/__init__.py
+-rw-r--r--   0        0        0     5486 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/_core.py
+-rw-r--r--   0        0        0     2106 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/benchmarking.py
+-rw-r--r--   0        0        0     2105 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/dayahead.py
+-rw-r--r--   0        0        0      961 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/market.py
+-rw-r--r--   0        0        0    10827 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/rkom.py
+-rw-r--r--   0        0        0      417 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/__init__.py
+-rw-r--r--   0        0        0      830 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/connections.py
+-rw-r--r--   0        0        0     1414 2024-05-07 07:54:21.448862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/generator.py
+-rw-r--r--   0        0        0     5675 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/plant.py
+-rw-r--r--   0        0        0     2868 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/watercourse.py
+-rw-r--r--   0        0        0      244 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/__init__.py
+-rw-r--r--   0        0        0     9185 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/cdf.py
+-rw-r--r--   0        0        0      442 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/echo.py
+-rw-r--r--   0        0        0    27692 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/main.py
+-rw-r--r--   0        0        0     2563 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/transform.py
+-rw-r--r--   0        0        0     2161 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/core/validation.py
+-rw-r--r--   0        0        0      474 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/diff/__init__.py
+-rw-r--r--   0        0        0     6774 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/diff/core.py
+-rw-r--r--   0        0        0    12631 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/diff/data_classes.py
+-rw-r--r--   0        0        0      424 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/__init__.py
+-rw-r--r--   0        0        0       82 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/__init__.py
+-rw-r--r--   0        0        0      811 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py
+-rw-r--r--   0        0        0    10495 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py
+-rw-r--r--   0        0        0     1143 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/market_model.py
+-rw-r--r--   0        0        0     8337 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/production_model.py
+-rw-r--r--   0        0        0      788 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/__init__.py
+-rw-r--r--   0        0        0    11195 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/asset_model.py
+-rw-r--r--   0        0        0     9602 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/asset_type.py
+-rw-r--r--   0        0        0     5251 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/cdf_resources.py
+-rw-r--r--   0        0        0    11641 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/data_model.py
+-rw-r--r--   0        0        0     1896 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/dms_models.py
+-rw-r--r--   0        0        0      592 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/graph_ql.py
+-rw-r--r--   0        0        0      148 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/helpers.py
+-rw-r--r--   0        0        0     6668 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/model.py
+-rw-r--r--   0        0        0     1705 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/resource_type.py
+-rw-r--r--   0        0        0     1302 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/__init__.py
+-rw-r--r--   0        0        0     8141 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/cogshop.py
+-rw-r--r--   0        0        0      243 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8940 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py
+-rw-r--r--   0        0        0    15631 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py
+-rw-r--r--   0        0        0     9726 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py
+-rw-r--r--   0        0        0      491 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/graphql_schemas/__init__.py
+-rw-r--r--   0        0        0      832 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql
+-rw-r--r--   0        0        0     3499 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/__init__.py
+-rw-r--r--   0        0        0     1291 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/base.py
+-rw-r--r--   0        0        0     3184 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/benchmark.py
+-rw-r--r--   0        0        0     2405 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/dayahead.py
+-rw-r--r--   0        0        0     2797 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/rkom.py
+-rw-r--r--   0        0        0     7801 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/production.py
+-rw-r--r--   0        0        0      395 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/config_to_model/__init__.py
+-rw-r--r--   0        0        0     8873 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py
+-rw-r--r--   0        0        0    27181 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/powerops_models.py
+-rw-r--r--   0        0        0     7631 2024-05-07 07:54:21.452862 cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/production_dm.py
+-rw-r--r--   0        0        0      150 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/time_series_mapping/__init__.py
+-rw-r--r--   0        0        0     2149 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/time_series_mapping/mapping.py
+-rw-r--r--   0        0        0     2456 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/time_series_mapping/static_mapping.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/v2/__init__.py
+-rw-r--r--   0        0        0      238 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/v2/main.py
+-rw-r--r--   0        0        0     7548 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/v2/shop_to_assets.py
+-rw-r--r--   0        0        0     4524 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/resync/validation.py
+-rw-r--r--   0        0        0        0 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/__init__.py
+-rw-r--r--   0        0        0      160 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/__init__.py
+-rw-r--r--   0        0        0     1389 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/_cdf_auth.py
+-rw-r--r--   0        0        0     3169 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/_settings.py
+-rw-r--r--   0        0        0     7517 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/calls.py
+-rw-r--r--   0        0        0    10874 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/extraction_pipelines.py
+-rw-r--r--   0        0        0      970 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/resource_creation.py
+-rw-r--r--   0        0        0     2540 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/lookup.py
+-rw-r--r--   0        0        0     1097 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/navigation.py
+-rw-r--r--   0        0        0      514 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/require.py
+-rw-r--r--   0        0        0      227 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/retry/__init__.py
+-rw-r--r--   0        0        0     5619 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/retry/api.py
+-rw-r--r--   0        0        0     7828 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/serialization.py
+-rw-r--r--   0        0        0     3667 2024-05-07 07:54:21.456862 cognite_power_ops-0.94.2/cognite/powerops/utils/time.py
+-rw-r--r--   0        0        0     3732 2024-05-07 07:54:21.460862 cognite_power_ops-0.94.2/pyproject.toml
+-rw-r--r--   0        0        0     5525 1970-01-01 00:00:00.000000 cognite_power_ops-0.94.2/PKG-INFO
```

### Comparing `cognite_power_ops-0.94.1/LICENSE` & `cognite_power_ops-0.94.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/README.md` & `cognite_power_ops-0.94.2/README.md`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/cdf_labels.py` & `cognite_power_ops-0.94.2/cognite/powerops/cdf_labels.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/cli.py` & `cognite_power_ops-0.94.2/cognite/powerops/cli.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,16 +19,16 @@
 
 
 class AFRRBidAPI:
     """
     AFRRBidAPI
 
     Generated with:
-        pygen = 0.99.19
-        cognite-sdk = 7.26.2
+        pygen = 0.99.22
+        cognite-sdk = 7.37.4
         pydantic = 2.7.0
 
     Data Model:
         space: power-ops-afrr-bid
         externalId: AFRRBid
         version: 1
     """
@@ -37,15 +37,15 @@
         if isinstance(config_or_client, CogniteClient):
             client = config_or_client
         elif isinstance(config_or_client, ClientConfig):
             client = CogniteClient(config_or_client)
         else:
             raise ValueError(f"Expected CogniteClient or ClientConfig, got {type(config_or_client)}")
         # The client name is used for aggregated logging of Pygen Usage
-        client.config.client_name = "CognitePygen:0.99.19"
+        client.config.client_name = "CognitePygen:0.99.22"
 
         view_by_read_class = {
             data_classes.Alert: dm.ViewId("power-ops-shared", "Alert", "1"),
             data_classes.BidDocument: dm.ViewId("power-ops-afrr-bid", "BidDocument", "1"),
             data_classes.BidMethod: dm.ViewId("power-ops-afrr-bid", "BidMethod", "1"),
             data_classes.BidRow: dm.ViewId("power-ops-afrr-bid", "BidRow", "1"),
             data_classes.PriceArea: dm.ViewId("power-ops-afrr-bid", "PriceArea", "1"),
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return values
 
     def as_read(self) -> Alert:
         """Convert this GraphQL format of alert to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Alert(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             time=self.time,
@@ -115,15 +115,15 @@
             event_ids=self.event_ids,
             calculation_run=self.calculation_run,
         )
 
     def as_write(self) -> AlertWrite:
         """Convert this GraphQL format of alert to the writing format."""
         return AlertWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             time=self.time,
             title=self.title,
             description=self.description,
             severity=self.severity,
             alert_type=self.alert_type,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         return value
 
     def as_read(self) -> BidDocument:
         """Convert this GraphQL format of bid document to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidDocument(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -123,15 +123,15 @@
             price_area=self.price_area.as_read() if isinstance(self.price_area, GraphQLCore) else self.price_area,
             bids=[bid.as_read() if isinstance(bid, GraphQLCore) else bid for bid in self.bids or []],
         )
 
     def as_write(self) -> BidDocumentWrite:
         """Convert this GraphQL format of bid document to the writing format."""
         return BidDocumentWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             delivery_date=self.delivery_date,
             start_calculation=self.start_calculation,
             end_calculation=self.end_calculation,
             is_complete=self.is_complete,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_method.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         return values
 
     def as_read(self) -> BidMethod:
         """Convert this GraphQL format of bid method to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMethod(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
         )
 
     def as_write(self) -> BidMethodWrite:
         """Convert this GraphQL format of bid method to the writing format."""
         return BidMethodWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
         )
 
 
 class BidMethod(DomainModel):
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_bid_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,15 +124,15 @@
         return value
 
     def as_read(self) -> BidRow:
         """Convert this GraphQL format of bid row to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidRow(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             price=self.price,
@@ -148,15 +148,15 @@
             method=self.method.as_read() if isinstance(self.method, GraphQLCore) else self.method,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> BidRowWrite:
         """Convert this GraphQL format of bid row to the writing format."""
         return BidRowWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             price=self.price,
             quantity_per_hour=self.quantity_per_hour,
             product=self.product,
             is_divisible=self.is_divisible,
             min_quantity=self.min_quantity,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/afrr_bid/data_classes/_price_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         return values
 
     def as_read(self) -> PriceArea:
         """Convert this GraphQL format of price area to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceArea(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/bid_method_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_is_available_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/generator_turbine_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_generators.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_p_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_p_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/plant_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_day_ahead_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_main_scenario_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_plants.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/price_area_watercourses.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/reservoir.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/reservoir_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/reservoir_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_plants.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_production_obligation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api/watercourse_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/_api_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,16 +22,16 @@
 
 
 class PowerAssetAPI:
     """
     PowerAssetAPI
 
     Generated with:
-        pygen = 0.99.19
-        cognite-sdk = 7.26.2
+        pygen = 0.99.22
+        cognite-sdk = 7.37.4
         pydantic = 2.7.0
 
     Data Model:
         space: power-ops-assets
         externalId: PowerAsset
         version: 1
     """
@@ -40,15 +40,15 @@
         if isinstance(config_or_client, CogniteClient):
             client = config_or_client
         elif isinstance(config_or_client, ClientConfig):
             client = CogniteClient(config_or_client)
         else:
             raise ValueError(f"Expected CogniteClient or ClientConfig, got {type(config_or_client)}")
         # The client name is used for aggregated logging of Pygen Usage
-        client.config.client_name = "CognitePygen:0.99.19"
+        client.config.client_name = "CognitePygen:0.99.22"
 
         view_by_read_class = {
             data_classes.BidMethod: dm.ViewId("power-ops-shared", "BidMethod", "1"),
             data_classes.Generator: dm.ViewId("power-ops-assets", "Generator", "1"),
             data_classes.GeneratorEfficiencyCurve: dm.ViewId("power-ops-assets", "GeneratorEfficiencyCurve", "1"),
             data_classes.Plant: dm.ViewId("power-ops-assets", "Plant", "1"),
             data_classes.PriceArea: dm.ViewId("power-ops-assets", "PriceArea", "1"),
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_bid_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         return values
 
     def as_read(self) -> BidMethod:
         """Convert this GraphQL format of bid method to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMethod(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
         )
 
     def as_write(self) -> BidMethodWrite:
         """Convert this GraphQL format of bid method to the writing format."""
         return BidMethodWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
         )
 
 
 class BidMethod(DomainModel):
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return value
 
     def as_read(self) -> Generator:
         """Convert this GraphQL format of generator to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Generator(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -147,15 +147,15 @@
                 for turbine_curve in self.turbine_curves or []
             ],
         )
 
     def as_write(self) -> GeneratorWrite:
         """Convert this GraphQL format of generator to the writing format."""
         return GeneratorWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             p_min=self.p_min,
             penstock=self.penstock,
             start_cost=self.start_cost,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_generator_efficiency_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,30 +73,30 @@
         return values
 
     def as_read(self) -> GeneratorEfficiencyCurve:
         """Convert this GraphQL format of generator efficiency curve to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return GeneratorEfficiencyCurve(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             ref=self.ref,
             power=self.power,
             efficiency=self.efficiency,
         )
 
     def as_write(self) -> GeneratorEfficiencyCurveWrite:
         """Convert this GraphQL format of generator efficiency curve to the writing format."""
         return GeneratorEfficiencyCurveWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             ref=self.ref,
             power=self.power,
             efficiency=self.efficiency,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_plant.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_plant.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         return value
 
     def as_read(self) -> Plant:
         """Convert this GraphQL format of plant to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Plant(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -202,15 +202,15 @@
                 for generator in self.generators or []
             ],
         )
 
     def as_write(self) -> PlantWrite:
         """Convert this GraphQL format of plant to the writing format."""
         return PlantWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             head_loss_factor=self.head_loss_factor,
             outlet_level=self.outlet_level,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_price_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -166,15 +166,15 @@
         return value
 
     def as_read(self) -> PriceArea:
         """Convert this GraphQL format of price area to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceArea(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -203,15 +203,15 @@
                 for watercourse in self.watercourses or []
             ],
         )
 
     def as_write(self) -> PriceAreaWrite:
         """Convert this GraphQL format of price area to the writing format."""
         return PriceAreaWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             description=self.description,
             timezone=self.timezone,
             capacity_price_up=self.capacity_price_up,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_reservoir.py`

 * *Files 6% similar despite different names*

```diff
@@ -77,30 +77,30 @@
         return values
 
     def as_read(self) -> Reservoir:
         """Convert this GraphQL format of reservoir to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Reservoir(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
         )
 
     def as_write(self) -> ReservoirWrite:
         """Convert this GraphQL format of reservoir to the writing format."""
         return ReservoirWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_turbine_efficiency_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,30 +73,30 @@
         return values
 
     def as_read(self) -> TurbineEfficiencyCurve:
         """Convert this GraphQL format of turbine efficiency curve to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TurbineEfficiencyCurve(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             head=self.head,
             flow=self.flow,
             efficiency=self.efficiency,
         )
 
     def as_write(self) -> TurbineEfficiencyCurveWrite:
         """Convert this GraphQL format of turbine efficiency curve to the writing format."""
         return TurbineEfficiencyCurveWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             head=self.head,
             flow=self.flow,
             efficiency=self.efficiency,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/assets/data_classes/_watercourse.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         return value
 
     def as_read(self) -> Watercourse:
         """Convert this GraphQL format of watercourse to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Watercourse(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -118,15 +118,15 @@
             penalty_limit=self.penalty_limit,
             plants=[plant.as_read() if isinstance(plant, GraphQLCore) else plant for plant in self.plants or []],
         )
 
     def as_write(self) -> WatercourseWrite:
         """Convert this GraphQL format of watercourse to the writing format."""
         return WatercourseWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             production_obligation=self.production_obligation,
             penalty_limit=self.penalty_limit,
             plants=[plant.as_write() if isinstance(plant, DomainModel) else plant for plant in self.plants or []],
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/model_template.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api/transformation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api/transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_commands_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_file_ref.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_model_template.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_processing_log.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/cogshop1/data_classes/_transformation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/basic_bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/bid_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/multi_scenario_matrix_scenario_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_main_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_multi_scenario_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/shop_price_scenario_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api/water_value_based_method_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 
 
 class DayAheadBidAPI:
     """
     DayAheadBidAPI
 
     Generated with:
-        pygen = 0.99.19
-        cognite-sdk = 7.26.2
+        pygen = 0.99.22
+        cognite-sdk = 7.37.4
         pydantic = 2.7.0
 
     Data Model:
         space: power-ops-day-ahead-bid
         externalId: DayAheadBid
         version: 1
     """
@@ -43,15 +43,15 @@
         if isinstance(config_or_client, CogniteClient):
             client = config_or_client
         elif isinstance(config_or_client, ClientConfig):
             client = CogniteClient(config_or_client)
         else:
             raise ValueError(f"Expected CogniteClient or ClientConfig, got {type(config_or_client)}")
         # The client name is used for aggregated logging of Pygen Usage
-        client.config.client_name = "CognitePygen:0.99.19"
+        client.config.client_name = "CognitePygen:0.99.22"
 
         view_by_read_class = {
             data_classes.Alert: dm.ViewId("power-ops-shared", "Alert", "1"),
             data_classes.BasicBidMatrix: dm.ViewId("power-ops-day-ahead-bid", "BasicBidMatrix", "1"),
             data_classes.BidDocument: dm.ViewId("power-ops-day-ahead-bid", "BidDocument", "1"),
             data_classes.BidMatrix: dm.ViewId("power-ops-day-ahead-bid", "BidMatrix", "1"),
             data_classes.BidMethod: dm.ViewId("power-ops-day-ahead-bid", "BidMethod", "1"),
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_alert.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return values
 
     def as_read(self) -> Alert:
         """Convert this GraphQL format of alert to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Alert(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             time=self.time,
@@ -115,15 +115,15 @@
             event_ids=self.event_ids,
             calculation_run=self.calculation_run,
         )
 
     def as_write(self) -> AlertWrite:
         """Convert this GraphQL format of alert to the writing format."""
         return AlertWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             time=self.time,
             title=self.title,
             description=self.description,
             severity=self.severity,
             alert_type=self.alert_type,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_basic_bid_matrix.py`

 * *Files 5% similar despite different names*

```diff
@@ -97,37 +97,37 @@
         return value
 
     def as_read(self) -> BasicBidMatrix:
         """Convert this GraphQL format of basic bid matrix to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BasicBidMatrix(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_read() if isinstance(self.method, GraphQLCore) else self.method,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> BasicBidMatrixWrite:
         """Convert this GraphQL format of basic bid matrix to the writing format."""
         return BasicBidMatrixWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_write() if isinstance(self.method, DomainModel) else self.method,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_document.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         return value
 
     def as_read(self) -> BidDocument:
         """Convert this GraphQL format of bid document to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidDocument(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -132,15 +132,15 @@
                 partial.as_read() if isinstance(partial, GraphQLCore) else partial for partial in self.partials or []
             ],
         )
 
     def as_write(self) -> BidDocumentWrite:
         """Convert this GraphQL format of bid document to the writing format."""
         return BidDocumentWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             delivery_date=self.delivery_date,
             start_calculation=self.start_calculation,
             end_calculation=self.end_calculation,
             is_complete=self.is_complete,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_matrix.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,37 +96,37 @@
         return value
 
     def as_read(self) -> BidMatrix:
         """Convert this GraphQL format of bid matrix to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMatrix(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_read() if isinstance(self.method, GraphQLCore) else self.method,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> BidMatrixWrite:
         """Convert this GraphQL format of bid matrix to the writing format."""
         return BidMatrixWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_write() if isinstance(self.method, DomainModel) else self.method,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_bid_method.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,28 +70,28 @@
         return values
 
     def as_read(self) -> BidMethod:
         """Convert this GraphQL format of bid method to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMethod(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
         )
 
     def as_write(self) -> BidMethodWrite:
         """Convert this GraphQL format of bid method to the writing format."""
         return BidMethodWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
         )
 
 
 class BidMethod(DomainModel):
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_multi_scenario_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,41 +106,41 @@
         return value
 
     def as_read(self) -> MultiScenarioMatrix:
         """Convert this GraphQL format of multi scenario matrix to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return MultiScenarioMatrix(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_read() if isinstance(self.method, GraphQLCore) else self.method,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             scenario_results=[
                 scenario_result.as_read() if isinstance(scenario_result, GraphQLCore) else scenario_result
                 for scenario_result in self.scenario_results or []
             ],
         )
 
     def as_write(self) -> MultiScenarioMatrixWrite:
         """Convert this GraphQL format of multi scenario matrix to the writing format."""
         return MultiScenarioMatrixWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             resource_cost=self.resource_cost,
-            matrix=self.matrix,
+            matrix=self.matrix["externalId"] if self.matrix and "externalId" in self.matrix else None,
             asset_type=self.asset_type,
             asset_id=self.asset_id,
             method=self.method.as_write() if isinstance(self.method, DomainModel) else self.method,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
             scenario_results=[
                 scenario_result.as_write() if isinstance(scenario_result, DomainModel) else scenario_result
                 for scenario_result in self.scenario_results or []
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_price_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
         return value
 
     def as_read(self) -> PriceArea:
         """Convert this GraphQL format of price area to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceArea(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -120,15 +120,15 @@
             main_scenario=self.main_scenario,
             price_scenarios=self.price_scenarios,
         )
 
     def as_write(self) -> PriceAreaWrite:
         """Convert this GraphQL format of price area to the writing format."""
         return PriceAreaWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             default_method=(
                 self.default_method.as_write() if isinstance(self.default_method, DomainModel) else self.default_method
             ),
             timezone=self.timezone,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_multi_scenario_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         return value
 
     def as_read(self) -> SHOPMultiScenarioMethod:
         """Convert this GraphQL format of shop multi scenario method to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return SHOPMultiScenarioMethod(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -106,15 +106,15 @@
                 for price_scenario in self.price_scenarios or []
             ],
         )
 
     def as_write(self) -> SHOPMultiScenarioMethodWrite:
         """Convert this GraphQL format of shop multi scenario method to the writing format."""
         return SHOPMultiScenarioMethodWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             shop_cases=self.shop_cases,
             price_scenarios=[
                 price_scenario.as_write() if isinstance(price_scenario, DomainModel) else price_scenario
                 for price_scenario in self.price_scenarios or []
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,29 +75,29 @@
         return values
 
     def as_read(self) -> SHOPPriceScenario:
         """Convert this GraphQL format of shop price scenario to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return SHOPPriceScenario(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
             price=self.price,
         )
 
     def as_write(self) -> SHOPPriceScenarioWrite:
         """Convert this GraphQL format of shop price scenario to the writing format."""
         return SHOPPriceScenarioWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             price=self.price,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_shop_price_scenario_result.py`

 * *Files 1% similar despite different names*

```diff
@@ -89,15 +89,15 @@
         return value
 
     def as_read(self) -> SHOPPriceScenarioResult:
         """Convert this GraphQL format of shop price scenario result to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return SHOPPriceScenarioResult(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             price=self.price,
@@ -106,15 +106,15 @@
                 self.price_scenario.as_read() if isinstance(self.price_scenario, GraphQLCore) else self.price_scenario
             ),
         )
 
     def as_write(self) -> SHOPPriceScenarioResultWrite:
         """Convert this GraphQL format of shop price scenario result to the writing format."""
         return SHOPPriceScenarioResultWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             price=self.price,
             production=self.production,
             price_scenario=(
                 self.price_scenario.as_write() if isinstance(self.price_scenario, DomainModel) else self.price_scenario
             ),
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/day_ahead_bid/data_classes/_water_value_based_method.py`

 * *Files 1% similar despite different names*

```diff
@@ -71,28 +71,28 @@
         return values
 
     def as_read(self) -> WaterValueBasedMethod:
         """Convert this GraphQL format of water value based method to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return WaterValueBasedMethod(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
         )
 
     def as_write(self) -> WaterValueBasedMethodWrite:
         """Convert this GraphQL format of water value based method to the writing format."""
         return WaterValueBasedMethodWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
         )
 
 
 class WaterValueBasedMethod(BidMethod):
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/alert.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/alert_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/alert_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_configuration_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_bids.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_partials.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_document_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_document_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_matrix_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/bid_row_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/bid_row_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/function_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/function_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_availability_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_start_stop_cost.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/generator_turbine_efficiency_curves.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/market_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/market_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_intermediate_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_multi_scenario_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/partial_bid_matrix_information_with_scenarios_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_information_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_feeding_fee_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_generators.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_head_direct_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_inlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_outlet_level_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_max_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_production_min_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/plant_water_value_based_water_value_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/power_asset.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/power_asset_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/power_asset_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_afrr_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_day_ahead_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_activation_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_capacity_price_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_main_price_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_own_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_price_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_relative_activation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_down.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_information_total_capacity_allocation_up.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_area_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_area_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_price.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_price.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_production.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/price_production_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/price_production_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_attribute_mapping_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_case_shop_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_commands.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_commands_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_file.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_file_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_file_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model_base_attribute_mappings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_model_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_model_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_price_production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_penalty_report.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_penalty_report_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_preprocessor_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_output_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_result_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_result_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_attribute_mappings_override.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_scenario_set_scenarios.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_time_series_time_series.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/shop_trigger_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_process_sub_tasks.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/task_dispatcher_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_partial_bid_matrices.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_alerts.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/total_bid_matrix_calculation_output_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/turbine_efficiency_curve_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_configuration_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/water_value_based_partial_bid_matrix_calculation_input_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api/watercourse_query.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api/watercourse_query.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/_api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -597,29 +597,29 @@
 
 
 class PowerOpsModelsV1Client:
     """
     PowerOpsModelsV1Client
 
     Generated with:
-        pygen = 0.99.19
-        cognite-sdk = 7.26.2
+        pygen = 0.99.22
+        cognite-sdk = 7.37.4
         pydantic = 2.7.0
 
     """
 
     def __init__(self, config_or_client: CogniteClient | ClientConfig):
         if isinstance(config_or_client, CogniteClient):
             client = config_or_client
         elif isinstance(config_or_client, ClientConfig):
             client = CogniteClient(config_or_client)
         else:
             raise ValueError(f"Expected CogniteClient or ClientConfig, got {type(config_or_client)}")
         # The client name is used for aggregated logging of Pygen Usage
-        client.config.client_name = "CognitePygen:0.99.19"
+        client.config.client_name = "CognitePygen:0.99.22"
 
         self.shop_based_day_ahead_bid_process = ShopBasedDayAheadBidProcesAPIs(client)
         self.total_bid_matrix_calculation = TotalBidMatrixCalculationAPIs(client)
         self.water_value_based_day_ahead_bid_process = WaterValueBasedDayAheadBidProcesAPIs(client)
         self.day_ahead_configuration = DayAheadConfigurationAPIs(client)
         self.afrr_bid = AFRRBidAPIs(client)
         self.power_asset = PowerAssetAPIs(client)
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_alert.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_alert.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return values
 
     def as_read(self) -> Alert:
         """Convert this GraphQL format of alert to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Alert(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             time=self.time,
@@ -127,15 +127,15 @@
             event_ids=self.event_ids,
             calculation_run=self.calculation_run,
         )
 
     def as_write(self) -> AlertWrite:
         """Convert this GraphQL format of alert to the writing format."""
         return AlertWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             time=self.time,
             workflow_execution_id=self.workflow_execution_id,
             title=self.title,
             description=self.description,
             severity=self.severity,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_configuration_day_ahead.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return value
 
     def as_read(self) -> BidConfigurationDayAhead:
         """Convert this GraphQL format of bid configuration day ahead to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidConfigurationDayAhead(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -120,15 +120,15 @@
                 partial.as_read() if isinstance(partial, GraphQLCore) else partial for partial in self.partials or []
             ],
         )
 
     def as_write(self) -> BidConfigurationDayAheadWrite:
         """Convert this GraphQL format of bid configuration day ahead to the writing format."""
         return BidConfigurationDayAheadWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             market_configuration=(
                 self.market_configuration.as_write()
                 if isinstance(self.market_configuration, DomainModel)
                 else self.market_configuration
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
         return value
 
     def as_read(self) -> BidDocument:
         """Convert this GraphQL format of bid document to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidDocument(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -121,15 +121,15 @@
             is_complete=self.is_complete,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> BidDocumentWrite:
         """Convert this GraphQL format of bid document to the writing format."""
         return BidDocumentWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             workflow_execution_id=self.workflow_execution_id,
             delivery_date=self.delivery_date,
             start_calculation=self.start_calculation,
             end_calculation=self.end_calculation,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document_afrr.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,15 +109,15 @@
         return value
 
     def as_read(self) -> BidDocumentAFRR:
         """Convert this GraphQL format of bid document afrr to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidDocumentAFRR(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -130,15 +130,15 @@
             price_area=self.price_area.as_read() if isinstance(self.price_area, GraphQLCore) else self.price_area,
             bids=[bid.as_read() if isinstance(bid, GraphQLCore) else bid for bid in self.bids or []],
         )
 
     def as_write(self) -> BidDocumentAFRRWrite:
         """Convert this GraphQL format of bid document afrr to the writing format."""
         return BidDocumentAFRRWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             workflow_execution_id=self.workflow_execution_id,
             delivery_date=self.delivery_date,
             start_calculation=self.start_calculation,
             end_calculation=self.end_calculation,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_document_day_ahead.py`

 * *Files 0% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         return value
 
     def as_read(self) -> BidDocumentDayAhead:
         """Convert this GraphQL format of bid document day ahead to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidDocumentDayAhead(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -148,15 +148,15 @@
                 partial.as_read() if isinstance(partial, GraphQLCore) else partial for partial in self.partials or []
             ],
         )
 
     def as_write(self) -> BidDocumentDayAheadWrite:
         """Convert this GraphQL format of bid document day ahead to the writing format."""
         return BidDocumentDayAheadWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             workflow_execution_id=self.workflow_execution_id,
             delivery_date=self.delivery_date,
             start_calculation=self.start_calculation,
             end_calculation=self.end_calculation,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,33 +74,33 @@
         return values
 
     def as_read(self) -> BidMatrix:
         """Convert this GraphQL format of bid matrix to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMatrix(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
         )
 
     def as_write(self) -> BidMatrixWrite:
         """Convert this GraphQL format of bid matrix to the writing format."""
         return BidMatrixWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
         )
 
 
 class BidMatrix(DomainModel):
     """This represents the reading version of bid matrix.
 
     It is used to when data is retrieved from CDF.
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_matrix_information.py`

 * *Files 5% similar despite different names*

```diff
@@ -93,42 +93,42 @@
         return value
 
     def as_read(self) -> BidMatrixInformation:
         """Convert this GraphQL format of bid matrix information to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidMatrixInformation(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_read()
                     if isinstance(intermediate_bid_matrice, GraphQLCore)
                     else intermediate_bid_matrice
                 )
                 for intermediate_bid_matrice in self.intermediate_bid_matrices or []
             ],
         )
 
     def as_write(self) -> BidMatrixInformationWrite:
         """Convert this GraphQL format of bid matrix information to the writing format."""
         return BidMatrixInformationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_write()
                     if isinstance(intermediate_bid_matrice, DomainModel)
                     else intermediate_bid_matrice
                 )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_bid_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,15 @@
         return value
 
     def as_read(self) -> BidRow:
         """Convert this GraphQL format of bid row to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return BidRow(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             price=self.price,
@@ -132,15 +132,15 @@
             power_asset=self.power_asset.as_read() if isinstance(self.power_asset, GraphQLCore) else self.power_asset,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> BidRowWrite:
         """Convert this GraphQL format of bid row to the writing format."""
         return BidRowWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             price=self.price,
             quantity_per_hour=self.quantity_per_hour,
             product=self.product,
             is_divisible=self.is_divisible,
             min_quantity=self.min_quantity,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_function_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return values
 
     def as_read(self) -> FunctionInput:
         """Convert this GraphQL format of function input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return FunctionInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -96,15 +96,15 @@
             function_name=self.function_name,
             function_call_id=self.function_call_id,
         )
 
     def as_write(self) -> FunctionInputWrite:
         """Convert this GraphQL format of function input to the writing format."""
         return FunctionInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_function_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_function_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -96,15 +96,15 @@
         return value
 
     def as_read(self) -> FunctionOutput:
         """Convert this GraphQL format of function output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return FunctionOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -114,15 +114,15 @@
             input_=self.input_.as_read() if isinstance(self.input_, GraphQLCore) else self.input_,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
         )
 
     def as_write(self) -> FunctionOutputWrite:
         """Convert this GraphQL format of function output to the writing format."""
         return FunctionOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -136,15 +136,15 @@
         return value
 
     def as_read(self) -> Generator:
         """Convert this GraphQL format of generator to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Generator(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -170,15 +170,15 @@
                 for turbine_efficiency_curve in self.turbine_efficiency_curves or []
             ],
         )
 
     def as_write(self) -> GeneratorWrite:
         """Convert this GraphQL format of generator to the writing format."""
         return GeneratorWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             production_min=self.production_min,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_generator_efficiency_curve.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,29 +70,29 @@
         return values
 
     def as_read(self) -> GeneratorEfficiencyCurve:
         """Convert this GraphQL format of generator efficiency curve to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return GeneratorEfficiencyCurve(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             power=self.power,
             efficiency=self.efficiency,
         )
 
     def as_write(self) -> GeneratorEfficiencyCurveWrite:
         """Convert this GraphQL format of generator efficiency curve to the writing format."""
         return GeneratorEfficiencyCurveWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             power=self.power,
             efficiency=self.efficiency,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_market_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
         return values
 
     def as_read(self) -> MarketConfiguration:
         """Convert this GraphQL format of market configuration to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return MarketConfiguration(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -118,15 +118,15 @@
             time_unit=self.time_unit,
             trade_lot=self.trade_lot,
         )
 
     def as_write(self) -> MarketConfigurationWrite:
         """Convert this GraphQL format of market configuration to the writing format."""
         return MarketConfigurationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             max_price=self.max_price,
             min_price=self.min_price,
             timezone=self.timezone,
             price_unit=self.price_unit,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return value
 
     def as_read(self) -> PartialBidConfiguration:
         """Convert this GraphQL format of partial bid configuration to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PartialBidConfiguration(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -106,15 +106,15 @@
             power_asset=self.power_asset.as_read() if isinstance(self.power_asset, GraphQLCore) else self.power_asset,
             add_steps=self.add_steps,
         )
 
     def as_write(self) -> PartialBidConfigurationWrite:
         """Convert this GraphQL format of partial bid configuration to the writing format."""
         return PartialBidConfigurationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             method=self.method,
             power_asset=self.power_asset.as_write() if isinstance(self.power_asset, DomainModel) else self.power_asset,
             add_steps=self.add_steps,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         return value
 
     def as_read(self) -> PartialBidMatrixCalculationInput:
         """Convert this GraphQL format of partial bid matrix calculation input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PartialBidMatrixCalculationInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -140,15 +140,15 @@
                 else self.partial_bid_configuration
             ),
         )
 
     def as_write(self) -> PartialBidMatrixCalculationInputWrite:
         """Convert this GraphQL format of partial bid matrix calculation input to the writing format."""
         return PartialBidMatrixCalculationInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             bid_date=self.bid_date,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_calculation_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         return value
 
     def as_read(self) -> PartialBidMatrixCalculationOutput:
         """Convert this GraphQL format of partial bid matrix calculation output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PartialBidMatrixCalculationOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -139,15 +139,15 @@
                 else self.bid_configuration
             ),
         )
 
     def as_write(self) -> PartialBidMatrixCalculationOutputWrite:
         """Convert this GraphQL format of partial bid matrix calculation output to the writing format."""
         return PartialBidMatrixCalculationOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,23 +108,23 @@
         return value
 
     def as_read(self) -> PartialBidMatrixInformation:
         """Convert this GraphQL format of partial bid matrix information to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PartialBidMatrixInformation(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_read()
                     if isinstance(intermediate_bid_matrice, GraphQLCore)
                     else intermediate_bid_matrice
                 )
@@ -138,19 +138,19 @@
                 else self.partial_bid_configuration
             ),
         )
 
     def as_write(self) -> PartialBidMatrixInformationWrite:
         """Convert this GraphQL format of partial bid matrix information to the writing format."""
         return PartialBidMatrixInformationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_write()
                     if isinstance(intermediate_bid_matrice, DomainModel)
                     else intermediate_bid_matrice
                 )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_partial_bid_matrix_information_with_scenarios.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,23 +120,23 @@
         return value
 
     def as_read(self) -> PartialBidMatrixInformationWithScenarios:
         """Convert this GraphQL format of partial bid matrix information with scenario to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PartialBidMatrixInformationWithScenarios(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_read()
                     if isinstance(intermediate_bid_matrice, GraphQLCore)
                     else intermediate_bid_matrice
                 )
@@ -158,19 +158,19 @@
                 for multi_scenario_input in self.multi_scenario_input or []
             ],
         )
 
     def as_write(self) -> PartialBidMatrixInformationWithScenariosWrite:
         """Convert this GraphQL format of partial bid matrix information with scenario to the writing format."""
         return PartialBidMatrixInformationWithScenariosWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             state=self.state,
-            bid_matrix=self.bid_matrix,
+            bid_matrix=self.bid_matrix["externalId"] if self.bid_matrix and "externalId" in self.bid_matrix else None,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
             intermediate_bid_matrices=[
                 (
                     intermediate_bid_matrice.as_write()
                     if isinstance(intermediate_bid_matrice, DomainModel)
                     else intermediate_bid_matrice
                 )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return values
 
     def as_read(self) -> Plant:
         """Convert this GraphQL format of plant to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Plant(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -97,15 +97,15 @@
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
 
     def as_write(self) -> PlantWrite:
         """Convert this GraphQL format of plant to the writing format."""
         return PlantWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         return value
 
     def as_read(self) -> PlantInformation:
         """Convert this GraphQL format of plant information to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PlantInformation(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -197,15 +197,15 @@
                 for generator in self.generators or []
             ],
         )
 
     def as_write(self) -> PlantInformationWrite:
         """Convert this GraphQL format of plant information to the writing format."""
         return PlantInformationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             head_loss_factor=self.head_loss_factor,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_plant_water_value_based.py`

 * *Files 1% similar despite different names*

```diff
@@ -164,15 +164,15 @@
         return value
 
     def as_read(self) -> PlantWaterValueBased:
         """Convert this GraphQL format of plant water value based to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PlantWaterValueBased(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -197,15 +197,15 @@
                 for generator in self.generators or []
             ],
         )
 
     def as_write(self) -> PlantWaterValueBasedWrite:
         """Convert this GraphQL format of plant water value based to the writing format."""
         return PlantWaterValueBasedWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             head_loss_factor=self.head_loss_factor,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_power_asset.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
         return values
 
     def as_read(self) -> PowerAsset:
         """Convert this GraphQL format of power asset to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PowerAsset(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -96,15 +96,15 @@
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
 
     def as_write(self) -> PowerAssetWrite:
         """Convert this GraphQL format of power asset to the writing format."""
         return PowerAssetWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return values
 
     def as_read(self) -> PriceArea:
         """Convert this GraphQL format of price area to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceArea(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -97,15 +97,15 @@
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
 
     def as_write(self) -> PriceAreaWrite:
         """Convert this GraphQL format of price area to the writing format."""
         return PriceAreaWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_afrr.py`

 * *Files 0% similar despite different names*

```diff
@@ -137,15 +137,15 @@
         return values
 
     def as_read(self) -> PriceAreaAFRR:
         """Convert this GraphQL format of price area afrr to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceAreaAFRR(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -162,15 +162,15 @@
             own_capacity_allocation_up=self.own_capacity_allocation_up,
             own_capacity_allocation_down=self.own_capacity_allocation_down,
         )
 
     def as_write(self) -> PriceAreaAFRRWrite:
         """Convert this GraphQL format of price area afrr to the writing format."""
         return PriceAreaAFRRWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             capacity_price_up=self.capacity_price_up,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_day_ahead.py`

 * *Files 1% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         return value
 
     def as_read(self) -> PriceAreaDayAhead:
         """Convert this GraphQL format of price area day ahead to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceAreaDayAhead(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -139,15 +139,15 @@
             main_price_scenario=self.main_price_scenario,
             price_scenarios=self.price_scenarios,
         )
 
     def as_write(self) -> PriceAreaDayAheadWrite:
         """Convert this GraphQL format of price area day ahead to the writing format."""
         return PriceAreaDayAheadWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             default_bid_configuration=(
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_area_information.py`

 * *Files 0% similar despite different names*

```diff
@@ -173,15 +173,15 @@
         return value
 
     def as_read(self) -> PriceAreaInformation:
         """Convert this GraphQL format of price area information to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceAreaInformation(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -205,15 +205,15 @@
             main_price_scenario=self.main_price_scenario,
             price_scenarios=self.price_scenarios,
         )
 
     def as_write(self) -> PriceAreaInformationWrite:
         """Convert this GraphQL format of price area information to the writing format."""
         return PriceAreaInformationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
             capacity_price_up=self.capacity_price_up,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_price_production.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_price_production.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,15 @@
         return value
 
     def as_read(self) -> PriceProduction:
         """Convert this GraphQL format of price production to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return PriceProduction(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -108,15 +108,15 @@
             production=self.production,
             shop_result=self.shop_result.as_read() if isinstance(self.shop_result, GraphQLCore) else self.shop_result,
         )
 
     def as_write(self) -> PriceProductionWrite:
         """Convert this GraphQL format of price production to the writing format."""
         return PriceProductionWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             price=self.price,
             production=self.production,
             shop_result=self.shop_result.as_write() if isinstance(self.shop_result, DomainModel) else self.shop_result,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_attribute_mapping.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return values
 
     def as_read(self) -> ShopAttributeMapping:
         """Convert this GraphQL format of shop attribute mapping to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopAttributeMapping(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             object_type=self.object_type,
@@ -114,15 +114,15 @@
             retrieve=self.retrieve,
             aggregation=self.aggregation,
         )
 
     def as_write(self) -> ShopAttributeMappingWrite:
         """Convert this GraphQL format of shop attribute mapping to the writing format."""
         return ShopAttributeMappingWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             object_type=self.object_type,
             object_name=self.object_name,
             attribute_name=self.attribute_name,
             time_series=self.time_series,
             transformations=self.transformations,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_based_partial_bid_configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         return value
 
     def as_read(self) -> ShopBasedPartialBidConfiguration:
         """Convert this GraphQL format of shop based partial bid configuration to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopBasedPartialBidConfiguration(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -113,15 +113,15 @@
                 self.scenario_set.as_read() if isinstance(self.scenario_set, GraphQLCore) else self.scenario_set
             ),
         )
 
     def as_write(self) -> ShopBasedPartialBidConfigurationWrite:
         """Convert this GraphQL format of shop based partial bid configuration to the writing format."""
         return ShopBasedPartialBidConfigurationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             method=self.method,
             power_asset=self.power_asset.as_write() if isinstance(self.power_asset, DomainModel) else self.power_asset,
             add_steps=self.add_steps,
             scenario_set=(
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_case.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         return value
 
     def as_read(self) -> ShopCase:
         """Convert this GraphQL format of shop case to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopCase(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             scenario=self.scenario.as_read() if isinstance(self.scenario, GraphQLCore) else self.scenario,
@@ -107,15 +107,15 @@
                 for shop_file in self.shop_files or []
             ],
         )
 
     def as_write(self) -> ShopCaseWrite:
         """Convert this GraphQL format of shop case to the writing format."""
         return ShopCaseWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             scenario=self.scenario.as_write() if isinstance(self.scenario, DomainModel) else self.scenario,
             start_time=self.start_time,
             end_time=self.end_time,
             shop_files=[
                 shop_file.as_write() if isinstance(shop_file, DomainModel) else shop_file
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_commands.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,29 +73,29 @@
         return values
 
     def as_read(self) -> ShopCommands:
         """Convert this GraphQL format of shop command to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopCommands(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
             commands=self.commands,
         )
 
     def as_write(self) -> ShopCommandsWrite:
         """Convert this GraphQL format of shop command to the writing format."""
         return ShopCommandsWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             commands=self.commands,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,37 +83,45 @@
         return values
 
     def as_read(self) -> ShopFile:
         """Convert this GraphQL format of shop file to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopFile(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
             label=self.label,
-            file_reference=self.file_reference,
+            file_reference=(
+                self.file_reference["externalId"]
+                if self.file_reference and "externalId" in self.file_reference
+                else None
+            ),
             order=self.order,
             is_ascii=self.is_ascii,
         )
 
     def as_write(self) -> ShopFileWrite:
         """Convert this GraphQL format of shop file to the writing format."""
         return ShopFileWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             label=self.label,
-            file_reference=self.file_reference,
+            file_reference=(
+                self.file_reference["externalId"]
+                if self.file_reference and "externalId" in self.file_reference
+                else None
+            ),
             order=self.order,
             is_ascii=self.is_ascii,
         )
 
 
 class ShopFile(DomainModel):
     """This represents the reading version of shop file.
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,51 +112,51 @@
         return value
 
     def as_read(self) -> ShopModel:
         """Convert this GraphQL format of shop model to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopModel(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
             version_=self.version_,
             shop_version=self.shop_version,
             penalty_limit=self.penalty_limit,
-            model=self.model,
+            model=self.model["externalId"] if self.model and "externalId" in self.model else None,
             cog_shop_files_config=self.cog_shop_files_config,
-            extra_files=self.extra_files,
+            extra_files=[item["externalId"] for item in self.extra_files or [] if "externalId" in item] or None,
             base_attribute_mappings=[
                 (
                     base_attribute_mapping.as_read()
                     if isinstance(base_attribute_mapping, GraphQLCore)
                     else base_attribute_mapping
                 )
                 for base_attribute_mapping in self.base_attribute_mappings or []
             ],
         )
 
     def as_write(self) -> ShopModelWrite:
         """Convert this GraphQL format of shop model to the writing format."""
         return ShopModelWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             version_=self.version_,
             shop_version=self.shop_version,
             penalty_limit=self.penalty_limit,
-            model=self.model,
+            model=self.model["externalId"] if self.model and "externalId" in self.model else None,
             cog_shop_files_config=self.cog_shop_files_config,
-            extra_files=self.extra_files,
+            extra_files=[item["externalId"] for item in self.extra_files or [] if "externalId" in item] or None,
             base_attribute_mappings=[
                 (
                     base_attribute_mapping.as_write()
                     if isinstance(base_attribute_mapping, DomainModel)
                     else base_attribute_mapping
                 )
                 for base_attribute_mapping in self.base_attribute_mappings or []
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_partial_bid_matrix_calculation_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
         return value
 
     def as_read(self) -> ShopPartialBidMatrixCalculationInput:
         """Convert this GraphQL format of shop partial bid matrix calculation input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopPartialBidMatrixCalculationInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -150,15 +150,15 @@
                 for price_production in self.price_production or []
             ],
         )
 
     def as_write(self) -> ShopPartialBidMatrixCalculationInputWrite:
         """Convert this GraphQL format of shop partial bid matrix calculation input to the writing format."""
         return ShopPartialBidMatrixCalculationInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             bid_date=self.bid_date,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_penalty_report.py`

 * *Files 1% similar despite different names*

```diff
@@ -113,15 +113,15 @@
         return values
 
     def as_read(self) -> ShopPenaltyReport:
         """Convert this GraphQL format of shop penalty report to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopPenaltyReport(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             time=self.time,
@@ -135,15 +135,15 @@
             calculation_run=self.calculation_run,
             penalties=self.penalties,
         )
 
     def as_write(self) -> ShopPenaltyReportWrite:
         """Convert this GraphQL format of shop penalty report to the writing format."""
         return ShopPenaltyReportWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             time=self.time,
             workflow_execution_id=self.workflow_execution_id,
             title=self.title,
             description=self.description,
             severity=self.severity,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -103,15 +103,15 @@
         return value
 
     def as_read(self) -> ShopPreprocessorInput:
         """Convert this GraphQL format of shop preprocessor input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopPreprocessorInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -122,15 +122,15 @@
             start_time=self.start_time,
             end_time=self.end_time,
         )
 
     def as_write(self) -> ShopPreprocessorInputWrite:
         """Convert this GraphQL format of shop preprocessor input to the writing format."""
         return ShopPreprocessorInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             scenario=self.scenario.as_write() if isinstance(self.scenario, DomainModel) else self.scenario,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_preprocessor_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         return value
 
     def as_read(self) -> ShopPreprocessorOutput:
         """Convert this GraphQL format of shop preprocessor output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopPreprocessorOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -123,15 +123,15 @@
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             case=self.case.as_read() if isinstance(self.case, GraphQLCore) else self.case,
         )
 
     def as_write(self) -> ShopPreprocessorOutputWrite:
         """Convert this GraphQL format of shop preprocessor output to the writing format."""
         return ShopPreprocessorOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -104,46 +104,54 @@
         return value
 
     def as_read(self) -> ShopResult:
         """Convert this GraphQL format of shop result to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopResult(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             case=self.case.as_read() if isinstance(self.case, GraphQLCore) else self.case,
-            objective_sequence=self.objective_sequence,
-            pre_run=self.pre_run,
-            post_run=self.post_run,
-            messages=self.messages,
-            cplex_logs=self.cplex_logs,
+            objective_sequence=(
+                self.objective_sequence["externalId"]
+                if self.objective_sequence and "externalId" in self.objective_sequence
+                else None
+            ),
+            pre_run=self.pre_run["externalId"] if self.pre_run and "externalId" in self.pre_run else None,
+            post_run=self.post_run["externalId"] if self.post_run and "externalId" in self.post_run else None,
+            messages=self.messages["externalId"] if self.messages and "externalId" in self.messages else None,
+            cplex_logs=self.cplex_logs["externalId"] if self.cplex_logs and "externalId" in self.cplex_logs else None,
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             output_time_series=[
                 output_time_series.as_read() if isinstance(output_time_series, GraphQLCore) else output_time_series
                 for output_time_series in self.output_time_series or []
             ],
         )
 
     def as_write(self) -> ShopResultWrite:
         """Convert this GraphQL format of shop result to the writing format."""
         return ShopResultWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             case=self.case.as_write() if isinstance(self.case, DomainModel) else self.case,
-            objective_sequence=self.objective_sequence,
-            pre_run=self.pre_run,
-            post_run=self.post_run,
-            messages=self.messages,
-            cplex_logs=self.cplex_logs,
+            objective_sequence=(
+                self.objective_sequence["externalId"]
+                if self.objective_sequence and "externalId" in self.objective_sequence
+                else None
+            ),
+            pre_run=self.pre_run["externalId"] if self.pre_run and "externalId" in self.pre_run else None,
+            post_run=self.post_run["externalId"] if self.post_run and "externalId" in self.post_run else None,
+            messages=self.messages["externalId"] if self.messages and "externalId" in self.messages else None,
+            cplex_logs=self.cplex_logs["externalId"] if self.cplex_logs and "externalId" in self.cplex_logs else None,
             alerts=[alert.as_write() if isinstance(alert, DomainModel) else alert for alert in self.alerts or []],
             output_time_series=[
                 output_time_series.as_write() if isinstance(output_time_series, DomainModel) else output_time_series
                 for output_time_series in self.output_time_series or []
             ],
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,15 +95,15 @@
         return value
 
     def as_read(self) -> ShopScenario:
         """Convert this GraphQL format of shop scenario to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopScenario(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -119,15 +119,15 @@
                 for attribute_mappings_override in self.attribute_mappings_override or []
             ],
         )
 
     def as_write(self) -> ShopScenarioWrite:
         """Convert this GraphQL format of shop scenario to the writing format."""
         return ShopScenarioWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             model=self.model.as_write() if isinstance(self.model, DomainModel) else self.model,
             commands=self.commands.as_write() if isinstance(self.commands, DomainModel) else self.commands,
             source=self.source,
             attribute_mappings_override=[
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_scenario_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
         return value
 
     def as_read(self) -> ShopScenarioSet:
         """Convert this GraphQL format of shop scenario set to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopScenarioSet(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -109,15 +109,15 @@
                 for scenario in self.scenarios or []
             ],
         )
 
     def as_write(self) -> ShopScenarioSetWrite:
         """Convert this GraphQL format of shop scenario set to the writing format."""
         return ShopScenarioSetWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             start_specification=self.start_specification,
             end_specification=self.end_specification,
             scenarios=[
                 scenario.as_write() if isinstance(scenario, DomainModel) else scenario
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_time_series.py`

 * *Files 2% similar despite different names*

```diff
@@ -82,15 +82,15 @@
         return values
 
     def as_read(self) -> ShopTimeSeries:
         """Convert this GraphQL format of shop time series to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopTimeSeries(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             object_type=self.object_type,
@@ -98,15 +98,15 @@
             attribute_name=self.attribute_name,
             time_series=self.time_series,
         )
 
     def as_write(self) -> ShopTimeSeriesWrite:
         """Convert this GraphQL format of shop time series to the writing format."""
         return ShopTimeSeriesWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             object_type=self.object_type,
             object_name=self.object_name,
             attribute_name=self.attribute_name,
             time_series=self.time_series,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return value
 
     def as_read(self) -> ShopTriggerInput:
         """Convert this GraphQL format of shop trigger input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopTriggerInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -129,15 +129,15 @@
                 else self.preprocessor_input
             ),
         )
 
     def as_write(self) -> ShopTriggerInputWrite:
         """Convert this GraphQL format of shop trigger input to the writing format."""
         return ShopTriggerInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             cog_shop_tag=self.cog_shop_tag,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_shop_trigger_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return value
 
     def as_read(self) -> ShopTriggerOutput:
         """Convert this GraphQL format of shop trigger output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return ShopTriggerOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -119,15 +119,15 @@
             alerts=[alert.as_read() if isinstance(alert, GraphQLCore) else alert for alert in self.alerts or []],
             shop_result=self.shop_result.as_read() if isinstance(self.shop_result, GraphQLCore) else self.shop_result,
         )
 
     def as_write(self) -> ShopTriggerOutputWrite:
         """Convert this GraphQL format of shop trigger output to the writing format."""
         return ShopTriggerOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
         return value
 
     def as_read(self) -> TaskDispatcherInput:
         """Convert this GraphQL format of task dispatcher input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TaskDispatcherInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -126,15 +126,15 @@
             ),
             bid_date=self.bid_date,
         )
 
     def as_write(self) -> TaskDispatcherInputWrite:
         """Convert this GraphQL format of task dispatcher input to the writing format."""
         return TaskDispatcherInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             bid_configuration=(
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_task_dispatcher_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,15 +100,15 @@
         return value
 
     def as_read(self) -> TaskDispatcherOutput:
         """Convert this GraphQL format of task dispatcher output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TaskDispatcherOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -122,15 +122,15 @@
                 for process_sub_task in self.process_sub_tasks or []
             ],
         )
 
     def as_write(self) -> TaskDispatcherOutputWrite:
         """Convert this GraphQL format of task dispatcher output to the writing format."""
         return TaskDispatcherOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_input.py`

 * *Files 2% similar despite different names*

```diff
@@ -107,15 +107,15 @@
         return value
 
     def as_read(self) -> TotalBidMatrixCalculationInput:
         """Convert this GraphQL format of total bid matrix calculation input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TotalBidMatrixCalculationInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -133,15 +133,15 @@
                 for partial_bid_matrice in self.partial_bid_matrices or []
             ],
         )
 
     def as_write(self) -> TotalBidMatrixCalculationInputWrite:
         """Convert this GraphQL format of total bid matrix calculation input to the writing format."""
         return TotalBidMatrixCalculationInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             bid_configuration=(
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_total_bid_matrix_calculation_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,15 +106,15 @@
         return value
 
     def as_read(self) -> TotalBidMatrixCalculationOutput:
         """Convert this GraphQL format of total bid matrix calculation output to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TotalBidMatrixCalculationOutput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -127,15 +127,15 @@
                 self.bid_document.as_read() if isinstance(self.bid_document, GraphQLCore) else self.bid_document
             ),
         )
 
     def as_write(self) -> TotalBidMatrixCalculationOutputWrite:
         """Convert this GraphQL format of total bid matrix calculation output to the writing format."""
         return TotalBidMatrixCalculationOutputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             input_=self.input_.as_write() if isinstance(self.input_, DomainModel) else self.input_,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_turbine_efficiency_curve.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,30 +73,30 @@
         return values
 
     def as_read(self) -> TurbineEfficiencyCurve:
         """Convert this GraphQL format of turbine efficiency curve to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return TurbineEfficiencyCurve(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             head=self.head,
             flow=self.flow,
             efficiency=self.efficiency,
         )
 
     def as_write(self) -> TurbineEfficiencyCurveWrite:
         """Convert this GraphQL format of turbine efficiency curve to the writing format."""
         return TurbineEfficiencyCurveWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             head=self.head,
             flow=self.flow,
             efficiency=self.efficiency,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_configuration.py`

 * *Files 1% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         return value
 
     def as_read(self) -> WaterValueBasedPartialBidConfiguration:
         """Convert this GraphQL format of water value based partial bid configuration to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return WaterValueBasedPartialBidConfiguration(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -107,15 +107,15 @@
             power_asset=self.power_asset.as_read() if isinstance(self.power_asset, GraphQLCore) else self.power_asset,
             add_steps=self.add_steps,
         )
 
     def as_write(self) -> WaterValueBasedPartialBidConfigurationWrite:
         """Convert this GraphQL format of water value based partial bid configuration to the writing format."""
         return WaterValueBasedPartialBidConfigurationWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             method=self.method,
             power_asset=self.power_asset.as_write() if isinstance(self.power_asset, DomainModel) else self.power_asset,
             add_steps=self.add_steps,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_water_value_based_partial_bid_matrix_calculation_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,15 +118,15 @@
         return value
 
     def as_read(self) -> WaterValueBasedPartialBidMatrixCalculationInput:
         """Convert this GraphQL format of water value based partial bid matrix calculation input to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return WaterValueBasedPartialBidMatrixCalculationInput(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             workflow_execution_id=self.workflow_execution_id,
@@ -145,15 +145,15 @@
                 else self.partial_bid_configuration
             ),
         )
 
     def as_write(self) -> WaterValueBasedPartialBidMatrixCalculationInputWrite:
         """Convert this GraphQL format of water value based partial bid matrix calculation input to the writing format."""
         return WaterValueBasedPartialBidMatrixCalculationInputWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             workflow_execution_id=self.workflow_execution_id,
             workflow_step=self.workflow_step,
             function_name=self.function_name,
             function_call_id=self.function_call_id,
             bid_date=self.bid_date,
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_generated/v1/data_classes/_watercourse.py`

 * *Files 2% similar despite different names*

```diff
@@ -81,15 +81,15 @@
         return values
 
     def as_read(self) -> Watercourse:
         """Convert this GraphQL format of watercourse to the reading format."""
         if self.data_record is None:
             raise ValueError("This object cannot be converted to a read format because it lacks a data record.")
         return Watercourse(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecord(
                 version=0,
                 last_updated_time=self.data_record.last_updated_time,
                 created_time=self.data_record.created_time,
             ),
             name=self.name,
@@ -97,15 +97,15 @@
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
 
     def as_write(self) -> WatercourseWrite:
         """Convert this GraphQL format of watercourse to the writing format."""
         return WatercourseWrite(
-            space=self.space,
+            space=self.space or DEFAULT_INSTANCE_SPACE,
             external_id=self.external_id,
             data_record=DataRecordWrite(existing_version=0),
             name=self.name,
             display_name=self.display_name,
             ordering=self.ordering,
             asset_type=self.asset_type,
         )
```

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/_logger.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/_logger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/data_set_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/data_set_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/powerops_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/powerops_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/_api_client.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/_api_client.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/dayahead_trigger_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/dayahead_trigger_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_result_files_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_result_files_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_results_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_results_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/api/shop_run_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/api/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/dayahead_trigger.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/dayahead_trigger.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/helpers.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/helpers.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/plotting.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/plotting.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_result_files.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_result_files.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_results.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_results_compare.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_results_compare.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/data_classes/shop_run_event.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/data_classes/shop_run_event.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_case.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_case.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_file_reference.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_file_reference.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_api.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run_api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/shop_run_filter.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/shop_run_filter.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/client/shop/utils.py` & `cognite_power_ops-0.94.2/cognite/powerops/client/shop/utils.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/cognite_modules/_system.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/cognite_modules/_system.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/config.dev.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/config.dev.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/AFRRBid-BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/asset-EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Asset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Generator.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Plant.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-PriceArea.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/base-Watercourse.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-BidMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-MultiScenarioMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/containers/dayAheadBids-SHOPMultiScenario.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/AFRRBid-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-GeneratorEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Reservoir.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-TurbineEfficiency.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/asset-Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/baseBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BasicBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-BidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-CustomBidMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-MultiScenarioMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPMultiScenarioMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-SHOPPriceScenarioResult.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v0/data_models/views/dayAheadBids-WaterValueBasedMethod.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/all_DayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/all_PowerOps.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_DayAheadBenchmarking.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_SHOPBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_TotalBidMatrixCalculation.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/compute_WaterValueBasedDayAhead.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/config_DayAheadConfiguration.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/config_Resync.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Alert.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidDocument.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidMatrix.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/BidRow.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/EfficiencyCurve.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/FunctionData.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/Generator.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/MarketConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PartialBidConfiguration.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PlantWaterValueBased.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PowerAsset.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaAFRR.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceAreaDayAhead.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/PriceProduction.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPResult.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/SHOPTimeSeries.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopAttributeMapping.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopCase.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopFile.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopModel.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenario.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/containers/ShopScenarioSet.container.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_AFRRBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_Asset.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/frontend_DayAheadBid.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/node_types/power-ops-types.powerops_nodes.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/product_CogShop.datamodel.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/BidRow.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/MarketConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/1-interface.Alert.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/alerts/ShopPenaltyReport.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/1-interface.PowerAsset.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/Generator.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/GeneratorEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/generator/TurbineEfficiencyCurve.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/1-interface.Plant.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/plant/PlantWaterValueBased.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/1-interface.PriceArea.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/price_area/PriceAreaInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/assets/watercourse/1-interface.Watercourse.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/1-interface.PartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/BidConfigurationDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/ShopBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_configuration/WaterValueBasedPartialBidConfiguration.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/1-interface.BidDocument.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentAFRR.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAhead.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_document/BidDocumentDayAheadSimple.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrix.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.BidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/1-interface.PartialBidMatrixInformation.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/bid_matrix/PartialBidMatrixInformationWithScenarios.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopAttributeMapping.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCase.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopCommands.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopFile.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopModel.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenario.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/cogshop/ShopScenarioSet.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.FunctionInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/1-interface.PartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/BenchmarkingCollectorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopPreprocessorInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/ShopTriggerInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherBenchmarkingInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TaskDispatcherInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/TotalBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_inputs/WaterPartialBidMatrixCalculationInput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/1-interface.FunctionOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/BenchmarkingCollectorOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/PartialBidMatrixCalculationOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/SHOPTriggerOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/ShopPreprocessorOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherBenchmarkingOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TaskDispatcherOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/function_outputs/TotalBidMatrixCalculationOutput.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/PriceProduction.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPResult.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/SHOPTimeSeries.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml` & `cognite_power_ops-0.94.2/cognite/powerops/custom_modules/power_model_v1/data_models/views/shop_result/ShopObjectiveValue.view.yaml`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/prerun_transformations/transformations.py` & `cognite_power_ops-0.94.2/cognite/powerops/prerun_transformations/transformations.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_main.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/_main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_settings.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/_shared.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/_shared.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/cogshop/shop_file_config.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/cogshop/shop_file_config.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/_core.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/_core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/benchmarking.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/benchmarking.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/dayahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/market.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/market.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/market/rkom.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/connections.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/connections.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/generator.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/generator.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/plant.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/plant.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/config/production/watercourse.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/config/production/watercourse.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/core/cdf.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/core/cdf.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/core/main.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/core/main.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/core/transform.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/core/transform.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/core/validation.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/core/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/diff/core.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/diff/core.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/diff/data_classes.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/diff/data_classes.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/_to_instances.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/market_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/_shared_v1_v2/production_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/_shared_v1_v2/production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/asset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/asset_type.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/asset_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/cdf_resources.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/cdf_resources.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/data_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/data_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/dms_models.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/dms_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/graph_ql.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/graph_ql.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/base/resource_type.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/base/resource_type.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/cogshop.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/cogshop.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_cogshop_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_market_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/config_to_model/to_production_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/graphql_schemas/cogshop1.graphql`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/__init__.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/__init__.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/base.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/base.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/benchmark.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/benchmark.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/dayahead.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/dayahead.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/market/rkom.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/market/rkom.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v1/production.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v1/production.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/config_to_model/to_powerasset_model.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/powerops_models.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/powerops_models.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/models/v2/production_dm.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/models/v2/production_dm.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/time_series_mapping/mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/time_series_mapping/static_mapping.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/time_series_mapping/static_mapping.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/v2/shop_to_assets.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/v2/shop_to_assets.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/resync/validation.py` & `cognite_power_ops-0.94.2/cognite/powerops/resync/validation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_cdf_auth.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/_cdf_auth.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/_settings.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/_settings.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/calls.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/calls.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/extraction_pipelines.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/extraction_pipelines.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/cdf/resource_creation.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/cdf/resource_creation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/lookup.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/lookup.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/navigation.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/navigation.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/require.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/require.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/retry/api.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/retry/api.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/serialization.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/serialization.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/cognite/powerops/utils/time.py` & `cognite_power_ops-0.94.2/cognite/powerops/utils/time.py`

 * *Files identical despite different names*

### Comparing `cognite_power_ops-0.94.1/pyproject.toml` & `cognite_power_ops-0.94.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cognite-power-ops"
-version = "0.94.1"
+version = "0.94.2"
 description = "SDK for power markets operations on Cognite Data Fusion"
 readme = "README.md"
 authors = ["Cognite <support@cognite.com>"]
 license = "Apache 2.0"
 documentation = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 homepage = "https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/"
 repository = "https://github.com/cognitedata/power-ops-sdk"
@@ -49,63 +49,62 @@
 allow_redefinition = true
 
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 typer = {version="^0.9.0", extras=["rich"]}
 PyYAML = "^6.0"
-cognite-sdk = {version = ">=7.13.8", extras = ["pandas"]}
+cognite-sdk = {version = ">=7.37", extras = ["pandas"]}
 pydantic = "^2.0"
 pydantic-settings = "^2.0"
-cachelib = "^0.10.2"
 loguru = "^0.7.0"
 deepdiff = "^6.3.0"
 matplotlib = "^3.7.1"
 dacite = "^1.8.1"
 python-dotenv = "^1.0.0"
 arrow = "^1.2.0"
 typing_extensions = ">= 4"
 tomli = {version = "^2.0.1", python = "<3.11"}
 StrEnum = {version = "^0.4.15", python = "<3.11"}
 tomli-w = "^1.0.0"
 tabulate = "^0.9"
-cognite-toolkit = {version="0.1.1"}
-cognite-pygen = {version = ">=0.99.19", extras = ["all"]}
-
+cognite-pygen = "^0.99.22"
 mkdocs =  {version="*", optional=true}
 mkdocs-jupyter = {version="*", optional=true}
 mkdocs-material = {version="*", optional=true}
 mkdocs-material-extensions = {version="*", optional=true}
 mkdocs-git-revision-date-localized-plugin = {version="*", optional=true}
 mkdocs-git-authors-plugin = {version="*", optional=true}
 mkdocs-gitbook = {version="*", optional=true}
 mkdocs-glightbox = {version="*", optional=true}
 pymdown-extensions = {version="*", optional=true}
 mkdocstrings = {version="*", optional=true, extras=["python"]}
+cachelib = "^0.13.0"
+cognite-toolkit = "^0.1.2"
 
 [tool.poetry.extras]
 docs = ["mkdocs", "mkdocs-jupyter", "mkdocs-material", "mkdocs-material-extensions", "mkdocs-git-revision-date-localized-plugin",
     "mkdocs-git-authors-plugin", "mkdocs-gitbook", "mkdocs-glightbox", "pymdown-extensions", "mkdocstrings"]
 
 [tool.poetry.scripts]
 powerops = "cognite.powerops.cli:main"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.2.2"
 profilehooks = "^1.12.0"
-pytest = "^7.3.1"
-pytest-cov = "^4.0.0"
 pytest-mock = "^3.10.0"
 pytest-regressions = "^2.4.2"
 ipykernel="6.24.0"
-twine = "^4.0.2"
 jupyter = "^1.0.0"
 mypy = "^1.4"
 pandas-stubs = "^2"
 types-PyYAML = "^6"
+pytest = "^8.1.1"
+pytest-cov = "^5.0.0"
+twine = "^5.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.pytest.ini_options]
 addopts = "--doctest-modules --ignore=customers/ --ignore=examples/ --ignore=playground/ --ignore=cognite/powerops/client"
```

### Comparing `cognite_power_ops-0.94.1/PKG-INFO` & `cognite_power_ops-0.94.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognite-power-ops
-Version: 0.94.1
+Version: 0.94.2
 Summary: SDK for power markets operations on Cognite Data Fusion
 Home-page: https://cognite-power-ops-sdk.readthedocs-hosted.com/en/latest/
 License: Apache 2.0
 Author: Cognite
 Author-email: support@cognite.com
 Requires-Python: >=3.9,<3.13
 Classifier: License :: Other/Proprietary License
@@ -13,18 +13,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: docs
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: StrEnum (>=0.4.15,<0.5.0) ; python_version < "3.11"
 Requires-Dist: arrow (>=1.2.0,<2.0.0)
-Requires-Dist: cachelib (>=0.10.2,<0.11.0)
-Requires-Dist: cognite-pygen[all] (>=0.99.19)
-Requires-Dist: cognite-sdk[pandas] (>=7.13.8)
-Requires-Dist: cognite-toolkit (==0.1.1)
+Requires-Dist: cachelib (>=0.13.0,<0.14.0)
+Requires-Dist: cognite-pygen (>=0.99.22,<0.100.0)
+Requires-Dist: cognite-sdk[pandas] (>=7.37)
+Requires-Dist: cognite-toolkit (>=0.1.2,<0.2.0)
 Requires-Dist: dacite (>=1.8.1,<2.0.0)
 Requires-Dist: deepdiff (>=6.3.0,<7.0.0)
 Requires-Dist: loguru (>=0.7.0,<0.8.0)
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: mkdocs ; extra == "docs"
 Requires-Dist: mkdocs-git-authors-plugin ; extra == "docs"
 Requires-Dist: mkdocs-git-revision-date-localized-plugin ; extra == "docs"
```

