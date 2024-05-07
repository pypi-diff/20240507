# Comparing `tmp/geojson_modelica_translator-0.6.0rc2.tar.gz` & `tmp/geojson_modelica_translator-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geojson_modelica_translator-0.6.0rc2.tar", max compression
+gzip compressed data, was "geojson_modelica_translator-0.7.0.tar", max compression
```

## Comparing `geojson_modelica_translator-0.6.0rc2.tar` & `geojson_modelica_translator-0.7.0.tar`

### file list

```diff
@@ -1,213 +1,216 @@
--rw-r--r--   0        0        0     5237 2023-09-28 18:56:21.265561 geojson_modelica_translator-0.6.0rc2/LICENSE.md
--rw-r--r--   0        0        0     5910 2023-08-18 13:32:58.502457 geojson_modelica_translator-0.6.0rc2/README.rst
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.602417 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/__init__.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.608869 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/__init__.py
--rw-r--r--   0        0        0    21238 2022-04-27 21:48:45.736618 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/building_properties.json
--rw-r--r--   0        0        0     4477 2022-04-18 22:19:44.856964 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json
--rw-r--r--   0        0        0     5820 2022-04-18 22:19:44.857230 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json
--rw-r--r--   0        0        0     1679 2021-03-23 22:50:43.555533 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json
--rw-r--r--   0        0        0     2326 2021-03-22 17:09:40.711956 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/region_properties.json
--rw-r--r--   0        0        0     2510 2022-04-18 22:19:44.857555 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/site_properties.json
--rw-r--r--   0        0        0     2869 2021-03-23 22:50:43.555931 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json
--rw-r--r--   0        0        0     2236 2021-03-23 22:50:43.556356 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json
--rw-r--r--   0        0        0     1681 2023-06-09 02:59:16.642371 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/schemas.py
--rw-r--r--   0        0        0     3280 2023-09-14 01:43:00.225469 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/urbanopt_geojson.py
--rw-r--r--   0        0        0     7173 2023-08-08 20:28:37.106641 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson_modelica_translator.py
--rw-r--r--   0        0        0      287 2023-09-29 00:46:31.962334 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/jinja_filters.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.596404 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/__init__.py
--rw-r--r--   0        0        0       65 2023-06-09 02:59:16.642933 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      347 2023-08-08 20:28:37.107050 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ConnectStatements.mopt
--rw-r--r--   0        0        0       59 2023-08-08 20:28:37.107771 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_Borefield/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      349 2023-08-08 20:28:37.108018 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_Borefield/ConnectStatements.mopt
--rw-r--r--   0        0        0     1365 2023-08-08 20:28:37.108616 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      445 2023-08-08 20:28:37.108818 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ConnectStatements.mopt
--rw-r--r--   0        0        0     1913 2023-06-09 02:59:16.643531 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1294 2023-06-09 02:59:16.643843 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1262 2023-08-08 20:28:37.109084 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1426 2023-08-08 20:28:37.109256 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ConnectStatements.mopt
--rw-r--r--   0        0        0      273 2023-03-13 19:30:06.541737 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/__init__.py
--rw-r--r--   0        0        0     7109 2023-03-13 19:30:06.542467 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/coupling.py
--rw-r--r--   0        0        0    21075 2023-03-13 19:30:06.543266 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/diagram.py
--rw-r--r--   0        0        0     5112 2023-03-13 19:30:06.543845 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/graph.py
--rw-r--r--   0        0        0       70 2021-03-14 00:14:54.963794 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      470 2021-03-14 00:14:54.964070 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ConnectStatements.mopt
--rw-r--r--   0        0        0      388 2021-03-14 00:14:54.964356 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      460 2021-03-14 00:14:54.964580 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0       70 2021-03-14 00:14:54.965478 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      472 2021-03-14 00:14:54.965633 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ConnectStatements.mopt
--rw-r--r--   0        0        0      488 2021-03-14 00:14:54.965822 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      457 2021-03-14 00:14:54.965961 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0       46 2021-03-14 00:14:54.966128 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      946 2021-03-14 00:14:54.966237 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0      914 2022-11-07 13:45:19.274215 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      759 2021-03-14 00:14:54.966508 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0      439 2022-07-18 20:07:47.614321 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1183 2022-07-18 20:07:47.614452 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0     1003 2022-11-07 13:45:19.274477 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt
--rw-r--r--   0        0        0     1133 2022-07-18 20:07:47.614785 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt
--rw-r--r--   0        0        0     1353 2022-07-18 20:07:47.615510 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      636 2022-04-27 21:48:45.742594 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:53:19.413863 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      541 2021-03-14 00:14:54.966779 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-03-14 00:14:54.966937 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      540 2021-03-14 00:14:54.967052 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1440 2022-07-18 20:07:47.615776 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      633 2022-04-27 21:48:45.743210 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     1360 2022-07-18 20:07:47.615997 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      639 2022-04-27 21:48:45.743822 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:53:20.732123 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      544 2021-03-14 00:14:54.967320 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      265 2021-05-06 14:52:26.050913 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      543 2021-03-14 00:14:54.967575 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1443 2022-07-18 20:07:47.616197 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      635 2022-04-27 21:48:45.744794 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      562 2022-07-18 20:07:47.616508 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      542 2023-06-09 02:59:16.644146 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      610 2022-07-18 20:07:47.616719 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      529 2023-06-09 02:59:16.644529 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     1310 2022-11-07 13:45:16.520801 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      682 2021-03-14 00:14:54.968406 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0      246 2022-11-07 13:45:16.521273 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      541 2022-11-07 14:12:33.906104 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0      292 2022-11-07 13:45:16.521689 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      540 2021-03-14 00:14:54.968920 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt
--rw-r--r--   0        0        0     1453 2022-11-07 13:45:16.522323 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt
--rw-r--r--   0        0        0      682 2022-11-07 14:12:33.906568 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt
--rw-r--r--   0        0        0     3618 2023-03-13 19:30:06.544501 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/utils.py
--rw-r--r--   0        0        0      226 2023-03-13 19:30:06.545033 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/__init__.py
--rw-r--r--   0        0        0     7191 2023-10-09 16:28:49.936782 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/district.py
--rw-r--r--   0        0        0     1925 2023-06-09 02:59:16.645829 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot
--rw-r--r--   0        0        0     2212 2023-06-09 02:59:16.646190 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot
--rw-r--r--   0        0        0      427 2023-03-13 19:30:06.547411 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/__init__.py
--rw-r--r--   0        0        0     2957 2023-10-09 16:28:49.937460 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py
--rw-r--r--   0        0        0      698 2023-03-13 19:30:06.548545 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py
--rw-r--r--   0        0        0     1098 2023-03-13 19:30:06.549448 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py
--rw-r--r--   0        0        0     1142 2023-03-13 19:30:06.550615 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py
--rw-r--r--   0        0        0     2957 2023-10-09 16:28:49.938018 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py
--rw-r--r--   0        0        0    16351 2023-10-22 16:24:31.650100 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot
--rw-r--r--   0        0        0      738 2023-06-09 02:59:16.647026 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt
--rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973843 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt
--rw-r--r--   0        0        0      554 2021-03-14 00:14:54.973955 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt
--rw-r--r--   0        0        0    15722 2023-10-22 16:24:31.604318 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot
--rw-r--r--   0        0        0      700 2023-06-09 02:59:16.647707 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt
--rw-r--r--   0        0        0      381 2023-03-13 19:30:06.551862 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/__init__.py
--rw-r--r--   0        0        0    10507 2023-06-09 02:59:16.648674 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/load_base.py
--rw-r--r--   0        0        0    11696 2023-10-09 16:28:49.938729 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/spawn.py
--rw-r--r--   0        0        0    30335 2023-10-09 16:28:49.939452 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/teaser.py
--rw-r--r--   0        0        0     3283 2021-03-14 00:14:54.976624 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most
--rw-r--r--   0        0        0     1606 2021-03-14 00:14:54.977435 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most
--rw-r--r--   0        0        0    12856 2023-10-22 16:24:32.485273 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot
--rw-r--r--   0        0        0     5179 2023-10-22 16:24:32.324024 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot
--rw-r--r--   0        0        0      777 2023-06-09 02:59:16.650701 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt
--rw-r--r--   0        0        0     8397 2023-10-22 16:24:32.561459 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot
--rw-r--r--   0        0        0     4925 2023-10-22 16:24:32.442439 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot
--rw-r--r--   0        0        0      257 2021-03-14 00:14:54.978638 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/Teaser_Instance.mopt
--rw-r--r--   0        0        0    17163 2023-10-22 16:24:32.365521 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot
--rw-r--r--   0        0        0     5864 2023-10-22 16:24:32.415444 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot
--rw-r--r--   0        0        0      116 2021-03-14 00:14:54.979175 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMFT_Instance.mopt
--rw-r--r--   0        0        0     9486 2023-10-22 16:24:32.528633 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot
--rw-r--r--   0        0        0      884 2023-08-08 20:28:37.112310 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt
--rw-r--r--   0        0        0     3233 2023-10-22 16:24:32.386217 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot
--rw-r--r--   0        0        0     9547 2023-10-09 16:28:49.940016 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/time_series.py
--rw-r--r--   0        0        0     7122 2023-10-09 16:28:49.940235 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py
--rw-r--r--   0        0        0     7838 2023-08-17 19:16:33.800717 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/model_base.py
--rw-r--r--   0        0        0      390 2023-06-09 02:59:16.655120 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/__init__.py
--rw-r--r--   0        0        0      893 2023-03-13 19:30:06.553864 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py
--rw-r--r--   0        0        0      878 2023-03-13 19:30:06.554241 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py
--rw-r--r--   0        0        0      532 2023-03-13 19:30:06.555175 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_base.py
--rw-r--r--   0        0        0      878 2023-03-13 19:30:06.555907 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py
--rw-r--r--   0        0        0      878 2023-08-08 20:28:37.113787 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_distribution_pump.py
--rw-r--r--   0        0        0      875 2023-03-13 19:30:06.556381 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py
--rw-r--r--   0        0        0     1917 2023-06-09 02:59:16.655491 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt
--rw-r--r--   0        0        0     1264 2023-09-24 14:14:55.788526 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt
--rw-r--r--   0        0        0      729 2022-11-07 14:12:33.910744 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt
--rw-r--r--   0        0        0     1574 2023-08-08 20:28:37.113986 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkDistributionPump_Instance.mopt
--rw-r--r--   0        0        0      935 2022-11-07 14:12:33.911009 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt
--rw-r--r--   0        0        0      294 2023-03-13 19:30:06.556779 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/__init__.py
--rw-r--r--   0        0        0    10939 2023-10-09 16:28:49.940689 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/borefield.py
--rw-r--r--   0        0        0     5317 2023-10-09 16:28:49.941142 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/chp.py
--rw-r--r--   0        0        0     7433 2023-10-09 16:28:49.941573 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/cooling_plant.py
--rw-r--r--   0        0        0      524 2023-03-13 19:30:06.558122 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/plant_base.py
--rw-r--r--   0        0        0     8784 2023-10-22 16:24:32.288036 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo
--rw-r--r--   0        0        0     4815 2023-10-22 16:24:32.117808 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo
--rw-r--r--   0        0        0    16166 2023-10-22 16:24:31.699080 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot
--rw-r--r--   0        0        0    16166 2023-10-22 16:24:32.002789 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BorefieldTwoUTubes.mot
--rw-r--r--   0        0        0      133 2023-06-09 02:59:16.658004 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/Borefield_Instance.mopt
--rw-r--r--   0        0        0    20277 2023-10-22 16:24:32.084024 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot
--rw-r--r--   0        0        0    13292 2023-10-22 16:24:31.890267 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo
--rw-r--r--   0        0        0     4455 2023-10-22 16:24:31.843022 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo
--rw-r--r--   0        0        0     6161 2023-10-22 16:24:31.928131 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo
--rw-r--r--   0        0        0     3189 2023-06-09 02:59:16.659311 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt
--rw-r--r--   0        0        0    10560 2023-10-22 16:24:31.774175 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo
--rw-r--r--   0        0        0    14157 2023-10-22 16:24:32.192885 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo
--rw-r--r--   0        0        0    16335 2023-10-22 16:24:31.810165 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/GroundTemperatureResponse.mo
--rw-r--r--   0        0        0    15906 2023-10-22 16:24:32.248258 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot
--rw-r--r--   0        0        0     2060 2022-07-18 20:07:47.633512 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt
--rw-r--r--   0        0        0     6798 2023-10-22 16:24:31.732731 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo
--rw-r--r--   0        0        0     2874 2023-10-22 16:24:32.026431 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo
--rw-r--r--   0        0        0      899 2023-10-22 16:24:32.144517 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo
--rw-r--r--   0        0        0     4245 2023-10-22 16:24:31.953817 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo
--rw-r--r--   0        0        0     1377 2023-06-09 02:59:16.661511 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo
--rw-r--r--   0        0        0     1898 2022-07-18 20:07:47.634583 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos
--rw-r--r--   0        0        0     1600 2023-06-09 02:59:16.661760 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot
--rw-r--r--   0        0        0     1562 2023-09-28 17:43:53.363756 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/BoilerPolynomial.mot
--rw-r--r--   0        0        0     1060 2023-09-28 17:43:53.363933 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/boiler_polynomial.py
--rw-r--r--   0        0        0    15069 2023-09-14 01:43:00.226194 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_partial.mot
--rw-r--r--   0        0        0     4416 2023-09-14 01:43:00.226815 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.mot
--rw-r--r--   0        0        0     5358 2023-10-09 16:28:49.941841 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.py
--rw-r--r--   0        0        0     1505 2023-09-24 14:14:55.788751 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.mot
--rw-r--r--   0        0        0     1205 2023-09-24 14:14:55.788936 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.634988 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACDCConverter.py
--rw-r--r--   0        0        0     2125 2023-09-24 14:14:55.789182 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot
--rw-r--r--   0        0        0     1911 2023-03-13 19:30:06.558713 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py
--rw-r--r--   0        0        0     1263 2023-09-24 14:14:55.789786 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Capacitive.mot
--rw-r--r--   0        0        0     1092 2023-06-09 02:59:16.666056 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.mot
--rw-r--r--   0        0        0     1329 2023-08-08 20:28:37.117064 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py
--rw-r--r--   0        0        0     1334 2023-09-24 14:14:55.790277 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitive.py
--rw-r--r--   0        0        0     1202 2023-06-09 02:59:16.666574 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Generator.mot
--rw-r--r--   0        0        0     1088 2023-06-09 02:59:16.666860 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Grid.mot
--rw-r--r--   0        0        0     1228 2023-06-09 02:59:16.667220 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot
--rw-r--r--   0        0        0     1333 2023-06-09 02:59:16.667461 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot
--rw-r--r--   0        0        0     1156 2022-07-18 20:07:47.636337 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py
--rw-r--r--   0        0        0     1680 2023-08-08 20:28:37.117451 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py
--rw-r--r--   0        0        0      958 2023-06-09 02:59:16.667963 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/grid.py
--rw-r--r--   0        0        0     1788 2022-11-07 14:12:33.911571 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py
--rw-r--r--   0        0        0     1040 2023-06-09 02:59:16.668147 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/AcBattery.mot
--rw-r--r--   0        0        0     1179 2023-06-09 02:59:16.668362 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py
--rw-r--r--   0        0        0      935 2023-09-24 14:14:55.790470 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/capacitor.py
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.636990 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/DC/Loads/Conductor.py
--rw-r--r--   0        0        0     5907 2023-09-24 14:14:55.790685 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/PVsubsystem.mot
--rw-r--r--   0        0        0     3754 2022-07-18 20:07:47.637256 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot
--rw-r--r--   0        0        0      581 2023-09-24 14:14:55.790820 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/pv_subsystem.py
--rw-r--r--   0        0        0        0 2023-04-21 14:45:45.425849 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/__init__.py
--rw-r--r--   0        0        0     8103 2023-03-13 19:30:06.559223 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/csv_modelica.py
--rw-r--r--   0        0        0    12475 2023-10-09 16:28:49.943301 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/input_parser.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.607601 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/__init__.py
--rw-r--r--   0        0        0      708 2023-08-08 20:28:37.118456 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/Dockerfile
--rw-r--r--   0        0        0      996 2023-06-09 02:59:16.669756 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/README.md
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.613657 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/__init__.py
--rw-r--r--   0        0        0      203 2023-06-09 02:59:16.669975 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/compile_fmu.most
--rw-r--r--   0        0        0     6628 2023-08-08 20:28:37.118981 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/om.py
--rwxr-xr-x   0        0        0     3852 2023-08-08 20:28:37.119289 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/om_docker.sh
--rw-r--r--   0        0        0      642 2023-08-08 20:28:37.119578 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/simulate.most
--rw-r--r--   0        0        0      959 2020-09-30 19:56:12.680802 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot
--rw-r--r--   0        0        0     3060 2022-07-18 20:07:47.638320 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot
--rw-r--r--   0        0        0    20648 2023-08-18 13:32:58.504312 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/modelica_runner.py
--rw-r--r--   0        0        0     3944 2023-10-09 16:28:49.943705 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/simple_gmt_base.py
--rw-r--r--   0        0        0     3802 2023-06-09 02:59:16.672705 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/scaffold.py
--rwxr-xr-x   0        0        0    52346 2023-09-28 17:43:53.365491 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/schema.json
--rw-r--r--   0        0        0    40588 2023-09-24 14:14:55.792537 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/system_parameters.py
--rw-r--r--   0        0        0     3164 2023-09-28 17:43:53.366654 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json
--rw-r--r--   0        0        0     4440 2023-09-28 17:43:53.368601 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/time_series_template.json
--rw-r--r--   0        0        0     4924 2023-10-09 16:28:49.945822 geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/utils.py
--rw-r--r--   0        0        0        0 2020-06-18 17:43:32.593171 geojson_modelica_translator-0.6.0rc2/management/__init__.py
--rw-r--r--   0        0        0     9963 2023-03-13 19:30:06.565467 geojson_modelica_translator-0.6.0rc2/management/check_sys_params.py
--rw-r--r--   0        0        0     2634 2022-07-18 20:07:47.641868 geojson_modelica_translator-0.6.0rc2/management/data/baseline_geojson.json
--rw-r--r--   0        0        0     4429 2023-09-28 17:43:53.368918 geojson_modelica_translator-0.6.0rc2/management/data/baseline_sys_params.json
--rw-r--r--   0        0        0        0 2022-07-18 20:07:47.642053 geojson_modelica_translator-0.6.0rc2/management/data/baseline_time_series.mos
--rw-r--r--   0        0        0  1148813 2022-07-18 20:07:47.647980 geojson_modelica_translator-0.6.0rc2/management/data/baseline_weather.mos
--rw-r--r--   0        0        0     6648 2023-03-13 19:30:06.566021 geojson_modelica_translator-0.6.0rc2/management/format_modelica_files.py
--rw-r--r--   0        0        0     7952 2023-08-08 20:28:37.123485 geojson_modelica_translator-0.6.0rc2/management/uo_des.py
--rw-r--r--   0        0        0     1280 2023-03-13 19:30:06.567076 geojson_modelica_translator-0.6.0rc2/management/update_schemas.py
--rw-r--r--   0        0        0     3062 2023-10-22 16:23:01.952742 geojson_modelica_translator-0.6.0rc2/pyproject.toml
--rw-r--r--   0        0        0     7319 1970-01-01 00:00:00.000000 geojson_modelica_translator-0.6.0rc2/PKG-INFO
+-rw-r--r--   0        0        0      825 2024-05-07 15:30:38.265318 geojson_modelica_translator-0.7.0/AUTHORS.md
+-rw-r--r--   0        0        0     5237 2024-05-07 15:30:38.265318 geojson_modelica_translator-0.7.0/LICENSE.md
+-rw-r--r--   0        0        0     6213 2024-05-07 15:30:38.265318 geojson_modelica_translator-0.7.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/__init__.py
+-rw-r--r--   0        0        0    21238 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/building_properties.json
+-rw-r--r--   0        0        0     4477 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json
+-rw-r--r--   0        0        0     5820 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json
+-rw-r--r--   0        0        0     1679 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json
+-rw-r--r--   0        0        0     2326 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/region_properties.json
+-rw-r--r--   0        0        0     2510 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/site_properties.json
+-rw-r--r--   0        0        0     2869 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json
+-rw-r--r--   0        0        0     2236 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json
+-rw-r--r--   0        0        0     1610 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/schemas.py
+-rw-r--r--   0        0        0     3303 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/urbanopt_geojson.py
+-rw-r--r--   0        0        0     6892 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson_modelica_translator.py
+-rw-r--r--   0        0        0      282 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/jinja_filters.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/__init__.py
+-rw-r--r--   0        0        0       65 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      347 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkAmbientWaterStub_Borefield/ConnectStatements.mopt
+-rw-r--r--   0        0        0       59 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_Borefield/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      344 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_Borefield/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1338 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1200 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1913 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1130 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1237 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1426 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ConnectStatements.mopt
+-rw-r--r--   0        0        0      273 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/__init__.py
+-rw-r--r--   0        0        0     7073 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/coupling.py
+-rw-r--r--   0        0        0    20814 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/diagram.py
+-rw-r--r--   0        0        0     5090 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/graph.py
+-rw-r--r--   0        0        0       70 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      470 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_Network2Pipe/ConnectStatements.mopt
+-rw-r--r--   0        0        0      388 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      460 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/CoolingIndirect_NetworkChilledWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0       70 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      472 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_Network2Pipe/ConnectStatements.mopt
+-rw-r--r--   0        0        0      488 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      457 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/HeatingIndirect_NetworkHeatedWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0       46 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      946 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0      914 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      759 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0      439 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1183 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1003 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0     1133 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1353 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      636 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      541 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      540 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1440 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      633 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1360 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      639 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      544 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      265 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      543 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1443 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      635 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      562 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      542 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      610 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      529 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1310 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      682 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0      246 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      541 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0      292 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      540 2024-05-07 15:30:38.277318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt
+-rw-r--r--   0        0        0     1453 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt
+-rw-r--r--   0        0        0      682 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt
+-rw-r--r--   0        0        0     3648 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/utils.py
+-rw-r--r--   0        0        0      226 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/__init__.py
+-rw-r--r--   0        0        0     9136 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/district.py
+-rw-r--r--   0        0        0     1925 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot
+-rw-r--r--   0        0        0     2212 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot
+-rw-r--r--   0        0        0      427 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/__init__.py
+-rw-r--r--   0        0        0     2911 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py
+-rw-r--r--   0        0        0      689 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py
+-rw-r--r--   0        0        0     1081 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py
+-rw-r--r--   0        0        0     1125 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py
+-rw-r--r--   0        0        0     2911 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py
+-rw-r--r--   0        0        0    16351 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot
+-rw-r--r--   0        0        0      738 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt
+-rw-r--r--   0        0        0      554 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      554 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt
+-rw-r--r--   0        0        0    15722 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot
+-rw-r--r--   0        0        0      700 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt
+-rw-r--r--   0        0        0      381 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/__init__.py
+-rw-r--r--   0        0        0    10416 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/load_base.py
+-rw-r--r--   0        0        0    11896 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/spawn.py
+-rw-r--r--   0        0        0    30674 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/teaser.py
+-rw-r--r--   0        0        0     3263 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most
+-rw-r--r--   0        0        0     1586 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most
+-rw-r--r--   0        0        0    12836 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot
+-rw-r--r--   0        0        0     5179 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot
+-rw-r--r--   0        0        0      777 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt
+-rw-r--r--   0        0        0     8382 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot
+-rw-r--r--   0        0        0     4925 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot
+-rw-r--r--   0        0        0      257 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Teaser_Instance.mopt
+-rw-r--r--   0        0        0    17082 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot
+-rw-r--r--   0        0        0     5740 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot
+-rw-r--r--   0        0        0      116 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMFT_Instance.mopt
+-rw-r--r--   0        0        0     9486 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot
+-rw-r--r--   0        0        0      910 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt
+-rw-r--r--   0        0        0     3233 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot
+-rw-r--r--   0        0        0     9811 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/time_series.py
+-rw-r--r--   0        0        0     7219 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py
+-rw-r--r--   0        0        0     7187 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/model_base.py
+-rw-r--r--   0        0        0      390 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/__init__.py
+-rw-r--r--   0        0        0      927 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py
+-rw-r--r--   0        0        0     1082 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py
+-rw-r--r--   0        0        0      523 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_base.py
+-rw-r--r--   0        0        0      922 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py
+-rw-r--r--   0        0        0      923 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_distribution_pump.py
+-rw-r--r--   0        0        0      919 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py
+-rw-r--r--   0        0        0     1917 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt
+-rw-r--r--   0        0        0     1235 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      729 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt
+-rw-r--r--   0        0        0     2650 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkDistributionPump_Instance.mopt
+-rw-r--r--   0        0        0      935 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt
+-rw-r--r--   0        0        0      294 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/__init__.py
+-rw-r--r--   0        0        0    11486 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/borefield.py
+-rw-r--r--   0        0        0     5547 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/chp.py
+-rw-r--r--   0        0        0     7274 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/cooling_plant.py
+-rw-r--r--   0        0        0      515 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/plant_base.py
+-rw-r--r--   0        0        0     8784 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo
+-rw-r--r--   0        0        0     4815 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo
+-rw-r--r--   0        0        0     4926 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel_v10.mo
+-rw-r--r--   0        0        0    16545 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot
+-rw-r--r--   0        0        0    16545 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldTwoUTubes.mot
+-rw-r--r--   0        0        0      133 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/Borefield_Instance.mopt
+-rw-r--r--   0        0        0    20304 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot
+-rw-r--r--   0        0        0    13167 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo
+-rw-r--r--   0        0        0     4527 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo
+-rw-r--r--   0        0        0     6161 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo
+-rw-r--r--   0        0        0     3298 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt
+-rw-r--r--   0        0        0    10560 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo
+-rw-r--r--   0        0        0    14157 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo
+-rw-r--r--   0        0        0    16738 2024-05-07 15:30:38.281318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/GroundTemperatureResponse.mo
+-rw-r--r--   0        0        0    15862 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot
+-rw-r--r--   0        0        0     2028 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt
+-rw-r--r--   0        0        0     6810 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo
+-rw-r--r--   0        0        0     2874 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo
+-rw-r--r--   0        0        0      899 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo
+-rw-r--r--   0        0        0     2777 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel_v10.mo
+-rw-r--r--   0        0        0     4245 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo
+-rw-r--r--   0        0        0     1407 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo
+-rw-r--r--   0        0        0     1878 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos
+-rw-r--r--   0        0        0     1600 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot
+-rw-r--r--   0        0        0     1563 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/BoilerPolynomial.mot
+-rw-r--r--   0        0        0      946 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/boiler_polynomial.py
+-rw-r--r--   0        0        0    16370 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_partial.mot
+-rw-r--r--   0        0        0     4434 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.mot
+-rw-r--r--   0        0        0     6424 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.py
+-rw-r--r--   0        0        0     5799 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX_variable.mot
+-rw-r--r--   0        0        0     6357 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX_variable.py
+-rw-r--r--   0        0        0     1505 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.mot
+-rw-r--r--   0        0        0     1235 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACDCConverter.py
+-rw-r--r--   0        0        0     2125 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot
+-rw-r--r--   0        0        0     1911 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py
+-rw-r--r--   0        0        0     1263 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Capacitive.mot
+-rw-r--r--   0        0        0     1092 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.mot
+-rw-r--r--   0        0        0     1145 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py
+-rw-r--r--   0        0        0     1150 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitive.py
+-rw-r--r--   0        0        0     1202 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Generator.mot
+-rw-r--r--   0        0        0     1088 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Grid.mot
+-rw-r--r--   0        0        0     1228 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot
+-rw-r--r--   0        0        0     1333 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot
+-rw-r--r--   0        0        0     1156 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py
+-rw-r--r--   0        0        0     1497 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py
+-rw-r--r--   0        0        0      823 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/grid.py
+-rw-r--r--   0        0        0     1697 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py
+-rw-r--r--   0        0        0     1040 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/AcBattery.mot
+-rw-r--r--   0        0        0     1131 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py
+-rw-r--r--   0        0        0      935 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/capacitor.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/DC/Loads/Conductor.py
+-rw-r--r--   0        0        0     5908 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/PVsubsystem.mot
+-rw-r--r--   0        0        0     3754 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot
+-rw-r--r--   0        0        0      581 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/pv_subsystem.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/__init__.py
+-rw-r--r--   0        0        0     8248 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/csv_modelica.py
+-rw-r--r--   0        0        0    12391 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/input_parser.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/__init__.py
+-rw-r--r--   0        0        0     1843 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/Dockerfile
+-rw-r--r--   0        0        0     2674 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/__init__.py
+-rw-r--r--   0        0        0      199 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/compile_fmu.most
+-rw-r--r--   0        0        0      642 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/simulate.most
+-rw-r--r--   0        0        0      934 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot
+-rw-r--r--   0        0        0     3060 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot
+-rw-r--r--   0        0        0    21392 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/modelica_runner.py
+-rw-r--r--   0        0        0     3995 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/simple_gmt_base.py
+-rw-r--r--   0        0        0      161 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/templates/package_base.mot
+-rw-r--r--   0        0        0     3810 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/scaffold.py
+-rw-r--r--   0        0        0    53051 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/schema.json
+-rw-r--r--   0        0        0    41280 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/system_parameters.py
+-rw-r--r--   0        0        0     6209 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/time_series_template.json
+-rw-r--r--   0        0        0     5193 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/geojson_modelica_translator/utils.py
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/management/__init__.py
+-rw-r--r--   0        0        0     9983 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/management/check_sys_params.py
+-rw-r--r--   0        0        0     2634 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/management/data/baseline_geojson.json
+-rw-r--r--   0        0        0     4507 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/management/data/baseline_sys_params.json
+-rw-r--r--   0        0        0        0 2024-05-07 15:30:38.285318 geojson_modelica_translator-0.7.0/management/data/baseline_time_series.mos
+-rw-r--r--   0        0        0  1148813 2024-05-07 15:30:38.293318 geojson_modelica_translator-0.7.0/management/data/baseline_weather.mos
+-rw-r--r--   0        0        0     6592 2024-05-07 15:30:38.293318 geojson_modelica_translator-0.7.0/management/format_modelica_files.py
+-rw-r--r--   0        0        0     8403 2024-05-07 15:30:38.293318 geojson_modelica_translator-0.7.0/management/uo_des.py
+-rw-r--r--   0        0        0     1345 2024-05-07 15:30:38.293318 geojson_modelica_translator-0.7.0/management/update_schemas.py
+-rw-r--r--   0        0        0     4638 2024-05-07 15:30:38.293318 geojson_modelica_translator-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0     7671 1970-01-01 00:00:00.000000 geojson_modelica_translator-0.7.0/PKG-INFO
```

### Comparing `geojson_modelica_translator-0.6.0rc2/LICENSE.md` & `geojson_modelica_translator-0.7.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-URBANopt™, Copyright (c) 2019, 2023 Alliance for Sustainable Energy, LLC, and other contributors.
+URBANopt™, Copyright (c) 2019, 2024 Alliance for Sustainable Energy, LLC, and other contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without modification, are permitted
 provided that the following conditions are met:
 
 (1) Redistributions of source code must retain the above copyright notice, this list of conditions
 and the following disclaimer.
```

### Comparing `geojson_modelica_translator-0.6.0rc2/README.rst` & `geojson_modelica_translator-0.7.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,80 +1,63 @@
-GeoJSON Modelica Translator (GMT)
----------------------------------
+# GeoJSON Modelica Translator (GMT)
 
-.. image:: https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml/badge.svg?branch=develop
-    :target: https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml
+[![image](https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml/badge.svg?branch=develop)](https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml)
+[![image](https://coveralls.io/repos/github/urbanopt/geojson-modelica-translator/badge.svg?branch=develop)](https://coveralls.io/github/urbanopt/geojson-modelica-translator?branch=develop)
+[![image](https://badge.fury.io/py/geojson-modelica-translator.svg)](https://badge.fury.io/py/geojson-modelica-translator)
 
-.. image:: https://coveralls.io/repos/github/urbanopt/geojson-modelica-translator/badge.svg?branch=develop
-    :target: https://coveralls.io/github/urbanopt/geojson-modelica-translator?branch=develop
-
-.. image:: https://badge.fury.io/py/geojson-modelica-translator.svg
-    :target: https://badge.fury.io/py/geojson-modelica-translator
-
-Description
------------
-
-The GeoJSON Modelica Translator (GMT) is a one-way trip from GeoJSON in combination with a well-defined instance of the system parameters schema to a Modelica package with multiple buildings loads, energy transfer stations, distribution networks, and central plants. The project will eventually allow multiple paths to build up different district heating and cooling system topologies; however, the initial implementation is limited to 1GDH and 4GDHC.
+The GeoJSON Modelica Translator (GMT) is a one-way trip from GeoJSON in combination with a well-defined instance of the system parameters schema to a Modelica package with multiple buildings loads, energy transfer stations, distribution networks, and central plants. The project will eventually allow multiple paths to build up different district heating and cooling system topologies; however, the initial implementation is limited to 4GDHC and 5GDHC.
 
 The project is motivated by the need to easily evaluate district energy systems. The goal is to eventually cover the various generations of heating and cooling systems as shown in the figure below. The need to move towards 5GDHC systems results in higher efficiencies and greater access to additional waste-heat sources.
 
-.. image:: https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-generations.png
-
-Getting Started
----------------
+![image](https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-generations.png)
 
-It is possible to test the GeoJSON to Modelica Translator (GMT) by simply installing the Python package and running the
-command line interface (CLI) with results from and URBANopt SDK set of results. However, to fully leverage the
-functionality of this package (e.g., running simulations), then you must also install the Modelica Buildings
-library (MBL) and Docker. Instructions for installing and configuring the MBL and Docker are available
-`here <docs/getting_started.rst>`_.
+## Getting Started
 
-To simply scaffold out a Modelica package that can be inspected in a Modelica environment (e.g., Dymola) then
-run the following code below up to the point of run-model. The example generates a complete 4th Generation District
-Heating and Cooling (4GDHC) system with time series loads that were generated from the URBANopt SDK using
-OpenStudio/EnergyPlus simulations.
+It is possible to test the GeoJSON to Modelica Translator (GMT) by simply installing the Python package and running the command line interface (CLI) with results from and URBANopt SDK set of results. However, to fully leverage the functionality of this package (e.g., running simulations), then you must also install the Modelica Buildings library (MBL) and Docker. Instructions for installing and configuring the MBL and Docker are available [here](docs/getting_started.rst).
 
-.. code-block:: bash
+To simply scaffold out a Modelica package that can be inspected in a Modelica environment (e.g., Dymola, OpenModelica) then run the following code below up to the point of run-model. The example generates a complete 4th Generation District Heating and Cooling (4GDHC) system with time series loads that were generated from the URBANopt SDK using OpenStudio/EnergyPlus simulations.
 
-    pip install geojson-modelica-translator
+``` bash
+pip install geojson-modelica-translator
 
-    # from the simulation results within a checkout of this repository
-    # in the ./tests/management/data/sdk_project_scraps path.
+# from the simulation results within a checkout of this repository
+# in the ./tests/management/data/sdk_project_scraps path.
 
-    # generate the system parameter from the results of the URBANopt SDK and OpenStudio Simulations
-    uo_des build-sys-param sys_param.json baseline_scenario.csv example_project.json
+# generate the system parameter from the results of the URBANopt SDK and OpenStudio Simulations
+uo_des build-sys-param sys_param.json baseline_scenario.csv example_project.json
 
-    # create the modelica package (requires installation of the MBL)
-    uo_des create-model sys_param.json example_project.json model_from_sdk
+# create the modelica package (requires installation of the MBL)
+uo_des create-model sys_param.json example_project.json model_from_sdk
 
-    # test running the new Modelica package (requires installation of Docker)
-    uo_des run-model model_from_sdk
+# test running the new Modelica package (requires installation of Docker)
+uo_des run-model model_from_sdk
+```
 
-More example projects are available in an accompanying
-`example repository <https://github.com/urbanopt/geojson-modelica-translator-examples>`_.
+More example projects are available in an accompanying [example repository](https://github.com/urbanopt/geojson-modelica-translator-examples).
 
-Architecture Overview
----------------------
+## Architecture Overview
 
-The GMT is designed to enable "easy" swapping of building loads, district systems, and network topologies. Some
-of these functionalities are more developed than others, for instance swapping building loads between Spawn and
-RC models (using TEASER) is fleshed out; however, swapping between a first and fifth generation heating system has
-yet to be fully implemented.
+The GMT is designed to enable "easy" swapping of building loads, district systems, and network topologies. Some of these functionalities are more developed than others, for instance swapping building loads between Spawn and RC models (using TEASER) is fleshed out; however, swapping between a first and fifth generation heating system has yet to be fully implemented.
 
-The diagram below is meant to illustrate the future proposed interconnectivity and functionality of the
-GMT project.
+The diagram below is meant to illustrate the future proposed interconnectivity and functionality of the GMT project.
 
-.. image:: https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-connections.png
+![image](https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-connections.png)
 
-As shown in the image, there are multiple building loads that can be deployed with the GMT and are described in the `Building Load Models`_ section below. These models, and the associated design parameters, are required to create a fully runnable Modelica model. The GMT leverages two file formats for generating the Modelica project and are the GeoJSON feature file and a System Parameter JSON file. See the more `comprehensive
-documentation on the GMT <https://docs.urbanopt.net/geojson-modelica-translator/>`_ or the `documentation on
-URBANopt SDK  <https://docs.urbanopt.net/>`_.
+As shown in the image, there are multiple building loads that can be deployed with the GMT and are described in the [Building Load Models](#building-load-models) section below. These models, and the associated design parameters, are required to create a fully runnable Modelica model. The GMT leverages two file formats for generating the Modelica project and are the GeoJSON feature file and a System Parameter JSON file. See the more [comprehensive documentation on the GMT](https://docs.urbanopt.net/geojson-modelica-translator/) or the [documentation on URBANopt SDK](https://docs.urbanopt.net/).
 
-Building Load Models
-++++++++++++++++++++
+### Building Load Models
 
 The building loads can be defined multiple ways depending on the fidelity of the required models. Each of the building load models are easily replaced using configuration settings within the System Parameters file. The 4 different building load models include:
 
-#. Time Series in Watts: This building load is the total heating, cooling, and domestic hot water loads represented in a CSV type file (MOS file). The units are Watts and should be reported at an hour interval; however, finer resolution is possible. The load is defined as the load seen by the ETS.
-#. Time Series as mass flow rate and delta temperature: This building load is similar to the other Time Series model but uses the load as seen by the ETS in the form of mass flow rate and delta temperature. The file format is similar to the other Time Series model but the columns are mass flow rate and delta temperature for heating and cooling separately.
-#. RC Model: This model leverages the TEASER framework to generate an RC model with the correct coefficients based on high level parameters that are extracted from the GeoJSON file including building area and building type.
-#. Spawn of EnergyPlus: This model uses EnergyPlus models to represent the thermal zone heat balance portion of the models while using Modelica for the remaining components. Spawn of EnergyPlus is still under development and currently only works on Linux-based systems.
+1. **Time Series in Watts**: This building load is the total heating, cooling, and domestic hot water loads represented in a CSV type file (MOS file). The units are Watts and should be reported at an hour interval; however, finer resolution is possible. The load is defined as the load seen by the ETS.
+2. **Time Series as mass flow rate and delta temperature**: This building load is similar to the other Time Series model but uses the load as seen by the ETS in the form of mass flow rate and delta temperature. The file format is similar to the other Time Series model but the columns are mass flow rate and delta temperature for heating and cooling separately.
+3. **RC Model**: This model leverages the TEASER framework to generate an RC model with the correct coefficients based on high level parameters that are extracted from the GeoJSON file including building area and building type.
+4. **Spawn of EnergyPlus**: This model uses EnergyPlus models to represent the thermal zone heat balance portion of the models while using Modelica for the remaining components. Spawn of EnergyPlus is still under development and currently only works on Linux-based systems.
+
+## Release Instructions
+
+1. Create a branch named `prep-0.x.y Release`
+2. Update CHANGELOG using GitHub's "Autogenerate Change Log" feature
+3. After tests pass, merge branch into develop
+4. Create new PR from develop into main named `Release 0.x.y`
+5. Using GitHub squash-merge into main
+6. From local repo, immediately merge main into develop (as a merge commit) and push. This can only be done with users that have bypass privileges on GitHub.
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/building_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/building_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/district_system_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/electrical_connector_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/electrical_junction_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/region_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/region_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/site_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/site_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/thermal_connector_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/data/schemas/thermal_junction_properties.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/schemas.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/schemas.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,49 +3,44 @@
 
 import json
 import os
 
 from jsonschema.validators import Draft202012Validator as LatestValidator
 
 
-class Schemas(object):
-    """
-    Class to hold the various schemas
-    """
+class Schemas:
+    """Class to hold the various schemas"""
 
     def __init__(self):
         """Load in the schemas"""
         self.schemas = {
             "building": None,
             "district_system": None,
             "electrical_connector": None,
             "electrical_junction": None,
             "region": None,
             "site": None,
             "thermal_connector": None,
             "thermal_junction": None,
         }
 
-        for s in self.schemas.keys():
-            path = os.path.join(
-                os.path.dirname(__file__), "data/schemas/%s_properties.json" % s
-            )
-            with open(path, "r") as f:
+        for s in self.schemas:
+            path = os.path.join(os.path.dirname(__file__), "data/schemas/%s_properties.json" % s)
+            with open(path) as f:
                 self.schemas[s] = json.load(f)
 
     def retrieve(self, name):
-        """name of the schema to retrieve"""
+        """Name of the schema to retrieve"""
         if self.schemas.get(name):
             return self.schemas[name]
         else:
-            raise Exception("Schema for %s does not exist" % name)
+            raise NameError(f"Schema for {name} does not exist")
 
     def validate(self, name, instance):
-        """
-        Validate an instance against a loaded schema
+        """Validate an instance against a loaded schema
 
         :param name: str, name of the schema to validate against
         :param instance: dict, instance to validate
         :return:
         """
         results = []
         s = self.retrieve(name)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson/urbanopt_geojson.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson/urbanopt_geojson.py`

 * *Files 11% similar despite different names*

```diff
@@ -12,17 +12,16 @@
 
 
 class GeoJsonValidationError(Exception):
     pass
 
 
 # TODO: Inherit from GeoJSON Feature class, move to its own file
-class UrbanOptLoad(object):
-    """
-    An UrbanOptLoad is a container for holding Building-related data in a dictionary. This object
+class UrbanOptLoad:
+    """An UrbanOptLoad is a container for holding Building-related data in a dictionary. This object
     does not do much work on the GeoJSON definition of the data at the moment, rather it creates
     an isolation layer between the GeoJSON data and the GMT.
     """
 
     def __init__(self, feature):
         self.feature = feature
         self.id = feature.get("properties", {}).get("id", None)
@@ -31,54 +30,54 @@
         if self.id is None:
             raise GeoJsonValidationError("GeoJSON feature requires an ID property but value was null")
 
     def __str__(self):
         return f"ID: {self.id}"
 
 
-class UrbanOptGeoJson(object):
-    """
-    Root class for parsing an URBANopt GeoJSON file. This class simply reads and parses
+class UrbanOptGeoJson:
+    """Root class for parsing an URBANopt GeoJSON file. This class simply reads and parses
     URBANopt GeoJSON files.
     """
 
     def __init__(self, filename, building_ids=None):
-        """
+        """Initialize the UrbanOptGeoJson object by reading the GeoJSON file
+
         :param filename: str, path to the GeoJSON file to parse
         :param building_ids: list[str | int] | None, optional, list of GeoJSON building
             IDs to parse from the file. If None or an empty list, parse all buildings.
         """
         if not Path(filename).exists():
             raise GeoJsonValidationError(f"URBANopt GeoJSON file does not exist: {filename}")
 
-        with open(filename, "r") as f:
+        with open(filename) as f:
             self.data = geojson.load(f)
 
         self.schemas = Schemas()
 
         errors = ""
         building_errors = {}
         self.buildings = []
         for feature in self.data.features:
             if feature["properties"]["type"] == "Building":
                 building = UrbanOptLoad(feature)
                 if not building_ids or building.id in building_ids:
-                    # Don't care about validation failures for features with 'detailed_model_filename' in the building properties
-                    # Buildings defined by an osm don't have all keys in geojson, they'll always fail validation
+                    # Ignore validation failures for features with 'detailed_model_filename' in the properties
+                    # Buildings defined by an osm don't have all keys in geojson, therefore will always fail validation
                     if "detailed_model_filename" not in feature["properties"]:
                         errors = self.schemas.validate("building", building.feature.properties)
                     if errors:
                         building_errors[building.id] = errors
                     else:
                         self.buildings.append(building)
 
         if building_errors:
-            formatted_errors = ''
+            formatted_errors = ""
             for building_id, errors in building_errors.items():
-                building_errors_bullets = ''.join([f'\n    * {error}' for error in errors])
-                formatted_errors += f'\n  ID {building_id}:{building_errors_bullets}'
+                building_errors_bullets = "".join([f"\n    * {error}" for error in errors])
+                formatted_errors += f"\n  ID {building_id}:{building_errors_bullets}"
 
-            message = f'GeoJSON file is not valid:{formatted_errors}'
+            message = f"GeoJSON file is not valid:{formatted_errors}"
             raise GeoJsonValidationError(message)
 
         if not self.buildings:
-            raise GeoJsonValidationError(f'No valid buildings found in GeoJSON file: {filename}')
+            raise GeoJsonValidationError(f"No valid buildings found in GeoJSON file: {filename}")
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/geojson_modelica_translator.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/geojson_modelica_translator.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,25 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import logging
 from pathlib import Path
 
-from geojson_modelica_translator.geojson.urbanopt_geojson import (
-    UrbanOptGeoJson
-)
-from geojson_modelica_translator.model_connectors.couplings import (
-    Coupling,
-    CouplingGraph
-)
+from geojson_modelica_translator.geojson.urbanopt_geojson import UrbanOptGeoJson
+from geojson_modelica_translator.model_connectors.couplings import Coupling, CouplingGraph
 from geojson_modelica_translator.model_connectors.districts import District
-from geojson_modelica_translator.model_connectors.energy_transfer_systems import (
-    CoolingIndirect,
-    HeatingIndirect
-)
-from geojson_modelica_translator.model_connectors.load_connectors import (
-    Spawn,
-    Teaser,
-    TimeSeries,
-    TimeSeriesMFT
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems import CoolingIndirect, HeatingIndirect
+from geojson_modelica_translator.model_connectors.load_connectors import Spawn, Teaser, TimeSeries, TimeSeriesMFT
 from geojson_modelica_translator.model_connectors.networks import Network2Pipe
-from geojson_modelica_translator.model_connectors.networks.network_distribution_pump import (
-    NetworkDistributionPump
-)
+from geojson_modelica_translator.model_connectors.networks.network_distribution_pump import NetworkDistributionPump
 from geojson_modelica_translator.model_connectors.plants import CoolingPlant
-from geojson_modelica_translator.model_connectors.plants.borefield import (
-    Borefield
-)
-from geojson_modelica_translator.model_connectors.plants.chp import (
-    HeatingPlantWithOptionalCHP
-)
+from geojson_modelica_translator.model_connectors.plants.borefield import Borefield
+from geojson_modelica_translator.model_connectors.plants.chp import HeatingPlantWithOptionalCHP
 from geojson_modelica_translator.modelica.modelica_runner import ModelicaRunner
-from geojson_modelica_translator.system_parameters.system_parameters import (
-    SystemParameters
-)
+from geojson_modelica_translator.system_parameters.system_parameters import SystemParameters
 
 _log = logging.getLogger(__name__)
 
 
 # map the system parameter "load_model" to Python class
 LOAD_MODEL_TO_CLASS = {
     "spawn": Spawn,
@@ -84,15 +63,15 @@
         # create borefield
         borefield = Borefield(sys_params)
         all_couplings.append(Coupling(borefield, ambient_water_stub, district_type))
         all_couplings.append(Coupling(ambient_water_stub, ambient_water_stub, district_type))
 
     # create the loads and their ETSes
     for building in geojson.buildings:
-        load_model_type = sys_params.get_param_by_building_id(building.id, "load_model")
+        load_model_type = sys_params.get_param_by_id(building.id, "load_model")
         load_class = LOAD_MODEL_TO_CLASS[load_model_type]
         load = load_class(sys_params, building)
 
         if district_type is None or district_type == "4G":
             cooling_indirect = CoolingIndirect(sys_params, building.id)
             all_couplings.append(Coupling(load, cooling_indirect))
             all_couplings.append(Coupling(cooling_indirect, cooling_network))
@@ -102,15 +81,15 @@
             all_couplings.append(Coupling(heating_indirect, heating_network))
         elif district_type == "5G":
             all_couplings.append(Coupling(load, ambient_water_stub, district_type))
 
     return all_couplings
 
 
-class ModelicaPackage(object):
+class ModelicaPackage:
     """Represents a modelica package which can be simulated"""
 
     def __init__(self, file_to_run, project_path, project_name):
         self._file_to_run = file_to_run
         self._project_path = project_path
         self._project_name = project_name
 
@@ -118,24 +97,20 @@
         """Simulate the package.
 
         :return: tuple(bool, pathlib.Path), True or False depending on simulation success
             followed by the path to the results directory
         """
         modelica_runner = ModelicaRunner()
         return modelica_runner.run_in_docker(
-            self._file_to_run,
-            run_path=self._project_path,
-            project_name=self._project_name
+            self._file_to_run, run_path=self._project_path, project_name=self._project_name
         )
 
 
-class GeoJsonModelicaTranslator(object):
-    """
-    Main class for using the GeoJSON to Modelica Translator.
-    """
+class GeoJsonModelicaTranslator:
+    """Main class for using the GeoJSON to Modelica Translator."""
 
     def __init__(
         self,
         geojson_filepath,
         sys_params_filepath,
         root_dir,
         project_name,
@@ -144,50 +119,38 @@
 
         :param geojson_filepath: str, path to GeoJSON file
         :param sys_params_filepath: str, path to system parameters file
         :param root_dir: str, where to create the package
         :project_name: str, name of the package
         """
         if not Path(geojson_filepath).exists():
-            raise FileNotFoundError(f'GeoJSON file path does not exist: {geojson_filepath}')
+            raise FileNotFoundError(f"GeoJSON file path does not exist: {geojson_filepath}")
         if not Path(sys_params_filepath).exists():
-            raise FileNotFoundError(f'System parameters file path does not exist: {sys_params_filepath}')
+            raise FileNotFoundError(f"System parameters file path does not exist: {sys_params_filepath}")
 
         self._system_parameters = SystemParameters(sys_params_filepath)
 
-        geojson_ids = self._system_parameters.get_default(
-            '$.buildings.[*].geojson_id',
-            []
-        )
+        geojson_ids = self._system_parameters.get_default("$.buildings.[*].geojson_id", [])
         self._geojson = UrbanOptGeoJson(geojson_filepath, geojson_ids)
 
         # Use different couplings for each district system type
         district_type = self._system_parameters.get_param("district_system")
-        if 'fifth_generation' in district_type:
-            self._couplings = _parse_couplings(self._geojson, self._system_parameters, district_type='5G')
-        elif 'fourth_generation' in district_type:
+        if "fifth_generation" in district_type:
+            self._couplings = _parse_couplings(self._geojson, self._system_parameters, district_type="5G")
+        elif "fourth_generation" in district_type:
             self._couplings = _parse_couplings(self._geojson, self._system_parameters)
 
         self._root_dir = root_dir
         self._project_name = project_name
         self._coupling_graph = CouplingGraph(self._couplings)
-        self._district = District(
-            self._root_dir,
-            self._project_name,
-            self._system_parameters,
-            self._coupling_graph
-        )
+        self._district = District(self._root_dir, self._project_name, self._system_parameters, self._coupling_graph)
         self._package_created = False
 
     def to_modelica(self):
         """Generate the modelica package. Call `simulate` method on the result
         to run the package
 
         :return: ModelicaPackage
         """
         self._district.to_modelica()
 
-        return ModelicaPackage(
-            self._district.district_model_filepath,
-            self._root_dir,
-            self._project_name
-        )
+        return ModelicaPackage(self._district.district_model_filepath, self._root_dir, self._project_name)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/NetworkDistributionPump_NetworkDistributionPump/ComponentDefinitions.mopt`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,23 @@
   inner parameter
     Buildings.Experimental.DHC.Examples.Combined.BaseClasses.DesignDataSeries
     datDes(
     nBui={{ sys_params.num_buildings }},
     {% if sys_params.district_system.fifth_generation.ghe_parameters.design.flow_type == 'borehole' %}
-    mPumDis_flow_nominal={{ 10*sys_params.district_system.fifth_generation.ghe_parameters.design.flow_rate*
+    mPumDis_flow_nominal={{ sys_params.district_system.fifth_generation.ghe_parameters.design.flow_rate*
     sys_params.district_system.fifth_generation.ghe_parameters.ghe_specific_params[0].borehole.number_of_boreholes }},
     {% else %}
-    mPumDis_flow_nominal={{ 10*sys_params.district_system.fifth_generation.ghe_parameters.design.flow_rate }},
+    mPumDis_flow_nominal={{ sys_params.district_system.fifth_generation.ghe_parameters.design.flow_rate }},
     {% endif %}
     mPipDis_flow_nominal=datDes.mPumDis_flow_nominal,
     dp_length_nominal=250,
     final mCon_flow_nominal={
     {% for building in range( sys_params.num_buildings-1 ) %}
     {{ graph.couplings_by_type(coupling.network.id).load_couplings[building].load.id }}.ets.mSerWat_flow_nominal,
     {% endfor %}
     {{ graph.couplings_by_type(coupling.network.id).load_couplings[sys_params.num_buildings-1].load.id }}.ets.mSerWat_flow_nominal})
     "Design data"
     {% raw %}annotation (Placement(transformation(extent={{-140,100},{-120,120}})));
-  {% endraw %}parameter Boolean allowFlowReversalSer = true
+  parameter Boolean allowFlowReversalSer = true
     "Set to true to allow flow reversal in the service lines"
-    {% raw %}annotation(Dialog(tab="Assumptions"), Evaluate=true);
+    annotation(Dialog(tab="Assumptions"), Evaluate=true);
   {% endraw %}
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkAmbientWaterStub/ConnectStatements.mopt`

 * *Files 4% similar despite different names*

```diff
@@ -5,13 +5,11 @@
   annotation ({{ diagram.line.ts_load.t_hea_wat_max_set.t_hea_wat_set.y }});
 connect({{ coupling.load.id }}.THotWatSupSet, THeaWatSet_{{ coupling.id }}.y)
   annotation ({{ diagram.line.ts_load.t_hot_wat_set.t_hea_wat_set.y }});
 connect({{ coupling.load.id }}.TChiWatSupSet, THeaWatSet_{{ coupling.id }}.y)
   annotation ({{ diagram.line.ts_load.t_chi_wat_set.t_hea_wat_set.y }});
 connect(TCooWatSet_{{ coupling.id }}.y, {{ coupling.load.id }}.TColWat)
   annotation ({{ diagram.line.t_coo_wat_set.y.ts_load.t_col_wat }});
-connect(secMasFloRat_{{ coupling.id }}.y, supHeaWat_{{ sys_params.load_num }}.m_flow_in)
-  annotation ({{ diagram.line.sec_mas_flo_rat.y.sup_hea_wat.m_flow_in }});
 connect(supHeaWat_{{ sys_params.load_num }}.ports[1], {{ coupling.load.id }}.port_aSerAmb)
   annotation ({{ diagram.line.sup_hea_wat.ports.ts_load.port_a_amb }});
 connect({{ coupling.load.id }}.port_bSerAmb, sinHeaWat.ports[{{ sys_params.load_num }}])
   annotation ({{ diagram.line.ts_load.port_b_amb.sin_hea_wat.ports }});
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ComponentDefinitions.mopt`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THeaWatSupMaxSet_{{ coupling.id }}(k=38 +
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant THeaWatSupMaxSet_{{ coupling.id }}(k=38 +
         273.15) "Heating water supply temperature set point - Maximum value"
     {% raw %}annotation (Placement(transformation(extent={{-120,40},{-100,60}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant TChiWatSupSet_{{ coupling.id }}(k=18 + 273.15)
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant TChiWatSupSet_{{ coupling.id }}(k=18 + 273.15)
     "Chilled water supply temperature set point"
     {% raw %}annotation (Placement(transformation(extent={{-120,10},{-100,30}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THeaWatSupMinSet_{{ coupling.id }}(k=28
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant THeaWatSupMinSet_{{ coupling.id }}(k=28
          + 273.15) "Heating water supply temperature set point - Minimum value"
     {% raw %}annotation (Placement(transformation(extent={{-120,70},{-100,90}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THotWatSupSet_{{ coupling.id }}(k=63 + 273.15)
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant THotWatSupSet_{{ coupling.id }}(k=63 + 273.15)
     "Hot water supply temperature set point"
     {% raw %}annotation (Placement(transformation(extent={{-120,-20},{-100,0}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant TColWat_{{ coupling.id }}(k=15 + 273.15)
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant TColWat_{{ coupling.id }}(k=15 + 273.15)
     "Cold water temperature"
     {% raw %}annotation (Placement(transformation(extent={{-120,-50},{-100,-30}})));
   {% endraw %}
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/5G_templates/TimeSeries_NetworkDistributionPump/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/coupling.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/coupling.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,53 +2,46 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 from pathlib import Path
 
 from jinja2 import Environment, FileSystemLoader, StrictUndefined, meta
 
 from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
-from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import (
-    EnergyTransferBase
-)
-from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
-    LoadBase
-)
-from geojson_modelica_translator.model_connectors.networks.network_base import (
-    NetworkBase
-)
-from geojson_modelica_translator.model_connectors.plants.plant_base import (
-    PlantBase
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import EnergyTransferBase
+from geojson_modelica_translator.model_connectors.load_connectors.load_base import LoadBase
+from geojson_modelica_translator.model_connectors.networks.network_base import NetworkBase
+from geojson_modelica_translator.model_connectors.plants.plant_base import PlantBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
-class Coupling(object):
-    """A Coupling represents a connection/relationship between two models (e.g. a load and ets).
+class Coupling:
+    """A Coupling represents a connection/relationship between two models (e.g., a load and ets).
     More specifically, is used to create the required components and connections between two models.
     """
-    _template_component_definitions = 'ComponentDefinitions.mopt'
-    _template_connect_statements = 'ConnectStatements.mopt'
+
+    _template_component_definitions = "ComponentDefinitions.mopt"
+    _template_connect_statements = "ConnectStatements.mopt"
 
     def __init__(self, model_a, model_b, district_type=None):
         model_a, model_b = self._sort_models(model_a, model_b)
         self._model_a = model_a
         self._model_b = model_b
         self.district_type = district_type
-        self._template_base_name = f'{model_a.model_name}_{model_b.model_name}'
+        self._template_base_name = f"{model_a.model_name}_{model_b.model_name}"
 
-        if self.district_type == '5G':
+        if self.district_type == "5G":
             self._template_dir = Path(__file__).parent / "5G_templates" / self._template_base_name
         else:
             self._template_dir = Path(__file__).parent / "templates" / self._template_base_name
         if not Path(self._template_dir).exists():
-            raise Exception(f'Invalid coupling. Missing {self._template_dir} directory.')
+            raise Exception(f"Invalid coupling. Missing {self._template_dir} directory.")
 
         self._template_env = Environment(
-            loader=FileSystemLoader(searchpath=self._template_dir),
-            undefined=StrictUndefined)
+            loader=FileSystemLoader(searchpath=self._template_dir), undefined=StrictUndefined
+        )
         self._template_env.filters.update(ALL_CUSTOM_FILTERS)
 
         self._id = simple_uuid()
 
     @property
     def id(self):
         return self._id
@@ -59,34 +52,36 @@
 
     @property
     def model_b(self):
         return self._model_b
 
     def to_dict(self):
         return {
-            'id': self._id,
+            "id": self._id,
             self._model_a.simple_gmt_type: {
-                'id': self._model_a.id,
+                "id": self._model_a.id,
             },
             self._model_b.simple_gmt_type: {
-                'id': self._model_b.id,
-            }
+                "id": self._model_b.id,
+            },
         }
 
     def get_other_model(self, model):
         """Returns the other model in the coupling
 
         :param model: Model
         :return: Model
         """
         if model == self._model_a:
             return self._model_b
         elif model == self._model_b:
             return self._model_a
-        raise Exception(f'Provided model, "{model.id}", is not part of the coupling ({self._model_a.id}, {self._model_b.id})')
+        raise Exception(
+            f'Provided model, "{model.id}", is not part of the coupling ({self._model_a.id}, {self._model_b.id})'
+        )
 
     def _get_model_superclass(self, model):
         valid_superclasses = [LoadBase, EnergyTransferBase, NetworkBase, PlantBase]
         superclasses = [cls_ for cls_ in model.__class__.mro() if cls_ in valid_superclasses]
         if len(superclasses) != 1:
             return None
         return superclasses[0]
@@ -119,48 +114,47 @@
         :param template_name: string
         :param template_params: dict
         :return: string
         """
         template = self._template_env.get_template(template_name)
 
         def _get_model_id(model):
-            superclass_dict = {
-                LoadBase: 'load_id',
-                EnergyTransferBase: 'ets_id',
-                NetworkBase: 'network_id'
-            }
+            superclass_dict = {LoadBase: "load_id", EnergyTransferBase: "ets_id", NetworkBase: "network_id"}
             superclass = self._get_model_superclass(model)
             return superclass_dict[superclass]
 
-        assert 'coupling' not in template_params, 'Template parameters for Coupling must not include the key "coupling"'
-        updated_template_params = {
-            'coupling': self.to_dict()
-        }
+        if "coupling" in template_params:
+            raise SystemExit('Template parameters for Coupling must not include the key "coupling"')
+        updated_template_params = {"coupling": self.to_dict()}
         updated_template_params.update(template_params)
 
         # get the template file path relative to the package
         template_filename = Path(template.filename).as_posix()
-        _, template_filename = template_filename.rsplit('geojson_modelica_translator', 1)
+        _, template_filename = template_filename.rsplit("geojson_modelica_translator", 1)
 
         return template.render(updated_template_params), template_filename
 
     def render_templates(self, template_params):
         """Renders the shared components and connect statements for the coupling.
 
         :param template_params: dict, parameters for the templates
         :return: dict, containing key, values: component_definitions, string; connect_statements, string
         """
-        component_result, component_template_path = self._render_template(self._template_component_definitions, template_params)
-        connect_result, connect_template_path = self._render_template(self._template_connect_statements, template_params)
+        component_result, component_template_path = self._render_template(
+            self._template_component_definitions, template_params
+        )
+        connect_result, connect_template_path = self._render_template(
+            self._template_connect_statements, template_params
+        )
 
         return {
-            'component_definitions': component_result,
-            'connect_statements': connect_result,
-            'component_definitions_template_path': component_template_path,
-            'connect_statements_template_path': connect_template_path,
+            "component_definitions": component_result,
+            "connect_statements": connect_result,
+            "component_definitions_template_path": component_template_path,
+            "connect_statements_template_path": connect_template_path,
         }
 
     def get_load(self):
         """If there's a load model in the coupling, it returns the load model. Else
         it returns None.
 
         This is used by the district model to find the building's sys params so
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/diagram.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/diagram.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,65 +7,64 @@
 from random import uniform
 from string import Template
 
 from geojson_modelica_translator.model_connectors.couplings.utils import (
     DiagramLine,
     DiagramTransformation,
     find_path_bfs,
-    parse_diagram_commands
+    parse_diagram_commands,
 )
 
-NodePort = namedtuple('NodePort', ['node', 'port'])
+NodePort = namedtuple("NodePort", ["node", "port"])
 
 
 class DiagramNode:
     def __init__(self, context_id, model_name, model_type):
-        """
-        :param context_id: str, used for "grouping" nodes. E.g. this would be
+        """DiagramNode represents a node in the diagram graph
+
+        :param context_id: str, used for "grouping" nodes, e.g., this would be
           either the coupling id or the model id (depending on where the icon is declared)
         :param model_name: str
-        :param model_type: str, general type of the component (e.g. load, network, etc)
+        :param model_type: str, general type of the component (e.g., load, network, etc)
         """
         self.context_id = context_id
         self.model_name = model_name
         self.model_type = model_type
         self.icon = DiagramIcon.get_icon(model_type)
         self.connections = defaultdict(list)
         self.grid_col = None
         self.grid_row = None
 
     def __eq__(self, other):
         if not isinstance(other, DiagramNode):
             return False
 
         def _simple_eq(a, b):
-            return (
-                a.context_id == b.context_id
-                and a.model_name == b.model_name
-            )
+            return a.context_id == b.context_id and a.model_name == b.model_name
 
         if not _simple_eq(self, other):
             return False
 
         # check connections iteratively to avoid infinite recursion
         if self.connections.keys() != other.connections.keys():
             return False
 
-        for port_name in self.connections.keys():
+        for port_name in self.connections:
             for self_conn, other_conn in zip(self.connections[port_name], other.connections[port_name]):
                 if not _simple_eq(self_conn.node, other_conn.node) or self_conn.port != other_conn.port:
                     return False
 
         return True
 
     def __hash__(self):
         return hash((self.context_id, self.model_name, self.model_type))
 
     def add_connection(self, this_port, other_node, other_port):
-        """
+        """Add a connection to the diagram
+
         :param this_port: str, name or dotted path of port for this node (should not start with '.' though)
         :param other_node: DiagramNode, other node connecting to
         :param other_port: str, name or dotted path of port for other node (should not start with '.' though)
         """
         self.connections[this_port].append(NodePort(other_node, other_port))
 
 
@@ -87,15 +86,15 @@
     def extent(self):
         """Returns extent as a string for templating into the district model
 
         :return: str
         """
         half_width = self.grid_width_px / 2
         half_height = self.grid_height_px / 2
-        return f'{{{{-{half_width},-{half_height}}},{{{half_width},{half_height}}}}}'
+        return f"{{{{-{half_width},-{half_height}}},{{{half_width},{half_height}}}}}"
 
     def _grid_to_coord(self, col, row):
         return self.grid_cell_size * col, self.grid_cell_size * row
 
     def _translate_x(self, pos):
         # translate from origin at upper left of grid to center of grid
         return pos - (self.grid_width_px / 2)
@@ -126,27 +125,27 @@
                     }
                 }
             }
         }
         """
         transformations = defaultdict(dict)
         lines = defaultdict(dict)
-        transformation_template = Template('transformation(extent={{$x1,$y1},{$x2,$y2}})')
-        line_template = Template('Line(points={$points},color={0,0,127})')
+        transformation_template = Template("transformation(extent={{$x1,$y1},{$x2,$y2}})")
+        line_template = Template("Line(points={$points},color={0,0,127})")
 
         # add transformations defined within this id's context
-        # e.g. if id is for a model, add all transformations defined in the model instance template
+        # e.g., if id is for a model, add all transformations defined in the model instance template
         for component_name, diagram_node in self._initial_diagram_graph.get(context_id, {}).items():
             # x1, y1 is lower left of icon, x2, y2 is upper right
             x_pos, y_pos = self._grid_to_coord(diagram_node.grid_col, diagram_node.grid_row)
             coords = {
-                'x1': self._translate_x(x_pos),
-                'y1': self._translate_y(y_pos + (diagram_node.icon.height * self.grid_cell_size)),
-                'x2': self._translate_x(x_pos + (diagram_node.icon.width * self.grid_cell_size)),
-                'y2': self._translate_y(y_pos),
+                "x1": self._translate_x(x_pos),
+                "y1": self._translate_y(y_pos + (diagram_node.icon.height * self.grid_cell_size)),
+                "x2": self._translate_x(x_pos + (diagram_node.icon.width * self.grid_cell_size)),
+                "y2": self._translate_y(y_pos),
             }
             transformations[component_name][diagram_node.model_type] = transformation_template.substitute(coords)
 
         diagram_ids = [context_id]
         if is_coupling:
             coupling = self._coupling_graph.get_coupling(context_id)
             diagram_ids += [coupling.model_a.id, coupling.model_b.id]
@@ -156,165 +155,147 @@
             for component_name, diagram_node in self._initial_diagram_graph.get(this_context_id, {}).items():
                 for component_port, others in diagram_node.connections.items():
                     for other in others:
                         other_node, other_port = other.node, other.port
                         # include this connection if either:
                         #   - we're working on the coupling lines
                         #   - this connects to another model we might be interested in
-                        #     (e.g. model a instance connecting to model b instance)
+                        #     (e.g., model a instance connecting to model b instance)
                         include_line = this_context_id == context_id or other_node.context_id in diagram_ids
                         if include_line:
                             points = self._calculate_connector_line(
-                                diagram_node,
-                                component_port,
-                                other_node,
-                                other_port
-                            )
-                            formatted_points = [f'{{{x},{y}}}' for x, y in points]
-                            line = line_template.substitute(
-                                points=','.join(formatted_points)
+                                diagram_node, component_port, other_node, other_port
                             )
+                            formatted_points = [f"{{{x},{y}}}" for x, y in points]
+                            line = line_template.substitute(points=",".join(formatted_points))
                             if component_port not in lines[component_name]:
-                                lines[component_name][component_port] = {
-                                    other_node.model_name: {
-                                        other_port: line
-                                    }
-                                }
+                                lines[component_name][component_port] = {other_node.model_name: {other_port: line}}
                             else:
-                                lines[component_name][component_port][other_node.model_name] = {
-                                    other_port: line
-                                }
+                                lines[component_name][component_port][other_node.model_name] = {other_port: line}
 
         return {
-            'transformation': transformations,
-            'line': lines,
+            "transformation": transformations,
+            "line": lines,
         }
 
     def _calculate_connector_line(self, node_a, port_a, node_b, port_b):
         """Determines a coordinate path to get from node a's port to node b's port
 
         :param node_a: DiagramNode
         :param port_a: str
         :param node_b: DiagramNode
         :param port_b: str
         :return: list, list of x,y tuples
         """
         grid_path = find_path_bfs(
-            self._diagram_matrix,
-            node_a.grid_row,
-            node_a.grid_col,
-            node_b.grid_row,
-            node_b.grid_col
+            self._diagram_matrix, node_a.grid_row, node_a.grid_col, node_b.grid_row, node_b.grid_col
         )
 
         # convert grid path into a coordinate path for the diagram
         diagram_path = []
         half_cell = self.grid_cell_size / 2
         # hack: add a random offsets to make lines overlap less
-        x_offset = uniform(half_cell * -1, half_cell)
-        y_offset = uniform(half_cell * -1, half_cell)
+        x_offset = uniform(half_cell * -1, half_cell)  # noqa: S311
+        y_offset = uniform(half_cell * -1, half_cell)  # noqa: S311
         for pos in grid_path:
             x, y = self._grid_to_coord(pos[1] + 0.5, pos[0] + 0.5)
-            diagram_path.append((
-                self._translate_x(x + x_offset),
-                self._translate_y(y + y_offset)
-            ))
+            diagram_path.append((self._translate_x(x + x_offset), self._translate_y(y + y_offset)))
 
         return diagram_path
 
     def _resolve_icon_placements(self):
         """Calculate and add locations to all diagram graph nodes. This should be
         called automatically when initializing the class.
         """
 
         def get_nodes_of_type(node_type):
             nodes = []
             for _, context_nodes in self._initial_diagram_graph.items():
                 for _, node in context_nodes.items():
-                    if node_type != 'auxillary' and node.model_type == node_type:
+                    if node_type != "auxillary" and node.model_type == node_type:
                         nodes.append(node)
-                    if node_type == 'auxillary' and node.model_type not in ['load', 'ets', 'plant', 'network']:
+                    if node_type == "auxillary" and node.model_type not in ["load", "ets", "plant", "network"]:
                         nodes.append(node)
             return nodes
 
         def get_connected_nodes_of_type(node, other_node_type):
             # use a set to avoid duplicates (a node might have multiple connections to another node)
             nodes = set()
             for _, connections in node.connections.items():
                 for connection in connections:
                     other_node = connection.node
                     if other_node.model_type == other_node_type:
                         nodes.add(other_node)
             return list(nodes)
 
-        MAX_ICONS_PER_ROW = 4
+        max_icons_per_row = 4
 
         load_ets_rows = []
         # add loads and etses
-        loads = get_nodes_of_type('load')
+        loads = get_nodes_of_type("load")
         for load_node in loads:
-            etses = get_connected_nodes_of_type(load_node, 'ets')
+            etses = get_connected_nodes_of_type(load_node, "ets")
             for load_ets_pair in zip_longest(etses, [load_node], fillvalue=None):
                 load_ets_rows.append(list(load_ets_pair))
 
         network_plant_rows = []
         # add networks and plants
-        for i, plant in enumerate(get_nodes_of_type('plant')):
+        for i, plant in enumerate(get_nodes_of_type("plant")):
             grid_row = []
             grid_row.append(plant)
             # NOTE: should only have one plant connected to a network
-            for network in get_connected_nodes_of_type(plant, 'network'):
+            for network in get_connected_nodes_of_type(plant, "network"):
                 grid_row.append(network)
 
             network_plant_rows.append(grid_row)
 
         # make sure each set of rows has the same length
         num_network_plant_rows = len(network_plant_rows)
         num_load_ets_rows = len(load_ets_rows)
         if num_network_plant_rows < num_load_ets_rows:
             # pad the network plant rows
             num_pad_rows = num_load_ets_rows - num_network_plant_rows
-            NUM_ICONS = 2  # dehardcode
+            num_icons = 2  # dehardcode
             for _ in range(num_pad_rows):
-                network_plant_rows.append([None] * NUM_ICONS)
+                network_plant_rows.append([None] * num_icons)
         elif num_load_ets_rows < num_network_plant_rows:
             # pad the load ets rows
             num_pad_rows = num_network_plant_rows - num_load_ets_rows
-            NUM_ICONS = 2  # dehardcode
+            num_icons = 2  # dehardcode
             for _ in range(num_pad_rows):
-                load_ets_rows.append([None] * NUM_ICONS)
+                load_ets_rows.append([None] * num_icons)
 
         # merge all of the rows
         merged_rows = []
         for left, right in zip(network_plant_rows, load_ets_rows):
             merged_rows.append(left + right)
 
         # add auxillary rows
         grid_row = []
-        for node in get_nodes_of_type('auxillary'):
-            if len(grid_row) == MAX_ICONS_PER_ROW:
+        for node in get_nodes_of_type("auxillary"):
+            if len(grid_row) == max_icons_per_row:
                 # start a new row
                 merged_rows.append(grid_row)
                 grid_row = [node]
             else:
                 # continue building row
                 grid_row.append(node)
         # add remaining row
         merged_rows.append(grid_row)
 
         # make sure all rows have the same number of columns by adding `None`s
         # to the end of shorter rows
         # TODO: find better solution
         longest_row = max([len(row) for row in merged_rows])
         for row in merged_rows:
-            row += [None] * (longest_row - len(row))
+            row += [None] * (longest_row - len(row))  # noqa: PLW2901
 
         # add padding between icons by building an updated grid
         # first row should be empty (+1 to make sure there's pad on both sides)
-        grid_cells_per_row = 1 + MAX_ICONS_PER_ROW + (MAX_ICONS_PER_ROW * self.icon_padding)
+        grid_cells_per_row = 1 + max_icons_per_row + (max_icons_per_row * self.icon_padding)
         diagram_matrix = [[None] * grid_cells_per_row]
         for row in merged_rows:
             # first col of row should be empty
             final_row = [None]
             for col in row:
                 final_row += [col] + ([None] * self.icon_padding)
             diagram_matrix.append(final_row)
@@ -335,15 +316,15 @@
 
     @classmethod
     def _parse_coupling_graph(cls, coupling_graph):
         """Returns a data structure representing the visual (ie diagram) of the graph
         {
             '<model instance or coupling id>' : {
                 '<component name>': {
-                    'type': '<component type e.g. load>',
+                    'type': '<component type, e.g., load>',
                     'edges': {
                         '<component port name>': [
                             ('<other model instance or coupling id>', '<other component name>', '<other component port>'), ...
                         ]
                     }
                 }, ...
             }, ...
@@ -360,16 +341,17 @@
 
         diagram_commands_by_id = defaultdict(list)
         for id_, template_files in template_files_by_id.items():
             for template_file in template_files:
                 try:
                     with open(template_file) as f:
                         diagram_commands_by_id[id_].extend(parse_diagram_commands(f.read()))
-                except Exception as e:
-                    raise Exception(f'Failed to parse diagram commands for {template_file}: {str(e)}')
+                except Exception as e:  # noqa: BLE001
+                    # TODO: Determine what error we are catching here
+                    raise Exception(f"Failed to parse diagram commands for {template_file}: {e!s}")
 
         return cls._diagram_commands_to_graph(diagram_commands_by_id, coupling_graph.couplings)
 
     @staticmethod
     def _diagram_commands_to_graph(diagram_commands_by_id, couplings):
         """Convert commands into a diagram graph.
 
@@ -398,46 +380,48 @@
                 # if our current context is a coupling, check the models we are coupling for the name
                 # if our current context isn't a coupling (ie a model), fail
                 #   (models should only connect to components within their own contexts)
                 coupling = [c for c in couplings if c.id == diagram_context_id]
                 if coupling:
                     coupling = coupling[0]
                 else:
-                    raise Exception(f'Invalid diagram line command: unable to find "{name}" in the context of {diagram_context_id}')
+                    raise Exception(
+                        f'Invalid diagram line command: unable to find "{name}" in the context of {diagram_context_id}'
+                    )
 
                 # search each of the coupling's models nodes for the element
                 model_a_id = coupling._model_a.id
                 found_in_model_a = model_a_id in diagram_graph_by_id and name in diagram_graph_by_id[model_a_id]
                 model_b_id = coupling._model_b.id
                 found_in_model_b = model_b_id in diagram_graph_by_id and name in diagram_graph_by_id[model_b_id]
 
                 if found_in_model_a and found_in_model_b:
                     raise Exception(
                         f'Invalid diagram line command: unable to determine which model "{name}" '
-                        'should connect to since it was not in the coupling and was found in both '
-                        'of the coupling\'s models'
+                        "should connect to since it was not in the coupling and was found in both "
+                        "of the coupling's models"
                     )
                 elif found_in_model_a:
                     return model_a_id
                 elif found_in_model_b:
                     return model_b_id
                 else:
                     available_names_by_context_id = {
-                        'coupling ' + diagram_context_id: list(diagram_graph_by_id[diagram_context_id].keys()),
+                        "coupling " + diagram_context_id: list(diagram_graph_by_id[diagram_context_id].keys()),
                         model_a_id: list(diagram_graph_by_id[model_a_id].keys()),
-                        model_b_id: list(diagram_graph_by_id[model_b_id].keys())
+                        model_b_id: list(diagram_graph_by_id[model_b_id].keys()),
                     }
-                    available_names_formatted = 'Available names (source):'
+                    available_names_formatted = "Available names (source):"
                     for ctx, available_names in available_names_by_context_id.items():
                         for available_name in available_names:
-                            available_names_formatted += f'\n  {available_name} ({ctx})'
+                            available_names_formatted += f"\n  {available_name} ({ctx})"
                     raise Exception(
                         f'Invalid diagram line command: failed to find "{name}" '
-                        f'in the coupling or either of the coupled models ({model_a_id} and {model_b_id}).\n'
-                        f'{available_names_formatted}'
+                        f"in the coupling or either of the coupled models ({model_a_id} and {model_b_id}).\n"
+                        f"{available_names_formatted}"
                     )
 
         # add connections between nodes
         for diagram_context_id, commands in diagram_commands_by_id.items():
             line_cmds = [cmd for cmd in commands if isinstance(cmd, DiagramLine)]
             for cmd in line_cmds:
                 a_name, a_port, b_name, b_port = cmd.a_name, cmd.a_port, cmd.b_name, cmd.b_port
@@ -454,26 +438,26 @@
         return diagram_graph_by_id
 
 
 class DiagramIcon(ABC):
     @property
     @abstractmethod
     def height(self):
-        """fraction of a diagram grid cell height (1 is full height, 0.5 is half, etc)"""
+        """Fraction of a diagram grid cell height (1 is full height, 0.5 is half, etc)"""
 
     @property
     @abstractmethod
     def width(self):
-        """fraction of a diagram grid cell width (1 is full width, 0.5 is half, etc)"""
+        """Fraction of a diagram grid cell width (1 is full width, 0.5 is half, etc)"""
 
     @staticmethod
     def get_icon(icon_type):
-        if icon_type == 'load':
+        if icon_type == "load":
             return LoadIcon()
-        elif icon_type == 'network':
+        elif icon_type == "network":
             return NetworkIcon()
         else:
             # use load icon as default for now
             return LoadIcon()
 
 
 class LoadIcon(DiagramIcon):
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/graph.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/graph.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 
 class CouplingGraph:
     """Manages coupling relationships"""
 
     def __init__(self, couplings):
         if len(couplings) == 0:
-            raise Exception('At least one coupling must be provided')
+            raise Exception("At least one coupling must be provided")
         self._couplings = couplings
 
         self._models_by_id = {}
         for coupling in self._couplings:
             a, b = coupling._model_a, coupling._model_b
             self._models_by_id[a.id] = a
             self._models_by_id[b.id] = b
@@ -35,22 +35,22 @@
         #   ...
         # }
         self._grouped_couplings_by_model_id = {}
         for model_id, couplings in self._couplings_by_model_id.items():
             grouped_couplings = defaultdict(list)
             for coupling in couplings:
                 other_model = coupling.get_other_model(self._models_by_id[model_id])
-                coupling_type = f'{other_model.simple_gmt_type}_couplings'
+                coupling_type = f"{other_model.simple_gmt_type}_couplings"
                 grouped_couplings[coupling_type].append(coupling)
 
             self._grouped_couplings_by_model_id[model_id] = grouped_couplings
 
     @property
     def couplings(self):
-        return [coupling for coupling in self._couplings]
+        return list(self._couplings)
 
     @property
     def models(self):
         return [model for _, model in self._models_by_id.items()]
 
     def couplings_by_type(self, model_id):
         """Returns the model's associated couplings keyed by the types of the
@@ -93,43 +93,43 @@
         Then this method would return 0, because it's at index 0
 
         :param model_a_id: str, id of model_a
         :param model_b_id: str, id of model_b
         :return: int
         """
         if model_a_id not in self._models_by_id:
-            raise Exception('Model A id was not found')
+            raise Exception("Model A id was not found")
         if model_b_id not in self._models_by_id:
-            raise Exception('Model B id was not found')
+            raise Exception("Model B id was not found")
 
         model_a, model_b = self._models_by_id[model_a_id], self._models_by_id[model_b_id]
         grouped_couplings = self._grouped_couplings_by_model_id[model_a.id]
-        coupling_type = f'{model_b.simple_gmt_type}_couplings'
+        coupling_type = f"{model_b.simple_gmt_type}_couplings"
         try:
             couplings = grouped_couplings[coupling_type]
             other_models = [coupling.get_other_model(model_a) for coupling in couplings]
             other_model_ids = [m.id for m in other_models]
             return other_model_ids.index(model_b.id)
         except KeyError:
-            raise Exception(f'model_a has no coupling with model_b\'s type ({model_b.simple_gmt_type})')
+            raise Exception(f"model_a has no coupling with model_b's type ({model_b.simple_gmt_type})")
         except ValueError:
-            raise Exception('model_a has no coupling with model_b')
+            raise Exception("model_a has no coupling with model_b")
 
     def get_coupled_load(self, ets_id):
         """Returns the load coupled to the provided ets
 
         :param ets_id: str
         :return: dict
         """
         if ets_id not in self._grouped_couplings_by_model_id:
-            raise Exception(f'No ETS with id {ets_id}')
+            raise Exception(f"No ETS with id {ets_id}")
         try:
-            load_couplings = self._grouped_couplings_by_model_id[ets_id]['load_couplings']
-            return load_couplings[0].to_dict()['load']
+            load_couplings = self._grouped_couplings_by_model_id[ets_id]["load_couplings"]
+            return load_couplings[0].to_dict()["load"]
         except (KeyError, IndexError):
-            raise Exception('ETS is not coupled to a load')
+            raise Exception("ETS is not coupled to a load")
 
     def get_coupling(self, coupling_id):
         for coupling in self._couplings:
             if coupling.id == coupling_id:
                 return coupling
         raise Exception(f'No coupling found with id "{coupling_id}"')
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_CoolingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Network2Pipe_HeatingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkChilledWaterStub_CoolingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/NetworkHeatedWaterStub_HeatingPlant/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Spawn_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/Teaser_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeriesMFT_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_CoolingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsColdWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_EtsHotWaterStub/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ComponentDefinitions.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/templates/TimeSeries_HeatingIndirect/ConnectStatements.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/couplings/utils.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/couplings/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import re
 from collections import deque, namedtuple
 
-DiagramTransformation = namedtuple('DiagramTransformation', ['model_name', 'model_type'])
-DiagramLine = namedtuple('DiagramLine', ['a_name', 'a_port', 'b_name', 'b_port'])
+DiagramTransformation = namedtuple("DiagramTransformation", ["model_name", "model_type"])
+DiagramLine = namedtuple("DiagramLine", ["a_name", "a_port", "b_name", "b_port"])
 
-JINJA_EXPRESSION_REGEX = re.compile(r'{{\s*(.*?)\s*}}')
+JINJA_EXPRESSION_REGEX = re.compile(r"{{\s*(.*?)\s*}}")
 
 
 def parse_diagram_command(str_cmd):
     """Returns a diagram command or None if it's not a diagram command"""
-    cmd_args_list = str_cmd.split('.')
+    cmd_args_list = str_cmd.split(".")
     if len(cmd_args_list) <= 1:
         return None
 
     context = cmd_args_list.pop(0)
-    if context != 'diagram':
+    if context != "diagram":
         return None
 
     command = cmd_args_list.pop(0)
-    if command == 'transformation':
+    if command == "transformation":
         if len(cmd_args_list) != 2:
-            raise Exception(f'Invalid diagram templating command: "transformation" expects 2 arguments but got {cmd_args_list}')
+            raise TypeError(
+                f'Invalid diagram templating command: "transformation" expects 2 arguments but got {cmd_args_list}'
+            )
         return DiagramTransformation(*cmd_args_list)
-    elif command == 'line':
+    elif command == "line":
         if len(cmd_args_list) != 4:
-            raise Exception(f'Invalid diagram templating command: "line" expects 4 arguments but got {cmd_args_list}')
+            raise TypeError(f'Invalid diagram templating command: "line" expects 4 arguments but got {cmd_args_list}')
         return DiagramLine(*cmd_args_list)
     else:
-        raise Exception(f'Invalid diagram templating command "{command}"')
+        raise TypeError(f'Invalid diagram templating command "{command}"')
 
 
 def parse_diagram_commands(template_contents):
     """Returns a list of diagram commands parsed from the template modelica contents
     i.e. it will find any instances of {{ diagram.<cmd>.* }} in the template
 
     :param template_contents: str, modelica template code
@@ -99,11 +101,11 @@
             return path
         if current in visited:
             continue
 
         visited.append(current)
 
         for neighbor in get_neighbors(current):
-            queue.append((path + [neighbor], neighbor))
+            queue.append(([*path, neighbor], neighbor))
 
     # failed to find a path
-    raise Exception(f'Failed to find path from {start} to {finish}')
+    raise Exception(f"Failed to find path from {start} to {finish}")
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/districts/templates/DistrictEnergySystem5G.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import (
-    EnergyTransferBase
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import EnergyTransferBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
-class CoolingIndirect(EnergyTransferBase):
-    model_name = 'CoolingIndirect'
+class HeatingIndirect(EnergyTransferBase):
+    model_name = "HeatingIndirect"
 
     def __init__(self, system_parameters, geojson_load_id):
         super().__init__(system_parameters, geojson_load_id)
-        self.id = 'cooInd_' + simple_uuid()
+        self.id = "heaInd_" + simple_uuid()
         # _model_filename is the name of the file we generate, and thus the actual
         # model to be referenced when instantiating in the District model
         # TODO: refactor these property names (model_name and model_filename) because
         # it's confusing
-        self._model_filename = f'CoolingIndirect_{self._geojson_load_id}'
+        self._model_filename = f"HeatingIndirect_{self._geojson_load_id}"
 
     def to_modelica(self, scaffold):
-        """
-        Create indirect cooling models based on the data in the buildings and geojsons
+        """Create indirect heating models based on the data in the buildings and geojsons
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
-        cooling_indirect_template = self.template_env.get_template("CoolingIndirect.mot")
+        heating_indirect_template = self.template_env.get_template("HeatingIndirect.mot")
 
-        ets_data = self.system_parameters.get_param_by_building_id(
-            self._geojson_load_id,
-            'ets_indirect_parameters'
-        )
+        ets_data = self.system_parameters.get_param_by_id(self._geojson_load_id, "ets_indirect_parameters")
 
         combined_template_data = {**ets_data, **self.district_template_data}
 
         self.run_template(
-            template=cooling_indirect_template,
-            save_file_name=os.path.join(scaffold.project_path, 'Substations', f'{self._model_filename}.mo'),
+            template=heating_indirect_template,
+            save_file_name=os.path.join(scaffold.project_path, "Substations", f"{self._model_filename}.mo"),
             project_name=scaffold.project_name,
             model_filename=self._model_filename,
             ets_data=combined_template_data,
         )
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         package = PackageParser(scaffold.project_path)
-        if 'Substations' not in package.order:
-            package.add_model('Substations')
+        if "Substations" not in package.order:
+            package.add_model("Substations")
             package.save()
 
         package_models = [self._model_filename]
         ets_package = PackageParser(scaffold.substations_path.files_dir)
         if ets_package.order_data is None:
             ets_package = PackageParser.new_from_template(
                 path=scaffold.substations_path.files_dir,
                 name="Substations",
                 order=package_models,
-                within=scaffold.project_name)
+                within=scaffold.project_name,
+            )
         else:
             for model_name in package_models:
                 if model_name not in ets_package.order:
                     ets_package.add_model(model_name)
         ets_package.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Substations.{self._model_filename}'
+        return f"Substations.{self._model_filename}"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/energy_transfer_base.py`

 * *Files 18% similar despite different names*

```diff
@@ -3,17 +3,16 @@
 
 from pathlib import Path
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 
 
 class EnergyTransferBase(ModelBase):
-    """
-    Base class of the energy transfer connectors.
-    """
-    simple_gmt_type = 'ets'
+    """Base class of the energy transfer connectors."""
+
+    simple_gmt_type = "ets"
 
     def __init__(self, system_parameters, geojson_load_id):
-        super().__init__(system_parameters, Path(__file__).parent / 'templates')
+        super().__init__(system_parameters, Path(__file__).parent / "templates")
 
         # geojson load id is used for fetching load-specific ETS configs from sys params
         self._geojson_load_id = geojson_load_id
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_cold_water_stub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import (
-    EnergyTransferBase
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import EnergyTransferBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
 class EtsColdWaterStub(EnergyTransferBase):
-    model_name = 'EtsColdWaterStub'
+    model_name = "EtsColdWaterStub"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters, None)
-        self.id = 'etsColWatStub_' + simple_uuid()
+        self.id = "etsColWatStub_" + simple_uuid()
 
     def to_modelica(self, scaffold):
-        """
-        Create cooling water stub models
+        """Create cooling water stub models
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         # this stub does not have any modelica files to generate as it's not its own model
         # It's contained within the coupling files
 
     def get_modelica_type(self, scaffold):
         # this stub does not have a type as it's not packaged into its own model currently
-        return 'UNIMPLEMENTED'
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/ets_hot_water_stub.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import (
-    EnergyTransferBase
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import EnergyTransferBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
 class EtsHotWaterStub(EnergyTransferBase):
-    model_name = 'EtsHotWaterStub'
+    model_name = "EtsHotWaterStub"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters, None)
-        self.id = 'etsHotWatStub_' + simple_uuid()
+        self.id = "etsHotWatStub_" + simple_uuid()
 
     def to_modelica(self, scaffold):
-        """
-        Create indirect cooling models based on the data in the buildings and geojsons
+        """Create indirect cooling models based on the data in the buildings and geojsons
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         # this stub does not have any modelica files to generate as it's not its own model
         # It's contained within the coupling files
 
     def get_modelica_type(self, scaffold):
         # this stub does not have a type as it's not packaged into its own model currently
-        return 'UNIMPLEMENTED'
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/heating_indirect.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/cooling_indirect.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,66 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import (
-    EnergyTransferBase
-)
+from geojson_modelica_translator.model_connectors.energy_transfer_systems.energy_transfer_base import EnergyTransferBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
-class HeatingIndirect(EnergyTransferBase):
-    model_name = 'HeatingIndirect'
+class CoolingIndirect(EnergyTransferBase):
+    model_name = "CoolingIndirect"
 
     def __init__(self, system_parameters, geojson_load_id):
         super().__init__(system_parameters, geojson_load_id)
-        self.id = 'heaInd_' + simple_uuid()
+        self.id = "cooInd_" + simple_uuid()
         # _model_filename is the name of the file we generate, and thus the actual
         # model to be referenced when instantiating in the District model
         # TODO: refactor these property names (model_name and model_filename) because
         # it's confusing
-        self._model_filename = f'HeatingIndirect_{self._geojson_load_id}'
+        self._model_filename = f"CoolingIndirect_{self._geojson_load_id}"
 
     def to_modelica(self, scaffold):
-        """
-        Create indirect heating models based on the data in the buildings and geojsons
+        """Create indirect cooling models based on the data in the buildings and geojsons
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
-        heating_indirect_template = self.template_env.get_template("HeatingIndirect.mot")
+        cooling_indirect_template = self.template_env.get_template("CoolingIndirect.mot")
 
-        ets_data = self.system_parameters.get_param_by_building_id(
-            self._geojson_load_id,
-            "ets_indirect_parameters"
-        )
+        ets_data = self.system_parameters.get_param_by_id(self._geojson_load_id, "ets_indirect_parameters")
 
         combined_template_data = {**ets_data, **self.district_template_data}
 
         self.run_template(
-            template=heating_indirect_template,
-            save_file_name=os.path.join(scaffold.project_path, 'Substations', f'{self._model_filename}.mo'),
+            template=cooling_indirect_template,
+            save_file_name=os.path.join(scaffold.project_path, "Substations", f"{self._model_filename}.mo"),
             project_name=scaffold.project_name,
             model_filename=self._model_filename,
             ets_data=combined_template_data,
         )
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         package = PackageParser(scaffold.project_path)
-        if 'Substations' not in package.order:
-            package.add_model('Substations')
+        if "Substations" not in package.order:
+            package.add_model("Substations")
             package.save()
 
         package_models = [self._model_filename]
         ets_package = PackageParser(scaffold.substations_path.files_dir)
         if ets_package.order_data is None:
             ets_package = PackageParser.new_from_template(
                 path=scaffold.substations_path.files_dir,
                 name="Substations",
                 order=package_models,
-                within=scaffold.project_name)
+                within=scaffold.project_name,
+            )
         else:
             for model_name in package_models:
                 if model_name not in ets_package.order:
                     ets_package.add_model(model_name)
         ets_package.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Substations.{self._model_filename}'
+        return f"Substations.{self._model_filename}"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/CoolingIndirect_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsColdWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/EtsHotWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/energy_transfer_systems/templates/HeatingIndirect_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/load_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/load_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,169 +4,179 @@
 from pathlib import Path
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 from geojson_modelica_translator.utils import convert_c_to_k
 
 
 class LoadBase(ModelBase):
-    """
-    Base class of the load connectors.
-    """
-    simple_gmt_type = 'load'
+    """Base class of the load connectors."""
+
+    simple_gmt_type = "load"
 
     def __init__(self, system_parameters, geojson_load):
-        """
-        Base class for load connectors.
+        """Base class for load connectors.
 
         :param system_parameters: SystemParameter object, the entire system parameter file which will be used to
                                   generate this load.
         :param geojson_load: dict, the GeoJSON portion of the load to be added (a single feature).
-                             This is now a required field.
         """
-        super().__init__(system_parameters, Path(__file__).parent / 'templates')
+        super().__init__(system_parameters, Path(__file__).parent / "templates")
 
         # previously geojson_load could be None, prevent that now.
         if geojson_load is None:
-            raise SystemExit('Error initializing LoadBase with empty GeoJSON')
+            raise SystemExit("Error initializing LoadBase with empty GeoJSON")
 
         # we have to resolve some naming/object issues, there is a GeoJSON load, an URBANopt Building, and then the
         # building object. Ideally we have only one, but we need to investigate that. The UOBuilding allows for
         # access such as building.feature.properties.
         self.building_id = geojson_load.feature.properties["id"]
         self.building = self.add_building(geojson_load)
 
         # This ets_template_data gets added to building_template_data when the template is run
         # First if statement is for cases of no sys-param file provided
         # Second if statement is for cases of a sys-param file not including ets data
         # TODO: Decide if we're requiring sys-param file, and if all loads have an ets.
         # test_base.py and test_time_series.py test these cases
-        if system_parameters is not None:
-            if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "ets_indirect_parameters") is not None:
-                self.ets_template_data = {
-                    "heat_flow_nominal": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heat_flow_nominal"
-                    ),
-                    "heat_exchanger_efficiency": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heat_exchanger_efficiency"
-                    ),
-                    "nominal_mass_flow_district": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.nominal_mass_flow_district"
-                    ),
-                    "nominal_mass_flow_building": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.nominal_mass_flow_building"
-                    ),
-                    "valve_pressure_drop": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.valve_pressure_drop"
-                    ),
-                    "heat_exchanger_secondary_pressure_drop": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heat_exchanger_secondary_pressure_drop"
-                    ),
-                    "heat_exchanger_primary_pressure_drop": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heat_exchanger_primary_pressure_drop"
-                    ),
-                    "cooling_supply_water_temperature_building": convert_c_to_k(self.system_parameters.get_param_by_building_id(
+        if (
+            system_parameters is not None
+            and self.system_parameters.get_param_by_id(self.building_id, "ets_indirect_parameters") is not None
+        ):
+            self.ets_template_data = {
+                "heat_flow_nominal": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heat_flow_nominal"
+                ),
+                "heat_exchanger_efficiency": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heat_exchanger_efficiency"
+                ),
+                "nominal_mass_flow_district": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.nominal_mass_flow_district"
+                ),
+                "nominal_mass_flow_building": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.nominal_mass_flow_building"
+                ),
+                "valve_pressure_drop": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.valve_pressure_drop"
+                ),
+                "heat_exchanger_secondary_pressure_drop": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heat_exchanger_secondary_pressure_drop"
+                ),
+                "heat_exchanger_primary_pressure_drop": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heat_exchanger_primary_pressure_drop"
+                ),
+                "cooling_supply_water_temperature_building": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
                         self.building_id, "ets_indirect_parameters.cooling_supply_water_temperature_building"
-                    )),
-                    "heating_supply_water_temperature_building": convert_c_to_k(self.system_parameters.get_param_by_building_id(
+                    )
+                ),
+                "heating_supply_water_temperature_building": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
                         self.building_id, "ets_indirect_parameters.heating_supply_water_temperature_building"
-                    )),
-                    "delta_temp_chw_building": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.delta_temp_chw_building"
-                    ),
-                    "delta_temp_chw_district": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.delta_temp_chw_district"
-                    ),
-                    "delta_temp_hw_building": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.delta_temp_hw_building"
-                    ),
-                    "delta_temp_hw_district": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.delta_temp_hw_district"
-                    ),
-                    "cooling_controller_y_max": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.cooling_controller_y_max"
-                    ),
-                    "cooling_controller_y_min": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.cooling_controller_y_min"
-                    ),
-                    "heating_controller_y_max": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heating_controller_y_max"
-                    ),
-                    "heating_controller_y_min": self.system_parameters.get_param_by_building_id(
-                        self.building_id, "ets_indirect_parameters.heating_controller_y_min"
                     )
-                }
+                ),
+                "delta_temp_chw_building": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.delta_temp_chw_building"
+                ),
+                "delta_temp_chw_district": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.delta_temp_chw_district"
+                ),
+                "delta_temp_hw_building": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.delta_temp_hw_building"
+                ),
+                "delta_temp_hw_district": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.delta_temp_hw_district"
+                ),
+                "cooling_controller_y_max": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.cooling_controller_y_max"
+                ),
+                "cooling_controller_y_min": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.cooling_controller_y_min"
+                ),
+                "heating_controller_y_max": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heating_controller_y_max"
+                ),
+                "heating_controller_y_min": self.system_parameters.get_param_by_id(
+                    self.building_id, "ets_indirect_parameters.heating_controller_y_min"
+                ),
+            }
 
     def add_building(self, urbanopt_building, mapper=None):
-        """
-        Add building to the load to be translated. This is simply a helper method.
+        """Add building to the load to be translated. This is simply a helper method.
 
         :param urbanopt_building: an urbanopt_building (also known as a geojson_load)
         :param mapper: placeholder object for mapping between urbanopt_building and load_connector building.
         """
 
         # TODO: Need to convert units, these should exist on the urbanopt_building object
         # TODO: Abstract out the GeoJSON functionality
         if mapper is None:
             if self.system_parameters:
-                for building in self.system_parameters.get_default('$.buildings', []):
+                for building in self.system_parameters.get_default("$.buildings", []):
                     # Only look at buildings in the sys-param file, not necessarily the entire feature file
                     if urbanopt_building.feature.properties["id"] == building["geojson_id"]:
                         try:
                             self.building_id = urbanopt_building.feature.properties["id"]
                             building_type = urbanopt_building.feature.properties["building_type"]
                             number_stories = urbanopt_building.feature.properties["number_of_stories"]
                         except KeyError as ke:
-                            raise SystemExit(f'\nMissing property {ke} for building {self.building_id} in geojson feature file')
+                            raise SystemExit(
+                                f"\nMissing property {ke} for building {self.building_id} in geojson feature file"
+                            )
 
                         try:
                             building_floor_area_m2 = self.ft2_to_m2(urbanopt_building.feature.properties["floor_area"])
                         except KeyError:
                             building_floor_area_m2 = 0
 
                         try:
-                            number_stories_above_ground = urbanopt_building.feature.properties["number_of_stories_above_ground"]
+                            number_stories_above_ground = urbanopt_building.feature.properties[
+                                "number_of_stories_above_ground"
+                            ]
                         except KeyError:
                             number_stories_above_ground = number_stories
-                            print(f"\nAssuming all building levels are above ground for building_id: {self.building_id}")
+                            print(
+                                f"\nAssuming all building levels are above ground for building_id: {self.building_id}"
+                            )
 
                         try:
                             floor_height = urbanopt_building.feature.properties["floor_height"]
                         except KeyError:
                             floor_height = 3  # Default height in meters from sdk
                             print(
                                 f"No floor_height found in geojson feature file for building {self.building_id}. "
-                                f"Using default value of {floor_height}.")
+                                f"Using default value of {floor_height}."
+                            )
 
                         # UO SDK defaults to current year, however TEASER only supports up to Year 2015
                         # https://github.com/urbanopt/TEASER/blob/master/teaser/data/input/inputdata/TypeBuildingElements.json#L818
                         try:
                             year_built = urbanopt_building.feature.properties["year_built"]
                             if urbanopt_building.feature.properties["year_built"] > 2015:
                                 year_built = 2015
                         except KeyError:
                             year_built = 2015
                             print(
                                 f"No year_built found in geojson feature file for building {self.building_id}. "
-                                f"Using default value of {year_built}.")
+                                f"Using default value of {year_built}."
+                            )
 
                         try:
                             return {
                                 "building_id": self.building_id,
                                 "area": building_floor_area_m2,
                                 "building_type": building_type,
                                 "floor_height": floor_height,
                                 "num_stories": number_stories,
                                 "num_stories_below_grade": number_stories - number_stories_above_ground,
                                 "year_built": year_built,
                             }
                         except UnboundLocalError:
                             print(
                                 f"Geojson feature file is missing data for building {self.building_id}. "
-                                "This may be caused by referencing a detailed osm in the feature file.")
+                                "This may be caused by referencing a detailed osm in the feature file."
+                            )
                     else:
                         continue
 
         else:
             raise SystemExit(f"Mapper {mapper} has been used")
 
     @property
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/spawn.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/spawn.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,101 +2,117 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
 import shutil
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
-    LoadBase
-)
-from geojson_modelica_translator.utils import (
-    ModelicaPath,
-    convert_c_to_k,
-    simple_uuid
-)
+from geojson_modelica_translator.model_connectors.load_connectors.load_base import LoadBase
+from geojson_modelica_translator.utils import ModelicaPath, convert_c_to_k, simple_uuid
 
 
 class Spawn(LoadBase):
-    model_name = 'Spawn'
+    model_name = "Spawn"
 
     def __init__(self, system_parameters, geojson_load):
         super().__init__(system_parameters, geojson_load)
-        self.id = 'SpawnLoad_' + simple_uuid()
+        self.id = "SpawnLoad_" + simple_uuid()
 
     def to_modelica(self, scaffold, keep_original_models=False):
-        """
-        Create spawn models based on the data in the buildings and geojsons
+        """Create spawn models based on the data in the buildings and geojsons
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         spawn_coupling_template = self.template_env.get_template("SpawnCouplingBuilding.mot")
         spawn_building_template = self.template_env.get_template("SpawnBuilding.mot")
         spawn_mos_template = self.template_env.get_template("RunSpawnCouplingBuilding.most")
 
         # create spawn building and save to the correct directory
         print(f"Creating spawn for building: {self.building_id}")
 
         # Path for building data
-        b_modelica_path = ModelicaPath(
-            self.building_name, scaffold.loads_path.files_dir, True
-        )
+        b_modelica_path = ModelicaPath(self.building_name, scaffold.loads_path.files_dir, True)
 
         mos_weather_filename = self.system_parameters.get_param("$.weather")
-        epw_filename = os.path.splitext(mos_weather_filename)[0] + '.epw'
+        epw_filename = os.path.splitext(mos_weather_filename)[0] + ".epw"
         # This assumes the epw and mos files are named the same and in the same directory.
         # If coming from the SDK, this is a safe assumption.
 
         # grab the data from the system_parameter file for this building id
         # TODO: create method in system_parameter class to make this easier
 
-        idf_filename = self.system_parameters.get_param_by_building_id(
+        idf_filename = self.system_parameters.get_param_by_id(
             self.building_id, "load_model_parameters.spawn.idf_filename"
         )
-        thermal_zones = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.thermal_zone_names",
-        )
-        zone_nom_htg_loads = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.zone_nom_htg_loads",
-        )
-        zone_nom_clg_loads = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.zone_nom_clg_loads",
+        thermal_zones = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.thermal_zone_names",
+        )
+        zone_nom_htg_loads = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.zone_nom_htg_loads",
+        )
+        zone_nom_clg_loads = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.zone_nom_clg_loads",
         )
         # TODO: pick up default value from schema if not specified in system_parameters,
         # to avoid the inline if/then statement in nominal_values below
-        has_liquid_heating = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.has_liquid_heating",
+        has_liquid_heating = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.has_liquid_heating",
+        )
+        has_liquid_cooling = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.has_liquid_cooling",
+        )
+        has_electric_heating = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.has_electric_heating",
+        )
+        has_electric_cooling = self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.spawn.has_electric_cooling",
+        )
+        hhw_supply_temp = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_hw_supply",
+            )
+        )
+        hhw_return_temp = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_hw_return",
+            )
+        )
+        chw_supply_temp = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_chw_supply",
+            )
+        )
+        chw_return_temp = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_chw_return",
+            )
         )
-        has_liquid_cooling = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.has_liquid_cooling",
+        temp_setpoint_cooling = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_setpoint_cooling",
+            )
         )
-        has_electric_heating = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.has_electric_heating",
+        temp_setpoint_heating = convert_c_to_k(
+            self.system_parameters.get_param_by_id(
+                self.building_id,
+                "load_model_parameters.spawn.temp_setpoint_heating",
+            )
         )
-        has_electric_cooling = self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.has_electric_cooling",
-        )
-        hhw_supply_temp = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_hw_supply",
-        ))
-        hhw_return_temp = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_hw_return",
-        ))
-        chw_supply_temp = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_chw_supply",
-        ))
-        chw_return_temp = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_chw_return",
-        ))
-        temp_setpoint_cooling = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_setpoint_cooling",
-        ))
-        temp_setpoint_heating = convert_c_to_k(self.system_parameters.get_param_by_building_id(
-            self.building_id, "load_model_parameters.spawn.temp_setpoint_heating",
-        ))
 
         # construct the dict to pass into the template
         building_template_data = {
             "load_resources_path": b_modelica_path.resources_relative_dir,
             "idf": {
                 "idf_filename": idf_filename,
                 "filename": os.path.basename(idf_filename),
@@ -123,95 +139,97 @@
                 "temp_setpoint_cooling": temp_setpoint_cooling,
                 "has_liquid_heating": "true" if has_liquid_heating else "false",
                 "has_liquid_cooling": "true" if has_liquid_cooling else "false",
                 "has_electric_heating": "true" if has_electric_heating else "false",
                 "has_electric_cooling": "true" if has_electric_cooling else "false",
             },
             # Reformatting lists for Modelica
-            "zone_nom_htg_loads": str(repr(zone_nom_htg_loads)).replace("[", "{").replace("]", "}").split("rray(", 1)[-1],
-            "zone_nom_clg_loads": str(repr(zone_nom_clg_loads)).replace("[", "{").replace("]", "}").split("rray(", 1)[-1],
+            "zone_nom_htg_loads": str(repr(zone_nom_htg_loads))
+            .replace("[", "{")
+            .replace("]", "}")
+            .split("rray(", 1)[-1],
+            "zone_nom_clg_loads": str(repr(zone_nom_clg_loads))
+            .replace("[", "{")
+            .replace("]", "}")
+            .split("rray(", 1)[-1],
         }
         for tz in thermal_zones:
             # TODO: method for creating nice zone names for modelica
-            building_template_data["thermal_zones"].append(
-                {"modelica_object_name": f"zn{tz}", "spawn_object_name": tz}
-            )
+            building_template_data["thermal_zones"].append({"modelica_object_name": f"zn{tz}", "spawn_object_name": tz})
 
         # copy over the resource files for this building
         # TODO: move some of this over to a validation step
         if os.path.exists(building_template_data["idf"]["idf_filename"]):
             shutil.copy(
                 building_template_data["idf"]["idf_filename"],
                 os.path.join(
                     b_modelica_path.resources_dir,
                     building_template_data["idf"]["filename"],
                 ),
             )
         else:
-            raise Exception(
-                f"Missing IDF file for Spawn: {building_template_data['idf']['idf_filename']}"
-            )
+            raise Exception(f"Missing IDF file for Spawn: {building_template_data['idf']['idf_filename']}")
 
         if os.path.exists(building_template_data["epw"]["epw_filename"]):
-            shutil.copy(building_template_data["epw"]["epw_filename"],
-                        os.path.join(b_modelica_path.resources_dir, building_template_data["epw"]["filename"]))
+            shutil.copy(
+                building_template_data["epw"]["epw_filename"],
+                os.path.join(b_modelica_path.resources_dir, building_template_data["epw"]["filename"]),
+            )
         else:
             raise Exception(f"Missing EPW file for Spawn: {building_template_data['epw']['epw_filename']}")
 
         if os.path.exists(building_template_data["mos_weather"]["mos_weather_filename"]):
             shutil.copy(
                 building_template_data["mos_weather"]["mos_weather_filename"],
-                os.path.join(b_modelica_path.resources_dir, building_template_data["mos_weather"]["filename"])
+                os.path.join(b_modelica_path.resources_dir, building_template_data["mos_weather"]["filename"]),
             )
         else:
             raise Exception(
-                f"Missing MOS weather file for Spawn: {building_template_data['mos_weather']['mos_weather_filename']}")
+                f"Missing MOS weather file for Spawn: {building_template_data['mos_weather']['mos_weather_filename']}"
+            )
         # merge ets template values from load_base.py into the building nominal values
         # If there is no ets defined in sys-param file, use the building template data alone
         try:
-            nominal_values = {**building_template_data['nominal_values'], **self.ets_template_data}
+            nominal_values = {**building_template_data["nominal_values"], **self.ets_template_data}
             combined_template_data = {**building_template_data, **nominal_values}
         except AttributeError:
             combined_template_data = building_template_data
 
         self.run_template(
             spawn_building_template,
             os.path.join(b_modelica_path.files_dir, "building.mo"),
             project_name=scaffold.project_name,
             model_name=self.building_name,
-            data=combined_template_data
+            data=combined_template_data,
         )
 
         full_model_name = os.path.join(
-            scaffold.project_name,
-            scaffold.loads_path.files_relative_dir,
-            self.building_name,
-            "coupling").replace(os.path.sep, '.')
+            scaffold.project_name, scaffold.loads_path.files_relative_dir, self.building_name, "coupling"
+        ).replace(os.path.sep, ".")
 
         file_data = spawn_mos_template.render(full_model_name=full_model_name, model_name=self.model_name)
         with open(os.path.join(b_modelica_path.scripts_dir, "RunSpawnCouplingBuilding.mos"), "w") as f:
             f.write(file_data)
 
         self.run_template(
             spawn_coupling_template,
             os.path.join(b_modelica_path.files_dir, "coupling.mo"),
             project_name=scaffold.project_name,
             model_name=self.building_name,
-            data=combined_template_data
+            data=combined_template_data,
         )
 
         # Copy the required modelica files
-        self.copy_required_mo_files(b_modelica_path.files_dir, within=f'{scaffold.project_name}.Loads')
+        self.copy_required_mo_files(b_modelica_path.files_dir, within=f"{scaffold.project_name}.Loads")
 
         # run post process to create the remaining project files for this building
         self.post_process(scaffold, keep_original_models=keep_original_models)
 
     def post_process(self, scaffold, keep_original_models=False):
-        """
-        Cleanup the export of Spawn files into a format suitable for the district-based analysis. This includes
+        """Cleanup the export of Spawn files into a format suitable for the district-based analysis. This includes
         the following:
 
             * Add a Loads project
             * Add a project level project
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         :param keep_original_models: boolean, # TODO
@@ -220,26 +238,26 @@
         b_modelica_path = os.path.join(scaffold.loads_path.files_dir, self.building_name)
         new_package = PackageParser.new_from_template(
             b_modelica_path, self.building_name, ["building", "coupling"], within=f"{scaffold.project_name}.Loads"
         )
         new_package.save()
 
         # now create the Loads level package and package.order.
-        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, 'package.mo')):
+        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, "package.mo")):
             load_package = PackageParser.new_from_template(
                 scaffold.loads_path.files_dir, "Loads", [self.building_name], within=f"{scaffold.project_name}"
             )
             load_package.save()
         else:
             load_package = PackageParser(os.path.join(scaffold.loads_path.files_dir))
             load_package.add_model(self.building_name)
             load_package.save()
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         package = PackageParser(scaffold.project_path)
-        if 'Loads' not in package.order:
-            package.add_model('Loads')
+        if "Loads" not in package.order:
+            package.add_model("Loads")
             package.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Loads.{self.building_name}.building'
+        return f"Loads.{self.building_name}.building"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/teaser.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/teaser.py`

 * *Files 5% similar despite different names*

```diff
@@ -9,42 +9,37 @@
 from tempfile import mkstemp
 
 import numpy as np
 from modelica_builder.model import Model
 from modelica_builder.package_parser import PackageParser
 from teaser.project import Project
 
-from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
-    LoadBase
-)
-from geojson_modelica_translator.utils import (
-    ModelicaPath,
-    convert_c_to_k,
-    copytree,
-    simple_uuid
-)
+from geojson_modelica_translator.model_connectors.load_connectors.load_base import LoadBase
+from geojson_modelica_translator.utils import ModelicaPath, convert_c_to_k, copytree, simple_uuid
 
 
 class Teaser(LoadBase):
     """TEASER is different than the other model connectors since TEASER creates all of the building models with
     multiple thermal zones when running, at which point each building then needs to be processed."""
-    model_name = 'Teaser'
+
+    model_name = "Teaser"
 
     def __init__(self, system_parameters, geojson_load):
         super().__init__(system_parameters, geojson_load)
-        self.id = 'TeaserLoad_' + simple_uuid()
+        self.id = "TeaserLoad_" + simple_uuid()
 
     def lookup_building_type(self, building_type):
         """Look up the building type from the Enumerations in the building_properties.json schema. TEASER
         documentation on building types is here (look into the python files):
 
         https://github.com/RWTH-EBC/TEASER/tree/development/teaser/logic/archetypebuildings/bmvbs
         """
 
-        # Also look at using JSON as the input: https://github.com/RWTH-EBC/TEASER/blob/master/teaser/examples/examplefiles/ASHRAE140_600.json  # noqa
+        # Also look at using JSON as the input:
+        # https://github.com/RWTH-EBC/TEASER/blob/master/teaser/examples/examplefiles/ASHRAE140_600.json
         mapping = {
             # Single Family is not configured right now.
             "Single-Family": "SingleFamilyDwelling",
             "Office": "office",
             "Laboratory": "institute8",
             "Education": "institute",
             "Inpatient health care": "institute8",
@@ -68,22 +63,21 @@
         #         "Refrigerated warehouse",
         #         "Religious worship",
         #         "Public assembly",
         #         "Lodging",
         #         "Mixed use",
         #         "Uncovered Parking",
         #         "Covered Parking"
-        if building_type in mapping.keys():
+        if building_type in mapping:
             return mapping[building_type]
         else:
             raise Exception(f"Building type of {building_type} not defined in GeoJSON to TEASER mappings")
 
     def to_modelica(self, scaffold, keep_original_models=False):
-        """
-        Save the TEASER representation of a sinlge building to the filesystem. The path will
+        """Save the TEASER representation of a sinlge building to the filesystem. The path will
         be scaffold.loads_path.files_dir.
 
         :param scaffold: Scaffold object, contains all the paths of the project
         :param keep_original_models: boolean, whether or not to remove the models after exporting from Teaser
         """
         # Teaser changes the current dir, so make sure to reset it back to where we started
         curdir = os.getcwd()
@@ -100,15 +94,15 @@
                 office_layout=1,
                 window_layout=1,
                 with_ahu=False,
                 construction_type="heavy",
             )
 
             prj.used_library_calc = "IBPSA"
-            prj.number_of_elements_calc = self.system_parameters.get_param_by_building_id(
+            prj.number_of_elements_calc = self.system_parameters.get_param_by_id(
                 self.building_id, "load_model_parameters.rc.order"
             )
             prj.merge_windows_calc = False
 
             # calculate the properties of all the buildings (just one in this case)
             # and export to the Buildings library
             prj.calc_all_buildings()
@@ -124,23 +118,22 @@
             * makes the dimension of the matrix to 8761,4
             * adds in a timestep for t=0
 
         :param f: string, fully qualified path to file
         :return: None
         """
         fh, abs_path = mkstemp()  # make a temp file
-        with fdopen(fh, 'w') as new_file:
-            with open(f) as old_file:
-                for line in old_file:
-                    if "double Internals(8760" in line:  # Finding the line, which may have one of several #s of columns
-                        new_file.write("double Internals(8761, 4)\n")
-                    elif line.startswith("3600\t"):
-                        new_file.write(line.replace('3600\t', '0\t') + line)
-                    else:
-                        new_file.write(line)
+        with fdopen(fh, "w") as new_file, open(f) as old_file:
+            for line in old_file:
+                if "double Internals(8760" in line:  # Finding the line, which may have one of several #s of columns
+                    new_file.write("double Internals(8761, 4)\n")
+                elif line.startswith("3600\t"):
+                    new_file.write(line.replace("3600\t", "0\t") + line)
+                else:
+                    new_file.write(line)
         copymode(f, abs_path)  # copies permissions
         remove(f)
         move(abs_path, f)
 
     def post_process(self, scaffold, keep_original_models=False):
         """Cleanup the export of the TEASER files into a format suitable for the district-based analysis.
         This includes the following:
@@ -191,262 +184,272 @@
             new_file_name = os.path.basename(f).replace(self.building_name, "")
             os.rename(f, f"{b_modelica_path.resources_dir}/{new_file_name}")
 
             # The main branch of teaser has yet to merge in the changes to support the fixes to the
             # internal gain files. The next method can be removed once the TEASER development branch is
             # merged into master/main and released.
             self.fix_gains_file(f"{b_modelica_path.resources_dir}/{new_file_name}")
-            self.internal_gains_file = f"{scaffold.project_name}/Loads/{b_modelica_path.resources_relative_dir}/{new_file_name}"
+            self.internal_gains_file = (
+                f"{scaffold.project_name}/Loads/{b_modelica_path.resources_relative_dir}/{new_file_name}"
+            )
 
         # process each of the thermal zones
         thermal_zone_files = []
         mo_files = glob.glob(os.path.join(scaffold.loads_path.files_dir, f"{self.building_name}/*.mo"))
         for f in mo_files:
             # ignore the package.mo file
             if os.path.basename(f) in ["package.mo"]:
                 continue
 
             mofile = Model(f)
 
             # previous paths and replace with the new one.
             # Make sure to update the names of any resources as well.
-            mofile.set_within_statement(f'{scaffold.project_name}.Loads.{self.building_name}')
+            mofile.set_within_statement(f"{scaffold.project_name}.Loads.{self.building_name}")
 
             # remove ReaderTMY3
             mofile.remove_component("Buildings.BoundaryConditions.WeatherData.ReaderTMY3", "weaDat")
 
             # Remove `lat` from diffuse & direct solar gains (removed from MBL in version 9)
-            mofile.remove_component_argument("Buildings.BoundaryConditions.SolarIrradiation.DiffusePerez", "HDifTil", "lat")
-            mofile.remove_component_argument("Buildings.BoundaryConditions.SolarIrradiation.DiffusePerez", "HDifTilRoof", "lat")
-            mofile.remove_component_argument("Buildings.BoundaryConditions.SolarIrradiation.DirectTiltedSurface", "HDirTil", "lat")
-            mofile.remove_component_argument("Buildings.BoundaryConditions.SolarIrradiation.DirectTiltedSurface", "HDirTilRoof", "lat")
+            mofile.remove_component_argument(
+                "Buildings.BoundaryConditions.SolarIrradiation.DiffusePerez", "HDifTil", "lat"
+            )
+            mofile.remove_component_argument(
+                "Buildings.BoundaryConditions.SolarIrradiation.DiffusePerez", "HDifTilRoof", "lat"
+            )
+            mofile.remove_component_argument(
+                "Buildings.BoundaryConditions.SolarIrradiation.DirectTiltedSurface", "HDirTil", "lat"
+            )
+            mofile.remove_component_argument(
+                "Buildings.BoundaryConditions.SolarIrradiation.DirectTiltedSurface", "HDirTilRoof", "lat"
+            )
 
             # updating path to internal loads
 
             mofile.update_component_modification(
                 "Modelica.Blocks.Sources.CombiTimeTable",
                 "internalGains",
                 "fileName",
-                "Modelica.Utilities.Files.loadResource(filNam)"
+                "Modelica.Utilities.Files.loadResource(filNam)",
             )
 
             # add heat port convective heat flow.
             mofile.insert_component(
-                "Modelica.Thermal.HeatTransfer.Interfaces.HeatPort_a", "port_a",
-                string_comment='Heat port for convective heat flow.',
+                "Modelica.Thermal.HeatTransfer.Interfaces.HeatPort_a",
+                "port_a",
+                string_comment="Heat port for convective heat flow.",
                 annotations=[
                     "Placement(transformation(extent={{-10,90},{10,110}}), "
                     "iconTransformation(extent={{-10,90},{10,110}}))"
-                ]
+                ],
             )
             # add heat port radiative heat flow.
             mofile.insert_component(
-                "Modelica.Thermal.HeatTransfer.Interfaces.HeatPort_a", "port_b",
-                string_comment='Heat port for radiative heat flow.',
+                "Modelica.Thermal.HeatTransfer.Interfaces.HeatPort_a",
+                "port_b",
+                string_comment="Heat port for radiative heat flow.",
                 annotations=[
                     "Placement(transformation(extent={{30,-110},{50,-90}}, "
                     "iconTransformation(extent={{40,-112},{60,-92}})))"
-                ]
+                ],
             )
             # add fluid ports for the indoor air volume.
             mofile.insert_component(
-                "Modelica.Fluid.Vessels.BaseClasses.VesselFluidPorts_b", "ports[nPorts]",
-                string_comment='Auxiliary fluid inlets and outlets to indoor air volume.',
-                modifications={
-                    'redeclare each final package Medium': 'Buildings.Media.Air'
-                },
+                "Modelica.Fluid.Vessels.BaseClasses.VesselFluidPorts_b",
+                "ports[nPorts]",
+                string_comment="Auxiliary fluid inlets and outlets to indoor air volume.",
+                modifications={"redeclare each final package Medium": "Buildings.Media.Air"},
                 annotations=[
                     "Placement(transformation(extent={{-30, -8}, {30, 8}},origin={0, -100}), "
                     "iconTransformation(extent={{-23.25, -7.25}, {23.25, 7.25}},"
                     "origin={-0.75, -98.75}))"
-                ]
+                ],
             )
 
             fraction_latent_person = self.system_parameters.get_param(
                 "buildings.load_model_parameters.rc.fraction_latent_person", default=1.25
             )
 
             use_moisture_balance = self.system_parameters.get_param(
-                "buildings.load_model_parameters.rc.use_moisture_balance", default='false'
+                "buildings.load_model_parameters.rc.use_moisture_balance", default="false"
             )
 
-            n_ports = self.system_parameters.get_param(
-                "buildings.load_model_parameters.rc.nPorts", default=0
-            )
+            n_ports = self.system_parameters.get_param("buildings.load_model_parameters.rc.nPorts", default=0)
 
             # create a new parameter for fraction latent person
             mofile.add_parameter(
-                'Real', 'fraLat',
+                "Real",
+                "fraLat",
                 assigned_value=fraction_latent_person,
-                string_comment='Fraction latent of sensible persons load = 0.8 for home, 1.25 for office.'
+                string_comment="Fraction latent of sensible persons load = 0.8 for home, 1.25 for office.",
             )
             # create a new Boolean parameter to evaluate the persons latent loads.
             mofile.add_parameter(
-                'Boolean', 'use_moisture_balance',
+                "Boolean",
+                "use_moisture_balance",
                 assigned_value=use_moisture_balance,
-                string_comment='If true, input connector QLat_flow is enabled and room air computes'
-                               ' moisture balance.'
+                string_comment="If true, input connector QLat_flow is enabled and room air computes"
+                " moisture balance.",
             )
             # create a integer parameter to evaluate number of connected ports.
             mofile.add_parameter(
-                'Integer', 'nPorts',
+                "Integer",
+                "nPorts",
                 assigned_value=n_ports,
-                string_comment='Number of fluid ports.',
-                annotations=['connectorSizing=true']
+                string_comment="Number of fluid ports.",
+                annotations=["connectorSizing=true"],
             )
             # Add a parameter to put the load filename at the top of the model
             mofile.add_parameter(
-                'String', 'filNam',
+                "String",
+                "filNam",
                 assigned_value=f'"modelica://{self.internal_gains_file}"',
-                string_comment='modelica path to the internal gains file used in the model CombiTimeTable'
+                string_comment="modelica path to the internal gains file used in the model CombiTimeTable",
             )
 
             # Set the fraction latent person in the template by simply replacing the value
             mofile.insert_component(
-                'Modelica.Blocks.Sources.RealExpression', 'perLatLoa',
+                "Modelica.Blocks.Sources.RealExpression",
+                "perLatLoa",
                 modifications={
-                    'y': 'internalGains.y[2]*fraLat',
+                    "y": "internalGains.y[2]*fraLat",
                 },
-                conditional='if use_moisture_balance',
-                string_comment='Latent person loads',
-                annotations=['Placement(transformation(extent={{-80,-60},{-60,-40}}))']
+                conditional="if use_moisture_balance",
+                string_comment="Latent person loads",
+                annotations=["Placement(transformation(extent={{-80,-60},{-60,-40}}))"],
             )
 
             # add TRad output
             mofile.insert_component(
-                'Buildings.Controls.OBC.CDL.Interfaces.RealOutput', 'TRad',
+                "Buildings.Controls.OBC.CDL.Interfaces.RealOutput",
+                "TRad",
                 modifications={
-                    'quantity': '"ThermodynamicTemperature"',
-                    'unit': '"K"',
-                    'displayUnit': '"degC"',
+                    "quantity": '"ThermodynamicTemperature"',
+                    "unit": '"K"',
+                    "displayUnit": '"degC"',
                 },
-                string_comment='Mean indoor radiation temperature',
-                annotations=['Placement(transformation(extent={{100,-10},{120,10}}))']
+                string_comment="Mean indoor radiation temperature",
+                annotations=["Placement(transformation(extent={{100,-10},{120,10}}))"],
             )
 
             # All existing weaDat.weaBus connections need to be updated to simply weaBus
             # (except for the connections where 'weaBus' is port_b, we will just delete these)
-            mofile.edit_connect('weaDat.weaBus', '!weaBus', new_port_a='weaBus')
+            mofile.edit_connect("weaDat.weaBus", "!weaBus", new_port_a="weaBus")
             # Now remove the unnecessary weaDat.weaBus -> weaBus connection
-            mofile.remove_connect('weaDat.weaBus', 'weaBus')
+            mofile.remove_connect("weaDat.weaBus", "weaBus")
 
             # add new port connections
-            rc_order = self.system_parameters.get_param_by_building_id(
-                self.building_id, "load_model_parameters.rc.order"
-            )
+            rc_order = self.system_parameters.get_param_by_id(self.building_id, "load_model_parameters.rc.order")
             thermal_zone_name = None
             thermal_zone_type = None
             if rc_order == 1:
-                thermal_zone_type = 'OneElement'
-                thermal_zone_name = 'thermalZoneOneElement'
+                thermal_zone_type = "OneElement"
+                thermal_zone_name = "thermalZoneOneElement"
             elif rc_order == 2:
-                thermal_zone_type = 'TwoElements'
-                thermal_zone_name = 'thermalZoneTwoElements'
+                thermal_zone_type = "TwoElements"
+                thermal_zone_name = "thermalZoneTwoElements"
             elif rc_order == 3:
-                thermal_zone_type = 'ThreeElements'
-                thermal_zone_name = 'thermalZoneThreeElements'
+                thermal_zone_type = "ThreeElements"
+                thermal_zone_name = "thermalZoneThreeElements"
             elif rc_order == 4:
-                thermal_zone_type = 'FourElements'
-                thermal_zone_name = 'thermalZoneFourElements'
+                thermal_zone_type = "FourElements"
+                thermal_zone_name = "thermalZoneFourElements"
 
             if thermal_zone_name is not None and thermal_zone_type is not None:
                 # add TAir output - This has been moved away from the other insert_component blocks
                 # to use thermal_zone_name
                 mofile.insert_component(
-                    'Buildings.Controls.OBC.CDL.Interfaces.RealOutput', 'TAir',
+                    "Buildings.Controls.OBC.CDL.Interfaces.RealOutput",
+                    "TAir",
                     modifications={
-                        'quantity': '"ThermodynamicTemperature"',
-                        'unit': '"K"',
-                        'displayUnit': '"degC"',
+                        "quantity": '"ThermodynamicTemperature"',
+                        "unit": '"K"',
+                        "displayUnit": '"degC"',
                     },
-                    conditional=f'if {thermal_zone_name}.VAir > 0',
-                    string_comment='Room air temperature',
-                    annotations=['Placement(transformation(extent={{100,38},{120,58}}))']
+                    conditional=f"if {thermal_zone_name}.VAir > 0",
+                    string_comment="Room air temperature",
+                    annotations=["Placement(transformation(extent={{100,38},{120,58}}))"],
                 )
 
                 # In TEASER 0.7.5 the hConvWinOut, hConvExt, hConvWin, hConvInt, hConvFloor, hConvRoof in various of
                 # the ReducedOrder models should be hCon* not hConv*. This has been fixed on the development branch
                 # of TEASER, but the team doesn't appear to be releasing nor merging the development branch (yet).
                 mofile.rename_component_argument(
                     "Buildings.ThermalZones.ReducedOrder.EquivalentAirTemperature.VDI6007WithWindow",
                     "eqAirTemp",
                     "hConvWallOut",
-                    "hConWallOut"
+                    "hConWallOut",
                 )
                 mofile.rename_component_argument(
                     "Buildings.ThermalZones.ReducedOrder.EquivalentAirTemperature.VDI6007WithWindow",
                     "eqAirTemp",
                     "hConvWinOut",
-                    "hConWinOut"
+                    "hConWinOut",
                 )
 
                 mofile.rename_component_argument(
                     "Buildings.ThermalZones.ReducedOrder.EquivalentAirTemperature.VDI6007",
                     "eqAirTempVDI",
                     "hConvWallOut",
-                    "hConWallOut"
+                    "hConWallOut",
                 )
 
                 renames = {
                     "hConvExt": "hConExt",
                     "hConvFloor": "hConFloor",
                     "hConvRoof": "hConRoof",
                     "hConvWinOut": "hConWinOut",
                     "hConvWin": "hConWin",
                     "hConvInt": "hConInt",
                 }
                 for from_, to_ in renames.items():
                     mofile.rename_component_argument(
-                        f"Buildings.ThermalZones.ReducedOrder.RC.{thermal_zone_type}",
-                        thermal_zone_name,
-                        from_,
-                        to_
+                        f"Buildings.ThermalZones.ReducedOrder.RC.{thermal_zone_type}", thermal_zone_name, from_, to_
                     )
 
                 mofile.update_component_modifications(
                     f"Buildings.ThermalZones.ReducedOrder.RC.{thermal_zone_type}",
                     thermal_zone_name,
-                    {"use_moisture_balance": "use_moisture_balance"}
+                    {"use_moisture_balance": "use_moisture_balance"},
                 )
 
                 mofile.update_component_modifications(
                     f"Buildings.ThermalZones.ReducedOrder.RC.{thermal_zone_type}",
                     thermal_zone_name,
-                    {"nPorts": "nPorts"}
+                    {"nPorts": "nPorts"},
                 )
 
                 mofile.add_connect(
-                    'port_a', f'{thermal_zone_name}.intGainsConv',
-                    annotations=['Line(points={{0,100},{96,100},{96,20},{92,20}}, color={191,0,0})']
+                    "port_a",
+                    f"{thermal_zone_name}.intGainsConv",
+                    annotations=["Line(points={{0,100},{96,100},{96,20},{92,20}}, color={191,0,0})"],
                 )
 
                 mofile.add_connect(
-                    f'{thermal_zone_name}.TAir', 'TAir',
-                    annotations=[
-                        'Line(points={{93,32},{98,32},{98,48},{110,48}}, color={0,0,127})'
-                    ]
+                    f"{thermal_zone_name}.TAir",
+                    "TAir",
+                    annotations=["Line(points={{93,32},{98,32},{98,48},{110,48}}, color={0,0,127})"],
                 )
                 mofile.add_connect(
-                    f'{thermal_zone_name}.TRad', 'TRad',
-                    annotations=[
-                        'Line(points={{93,28},{98,28},{98,-20},{110,-20}}, color={0,0,127})'
-                    ]
+                    f"{thermal_zone_name}.TRad",
+                    "TRad",
+                    annotations=["Line(points={{93,28},{98,28},{98,-20},{110,-20}}, color={0,0,127})"],
                 )
                 mofile.add_connect(
-                    f'{thermal_zone_name}.QLat_flow', 'perLatLoa.y',
+                    f"{thermal_zone_name}.QLat_flow",
+                    "perLatLoa.y",
                     annotations=[
-                        'Line(points={{43,4},{40,4},{40,-28},{-40,-28},{-40,-50},{-59,-50}}, color={0, 0,127})'
-                    ]
+                        "Line(points={{43,4},{40,4},{40,-28},{-40,-28},{-40,-50},{-59,-50}}, color={0, 0,127})"
+                    ],
                 )
 
                 mofile.add_connect(
-                    f'{thermal_zone_name}.intGainsRad', 'port_b',
-                    annotations=[
-                        'Line(points={{92, 24}, {98, 24}, {98, -100}, {40, -100}}, color={191, 0, 0})'
-                    ]
+                    f"{thermal_zone_name}.intGainsRad",
+                    "port_b",
+                    annotations=["Line(points={{92, 24}, {98, 24}, {98, -100}, {40, -100}}, color={191, 0, 0})"],
                 )
                 mofile.insert_equation_for_loop(
                     index_identifier="i",
                     expression_raw="1:nPorts",
                     loop_body_raw_list=[
                         f"connect(ports[i], {thermal_zone_name}.ports[i])",
                         "\tannotation (Line(",
@@ -456,15 +459,15 @@
                     ],
                 )
 
                 # Fix the thermalZone medium model
                 mofile.overwrite_component_redeclaration(
                     f"Buildings.ThermalZones.ReducedOrder.RC.{thermal_zone_type}",
                     thermal_zone_name,
-                    "Medium = Buildings.Media.Air"
+                    "Medium = Buildings.Media.Air",
                 )
 
             # change the name of the modelica model to remove the building id, update in package too!
             original_model_name = mofile.get_name()
             new_model_name = original_model_name.split("_")[1]
             thermal_zone_files.append(new_model_name)
             package.rename_model(original_model_name, new_model_name)
@@ -479,153 +482,175 @@
 
         # Now connect all the thermal zone files into the teaser building
         # 1. Need to a map of thermal zone names and instances
         zone_list = []
         for index, tz in enumerate(thermal_zone_files):
             # take /a/file/Meeting.mo -> zone_map["Meeting"] = "meeting"
             tz_process = os.path.splitext(os.path.basename(tz))[0]
-            zone_list.append({
-                "index": index,
-                "model_name": tz_process,
-                "instance_name": tz_process.lower(),
-                # process where this will be stored in python otherwise too many {{}}, yes ridiculous.
-                # This needs to result in {{a,b},{x,y}}
-                "placement": f"{{{{{-160 + index * 40},-20}},{{{-140 + index * 40},0}}}}"
-            })
+            zone_list.append(
+                {
+                    "index": index,
+                    "model_name": tz_process,
+                    "instance_name": tz_process.lower(),
+                    # process where this will be stored in python otherwise too many {{}}, yes ridiculous.
+                    # This needs to result in {{a,b},{x,y}}
+                    "placement": f"{{{{{-160 + index * 40},-20}},{{{-140 + index * 40},0}}}}",
+                }
+            )
 
         # Handle setting nominal load for IT room zone
         nom_cool_flow = np.array([-10000] * len(zone_list))
         for i, dic in enumerate(zone_list):
             if dic["instance_name"] == "ict":
                 nom_cool_flow[i - 1] = -50000  # Need to offset for different indexing
         nom_heat_flow = np.array([10000] * len(zone_list))
         building_template_data = {
             "thermal_zones": zone_list,
-            "nominal_heat_flow": str(repr(nom_heat_flow))[1:-1].replace("[", "{").replace("]", "}").split("rray(", 1)[-1],
-            "nominal_cool_flow": str(repr(nom_cool_flow))[1:-1].replace("[", "{").replace("]", "}").split("rray(", 1)[-1],
+            "nominal_heat_flow": str(repr(nom_heat_flow))[1:-1]
+            .replace("[", "{")
+            .replace("]", "}")
+            .split("rray(", 1)[-1],
+            "nominal_cool_flow": str(repr(nom_cool_flow))[1:-1]
+            .replace("[", "{")
+            .replace("]", "}")
+            .split("rray(", 1)[-1],
             "load_resources_path": b_modelica_path.resources_relative_dir,
             "mos_weather": {
                 "mos_weather_filename": mos_weather_filename,
                 "filename": os.path.basename(mos_weather_filename),
                 "path": os.path.dirname(mos_weather_filename),
             },
             "nominal_values": {
-                "chw_supply_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_chw_supply"
-                )),
-                "chw_return_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_chw_return"
-                )),
-                "hhw_supply_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_hw_supply"
-                )),
-                "hhw_return_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_hw_return"
-                )),
-                "temp_setpoint_heating": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_setpoint_heating"
-                )),
-                "temp_setpoint_cooling": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.temp_setpoint_cooling"
-                )),
+                "chw_supply_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(self.building_id, "load_model_parameters.rc.temp_chw_supply")
+                ),
+                "chw_return_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(self.building_id, "load_model_parameters.rc.temp_chw_return")
+                ),
+                "hhw_supply_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(self.building_id, "load_model_parameters.rc.temp_hw_supply")
+                ),
+                "hhw_return_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(self.building_id, "load_model_parameters.rc.temp_hw_return")
+                ),
+                "temp_setpoint_heating": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.rc.temp_setpoint_heating"
+                    )
+                ),
+                "temp_setpoint_cooling": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.rc.temp_setpoint_cooling"
+                    )
+                ),
                 # FIXME: pick up default value from schema if not specified in system_parameters,
                 # FYI: Modelica insists on booleans being lowercase, so we need to explicitly set "true" and "false"
-                "has_liquid_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.has_liquid_heating",
-                ) else "false",
-                "has_liquid_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.has_liquid_cooling",
-                ) else "false",
-                "has_electric_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.has_electric_heating",
-                ) else "false",
-                "has_electric_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.rc.has_electric_cooling",
-                ) else "false",
-            }
+                "has_liquid_heating": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.rc.has_liquid_heating",
+                )
+                else "false",
+                "has_liquid_cooling": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.rc.has_liquid_cooling",
+                )
+                else "false",
+                "has_electric_heating": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.rc.has_electric_heating",
+                )
+                else "false",
+                "has_electric_cooling": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.rc.has_electric_cooling",
+                )
+                else "false",
+            },
         }
 
         # merge ets template values from load_base.py into the building nominal values
         # If there is no ets defined in sys-param file, use the building template data alone
         try:
-            nominal_values = {**building_template_data['nominal_values'], **self.ets_template_data}
+            nominal_values = {**building_template_data["nominal_values"], **self.ets_template_data}
             combined_template_data = {**building_template_data, **nominal_values}
         except AttributeError:
             combined_template_data = building_template_data
 
         self.run_template(
             teaser_building,
             os.path.join(b_modelica_path.files_dir, "building.mo"),
             project_name=scaffold.project_name,
             model_name=self.building_name,
-            data=combined_template_data
+            data=combined_template_data,
         )
 
         self.run_template(
             teaser_coupling,
             os.path.join(os.path.join(b_modelica_path.files_dir, "coupling.mo")),
             project_name=scaffold.project_name,
             model_name=self.building_name,
-            data=combined_template_data
+            data=combined_template_data,
         )
 
         full_model_name = os.path.join(
-            scaffold.project_name,
-            scaffold.loads_path.files_relative_dir,
-            self.building_name,
-            "coupling"
-        ).replace(os.path.sep, '.')
+            scaffold.project_name, scaffold.loads_path.files_relative_dir, self.building_name, "coupling"
+        ).replace(os.path.sep, ".")
 
         self.run_template(
             run_coupling_template,
             os.path.join(os.path.join(b_modelica_path.scripts_dir, "RunTeaserCouplingBuilding.mos")),
             full_model_name=full_model_name,
             model_name="coupling",
         )
 
         # copy over the required mo files and add the other models to the package order
-        mo_files = self.copy_required_mo_files(b_modelica_path.files_dir, within=f'{scaffold.project_name}.Loads')
+        mo_files = self.copy_required_mo_files(b_modelica_path.files_dir, within=f"{scaffold.project_name}.Loads")
         for f in mo_files:
             package.add_model(os.path.splitext(os.path.basename(f))[0])
-        package.add_model('building')
-        package.add_model('coupling')
+        package.add_model("building")
+        package.add_model("coupling")
 
         # save the updated package.mo and package.order in the Loads.B{} folder
         new_package = PackageParser.new_from_template(
             package.path, self.building_name, package.order, within=f"{scaffold.project_name}.Loads"
         )
         new_package.save()
         # AA added this 9/24
         if os.path.exists(building_template_data["mos_weather"]["mos_weather_filename"]):
             shutil.copy(
                 building_template_data["mos_weather"]["mos_weather_filename"],
-                os.path.join(b_modelica_path.resources_dir, building_template_data["mos_weather"]["filename"])
+                os.path.join(b_modelica_path.resources_dir, building_template_data["mos_weather"]["filename"]),
             )
         else:
             raise Exception(
-                f"Missing MOS weather file for Teaser: {building_template_data['mos_weather']['mos_weather_filename']}")
+                f"Missing MOS weather file for Teaser: {building_template_data['mos_weather']['mos_weather_filename']}"
+            )
         # end of what AA added 9/24
 
         # remaining clean up tasks across the entire exported project
         if not keep_original_models:
             shutil.rmtree(os.path.join(scaffold.loads_path.files_dir, "Project"))
 
         # now create the Loads level package and package.order.
-        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, 'package.mo')):
+        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, "package.mo")):
             load_package = PackageParser.new_from_template(
                 scaffold.loads_path.files_dir, "Loads", [self.building_name], within=f"{scaffold.project_name}"
             )
             load_package.save()
         else:
             load_package = PackageParser(os.path.join(scaffold.loads_path.files_dir))
             load_package.add_model(self.building_name)
             load_package.save()
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         package = PackageParser(scaffold.project_path)
-        if 'Loads' not in package.order:
-            package.add_model('Loads')
+        if "Loads" not in package.order:
+            package.add_model("Loads")
             package.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Loads.{self.building_name}.building'
+        return f"Loads.{self.building_name}.building"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunSpawnCouplingBuilding.most`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 old_hidden_avoid_double_computation=Hidden.AvoidDoubleComputation;
 Hidden.AvoidDoubleComputation=true;
 simulateModel("{{full_model_name}}",
-    method="cvode",
     tolerance=1e-6,
     numberOfIntervals=500,
     stopTime=604800.0,
     resultFile="{{model_name}}");
 Hidden.AvoidDoubleComputation=old_hidden_avoid_double_computation;
 createPlot(
     id=1,
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/RunTeaserCouplingBuilding.most`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 simulateModel("{{full_model_name}}",
-    method="cvode",
     tolerance=1e-6,
     numberOfIntervals=500,
     stopTime=604800.0,
     resultFile="{{model_name}}");
 
 createPlot(
         id=1,
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnBuilding.mot`

 * *Files 2% similar despite different names*

```diff
@@ -42,21 +42,21 @@
     "Path of the IDF file";
   parameter String weaName="modelica://{{project_name}}/Loads/{{data['load_resources_path']}}/{{data['mos_weather']['filename']}}"
     "Path of the mos weather file";
   parameter String epwName="modelica://{{project_name}}/Loads/{{data['load_resources_path']}}/{{data['epw']['filename']}}"
     "Name of the epw weather file";
   // TODO: Minimum and Maximum TSet: make a function of the outdoor air temperature, type of building,occupancy schedule or woking/idle days?
   // Set these based on cooling and heating setpoints for now based on current parameters in schema.
-  {% raw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant minTSet[nZon](
+  {% raw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant minTSet[nZon](
     {% endraw %}k=fill(
       {{ data["nominal_values"]["temp_setpoint_heating"] }},
       nZon))
     {% raw %} "Minimum temperature setpoint"
     annotation (Placement(transformation(extent={{-220,60},{-200,80}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant maxTSet[nZon](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant maxTSet[nZon](
     {% endraw %}k=fill(
       {{ data["nominal_values"]["temp_setpoint_cooling"] }},
       nZon))
     {% raw %} "Maximum temperature setpoint"
     annotation (Placement(transformation(extent={{-220,20},{-200,40}})));
   Modelica.Blocks.Sources.Constant qConGai_flow(
     k=0)
@@ -84,18 +84,18 @@
       idfName),
     epwName=Modelica.Utilities.Files.loadResource(
       epwName),
     weaName=Modelica.Utilities.Files.loadResource(
       weaName))
     "Building outer component"
     annotation (Placement(transformation(extent={{40,60},{60,80}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum mulSum(
+  Buildings.Controls.OBC.CDL.Reals.MultiSum mulSum(
     nin=nZon)
     annotation (Placement(transformation(extent={{260,110},{280,130}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum mulSum3(
+  Buildings.Controls.OBC.CDL.Reals.MultiSum mulSum3(
     nin=2) if have_pum
     annotation (Placement(transformation(extent={{260,70},{280,90}})));
   Buildings.Experimental.DHC.Loads.BaseClasses.Examples.BaseClasses.FanCoil4Pipe terUni[nZon](
     each T_aChiWat_nominal=T_aChiWat_nominal,
     each T_bChiWat_nominal=T_bChiWat_nominal,
     redeclare each final package Medium1=MediumW,
     redeclare each final package Medium2=MediumA,
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/SpawnCouplingBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/Spawn_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserBuilding.mot`

 * *Files 1% similar despite different names*

```diff
@@ -22,35 +22,35 @@
     pAtm(
       displayUnit="Pa")=101339,
     filNam=Modelica.Utilities.Files.loadResource(
       weaName),
     computeWetBulbTemperature=true)
     "Weather data reader"
     annotation (Placement(transformation(extent={{10,-10},{-10,10}},rotation=90,origin={56,96})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant minTSet[nZon](
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant minTSet[nZon](
     k=fill(
       {{ data['nominal_values']['temp_setpoint_heating']  }},
       nZon),
     y(
       each final unit="K",
       each displayUnit="degC"))
     "Minimum temperature set point"
     {% raw %} annotation (Placement(transformation(extent={{-290,230},{-270,250}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant maxTSet[nZon](
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant maxTSet[nZon](
     k=fill(
       {{ data['nominal_values']['temp_setpoint_cooling']  }},
       nZon),
     y(
       each final unit="K",
       each displayUnit="degC"))
     "Maximum temperature set point"
     {% raw %} annotation (Placement(transformation(extent={{-290,190},{-270,210}})));
   {% endraw %}{% for zone in data['thermal_zones'] %}{{zone['model_name']}} {{zone['instance_name']}}
     annotation (Placement(transformation(extent={{zone['placement']}})));
-  {% endfor %}Buildings.Controls.OBC.CDL.Continuous.MultiSum mulSum(
+  {% endfor %}Buildings.Controls.OBC.CDL.Reals.MultiSum mulSum(
     nin=2) if have_pum
     {% raw %} annotation (Placement(transformation(extent={{260,70},{280,90}})));
   {% endraw %}Buildings.Experimental.DHC.Loads.BaseClasses.Examples.BaseClasses.FanCoil4PipeHeatPorts terUni[nZon](
     redeclare each package Medium1=MediumW,
     redeclare each package Medium2=MediumA,
     each facMul=facMul,
     QHea_flow_nominal={{ data['nominal_heat_flow'] }},
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TeaserCouplingBuilding.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuilding.mot`

 * *Files 2% similar despite different names*

```diff
@@ -96,22 +96,22 @@
     y(
       each unit="W"),
     offset={0,0,0},
     columns={2,3,4},
     smoothness=Modelica.Blocks.Types.Smoothness.MonotoneContinuousDerivative1)
     "Reader for thermal loads (y[1] is cooling load, y[2] is heating load)"
     annotation (Placement(transformation(extent={{-280,-10},{-260,10}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant minTSet(
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant minTSet(
     k={{ data['nominal_values']['temp_setpoint_heating']  }},
     {% raw %}y(
       unit="K",
       displayUnit="degC"))
     "Minimum temperature set point"
     annotation (Placement(transformation(extent={{-280,170},{-260,190}})));
-  {% endraw %}Buildings.Controls.OBC.CDL.Continuous.Sources.Constant maxTSet(
+  {% endraw %}Buildings.Controls.OBC.CDL.Reals.Sources.Constant maxTSet(
     k={{ data['nominal_values']['temp_setpoint_cooling']  }},
     {% raw %}y(
       unit="K",
       displayUnit="degC"))
     "Maximum temperature set point"
     annotation (Placement(transformation(extent={{-280,210},{-260,230}})));
   replaceable Buildings.Experimental.DHC.Loads.BaseClasses.Validation.BaseClasses.FanCoil2PipeHeating terUniHea(
@@ -154,16 +154,15 @@
     "Chilled water distribution system"
     annotation (Placement(transformation(extent={{120,-270},{140,-250}})));
   replaceable Buildings.Experimental.DHC.Loads.BaseClasses.Validation.BaseClasses.FanCoil2PipeCooling terUniCoo(
     QHea_flow_nominal=QHea_flow_nominal/facMulHea,
     T_aLoaHea_nominal=T_aLoaHea_nominal,
     k=k,
     Ti=Ti,
-    TRooHea_nominal=T_aLoaHea_nominal,
-    QRooHea_flow_nominal=QHea_flow_nominal/facMulCoo) if have_chiWat
+    QEnv_flow_nominal=-QCoo_flow_nominal/facMulCoo) if have_chiWat
     constrainedby Buildings.Experimental.DHC.Loads.BaseClasses.PartialTerminalUnit(
       redeclare package Medium1=Medium,
       redeclare package Medium2=Medium2,
       allowFlowReversal=allowFlowReversal,
       facMul=facMulCoo,
       facMulZon=1,
       QCoo_flow_nominal=QCoo_flow_nominal/facMulCoo,
@@ -184,35 +183,35 @@
     "Heating load"
     annotation (Placement(transformation(extent={{300,20},{340,60}}),iconTransformation(extent={{-20,-20},{20,20}},rotation=-90,origin={200,-320})));
   Modelica.Blocks.Interfaces.RealOutput QReqCoo_flow(
     each quantity="HeatFlowRate",
     each unit="W") if have_cooLoa
     "Cooling load"
     annotation (Placement(transformation(extent={{300,-20},{340,20}}),iconTransformation(extent={{-20,-20},{20,20}},rotation=-90,origin={260,-320})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant noHea(
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant noHea(
     k=0) if not have_heaWat
     "No heating system"
     annotation (Placement(transformation(extent={{80,120},{100,140}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant noCoo(
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant noCoo(
     k=0) if not have_chiWat
     "No cooling system"
     annotation (Placement(transformation(extent={{80,78},{100,98}})));
-  Buildings.Controls.OBC.CDL.Continuous.Add addPFan
+  Buildings.Controls.OBC.CDL.Reals.Add addPFan
     "Sum fan power"
     annotation (Placement(transformation(extent={{222,120},{242,140}})));
-  Buildings.Controls.OBC.CDL.Continuous.Add addPPum
+  Buildings.Controls.OBC.CDL.Reals.Add addPPum
     "Sum pump power"
     annotation (Placement(transformation(extent={{222,70},{242,90}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiplyByParameter mulQReqHea_flow(
+  Buildings.Controls.OBC.CDL.Reals.MultiplyByParameter mulQReqHea_flow(
     u(
       unit="W"),
     k=facMul) if have_heaLoa
     "Scaling"
     annotation (Placement(transformation(extent={{272,30},{292,50}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiplyByParameter mulQReqCoo_flow(
+  Buildings.Controls.OBC.CDL.Reals.MultiplyByParameter mulQReqCoo_flow(
     u(
       unit="W"),
     k=facMul) if have_cooLoa
     "Scaling"
     annotation (Placement(transformation(extent={{272,-10},{292,10}})));
 protected
   parameter Modelica.Units.SI.SpecificHeatCapacity cp_air=1005
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesBuildingWithETS.mot`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 within {{ project_name }}.Loads.{{ model_name }};
 {% raw %}model building
   "Model of a building with an internal ETS. Building loads provided as time series"
   extends Buildings.Experimental.DHC.Loads.Combined.BaseClasses.PartialBuildingWithETS(
     final allowFlowReversalSer=true,
-    // redeclare Buildings.Experimental.DHC.Loads.BaseClasses.Examples.BaseClasses.BuildingTimeSeries bui(
     {% endraw %}redeclare {{ project_name }}.Loads.{{ model_name }}.TimeSeriesBuilding bui(
-      {% raw %}have_hotWat=false,
+      {% raw %}have_hotWat=true,
       T_aHeaWat_nominal=ets.THeaWatSup_nominal,
       T_bHeaWat_nominal=ets.THeaWatRet_nominal,
       T_aChiWat_nominal=ets.TChiWatSup_nominal,
       T_bChiWat_nominal=ets.TChiWatRet_nominal,
       facMulHea=10*QHea_flow_nominal/(1.7E5),
       facMulCoo=40*QCoo_flow_nominal/(-1.5E5)),
     ets(
-      have_hotWat=false,
+      have_hotWat=true,
       QChiWat_flow_nominal=QCoo_flow_nominal,
       QHeaWat_flow_nominal=QHea_flow_nominal,
       QHotWat_flow_nominal=QHot_flow_nominal));
   {% endraw %}parameter String filNam="modelica://{{project_name}}/Loads/{{data['load_resources_path']}}/{{data['time_series']['filename']}}"
     {% raw %} "Library path of the file with loads as time series";
   final parameter Modelica.Units.SI.HeatFlowRate QCoo_flow_nominal(
     max=-Modelica.Constants.eps)=bui.facMul*bui.QCoo_flow_nominal
@@ -39,27 +38,27 @@
     "Service hot water supply temperature set point"
     annotation (Placement(transformation(extent={{-20,-20},{20,20}},rotation=0,origin={-320,40}),iconTransformation(extent={{-20,-20},{20,20}},rotation=0,origin={-120,30})));
   Buildings.Controls.OBC.CDL.Interfaces.RealInput TColWat(
     final unit="K",
     displayUnit="degC")
     "Cold water temperature"
     annotation (Placement(transformation(extent={{-20,-20},{20,20}},rotation=0,origin={-320,0}),iconTransformation(extent={{-20,-20},{20,20}},rotation=90,origin={-80,-120})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiplyByParameter loaHeaNor(
+  Buildings.Controls.OBC.CDL.Reals.MultiplyByParameter loaHeaNor(
     k=1/QHea_flow_nominal)
     "Normalized heating load"
     annotation (Placement(transformation(extent={{-200,-110},{-180,-90}})));
-  Buildings.Controls.OBC.CDL.Continuous.GreaterThreshold enaHeaCoo[2](
+  Buildings.Controls.OBC.CDL.Reals.GreaterThreshold enaHeaCoo[2](
     each t=1e-4)
     "Threshold comparison to enable heating and cooling"
     annotation (Placement(transformation(extent={{-110,-130},{-90,-110}})));
   Modelica.Blocks.Sources.BooleanConstant enaSHW(
     final k=true) if have_hotWat
     "SHW production enable signal"
     annotation (Placement(transformation(extent={{0,-130},{-20,-110}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiplyByParameter loaCooNor(
+  Buildings.Controls.OBC.CDL.Reals.MultiplyByParameter loaCooNor(
     k=1/QCoo_flow_nominal)
     "Normalized cooling load"
     annotation (Placement(transformation(extent={{-200,-150},{-180,-130}})));
 equation
   connect(bui.QReqHotWat_flow,ets.loaSHW)
     annotation (Line(points={{28,4},{28,-10},{-64,-10},{-64,-74},{-34,-74}},color={0,0,127}));
   connect(THotWatSupSet,ets.THotWatSupSet)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeriesMassFlowTemperatures.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/TimeSeries_Instance.mopt`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,20 @@
   // time series load
   {{ model.modelica_type }} {{ model.id }}(
     {% if model.is_5g_district == 'bui' %}
     allowFlowReversalBui = true,
-    {{ model.is_5g_district }}(T_aHeaWat_nominal(displayUnit="K")=318.15,
+    {{ model.is_5g_district }}(
+    have_hotWat=true,
+    T_aHeaWat_nominal(displayUnit="K")=318.15,
     T_aChiWat_nominal(displayUnit="K")=291.15,
     delTAirCoo(displayUnit="degC")=10,
     delTAirHea(displayUnit="degC")=20,
     k=0.1,
     Ti=120
-    ), ets(have_hotWat = false)
+    ), ets(have_hotWat = true)
     {% else %}
     allowFlowReversal = true,
     T_aHeaWat_nominal(displayUnit="K")=318.15,
     T_aChiWat_nominal(displayUnit="K")=280.15,
     delTAirCoo(displayUnit="degC")=10,
     delTAirHea(displayUnit="degC")=20,
     k=0.1,
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/templates/getPeakMassFlowRate.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/time_series.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/time_series.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,186 +2,197 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import os
 import shutil
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
-    LoadBase
-)
-from geojson_modelica_translator.utils import (
-    ModelicaPath,
-    convert_c_to_k,
-    simple_uuid
-)
+from geojson_modelica_translator.model_connectors.load_connectors.load_base import LoadBase
+from geojson_modelica_translator.utils import ModelicaPath, convert_c_to_k, simple_uuid
 
 
 class TimeSeries(LoadBase):
-    model_name = 'TimeSeries'
+    model_name = "TimeSeries"
 
     def __init__(self, system_parameters, geojson_load):
         super().__init__(system_parameters, geojson_load)
-        self.id = 'TimeSerLoa_' + simple_uuid()
+        self.id = "TimeSerLoa_" + simple_uuid()
 
     def to_modelica(self, scaffold):
-        """
-        Create timeSeries models based on the data in the buildings and geojsons
+        """Create timeSeries models based on the data in the buildings and geojsons
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         time_series_building_template = self.template_env.get_template("TimeSeriesBuilding.mot")
         time_series_building_with_ets_template = self.template_env.get_template("TimeSeriesBuildingWithETS.mot")
         # These templates will be rendered in order for a 5G system. 4G system uses only the first.
         building_templates = {}
-        building_templates['TimeSeriesBuilding'] = time_series_building_template
-        building_templates['building'] = time_series_building_with_ets_template
+        building_templates["TimeSeriesBuilding"] = time_series_building_template
+        building_templates["building"] = time_series_building_with_ets_template
 
-        b_modelica_path = ModelicaPath(
-            self.building_name, scaffold.loads_path.files_dir, True
-        )
+        b_modelica_path = ModelicaPath(self.building_name, scaffold.loads_path.files_dir, True)
 
-        self.copy_required_mo_files(b_modelica_path.files_dir, within=f'{scaffold.project_name}.Loads')
+        self.copy_required_mo_files(b_modelica_path.files_dir, within=f"{scaffold.project_name}.Loads")
 
         # Note that the system_parameters object when accessing filepaths will fully resolve the
         # location of the file.
-        time_series_filename = self.system_parameters.get_param_by_building_id(
+        time_series_filename = self.system_parameters.get_param_by_id(
             self.building_id, "load_model_parameters.time_series.filepath"
         )
 
         if not os.path.exists(time_series_filename):
             raise Exception(f"Missing MOS file for time series: {time_series_filename}")
-        elif os.path.splitext(time_series_filename)[1].lower() == '.csv':
+        elif os.path.splitext(time_series_filename)[1].lower() == ".csv":
             raise Exception("The timeseries file is CSV format. This must be converted to an MOS file for use.")
 
         # construct the dict to pass into the template. Depending on the type of model, not all the parameters are
         # used. The `nominal_values` are only used when the time series is coupled to an ETS system.
         building_template_data = {
             "load_resources_path": b_modelica_path.resources_relative_dir,
             "time_series": {
                 "filepath": time_series_filename,
                 "filename": os.path.basename(time_series_filename),
                 "path": os.path.dirname(time_series_filename),
             },
-            "district_type": self.system_parameters.get_param(
-                "district_system"
-            ),
+            "district_type": self.system_parameters.get_param("district_system"),
             "nominal_values": {
-                "delta_temp_air_cooling": self.system_parameters.get_param_by_building_id(
+                "delta_temp_air_cooling": self.system_parameters.get_param_by_id(
                     self.building_id, "load_model_parameters.time_series.delta_temp_air_cooling"
                 ),
-                "delta_temp_air_heating": self.system_parameters.get_param_by_building_id(
+                "delta_temp_air_heating": self.system_parameters.get_param_by_id(
                     self.building_id, "load_model_parameters.time_series.delta_temp_air_heating"
                 ),
-                "temp_setpoint_heating": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_setpoint_heating"
-                )),
-                "temp_setpoint_cooling": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_setpoint_cooling"
-                )),
-                "chw_supply_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_chw_supply"
-                )),
-                "chw_return_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_chw_return"
-                )),
-                "hhw_supply_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_hw_supply"
-                )),
-                "hhw_return_temp": convert_c_to_k(self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.temp_hw_return"
-                )),
+                "temp_setpoint_heating": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_setpoint_heating"
+                    )
+                ),
+                "temp_setpoint_cooling": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_setpoint_cooling"
+                    )
+                ),
+                "chw_supply_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_chw_supply"
+                    )
+                ),
+                "chw_return_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_chw_return"
+                    )
+                ),
+                "hhw_supply_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_hw_supply"
+                    )
+                ),
+                "hhw_return_temp": convert_c_to_k(
+                    self.system_parameters.get_param_by_id(
+                        self.building_id, "load_model_parameters.time_series.temp_hw_return"
+                    )
+                ),
                 # FIXME: pick up default value from schema if not specified in system_parameters,
                 # FYI: Modelica insists on booleans being lowercase, so we need to explicitly set "true" and "false"
-                "has_liquid_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_liquid_heating",
-                ) else "false",
-                "has_liquid_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_liquid_cooling",
-                ) else "false",
-                "has_electric_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_electric_heating",
-                ) else "false",
-                "has_electric_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_electric_cooling",
-                ) else "false",
-            }
+                "has_liquid_heating": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.time_series.has_liquid_heating",
+                )
+                else "false",
+                "has_liquid_cooling": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.time_series.has_liquid_cooling",
+                )
+                else "false",
+                "has_electric_heating": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.time_series.has_electric_heating",
+                )
+                else "false",
+                "has_electric_cooling": "true"
+                if self.system_parameters.get_param_by_id(
+                    self.building_id,
+                    "load_model_parameters.time_series.has_electric_cooling",
+                )
+                else "false",
+            },
         }
 
         # merge ets template values from load_base.py into the building nominal values
         # If there is no ets defined in sys-param file, use the building template data alone
         try:
-            nominal_values = {**building_template_data['nominal_values'], **self.ets_template_data}
+            nominal_values = {**building_template_data["nominal_values"], **self.ets_template_data}
             combined_template_data = {**building_template_data, **nominal_values}
         except AttributeError:
             combined_template_data = building_template_data
 
         # copy over the resource files for this building
         # TODO: move some of this over to a validation step
         new_file = os.path.join(b_modelica_path.resources_dir, os.path.basename(time_series_filename))
         os.makedirs(os.path.dirname(new_file), exist_ok=True)
         shutil.copy(time_series_filename, new_file)
 
         # This if statement exists only because we can't use the 5G model to run a 4G building.
-        if 'fifth_generation' not in building_template_data['district_type']:
+        if "fifth_generation" not in building_template_data["district_type"]:
             self.run_template(
                 template=time_series_building_template,
                 save_file_name=os.path.join(b_modelica_path.files_dir, "TimeSeriesBuilding.mo"),
                 project_name=scaffold.project_name,
                 model_name=self.building_name,
-                data=combined_template_data
+                data=combined_template_data,
             )
         else:
             for k, v in building_templates.items():
                 self.run_template(
                     template=v,
                     save_file_name=os.path.join(b_modelica_path.files_dir, f"{k}.mo"),
                     project_name=scaffold.project_name,
                     model_name=self.building_name,
-                    data=combined_template_data
+                    data=combined_template_data,
                 )
 
         # run post process to create the remaining project files for this building
         self.post_process(scaffold)
 
     def post_process(self, scaffold):
-        """
-        Cleanup the export of time series files into a format suitable for the district-based analysis. This includes
+        """Cleanup the export of time series files into a format suitable for the district-based analysis. This includes
         the following:
 
             * Add a Loads project
             * Add a project level project
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         :return: None
         """
         b_modelica_path = os.path.join(scaffold.loads_path.files_dir, self.building_name)
         new_package = PackageParser.new_from_template(
-            b_modelica_path, self.building_name, self.template_files_to_include,
-            within=f"{scaffold.project_name}.Loads"
+            b_modelica_path, self.building_name, self.template_files_to_include, within=f"{scaffold.project_name}.Loads"
         )
         new_package.save()
 
         # now create the Loads level package and package.order.
-        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, 'package.mo')):
+        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, "package.mo")):
             load_package = PackageParser.new_from_template(
                 scaffold.loads_path.files_dir, "Loads", [self.building_name], within=f"{scaffold.project_name}"
             )
             load_package.save()
         else:
             load_package = PackageParser(os.path.join(scaffold.loads_path.files_dir))
             load_package.add_model(self.building_name)
             load_package.save()
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         package = PackageParser(scaffold.project_path)
-        if 'Loads' not in package.order:
-            package.add_model('Loads')
+        if "Loads" not in package.order:
+            package.add_model("Loads")
             package.save()
 
     def get_modelica_type(self, scaffold):
         district_params = self.system_parameters.get_param("district_system")
-        if 'fifth_generation' not in district_params:
-            return f'Loads.{self.building_name}.TimeSeriesBuilding'
+        if "fifth_generation" not in district_params:
+            return f"Loads.{self.building_name}.TimeSeriesBuilding"
         else:
-            return f'Loads.{self.building_name}.building'
+            return f"Loads.{self.building_name}.building"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/load_connectors/time_series_mft_ets_coupling.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,150 +3,156 @@
 
 import os
 import shutil
 from pathlib import Path
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.load_connectors.load_base import (
-    LoadBase
-)
-from geojson_modelica_translator.utils import ModelicaPath, simple_uuid
+from geojson_modelica_translator.model_connectors.load_connectors.load_base import LoadBase
+from geojson_modelica_translator.utils import ModelicaPath, mbl_version, simple_uuid
 
 
 class TimeSeriesMFT(LoadBase):
-    model_name = 'TimeSeriesMFT'
+    model_name = "TimeSeriesMFT"
 
     def __init__(self, system_parameters, geojson_load):
         super().__init__(system_parameters, geojson_load)
-        self.id = 'TimeSerMFTLoa_' + simple_uuid()
+        self.id = "TimeSerMFTLoa_" + simple_uuid()
 
         # Note that the order of the required MO files is important as it will be the order that
         # the "package.order" will be in.
         # self.required_mo_files.append(os.path.join(self.template_dir, 'getPeakMassFlowRate.mo'))
 
     def to_modelica(self, scaffold):
-        """
-        Create TimeSeries models based on the data in the building and geojson
+        """Create TimeSeries models based on the data in the building and geojson
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
 
         # MassFlowrate Temperature models
         time_series_mft_template = self.template_env.get_template("TimeSeriesMassFlowTemperatures.mot")
         peak_mfr_template = self.template_env.get_template("getPeakMassFlowRate.mot")
         templates = {"building.mo": time_series_mft_template, "getPeakMassFlowRate.mo": peak_mfr_template}
 
-        b_modelica_path = ModelicaPath(
-            self.building_name, scaffold.loads_path.files_dir, True
-        )
+        b_modelica_path = ModelicaPath(self.building_name, scaffold.loads_path.files_dir, True)
 
-        # grab the data from the system_parameter file for this building id
-        # TODO: create method in system_parameter class to make this easier and respect the defaults
-        time_series_filename = self.system_parameters.get_param_by_building_id(
+        # grab the data from the system_parameter file
+        time_series_filename = self.system_parameters.get_param_by_id(
             self.building_id, "load_model_parameters.time_series.filepath"
         )
 
         template_data = {
             "load_resources_path": b_modelica_path.resources_relative_dir,
             "time_series": {
                 "filepath": time_series_filename,
                 "filename": os.path.basename(time_series_filename),
                 "path": os.path.dirname(time_series_filename),
             },
             "nominal_values": {
-                "delTDisCoo": self.system_parameters.get_param_by_building_id(
+                "delTDisCoo": self.system_parameters.get_param_by_id(
                     self.building_id, "load_model_parameters.time_series.delTDisCoo"
                 ),
-                # FIXME: pick up default value from schema if not specified in system_parameters,
-                # FYI: Modelica insists on booleans being lowercase, so we need to explicitly set "true" and "false"
-                "has_liquid_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_liquid_heating",
-                ) else "false",
-                "has_liquid_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_liquid_cooling",
-                ) else "false",
-                "has_electric_heating": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_electric_heating",
-                ) else "false",
-                "has_electric_cooling": "true" if self.system_parameters.get_param_by_building_id(
-                    self.building_id, "load_model_parameters.time_series.has_electric_cooling",
-                ) else "false",
-            }
+            },
         }
 
+        # FYI: Modelica insists on booleans being lowercase, so we need to explicitly set "true" and "false"
+        if self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.time_series.has_liquid_heating",
+        ):
+            template_data["nominal_values"]["has_liquid_heating"] = "true"
+        else:
+            template_data["nominal_values"]["has_liquid_heating"] = "false"
+        if self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.time_series.has_liquid_cooling",
+        ):
+            template_data["nominal_values"]["has_liquid_cooling"] = "true"
+        else:
+            template_data["nominal_values"]["has_liquid_cooling"] = "false"
+        if self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.time_series.has_electric_heating",
+        ):
+            template_data["nominal_values"]["has_electric_heating"] = "true"
+        else:
+            template_data["nominal_values"]["has_electric_heating"] = "false"
+        if self.system_parameters.get_param_by_id(
+            self.building_id,
+            "load_model_parameters.time_series.has_electric_cooling",
+        ):
+            template_data["nominal_values"]["has_electric_cooling"] = "true"
+        else:
+            template_data["nominal_values"]["has_electric_cooling"] = "false"
+
         if os.path.exists(template_data["time_series"]["filepath"]):
             new_file = os.path.join(b_modelica_path.resources_dir, template_data["time_series"]["filename"])
             os.makedirs(os.path.dirname(new_file), exist_ok=True)
             shutil.copy(template_data["time_series"]["filepath"], new_file)
         else:
             raise Exception(f"Missing MOS file for time series: {template_data['time_series']['filepath']}")
 
         # Run templates to write actual Modelica models
-        ets_model_type = self.system_parameters.get_param_by_building_id(self.building_id, "ets_model")
+        ets_model_type = self.system_parameters.get_param_by_id(self.building_id, "ets_model")
 
         ets_data = None
         if ets_model_type == "Indirect Heating and Cooling":
-            ets_data = self.system_parameters.get_param_by_building_id(
-                self.building_id,
-                "ets_indirect_parameters"
-            )
+            ets_data = self.system_parameters.get_param_by_id(self.building_id, "ets_indirect_parameters")
         else:
             raise Exception("Only ETS Model of type 'Indirect Heating and Cooling' type enabled currently")
 
         # Run building templates to write actual Modelica models
         for template_filename, template in templates.items():
             self.run_template(
                 template=template,
                 save_file_name=Path(b_modelica_path.files_dir) / template_filename,
                 project_name=scaffold.project_name,
                 model_name=self.building_name,
                 data=template_data,
                 ets_data=ets_data,
             )
 
-        self.copy_required_mo_files(b_modelica_path.files_dir, within=f'{scaffold.project_name}.Loads')
+        self.copy_required_mo_files(b_modelica_path.files_dir, within=f"{scaffold.project_name}.Loads")
 
         # Run post process to create the remaining project files for this building
         self.post_process(scaffold)
 
     def post_process(self, scaffold):
-        """
-        Cleanup the export of TimeSeries files into a format suitable for the district-based analysis. This includes
+        """Cleanup the export of TimeSeries files into a format suitable for the district-based analysis. This includes
         the following:
             * Add a Loads project
             * Add a project level project
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         :return: None
         """
         order_files = [Path(mo).stem for mo in self.required_mo_files]
         order_files += self.template_files_to_include
         b_modelica_path = Path(scaffold.loads_path.files_dir) / self.building_name
         new_package = PackageParser.new_from_template(
-            path=b_modelica_path,
-            name=self.building_name,
-            order=order_files,
-            within=f"{scaffold.project_name}.Loads"
+            path=b_modelica_path, name=self.building_name, order=order_files, within=f"{scaffold.project_name}.Loads"
         )
         new_package.save()
 
         # now create the Loads level package and package.order.
-        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, 'package.mo')):
+        if not os.path.exists(os.path.join(scaffold.loads_path.files_dir, "package.mo")):
             load_package = PackageParser.new_from_template(
                 scaffold.loads_path.files_dir, "Loads", [self.building_name], within=f"{scaffold.project_name}"
             )
             load_package.save()
         else:
             load_package = PackageParser(os.path.join(scaffold.loads_path.files_dir))
             load_package.add_model(self.building_name)
             load_package.save()
 
         # now create the Package level package. This really needs to happen at the GeoJSON to modelica stage, but
         # do it here for now to aid in testing.
         pp = PackageParser.new_from_template(
-            scaffold.project_path, scaffold.project_name, ["Loads"]
+            scaffold.project_path,
+            scaffold.project_name,
+            ["Loads"],
+            mbl_version=mbl_version(),
         )
         pp.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Loads.{self.building_name}.building'
+        return f"Loads.{self.building_name}.building"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/model_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/model_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,72 +8,64 @@
 
 from jinja2 import Environment, FileSystemLoader, StrictUndefined, exceptions
 from modelica_builder.model import Model
 
 from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
-class ModelBase(object):
+class ModelBase:
     """Base class of the model connectors. The connectors can utilize various methods to create a building (or other
     feature) to a detailed Modelica connection. For example, a simple RC model (using TEASER), a ROM, CSV file, etc.
     """
+
     # model_name must be overridden in subclass
     model_name: Union[str, None] = None
 
     def __init__(self, system_parameters, template_dir):
-        """
-        Base initializer
+        """Base initializer
 
         :param system_parameters: SystemParameters object
         """
         self.system_parameters = system_parameters
 
         # initialize the templating framework (Jinja2)
         self.template_dir = template_dir
         self.template_env = Environment(
-            loader=FileSystemLoader(searchpath=self.template_dir),
-            undefined=StrictUndefined
+            loader=FileSystemLoader(searchpath=self.template_dir), undefined=StrictUndefined
         )
         self.template_env.filters.update(ALL_CUSTOM_FILTERS)
 
-        self._template_instance = f'{self.model_name}_Instance.mopt'
+        self._template_instance = f"{self.model_name}_Instance.mopt"
 
         # store a list of the templated files to include when building the package
         self.template_files_to_include = []
 
         # Note that the order of the required MO files is important as it will be the order that
         # the "package.order" will be in.
         self.required_mo_files = []
         # extract data out of the urbanopt_building object and store into the base object
 
         # Read district-level system params. Used when templating ets mofiles, for instance in heating_indirect.py
         if system_parameters is not None:
             # TODO: DRY up this handling of different generations
             district_params = self.system_parameters.get_param("district_system")
-            if 'fifth_generation' in district_params:
-                self.district_template_data = {
-                    # "temp_setpoint_hhw": district_params['fifth_generation']['central_heating_plant_parameters']['temp_setpoint_hhw'],
-                    # "temp_setpoint_chw": district_params['fifth_generation']['central_cooling_plant_parameters']['temp_setpoint_chw'],
-                }
-            elif 'fourth_generation' in district_params:
+            if "fourth_generation" in district_params:
                 self.district_template_data = {
-                    "temp_setpoint_hhw": district_params['fourth_generation']['central_heating_plant_parameters']['temp_setpoint_hhw'],
-                    "temp_setpoint_chw": district_params['fourth_generation']['central_cooling_plant_parameters']['temp_setpoint_chw'],
+                    "temp_setpoint_hhw": district_params["fourth_generation"]["central_heating_plant_parameters"][
+                        "temp_setpoint_hhw"
+                    ],
+                    "temp_setpoint_chw": district_params["fourth_generation"]["central_cooling_plant_parameters"][
+                        "temp_setpoint_chw"
+                    ],
                 }
 
     def ft2_to_m2(self, area_in_ft2: float) -> float:
-        """
-        Converts square feet to square meters
+        """Converts square feet to square meters
 
         :param area_in_ft2: Area in square feet to be converted to square meters
         """
         return area_in_ft2 * 0.092936
 
     def copy_required_mo_files(self, dest_folder, within=None):
         """Copy any required_mo_files to the destination and update the within clause if defined. The required mo
@@ -98,16 +90,15 @@
             else:
                 # simply copy the file over if no need to update within
                 result.append(shutil.copy(f, new_filename))
 
         return result
 
     def run_template(self, template, save_file_name, do_not_add_to_list=False, **kwargs):
-        """
-        Helper method to create the file from Jinja2's templating framework.
+        """Helper method to create the file from Jinja2's templating framework.
 
         :param template: object, Jinja template from the `template_env.get_template()` command.
         :param save_file_name: string, fully qualified path to save the rendered template to.
         :param do_not_add_to_list: boolean, set to true if you do not want the file to be added to the package.order
         :param kwargs: These are the arguments that need to be passed to the template.
 
         :return: None
@@ -140,33 +131,29 @@
         try:
             template = self.template_env.get_template(self._template_instance)
         except exceptions.TemplateNotFound:
             raise Exception(f"Could not find mopt template '{self._template_instance}' in {self.template_dir}")
 
         # get template path relative to the package
         template_filename = Path(template.filename).as_posix()
-        _, template_filename = template_filename.rsplit('geojson_modelica_translator', 1)
+        _, template_filename = template_filename.rsplit("geojson_modelica_translator", 1)
 
         return template.render(template_params), template_filename
 
     def to_dict(self, scaffold):
-        output_dict = {
-            'id': self.id,
-            'modelica_type': self.get_modelica_type(scaffold)
-        }
+        output_dict = {"id": self.id, "modelica_type": self.get_modelica_type(scaffold)}
         district_params = self.system_parameters.get_param("district_system")
-        if 'fifth_generation' in district_params:
+        if "fifth_generation" in district_params:
             # 'bui' is how a 5G model refers to the 4G model while the templates build the model.
             # 4G model is already self-sufficient so it needs that string to not exist.
             # This is templated in TimeSeries_Instance.mopt
             # FIXME: need a better variable name than 'is_5g_district' to be clearer in the template
-            # TODO: A better if statement using Jinja conditionals in the above file might allow us to remove the 'else' block here
-            output_dict['is_5g_district'] = 'bui'
+            output_dict["is_5g_district"] = "bui"
         else:
-            output_dict['is_5g_district'] = ''
+            output_dict["is_5g_district"] = ""
         return output_dict
 
     # This method needs to be defined in each of the derived model connectors
     # def get_modelica_type(self, scaffold)
 
     # This method needs to be defined in each of the derived model connectors
     # def to_modelica(self):
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_2_pipe.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.networks.network_base import (
-    NetworkBase
-)
-from geojson_modelica_translator.utils import simple_uuid
+from geojson_modelica_translator.model_connectors.networks.network_base import NetworkBase
 
 
-class Network2Pipe(NetworkBase):
-    model_name = 'Network2Pipe'
+class NetworkAmbientWaterStub(NetworkBase):
+    model_name = "NetworkAmbientWaterStub"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'disNet_' + simple_uuid()
+        self.id = "MyNetworkAmbientWaterStub"
 
     def to_modelica(self, scaffold):
-        """
+        """Convert the NetworkAmbientWaterStub to Modelica code
+
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
-        # no model to generate, its fully implemented in the Modelica Buildings library
+        # this stub has no model to generate, it's fully implemented in the coupling
 
     def get_modelica_type(self, scaffold):
-        return 'Buildings.Experimental.DHC.Networks.Distribution2Pipe'
+        """Get the Modelica type of the NetworkAmbientWaterStub
+
+        :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
+        """
+        # this stub has no model, so there's no type
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_ambient_water_stub.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_heated_water_stub.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.networks.network_base import (
-    NetworkBase
-)
+from geojson_modelica_translator.model_connectors.networks.network_base import NetworkBase
 
 
-class NetworkAmbientWaterStub(NetworkBase):
-    model_name = 'NetworkAmbientWaterStub'
+class NetworkHeatedWaterStub(NetworkBase):
+    model_name = "NetworkHeatedWaterStub"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'MyNetworkAmbientWaterStub'
+        self.id = "MyNetworkHeatedWaterStub"
 
     def to_modelica(self, scaffold):
-        """
+        """Convert the NetworkHeatedWaterStub to Modelica code
+
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         # this stub has no model to generate, its fully implemented in the coupling currently
 
     def get_modelica_type(self, scaffold):
         # this stub has no model, so there's no type
-        return 'UNIMPLEMENTED'
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_base.py`

 * *Files 21% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 
 from pathlib import Path
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 
 
 class NetworkBase(ModelBase):
-    """
-    Base class of the network connectors.
-    """
-    simple_gmt_type = 'network'
+    """Base class of the network connectors."""
+
+    simple_gmt_type = "network"
 
     def __init__(self, system_parameters):
-        super().__init__(system_parameters, Path(__file__).parent / 'templates')
+        super().__init__(system_parameters, Path(__file__).parent / "templates")
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_chilled_water_stub.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.networks.network_base import (
-    NetworkBase
-)
+from geojson_modelica_translator.model_connectors.networks.network_base import NetworkBase
 
 
 class NetworkChilledWaterStub(NetworkBase):
-    model_name = 'NetworkChilledWaterStub'
+    model_name = "NetworkChilledWaterStub"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'MyNetworkChilledWaterStub'
+        self.id = "MyNetworkChilledWaterStub"
 
     def to_modelica(self, scaffold):
-        """
+        """Convert the NetworkChilledWaterStub to Modelica code
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         # this stub has no model to generate, its fully implemented in the coupling currently
 
     def get_modelica_type(self, scaffold):
         # this stub has no model, so there's no type
-        return 'UNIMPLEMENTED'
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/network_distribution_pump.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/network_distribution_pump.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-from geojson_modelica_translator.model_connectors.networks.network_base import (
-    NetworkBase
-)
+from geojson_modelica_translator.model_connectors.networks.network_base import NetworkBase
 
 
 class NetworkDistributionPump(NetworkBase):
-    model_name = 'NetworkDistributionPump'
+    model_name = "NetworkDistributionPump"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'MyNetworkDistributionPump'
+        self.id = "MyNetworkDistributionPump"
 
     def to_modelica(self, scaffold):
-        """
+        """Convert the NetworkDistributionPump to Modelica code
+
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         # this stub has no model to generate, its fully implemented in the coupling currently
 
     def get_modelica_type(self, scaffold):
         # this stub has no model, so there's no type
-        return 'UNIMPLEMENTED'
+        return "UNIMPLEMENTED"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/Network2Pipe_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkAmbientWaterStub_Instance.mopt`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,12 @@
   // heated water stub
   // TODO: move these components into a single component
   {% for building in range( sys_params.num_buildings ) %}
-  Buildings.Fluid.Sources.MassFlowSource_T supHeaWat_{{ building + 1 }}(
+  Buildings.Fluid.Sources.Boundary_pT supHeaWat_{{ building + 1 }}(
     redeclare package Medium={{ globals.medium_w }},
-    use_m_flow_in=true,
     use_T_in=false,
     {% if 'ghe_parameters' in sys_params.district_system['fifth_generation'] %}
     T={{ sys_params.district_system.fifth_generation.ghe_parameters.soil.undisturbed_temp }}+273.15,
     {% else %}
     T={{ sys_params.district_system.fifth_generation.central_heating_plant_parameters.temp_setpoint_hhw }}+273.15,
     {% endif %}
     nPorts=1)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkChilledWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/networks/templates/NetworkHeatedWaterStub_Instance.mopt`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/borefield.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/borefield.py`

 * *Files 5% similar despite different names*

```diff
@@ -6,52 +6,45 @@
 import os
 from pathlib import Path
 
 import pandas as pd
 import scipy.io as sio
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.plants.plant_base import (
-    PlantBase
-)
+from geojson_modelica_translator.model_connectors.plants.plant_base import PlantBase
 from geojson_modelica_translator.utils import ModelicaPath, simple_uuid
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
 class Borefield(PlantBase):
-    model_name = 'Borefield'
+    model_name = "Borefield"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'borFie_' + simple_uuid()
-        self.borefield_name = 'Borefield_' + simple_uuid()
+        self.id = "borFie_" + simple_uuid()
+        self.borefield_name = "Borefield_" + simple_uuid()
 
-        self.required_mo_files.append(os.path.join(self.template_dir, 'GroundTemperatureResponse.mo'))
+        self.required_mo_files.append(os.path.join(self.template_dir, "GroundTemperatureResponse.mo"))
 
     def to_modelica(self, scaffold):
-        """
-        Create timeSeries models based on the data in the buildings and geojsons
+        """Convert the Borefield to Modelica code
+        Create timeSeries models based on the data in the buildings and GeoJSONs
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
 
         template_data = {
             "gfunction": {
                 "input_path": self.system_parameters.get_param(
                     "$.district_system.fifth_generation.ghe_parameters.ghe_dir"
                 ),
                 "ghe_id": self.system_parameters.get_param(
                     "$.district_system.fifth_generation.ghe_parameters.ghe_specific_params[0].ghe_id"
-                )
+                ),
             },
             "soil": {
                 "initial_ground_temperature": self.system_parameters.get_param(
                     "$.district_system.fifth_generation.ghe_parameters.soil.undisturbed_temp"
                 ),
                 "conductivity": self.system_parameters.get_param(
                     "$.district_system.fifth_generation.ghe_parameters.soil.conductivity"
@@ -105,109 +98,147 @@
                     "$.district_system.fifth_generation.ghe_parameters.pipe.shank_spacing"
                 ),
             },
         }
 
         # process g-function file
         if Path(template_data["gfunction"]["input_path"]).expanduser().is_absolute():
-            gfunction = pd.read_csv(Path(template_data["gfunction"]["input_path"]) / template_data["gfunction"]["ghe_id"] / "Gfunction.csv", header=0, usecols=[0, 2])
+            gfunction = pd.read_csv(
+                Path(template_data["gfunction"]["input_path"]) / template_data["gfunction"]["ghe_id"] / "Gfunction.csv",
+                header=0,
+                usecols=[0, 2],
+            )
         else:
             sys_param_dir = Path(self.system_parameters.filename).parent.resolve()
             try:
-                gfunction = pd.read_csv(sys_param_dir / template_data["gfunction"]["input_path"] / template_data["gfunction"]["ghe_id"] / "Gfunction.csv", header=0, usecols=[0, 2])
+                gfunction = pd.read_csv(
+                    sys_param_dir
+                    / template_data["gfunction"]["input_path"]
+                    / template_data["gfunction"]["ghe_id"]
+                    / "Gfunction.csv",
+                    header=0,
+                    usecols=[0, 2],
+                )
             except FileNotFoundError:
-                raise SystemExit(f'When using a relative path to your ghe_dir, your path \'{template_data["gfunction"]["input_path"]}\' must be relative to the dir your sys-param file is in.')
+                raise SystemExit(
+                    'When using a relative path to your ghe_dir, your path '
+                    f' \'{template_data["gfunction"]["input_path"]}\' must be relative to the dir your '
+                    'sys-param file is in.'
+                )
         template_data["gfunction"]["gfunction_file_rows"] = gfunction.shape[0] + 1
 
         # convert the values to match Modelica gfunctions
         for i in range(len(gfunction)):
-            gfunction[gfunction.columns[0]].iloc[i] = math.exp(gfunction[gfunction.columns[0]].iloc[i]) * template_data["configuration"]["borehole_height"]**2 / (9 * template_data["soil"]["conductivity"] / template_data["soil"]["volumetric_heat_capacity"])
-            gfunction[gfunction.columns[1]].iloc[i] = gfunction[gfunction.columns[1]].iloc[i] / (template_data["configuration"]["number_of_boreholes"] * 2 * math.pi * template_data["configuration"]["borehole_height"] * template_data["soil"]["conductivity"])
+            gfunction[gfunction.columns[0]].iloc[i] = (
+                math.exp(gfunction[gfunction.columns[0]].iloc[i])
+                * template_data["configuration"]["borehole_height"] ** 2
+                / (9 * template_data["soil"]["conductivity"] / template_data["soil"]["volumetric_heat_capacity"])
+            )
+            gfunction[gfunction.columns[1]].iloc[i] = gfunction[gfunction.columns[1]].iloc[i] / (
+                template_data["configuration"]["number_of_boreholes"]
+                * 2
+                * math.pi
+                * template_data["configuration"]["borehole_height"]
+                * template_data["soil"]["conductivity"]
+            )
 
         # add zeros to the first row
         new_row = pd.Series({gfunction.columns[0]: 0, gfunction.columns[1]: 0})
         gfunction = pd.concat([gfunction.iloc[:0], pd.DataFrame([new_row]), gfunction.iloc[0:]]).reset_index(drop=True)
 
         # create borefield package paths
         b_modelica_path = ModelicaPath(self.borefield_name, scaffold.plants_path.files_dir, True)
 
         # add to dict and save MAT file to the borefield's resources folder
-        data_dict = {'TStep': gfunction.values}
-        gfunction_path = os.path.join(b_modelica_path.resources_dir, 'Gfunction.mat')
+        data_dict = {"TStep": gfunction.to_numpy()}
+        gfunction_path = os.path.join(b_modelica_path.resources_dir, "Gfunction.mat")
         sio.savemat(gfunction_path, data_dict)
         template_data["gfunction"]["gfunction_file_path"] = b_modelica_path.resources_relative_dir + "/Gfunction.mat"
 
         # process nominal mass flow rate
         if template_data["configuration"]["flow_type"] == "system":
-            template_data["configuration"]["nominal_mass_flow_per_borehole"] = template_data["configuration"]["nominal_mass_flow_per_borehole"] / template_data["configuration"]["number_of_boreholes"]
+            template_data["configuration"]["nominal_mass_flow_per_borehole"] = (
+                template_data["configuration"]["nominal_mass_flow_per_borehole"]
+                / template_data["configuration"]["number_of_boreholes"]
+            )
 
         # process tube thickness
         if template_data["tube"]["outer_diameter"] and template_data["tube"]["inner_diameter"]:
-            template_data["tube"]["thickness"] = (template_data["tube"]["outer_diameter"] - template_data["tube"]["inner_diameter"]) / 2
+            template_data["tube"]["thickness"] = (
+                template_data["tube"]["outer_diameter"] - template_data["tube"]["inner_diameter"]
+            ) / 2
         else:
             template_data["tube"]["thickness"] = None
 
         # process shank spacing
         if template_data["tube"]["shank_spacing"] and template_data["tube"]["outer_diameter"]:
-            template_data["tube"]["shank_spacing"] = (template_data["tube"]["shank_spacing"] + template_data["tube"]["outer_diameter"]) / 2
+            template_data["tube"]["shank_spacing"] = (
+                template_data["tube"]["shank_spacing"] + template_data["tube"]["outer_diameter"]
+            ) / 2
         else:
             template_data["tube"]["shank_spacing"] = None
 
         # load templates
         oneutube_template = self.template_env.get_template("BorefieldOneUTube.mot")
         twoutube_template = self.template_env.get_template("BorefieldTwoUTubes.mot")
 
         if template_data["configuration"]["borehole_configuration"] == "singleutube":
             plant_template = oneutube_template
-            template_data["configuration"]["borehole_configuration"] = "Buildings.Fluid.Geothermal.Borefields.Types.BoreholeConfiguration.SingleUTube"
-            template_data["configuration"]["borehole_type"] = "Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.OneUTube"
+            template_data["configuration"]["borehole_configuration"] = (
+                "Buildings.Fluid.Geothermal.Borefields.Types.BoreholeConfiguration.SingleUTube"
+            )
+            template_data["configuration"]["borehole_type"] = (
+                "Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.OneUTube"
+            )
         elif template_data["configuration"]["borehole_configuration"] == "doubleutube":
             plant_template = twoutube_template
-            template_data["configuration"]["borehole_configuration"] = "Buildings.Fluid.Geothermal.Borefields.Types.BoreholeConfiguration.DoubleUTubeSeries"
-            template_data["configuration"]["borehole_type"] = "Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.TwoUTube"
+            template_data["configuration"]["borehole_configuration"] = (
+                "Buildings.Fluid.Geothermal.Borefields.Types.BoreholeConfiguration.DoubleUTubeSeries"
+            )
+            template_data["configuration"]["borehole_type"] = (
+                "Buildings.Fluid.Geothermal.Borefields.BaseClasses.Boreholes.TwoUTube"
+            )
         else:
             raise ValueError("The type of geothermal heat exchanger pipe arrangement is not supported.")
 
         self.run_template(
             plant_template,
             os.path.join(b_modelica_path.files_dir, "Borefield.mo"),
             project_name=scaffold.project_name,
             model_name=self.borefield_name,
-            ghe_data=template_data
+            ghe_data=template_data,
         )
 
         # generate Modelica package
         self.copy_required_mo_files(
-            dest_folder=scaffold.plants_path.files_dir,
-            within=f'{scaffold.project_name}.Plants')
+            dest_folder=scaffold.plants_path.files_dir, within=f"{scaffold.project_name}.Plants"
+        )
 
         # Borefield_ package
-        subpackage_models = ['Borefield']
+        subpackage_models = ["Borefield"]
         borefield_package = PackageParser.new_from_template(
             path=b_modelica_path.files_dir,
             name=self.borefield_name,
             order=subpackage_models,
-            within=f"{scaffold.project_name}.Plants"
+            within=f"{scaffold.project_name}.Plants",
         )
         borefield_package.save()
 
         # Plants package
         package = PackageParser(scaffold.project_path)
-        if 'Plants' not in package.order:
-            package.add_model('Plants')
+        if "Plants" not in package.order:
+            package.add_model("Plants")
             package.save()
 
         package_models = [self.borefield_name] + [Path(mo).stem for mo in self.required_mo_files]
         plants_package = PackageParser(scaffold.plants_path.files_dir)
         if plants_package.order_data is None:
             plants_package = PackageParser.new_from_template(
-                path=scaffold.plants_path.files_dir,
-                name="Plants",
-                order=package_models,
-                within=scaffold.project_name)
+                path=scaffold.plants_path.files_dir, name="Plants", order=package_models, within=scaffold.project_name
+            )
         else:
             for model_name in package_models:
                 plants_package.add_model(model_name)
         plants_package.save()
 
     def get_modelica_type(self, scaffold):
-        return f'Plants.{self.borefield_name}.Borefield'
+        return f"Plants.{self.borefield_name}.Borefield"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/chp.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/chp.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,43 +1,42 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 from pathlib import Path
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.plants.plant_base import (
-    PlantBase
-)
+from geojson_modelica_translator.model_connectors.plants.plant_base import PlantBase
 from geojson_modelica_translator.utils import convert_c_to_k, simple_uuid
 
 
 class HeatingPlantWithOptionalCHP(PlantBase):
-    model_name = 'HeatingPlant'
+    model_name = "HeatingPlant"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'chpPla_' + simple_uuid()
+        self.id = "chpPla_" + simple_uuid()
         self.chp_installed = self.system_parameters.get_param(
             "$.district_system.fourth_generation.central_heating_plant_parameters.chp_installed"
         )
         if self.chp_installed is not True:
-            self.required_mo_files.append(Path(self.template_dir) / 'CentralHeatingPlant.mo')
-            self.id = 'heaPla' + simple_uuid()
+            self.required_mo_files.append(Path(self.template_dir) / "CentralHeatingPlant.mo")
+            self.id = "heaPla" + simple_uuid()
 
-        self.required_mo_files.append(Path(self.template_dir) / 'Boiler_TParallel.mo')
-        self.required_mo_files.append(Path(self.template_dir) / 'BoilerStage.mo')
-        self.required_mo_files.append(Path(self.template_dir) / 'HeatingWaterPumpSpeed.mo')
-        self.required_mo_files.append(Path(self.template_dir) / 'PartialPlantParallel.mo')
-        self.required_mo_files.append(Path(self.template_dir) / 'PartialPlantParallelInterface.mo')
-        self.required_mo_files.append(Path(self.template_dir) / 'ValveParameters.mo')
+        self.required_mo_files.append(Path(self.template_dir) / "Boiler_TParallel.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "Boiler_TParallel_v10.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "BoilerStage.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "HeatingWaterPumpSpeed.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "PartialPlantParallel.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "PartialPlantParallel_v10.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "PartialPlantParallelInterface.mo")
+        self.required_mo_files.append(Path(self.template_dir) / "ValveParameters.mo")
 
     def to_modelica(self, scaffold):
-        """
-        Create timeSeries models based on the data in the buildings and geojsons
+        """Create time series models based on the data in the buildings and GeoJSONs
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         if self.chp_installed:
             template_data = {
                 "nominal_values": {
                     "heat_flow_nominal": self.system_parameters.get_param(
@@ -51,55 +50,57 @@
                     ),
                     "pressure_drop_hhw_nominal": self.system_parameters.get_param(
                         "$.district_system.fourth_generation.central_heating_plant_parameters.pressure_drop_hhw_nominal"
                     ),
                     "pressure_drop_setpoint": self.system_parameters.get_param(
                         "$.district_system.fourth_generation.central_heating_plant_parameters.pressure_drop_setpoint"
                     ),
-                    "temp_setpoint_hhw": convert_c_to_k(self.system_parameters.get_param(
-                        "$.district_system.fourth_generation.central_heating_plant_parameters.temp_setpoint_hhw"
-                    )),
+                    "temp_setpoint_hhw": convert_c_to_k(
+                        self.system_parameters.get_param(
+                            "$.district_system.fourth_generation.central_heating_plant_parameters.temp_setpoint_hhw"
+                        )
+                    ),
                     "pressure_drop_hhw_valve_nominal": self.system_parameters.get_param(
                         "$.district_system.fourth_generation.central_heating_plant_parameters.pressure_drop_hhw_valve_nominal"
                     ),
                 },
                 "signals": {
-                    "thermal_following": str(self.system_parameters.get_param(
-                        "$.district_system.fourth_generation.central_heating_plant_parameters.chp_thermal_following"
-                    )).lower(),  # Booleans in Python start with a capital letter. Modelica wants it lowercase, hence this.
+                    "thermal_following": str(
+                        self.system_parameters.get_param(
+                            "$.district_system.fourth_generation.central_heating_plant_parameters.chp_thermal_following"
+                        )
+                    ).lower(),  # Booleans in Python start with a capital letter but are lowercase in Modelica.
                 },
             }
             plant_template = self.template_env.get_template("HeatingPlantWithCHP.mot")
             self.run_template(
                 template=plant_template,
                 save_file_name=Path(scaffold.plants_path.files_dir) / "CentralHeatingPlant.mo",
                 project_name=scaffold.project_name,
-                data=template_data
+                data=template_data,
             )
 
         self.copy_required_mo_files(
-            dest_folder=scaffold.plants_path.files_dir,
-            within=f'{scaffold.project_name}.Plants')
+            dest_folder=scaffold.plants_path.files_dir, within=f"{scaffold.project_name}.Plants"
+        )
 
         package = PackageParser(scaffold.project_path)
-        if 'Plants' not in package.order:
-            package.add_model('Plants')
+        if "Plants" not in package.order:
+            package.add_model("Plants")
             package.save()
 
         if self.chp_installed:
-            package_models = ['CentralHeatingPlant'] + [Path(mo).stem for mo in self.required_mo_files]
+            package_models = ["CentralHeatingPlant"] + [Path(mo).stem for mo in self.required_mo_files]
         else:
             package_models = [Path(mo).stem for mo in self.required_mo_files]
         plants_package = PackageParser(scaffold.plants_path.files_dir)
         if plants_package.order_data is None:
             plants_package = PackageParser.new_from_template(
-                path=scaffold.plants_path.files_dir,
-                name="Plants",
-                order=package_models,
-                within=scaffold.project_name)
+                path=scaffold.plants_path.files_dir, name="Plants", order=package_models, within=scaffold.project_name
+            )
         else:
             for model_name in package_models:
                 plants_package.add_model(model_name)
         plants_package.save()
 
     def get_modelica_type(self, scaffold):
-        return 'Plants.CentralHeatingPlant'
+        return "Plants.CentralHeatingPlant"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/cooling_plant.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/cooling_plant.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,59 +3,54 @@
 
 import os
 import shutil
 from pathlib import Path
 
 from modelica_builder.package_parser import PackageParser
 
-from geojson_modelica_translator.model_connectors.plants.plant_base import (
-    PlantBase
-)
+from geojson_modelica_translator.model_connectors.plants.plant_base import PlantBase
 from geojson_modelica_translator.utils import simple_uuid
 
 
 class CoolingPlant(PlantBase):
-    model_name = 'CoolingPlant'
+    model_name = "CoolingPlant"
 
     def __init__(self, system_parameters):
         super().__init__(system_parameters)
-        self.id = 'cooPla_' + simple_uuid()
+        self.id = "cooPla_" + simple_uuid()
 
-        self.required_mo_files.append(os.path.join(self.template_dir, 'CoolingTowerWithBypass.mo'))
-        self.required_mo_files.append(os.path.join(self.template_dir, 'CoolingTowerParallel.mo'))
-        self.required_mo_files.append(os.path.join(self.template_dir, 'ChilledWaterPumpSpeed.mo'))
-        self.required_mo_files.append(os.path.join(self.template_dir, 'ChillerStage.mo'))
+        self.required_mo_files.append(os.path.join(self.template_dir, "CoolingTowerWithBypass.mo"))
+        self.required_mo_files.append(os.path.join(self.template_dir, "CoolingTowerParallel.mo"))
+        self.required_mo_files.append(os.path.join(self.template_dir, "ChilledWaterPumpSpeed.mo"))
+        self.required_mo_files.append(os.path.join(self.template_dir, "ChillerStage.mo"))
 
     def to_modelica(self, scaffold):
-        """
-        Create timeSeries models based on the data in the buildings and geojsons
+        """Create time series models based on the data in the buildings and GeoJSONs
 
         :param scaffold: Scaffold object, Scaffold of the entire directory of the project.
         """
         weather_filepath = Path(self.system_parameters.get_param("$.weather"))
 
         # verify that the weather file exists
         if not weather_filepath.exists():
-            raise FileNotFoundError(
-                f"Missing MOS weather file for CoolingPlant: {str(weather_filepath)}")
+            raise FileNotFoundError(f"Missing MOS weather file for CoolingPlant: {weather_filepath!s}")
         else:
             # copy the weather file to resources for the Plant and
             # update the string that will be in the .mo file (weather_file_modelica_string)
-            shutil.copy(
-                str(weather_filepath),
-                os.path.join(scaffold.plants_path.resources_dir, weather_filepath.name)
+            shutil.copy(str(weather_filepath), os.path.join(scaffold.plants_path.resources_dir, weather_filepath.name))
+            weather_file_modelica_string = (
+                f"modelica://{scaffold.project_name}/"
+                f"{scaffold.plants_path.resources_relative_dir}/"
+                f"{weather_filepath.name}"
             )
-            weather_file_modelica_string = f'modelica://{scaffold.project_name}/' \
-                                           f'{scaffold.plants_path.resources_relative_dir}/' \
-                                           f'{weather_filepath.name}'
 
         template_data = {
             "nominal_values": {
                 "delta_temp": self.system_parameters.get_param(
-                    "$.district_system.fourth_generation.central_cooling_plant_parameters.cooling_tower_water_temperature_difference_nominal"  # noqa: E501
+                    "$.district_system.fourth_generation.central_cooling_plant_parameters.cooling_tower_water_temperature_difference_nominal"
                 ),
                 "fan_power": self.system_parameters.get_param(
                     "$.district_system.fourth_generation.central_cooling_plant_parameters.cooling_tower_fan_power_nominal"
                 ),
                 "chilled_water_pump_pressure_head": self.system_parameters.get_param(
                     "$.district_system.fourth_generation.central_cooling_plant_parameters.chw_pump_head"
                 ),
@@ -111,34 +106,32 @@
         }
 
         plant_template = self.template_env.get_template("CentralCoolingPlant.mot")
         self.run_template(
             plant_template,
             os.path.join(scaffold.plants_path.files_dir, "CentralCoolingPlant.mo"),
             project_name=scaffold.project_name,
-            data=template_data
+            data=template_data,
         )
 
         self.copy_required_mo_files(
-            dest_folder=scaffold.plants_path.files_dir,
-            within=f'{scaffold.project_name}.Plants')
+            dest_folder=scaffold.plants_path.files_dir, within=f"{scaffold.project_name}.Plants"
+        )
 
         package = PackageParser(scaffold.project_path)
-        if 'Plants' not in package.order:
-            package.add_model('Plants')
+        if "Plants" not in package.order:
+            package.add_model("Plants")
             package.save()
 
-        package_models = ['CentralCoolingPlant'] + [Path(mo).stem for mo in self.required_mo_files]
+        package_models = ["CentralCoolingPlant"] + [Path(mo).stem for mo in self.required_mo_files]
         plants_package = PackageParser(scaffold.plants_path.files_dir)
         if plants_package.order_data is None:
             plants_package = PackageParser.new_from_template(
-                path=scaffold.plants_path.files_dir,
-                name="Plants",
-                order=package_models,
-                within=scaffold.project_name)
+                path=scaffold.plants_path.files_dir, name="Plants", order=package_models, within=scaffold.project_name
+            )
         else:
             for model_name in package_models:
                 plants_package.add_model(model_name)
         plants_package.save()
 
     def get_modelica_type(self, scaffold):
-        return 'Plants.CentralCoolingPlant'
+        return "Plants.CentralCoolingPlant"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/plant_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/plant_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,13 @@
 
 from pathlib import Path
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 
 
 class PlantBase(ModelBase):
-    """
-    Base class of the central plants.
-    """
-    simple_gmt_type = 'plant'
+    """Base class of the central plants."""
+
+    simple_gmt_type = "plant"
 
     def __init__(self, system_parameters):
-        super().__init__(system_parameters, Path(__file__).parent / 'templates')
+        super().__init__(system_parameters, Path(__file__).parent / "templates")
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BoilerStage.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/Boiler_TParallel.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldOneUTube.mot`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
   Modelica.Blocks.Interfaces.RealOutput TBorAve(
     final quantity="ThermodynamicTemperature",
     final unit="K",
     displayUnit="degC",
     start=TExt0_start)
     "Average borehole wall temperature in the borefield"
     annotation (Placement(transformation(extent={{100,34},{120,54}})));
+  Buildings.Controls.OBC.CDL.Interfaces.RealOutput Q_flow(
+    final unit="W")
+    "Rate at which heat is extracted from soil"
+    annotation (Placement(transformation(extent={{100,-50},{120,-30}}),iconTransformation(extent={{100,-64},{140,-24}})));
   {% endraw %}{{ project_name }}.Plants.GroundTemperatureResponse groTemRes(
     {% raw %}final tLoaAgg=tLoaAgg,
     final nCel=nCel,
     final borFieDat=borFieDat,
     final forceGFunCalc=forceGFunCalc,
     final gFunFilNam=gFunFilNam,
     final nTimTot=nTimTot)
@@ -207,14 +211,16 @@
     annotation (Line(points={{31,30},{36,30},{36,16},{48,16}},color={0,0,127}));
   connect(QBorHol.port_b,TemBorWal.port)
     annotation (Line(points={{4.44089e-16,0},{0,0},{0,4},{80,4},{80,16},{70,16}},color={191,0,0}));
   connect(TSoiDis.y,AveTBor.u)
     annotation (Line(points={{31,30},{36,30},{36,44},{48,44}},color={0,0,127}));
   connect(AveTBor.y,TBorAve)
     annotation (Line(points={{71,44},{110,44}},color={0,0,127}));
+  connect(gaiQ_flow.y,Q_flow)
+    annotation (Line(points={{1,80},{12,80},{12,60},{94,60},{94,-40},{110,-40}},color={0,0,127}));
   annotation (
     Icon(
       coordinateSystem(
         preserveAspectRatio=false,
         extent={{-100,-100},{100,100}}),
       graphics={
         Rectangle(
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/BorefieldTwoUTubes.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/BorefieldTwoUTubes.mot`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
   Modelica.Blocks.Interfaces.RealOutput TBorAve(
     final quantity="ThermodynamicTemperature",
     final unit="K",
     displayUnit="degC",
     start=TExt0_start)
     "Average borehole wall temperature in the borefield"
     annotation (Placement(transformation(extent={{100,34},{120,54}})));
+  Buildings.Controls.OBC.CDL.Interfaces.RealOutput Q_flow(
+    final unit="W")
+    "Rate at which heat is extracted from soil"
+    annotation (Placement(transformation(extent={{100,-50},{120,-30}}),iconTransformation(extent={{100,-64},{140,-24}})));
   {% endraw %}{{ project_name }}.Plants.GroundTemperatureResponse groTemRes(
     {% raw %}final tLoaAgg=tLoaAgg,
     final nCel=nCel,
     final borFieDat=borFieDat,
     final forceGFunCalc=forceGFunCalc,
     final gFunFilNam=gFunFilNam,
     final nTimTot=nTimTot)
@@ -207,14 +211,16 @@
     annotation (Line(points={{31,30},{36,30},{36,16},{48,16}},color={0,0,127}));
   connect(QBorHol.port_b,TemBorWal.port)
     annotation (Line(points={{4.44089e-16,0},{0,0},{0,4},{80,4},{80,16},{70,16}},color={191,0,0}));
   connect(TSoiDis.y,AveTBor.u)
     annotation (Line(points={{31,30},{36,30},{36,44},{48,44}},color={0,0,127}));
   connect(AveTBor.y,TBorAve)
     annotation (Line(points={{71,44},{110,44}},color={0,0,127}));
+  connect(gaiQ_flow.y,Q_flow)
+    annotation (Line(points={{1,80},{12,80},{12,60},{94,60},{94,-40},{110,-40}},color={0,0,127}));
   annotation (
     Icon(
       coordinateSystem(
         preserveAspectRatio=false,
         extent={{-100,-100},{100,100}}),
       graphics={
         Rectangle(
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CentralCoolingPlant.mot`

 * *Files 1% similar despite different names*

```diff
@@ -254,14 +254,15 @@
     p=Medium.p_default,
     X=Medium.X_default)
     "Medium state at default properties";
   final parameter Modelica.Units.SI.SpecificHeatCapacity cp_default=Medium.specificHeatCapacityCp(
     sta_default)
     "Specific heat capacity of the fluid";
 equation
+  connect(on,CHWPumCon.u);
   connect(weaDat.weaBus,weaBus)
     annotation (Line(points={{-120,-70},{-100,-70},{-100,-52}},color={255,204,51},thickness=0.5));
   connect(senTCHWSup.port_b,port_b)
     annotation (Line(points={{140,-50},{160,-50}},color={0,127,255}));
   connect(senMasFloByp.port_b,valByp.port_a)
     annotation (Line(points={{80,-20},{80,-10}},color={0,127,255}));
   connect(senMasFloByp.port_a,senTCHWSup.port_a)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CentralHeatingPlant.mo`

 * *Files 2% similar despite different names*

```diff
@@ -69,15 +69,15 @@
   Modelica.Blocks.Interfaces.BooleanInput on
     "On signal of the plant"
     annotation (Placement(transformation(extent={{-160,58},{-140,78}}),iconTransformation(extent={{-140,60},{-100,100}})));
   Modelica.Blocks.Interfaces.RealInput dpMea(
     final unit="Pa")
     "Measured pressure difference"
     annotation (Placement(transformation(extent={{-160,-40},{-140,-20}}),iconTransformation(extent={{-140,-50},{-100,-10}})));
-  Boiler_TParallel boiHotWat(
+  Boiler_TParallel_v10 boiHotWat(
     redeclare package Medium=Medium,
     m_flow_nominal=mBoi_flow_nominal,
     Q_flow_nominal=QBoi_flow_nominal,
     dp_nominal=dpBoi_nominal,
     numBoi=numBoi)
     "Parallel boilers."
     annotation (Placement(transformation(extent={{10,-60},{30,-40}})));
@@ -157,14 +157,15 @@
     displayUnit="degC")
     "Heating water setpoint."
     annotation (Placement(transformation(extent={{-160,-60},{-140,-40}}),iconTransformation(extent={{-140,-104},{-100,-64}})));
   Modelica.Blocks.Math.Product pumOn[numBoi]
     "Output pump speed"
     annotation (Placement(transformation(extent={{-80,0},{-60,20}})));
 equation
+  connect(on,heaWatPumCon.ON);
   connect(THeaSet,boiHotWat.THeaWatSet)
     annotation (Line(points={{-150,-50},{-72,-50},{-72,-56},{9,-56}},color={0,0,127}));
   connect(on,boiStaCon.on)
     annotation (Line(points={{-150,68},{-121,68}},color={255,0,255}));
   connect(dpMea,heaWatPumCon.dpMea)
     annotation (Line(points={{-150,-30},{-138,-30},{-138,-35},{-121,-35}},color={0,0,127}));
   connect(valByp.port_a,senMasFloByp.port_b)
@@ -201,16 +202,14 @@
     annotation (Line(points={{32,61},{32,86},{-126,86},{-126,76.6},{-121,76.6}},color={0,0,127}));
   connect(boiStaCon.y,pumOn.u1)
     annotation (Line(points={{-99,66},{-92,66},{-92,16},{-82,16}},color={0,0,127}));
   connect(heaWatPumCon.y,pumOn.u2)
     annotation (Line(points={{-99,-30},{-94,-30},{-94,4},{-82,4}},color={0,0,127}));
   connect(pumOn.y,pumHW.u)
     annotation (Line(points={{-59,10},{-46,10},{-46,72},{12,72},{12,54},{2,54}},color={0,0,127}));
-  connect(boiStaCon.y_On,heaWatPumCon.ON)
-    annotation (Line(points={{-99,70.6},{-88,70.6},{-88,24},{-128,24},{-128,-23.4},{-121,-23.4}},color={255,0,255}));
   connect(mPum_flow.y,heaWatPumCon.masFloPum)
     annotation (Line(points={{-121,40},{-134,40},{-134,-25.6},{-121,-25.6}},color={0,0,127}));
   annotation (
     Diagram(
       coordinateSystem(
         preserveAspectRatio=false,
         extent={{-140,-80},{120,100}})),
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ChilledWaterPumpSpeed.mo`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,17 @@
     k=1/dpSetPoi)
     "Multiplier gain for normalizing dp input"
     annotation (Placement(transformation(extent={{-80,-50},{-60,-30}})));
   Modelica.Blocks.Sources.Constant dpSetSca(
     k=1)
     "Scaled differential pressure setpoint"
     annotation (Placement(transformation(extent={{-100,-10},{-80,10}})));
+  Modelica.Blocks.Interfaces.BooleanInput u;
 equation
+  connect(u,pumStaCon.on);
   connect(pumStaCon.masFloPum,masFloPum)
     annotation (Line(points={{-12,8},{-20,8},{-20,40},{-120,40}},color={0,0,127}));
   connect(conPID.y,pumStaCon.speSig)
     annotation (Line(points={{-39,0},{-20,0},{-20,4},{-12,4}},color={0,0,127}));
   connect(pumStaCon.y,pumSpe.u1)
     annotation (Line(points={{11,0},{28,0},{28,6},{38,6}},color={0,0,127}));
   connect(conPID.y,pumSpe[1].u2)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ChillerStage.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingPlant_Instance.mopt` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlant_Instance.mopt`

 * *Files 22% similar despite different names*

```diff
@@ -1,58 +1,37 @@
-  parameter Modelica.Units.SI.MassFlowRate mCHW_flow_nominal_{{ model.id }}={{ model.id }}.numChi*({{ model.id }}.perChi.mEva_flow_nominal)
-    "Nominal chilled water mass flow rate";
-  parameter Modelica.Units.SI.MassFlowRate mCW_flow_nominal_{{ model.id }}={{ model.id }}.perChi.mCon_flow_nominal
-    "Nominal condenser water mass flow rate";
-  parameter Modelica.Units.SI.PressureDifference dpCHW_nominal_{{ model.id }}=44.8*1000
-    "Nominal chilled water side pressure";
-  parameter Modelica.Units.SI.PressureDifference dpCW_nominal_{{ model.id }}=46.2*1000
-    "Nominal condenser water side pressure";
-  parameter Modelica.Units.SI.Power QEva_nominal_{{ model.id }}=mCHW_flow_nominal_{{ model.id }}*4200*(5-14)
-    "Nominal cooling capaciaty (Negative means cooling)";
-  parameter Modelica.Units.SI.MassFlowRate mMin_flow_{{ model.id }}=0.2*mCHW_flow_nominal_{{ model.id }}/{{ model.id }}.numChi
-    "Minimum mass flow rate of single chiller";
-  // control settings
-  parameter Modelica.Units.SI.Pressure dpSetPoi_{{ model.id }}=70000
-    "Differential pressure setpoint";
-  parameter Modelica.Units.SI.Pressure pumDP_{{ model.id }}=dpCHW_nominal_{{ model.id }}+dpSetPoi_{{ model.id }}+200000;
+  // heating plant instance
+  parameter Modelica.Units.SI.MassFlowRate mHW_flow_nominal_{{ model.id }}=mBoi_flow_nominal_{{ model.id }}*{{ model.id }}.numBoi
+    "Nominal heating water mass flow rate";
+  parameter Modelica.Units.SI.MassFlowRate mBoi_flow_nominal_{{ model.id }}=QBoi_nominal_{{ model.id }}/(4200*{{ model.id }}.delT_nominal)
+    "Nominal heating water mass flow rate";
+  parameter Modelica.Units.SI.Power QBoi_nominal_{{ model.id }}=Q_flow_nominal_{{ model.id }}/{{ model.id }}.numBoi
+    "Nominal heating capaciaty";
+  parameter Modelica.Units.SI.HeatFlowRate Q_flow_nominal_{{ model.id }}=1000000*2
+    "Heating load";
+  parameter Modelica.Units.SI.MassFlowRate mMin_flow_{{ model.id }}=0.2*mBoi_flow_nominal_{{ model.id }}
+    "Minimum mass flow rate of single boiler";
+  // controls
+  parameter Modelica.Units.SI.Pressure pumDP=({{ model.id }}.dpBoi_nominal+dpSetPoi_{{ couplings.network_couplings[0].network.id }}+50000)
+    "Heating water pump pressure drop";
   parameter Modelica.Units.SI.Time tWai_{{ model.id }}=30
     "Waiting time";
-  // pumps
-  parameter Buildings.Fluid.Movers.Data.Generic perCHWPum_{{ model.id }}(
+  parameter Buildings.Fluid.Movers.Data.Generic perHWPum_{{ model.id }}(
     pressure=Buildings.Fluid.Movers.BaseClasses.Characteristics.flowParameters(
-      V_flow=((mCHW_flow_nominal_{{ model.id }}/numberofchillers)/1000)*{0.1,1,1.2},
-      dp=pumDP_{{ model.id }}*{1.2,1,0.1}))
-    "Performance data for chilled water pumps";
-  parameter Buildings.Fluid.Movers.Data.Generic perCWPum_{{ model.id }}(
-    pressure=Buildings.Fluid.Movers.BaseClasses.Characteristics.flowParameters(
-      V_flow=mCW_flow_nominal_{{ model.id }}/1000*{0.2,0.6,1.0,1.2},
-      dp=(dpCW_nominal_{{ model.id }}+60000+6000)*{1.2,1.1,1.0,0.6}))
-    "Performance data for condenser water pumps";
-
-
-  Modelica.Blocks.Sources.RealExpression TSetChiWatDis_{{ model.id }}(
-    y=5+273.15)
-    "Chilled water supply temperature set point on district level."
-    annotation (Placement({{ diagram.transformation.t_set_chi_wat_dis.real_expression }}));
-  Modelica.Blocks.Sources.BooleanConstant on_{{ model.id }}
-    "On signal of the plant"
-    annotation (Placement({{ diagram.transformation.on.boolean_constant }}));
+      V_flow=15/1000*{0.1,1.1},
+      dp=1000*{1.1,0.1}))
+    "Performance data for heating water pumps";
 
   {{ model.modelica_type }} {{ model.id }}(
-    numChi = numberofchillers,
-    redeclare Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_Carrier_19EX_5208kW_6_88COP_Vanes perChi,
-    perCHWPum=perCHWPum_{{ model.id }},
-    perCWPum=perCWPum_{{ model.id }},
-    mCHW_flow_nominal=mCHW_flow_nominal_{{ model.id }},
-    dpCHW_nominal=dpCHW_nominal_{{ model.id }},
-    QEva_nominal=QEva_nominal_{{ model.id }},
+    perHWPum=perHWPum_{{ model.id }},
+    mHW_flow_nominal=mHW_flow_nominal_{{ model.id }},
+    QBoi_flow_nominal=QBoi_nominal_{{ model.id }},
     mMin_flow=mMin_flow_{{ model.id }},
-    mCW_flow_nominal=mCW_flow_nominal_{{ model.id }},
-    dpCW_nominal=dpCW_nominal_{{ model.id }},
-    TAirInWB_nominal=298.7,
-    TCW_nominal=308.15,
-    TMin=288.15,
+    mBoi_flow_nominal=mBoi_flow_nominal_{{ model.id }},
+    dpBoi_nominal=10000,
+    delT_nominal(
+      displayUnit="degC")=15,
     tWai=tWai_{{ model.id }},
-    dpSetPoi=dpSetPoi_{{ model.id }}
+    // TODO: we're currently grabbing dpSetPoi from the Network instance -- need feedback to determine if that's the proper "home" for it
+    dpSetPoi=dpSetPoi_{{ couplings.network_couplings[0].network.id }}
     )
-    "District cooling plant."
-    annotation (Placement({{ diagram.transformation.cooling_plant.plant }}));
+    "District heating plant."
+    annotation (Placement({{ diagram.transformation.heating_plant.plant }}));
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerParallel.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/CoolingTowerWithBypass.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/GroundTemperatureResponse.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/GroundTemperatureResponse.mo`

 * *Files 2% similar despite different names*

```diff
@@ -13,14 +13,16 @@
     "Record containing all the parameters of the borefield model"
     annotation (choicesAllMatching=true,Placement(transformation(extent={{-80,-80},{-60,-60}})));
   parameter String gFunFilNam=Modelica.Utilities.Files.loadResource(
     "modelica://GHP/Resources/Data/System/SampleGFunction.mat")
     "File name of g-function data file in MAT format";
   parameter Integer nTimTot=76
     "Total length of g-function vector";
+  Boolean writegFun
+    "True if g-function was succesfully written to file";
   Modelica.Blocks.Interfaces.RealOutput delTBor(
     unit="K")
     "Temperature difference current borehole wall temperature minus initial borehole wall temperature"
     annotation (Placement(transformation(extent={{100,-14},{126,12}}),iconTransformation(extent={{100,-10},{120,10}})));
   Modelica.Blocks.Interfaces.RealInput QBor_flow(
     unit="W")
     "Heat flow from all boreholes combined (positive if heat from fluid into soil)"
@@ -140,15 +142,25 @@
       nSeg=nSeg,
       nTimSho=nTimSho,
       nTimLon=nTimLon,
       nTimTot=nTimTot,
       ttsMax=ttsMax,
       sha=SHAgfun,
       forceGFunCalc=forceGFunCalc);
-*/equation
+*/algorithm
+  Modelica.Utilities.Files.createDirectory(
+    "tmp");
+  Modelica.Utilities.Files.createDirectory(
+    "tmp/temperatureResponseMatrix");
+  writegFun := Modelica.Utilities.Streams.writeRealMatrix(
+    fileName="tmp/temperatureResponseMatrix/TStep.mat",
+    matrixName="TStep",
+    matrix=timSer,
+    append=false);
+equation
   der(
     delTBor)=dTStepdt*QBor_flow+derDelTBor0;
   der(
     U)=QBor_flow;
   when sample(
     t_start,
     tLoaAgg) then
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingPlantWithCHP.mot`

 * *Files 1% similar despite different names*

```diff
@@ -69,15 +69,15 @@
   Modelica.Blocks.Interfaces.BooleanInput on
     "On signal of the plant"
     annotation (Placement(transformation(extent={{-160,58},{-140,78}}),iconTransformation(extent={{-140,60},{-100,100}})));
   Modelica.Blocks.Interfaces.RealInput dpMea(
     final unit="Pa")
     "Measured pressure difference"
     annotation (Placement(transformation(extent={{-160,-40},{-140,-20}}),iconTransformation(extent={{-140,-50},{-100,-10}})));
-  Boiler_TParallel boiHotWat(
+  Boiler_TParallel_v10 boiHotWat(
     redeclare package Medium=Medium,
     m_flow_nominal=mBoi_flow_nominal,
     Q_flow_nominal=QBoi_flow_nominal,
     dp_nominal=dpBoi_nominal,
     numBoi=numBoi)
     "Parallel boilers."
     annotation (Placement(transformation(extent={{10,-60},{30,-40}})));
@@ -169,18 +169,17 @@
     annotation (Placement(transformation(extent={{-80,28},{-60,48}})));
   Modelica.Blocks.Sources.Constant ElePowDem(
     k=5500)
     annotation (Placement(transformation(extent={{-120,82},{-100,102}})));
   Modelica.Blocks.Sources.Constant TWatOutSet(
     k=273.15+60)
     annotation (Placement(transformation(extent={{-120,52},{-100,72}})));
-  Buildings.Fluid.Movers.FlowControlled_m_flow fan(
+  Buildings.Fluid.Movers.Preconfigured.FlowControlled_m_flow fan(
     redeclare package Medium=Medium,
-    m_flow_nominal=0.4,
-    nominalValuesDefineDefaultPressureCurve=true)
+    m_flow_nominal=0.4)
     annotation (Placement(transformation(extent={{-172,-132},{-152,-110}})));
   Buildings.HeatTransfer.Sources.FixedTemperature preTem(
     T(
       displayUnit="K")=273.15+25)
     annotation (Placement(transformation(extent={{-160,-180},{-140,-160}})));
 protected
   {% endraw %} Modelica.Blocks.Sources.BooleanExpression theFolSig(
@@ -236,15 +235,15 @@
     annotation (Line(points={{32,61},{32,86},{-126,86},{-126,76.6},{-121,76.6}},color={0,0,127}));
   connect(boiStaCon.y,pumOn.u1)
     annotation (Line(points={{-99,66},{-92,66},{-92,16},{-82,16}},color={0,0,127}));
   connect(heaWatPumCon.y,pumOn.u2)
     annotation (Line(points={{-99,-30},{-94,-30},{-94,4},{-82,4}},color={0,0,127}));
   connect(pumOn.y,pumHW.u)
     annotation (Line(points={{-59,10},{-46,10},{-46,72},{12,72},{12,54},{2,54}},color={0,0,127}));
-  connect(boiStaCon.y_On,heaWatPumCon.ON)
+  connect(on,heaWatPumCon.ON)
     annotation (Line(points={{-99,70.6},{-88,70.6},{-88,24},{-128,24},{-128,-23.4},{-121,-23.4}},color={255,0,255}));
   connect(mPum_flow.y,heaWatPumCon.masFloPum)
     annotation (Line(points={{-121,40},{-134,40},{-134,-25.6},{-121,-25.6}},color={0,0,127}));
   connect(theFolSig.y,eleFol.avaSig)
     annotation (Line(points={{-139,58},{-128,58},{-128,-139},{-120,-139}},color={255,0,255}));
   connect(port_a,fan.port_a)
     annotation (Line(points={{160,50},{-190,50},{-190,-121},{-172,-121}},color={0,127,255}));
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/HeatingWaterPumpSpeed.mo`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
   Buildings.Controls.OBC.CDL.Interfaces.RealInput meaFloByPas(
     final unit="kg/s")
     "Measured  bypass mass flow."
     annotation (Placement(transformation(extent={{-120,-98},{-100,-78}}),iconTransformation(extent={{-120,-98},{-100,-78}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealOutput deCouVal
     "Decoupler line valve."
     annotation (Placement(transformation(extent={{100,-60},{120,-40}})));
-  Buildings.Controls.OBC.CDL.Interfaces.BooleanInput ON[numPum]
+  Buildings.Controls.OBC.CDL.Interfaces.BooleanInput ON
     "Boiler on/off signal."
     annotation (Placement(transformation(extent={{-120,76},{-100,96}}),iconTransformation(extent={{-120,56},{-100,76}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealInput masFloPum(
     final unit="kg/s")
     "Total mass flowrate of heating water pumps"
     annotation (Placement(transformation(extent={{-120,34},{-100,54}}),iconTransformation(extent={{-120,34},{-100,54}})));
   Buildings.Controls.OBC.CDL.Interfaces.RealInput dpMea(
@@ -93,21 +93,22 @@
     annotation (Placement(transformation(extent={{-10,-60},{10,-40}})));
   Modelica.Blocks.Sources.RealExpression norDecSetMasFlo(
     y=1)
     "Normalized decoupler line mass flow rate."
     annotation (Placement(transformation(extent={{-40,-60},{-20,-40}})));
   Modelica.Blocks.Sources.RealExpression norDecMasFlo(
     y=meaFloByPas/(
-      if ON[numPum] then
+      if ON then
         numPum*mMin_flow
       else
         mMin_flow))
     "Normalised decoupler line measured mass flow rate."
     annotation (Placement(transformation(extent={{42,-84},{22,-64}})));
 equation
+  connect(ON,pumStaCon.on);
   connect(pumStaCon.masFloPum,masFloPum)
     annotation (Line(points={{-12,8},{-22,8},{-22,66},{-110,66}},color={0,0,127}));
   connect(conPID.y,pumStaCon.speSig)
     annotation (Line(points={{-39,0},{-20,0},{-20,4},{-12,4}},color={0,0,127}));
   connect(dpSetSca.y,conPID.u_s)
     annotation (Line(points={{-79,0},{-62,0}},color={0,0,127}));
   connect(dpMea,gai.u)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallel.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/PartialPlantParallelInterface.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/model_connectors/plants/templates/ValveParameters.mo`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mo`

 * *Files 12% similar despite different names*

```diff
@@ -1,38 +1,44 @@
 model CoolingPlant
   "This example is to validate template Central Cooling Plant component model."
-    extends Buildings.Experimental.DHC.CentralPlants.Cooling.Examples.Plant(
+
+  extends Buildings.Experimental.DHC.CentralPlants.Cooling.Examples.Plant(
     redeclare Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_York_YT_1055kW_5_96COP_Vanes perChi(
-      mEva_flow_nominal=mCHW_flow_nominal,
-      mCon_flow_nominal=mCW_flow_nominal,
-      QEva_flow_nominal=QChi_nominal),
+      mEva_flow_nominal = mCHW_flow_nominal,
+      mCon_flow_nominal = mCW_flow_nominal,
+      QEva_flow_nominal = QChi_nominal),
     redeclare Buildings.Experimental.DHC.CentralPlants.Cooling.Plant pla,
-    dTApp=3,
-    mCHW_flow_nominal=18.3,
-    dpCHW_nominal=44.8*1000,
-    mMin_flow=0.03,
-    mCW_flow_nominal=34.7,
-    dpCW_nominal=46.2*1000,
-    PFan_nominal=4999,
-    TCHWSet=273.15 + 7,
-    dpCooTowVal_nominal=5999,
-    dpCHWPumVal_nominal=5999,
-    dpCWPumVal_nominal=5999);
+    dTApp = 3,
+    mCHW_flow_nominal = 18.3,
+    dpCHW_nominal = 44.8 * 1000,
+    mMin_flow = 0.03,
+    mCW_flow_nominal = 34.7,
+    dpCW_nominal = 46.2 * 1000,
+    PFan_nominal = 4999,
+    TCHWSet = 273.15 + 7,
+    dpCooTowVal_nominal = 5999,
+    dpCHWPumVal_nominal = 5999,
+    dpCWPumVal_nominal = 5999);
+
   annotation (
-    Icon(coordinateSystem(preserveAspectRatio=false)),
-    Diagram(coordinateSystem(preserveAspectRatio=false)),
-    experiment(StopTime=86400, Tolerance=1e-06),
-    Documentation(info="<html>
+    Icon(coordinateSystem(preserveAspectRatio = false)),
+    Diagram(coordinateSystem(preserveAspectRatio = false)),
+    experiment(StopTime = 86400, Tolerance = 1e-06),
+    Documentation(
+      info = "<html>
       <p>This model validates the district central cooling plant template model
 GMT_Lib.DHC.Components.CentralPlants.Cooling.Cooling.mot</a>.
 </p>
-</html>", revisions="<html>
+</html>",
+      revisions = "<html>
 <ul>
 <li>
 October 20, 2021 by Chengnan Shi:<br/>
 First implementation.
 </li>
 </ul>
 </html>"),
-    __Dymola_Commands(file="CoolingPlant.mos"
-                                             "Simulate and Plot"));
+    __Dymola_Commands(
+      file = "CoolingPlant.mos"
+        "Simulate and Plot"));
+
 end CoolingPlant;
```

#### html2text {}

```diff
@@ -1,22 +1,22 @@
 model CoolingPlant "This example is to validate template Central Cooling Plant
 component model." extends
 Buildings.Experimental.DHC.CentralPlants.Cooling.Examples.Plant( redeclare
 Buildings.Fluid.Chillers.Data.ElectricEIR.ElectricEIRChiller_York_YT_1055kW_5_96COP_Vanes
-perChi( mEva_flow_nominal=mCHW_flow_nominal,
-mCon_flow_nominal=mCW_flow_nominal, QEva_flow_nominal=QChi_nominal), redeclare
-Buildings.Experimental.DHC.CentralPlants.Cooling.Plant pla, dTApp=3,
-mCHW_flow_nominal=18.3, dpCHW_nominal=44.8*1000, mMin_flow=0.03,
-mCW_flow_nominal=34.7, dpCW_nominal=46.2*1000, PFan_nominal=4999,
-TCHWSet=273.15 + 7, dpCooTowVal_nominal=5999, dpCHWPumVal_nominal=5999,
-dpCWPumVal_nominal=5999); annotation ( Icon(coordinateSystem
-(preserveAspectRatio=false)), Diagram(coordinateSystem
-(preserveAspectRatio=false)), experiment(StopTime=86400, Tolerance=1e-06),
-Documentation(info="
+perChi( mEva_flow_nominal = mCHW_flow_nominal, mCon_flow_nominal =
+mCW_flow_nominal, QEva_flow_nominal = QChi_nominal), redeclare
+Buildings.Experimental.DHC.CentralPlants.Cooling.Plant pla, dTApp = 3,
+mCHW_flow_nominal = 18.3, dpCHW_nominal = 44.8 * 1000, mMin_flow = 0.03,
+mCW_flow_nominal = 34.7, dpCW_nominal = 46.2 * 1000, PFan_nominal = 4999,
+TCHWSet = 273.15 + 7, dpCooTowVal_nominal = 5999, dpCHWPumVal_nominal = 5999,
+dpCWPumVal_nominal = 5999); annotation ( Icon(coordinateSystem
+(preserveAspectRatio = false)), Diagram(coordinateSystem(preserveAspectRatio =
+false)), experiment(StopTime = 86400, Tolerance = 1e-06), Documentation( info =
+"
 This model validates the district central cooling plant template model
 GMT_Lib.DHC.Components.CentralPlants.Cooling.Cooling.mot
 .
-", revisions="
+", revisions = "
     * October 20, 2021 by Chengnan Shi:
       First implementation.
-"), __Dymola_Commands(file="CoolingPlant.mos" "Simulate and Plot")); end
+"), __Dymola_Commands( file = "CoolingPlant.mos" "Simulate and Plot")); end
 CoolingPlant;
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mos`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 // Simulate
 simulateModel("GMT_Lib.DHC.Components.Plants.Cooling.CoolingPlant",
     stopTime=86400,
-    method="cvode",
     tolerance=1e-06,
     resultFile="CoolingPlant");
 // Plot commands
 removePlots(false);
 createPlot(
     id=1,
     position={24, 10, 831, 511},
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Cooling/CoolingPlant.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/BoilerPolynomial.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/Components/Plants/Heating/BoilerPolynomial.mot`

 * *Files 6% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     m_flow_nominal=m_flow_nominal_GMT),
   boi2(
     Q_flow_nominal=Q_flow_nominal_GMT,
     m_flow_nominal=m_flow_nominal_GMT));
 
 
 annotation (
-  uses(Buildings(version="9.1.0")),
+  uses(Buildings(version="10.0.0")),
   Icon(coordinateSystem(preserveAspectRatio=false)),
   Diagram(coordinateSystem(preserveAspectRatio=false)),
   experiment(Tolerance=1e-6, StopTime=3600),
   Documentation(info="<html>
     <p>This model validates the hot water boiler template model implemented in
 <a href=\"Buildings.Fluid.Boilers.Examples.BoilerPolynomial\">
 Buildings.Fluid.Boilers.Examples.BoilerPolynomial.mot</a>.
```

#### html2text {}

```diff
@@ -5,15 +5,15 @@
 Modelica.Units.SI.MassFlowRate m_flow_nominal_GMT = {{ data
 ["mass_hhw_flow_nominal"] }} "Nominal mass flow rate, (Note: can be calculated
 as Q_flow_nominal/dT_nominal/4200 or identify the relationship of m and Q from
 GMT top level user inputs)"; extends
 Buildings.Fluid.Boilers.Examples.BoilerPolynomial( boi1
 ( Q_flow_nominal=Q_flow_nominal_GMT, m_flow_nominal=m_flow_nominal_GMT), boi2
 ( Q_flow_nominal=Q_flow_nominal_GMT, m_flow_nominal=m_flow_nominal_GMT));
-annotation ( uses(Buildings(version="9.1.0")), Icon(coordinateSystem
+annotation ( uses(Buildings(version="10.0.0")), Icon(coordinateSystem
 (preserveAspectRatio=false)), Diagram(coordinateSystem
 (preserveAspectRatio=false)), experiment(Tolerance=1e-6, StopTime=3600),
 Documentation(info="
 This model validates the hot water boiler template model implemented in
 _B_u_i_l_d_i_n_g_s_._F_l_u_i_d_._B_o_i_l_e_r_s_._E_x_a_m_p_l_e_s_._B_o_i_l_e_r_P_o_l_y_n_o_m_i_a_l_._m_o_t.
 ", revisions="
     * September 25, 2023 by Nathan Moore:
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_partial.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_partial.mot`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 within {{ data['project_name'] }}.Districts;{% raw %}
 partial model PartialSeries "Partial model for series network"
   extends Modelica.Icons.Example;
   package Medium = Buildings.Media.Water "Medium model";
-  constant Real facMul = 10
+  constant Real facMul = 1
     "Building loads multiplier factor";
   parameter Real dpDis_length_nominal(final unit="Pa/m") = 250
     "Pressure drop per pipe length at nominal flow rate - Distribution line";
   parameter Real dpCon_length_nominal(final unit="Pa/m") = 250
     "Pressure drop per pipe length at nominal flow rate - Connection line";
   parameter Boolean allowFlowReversalSer = true
     "Set to true to allow flow reversal in the service lines"
@@ -17,17 +17,44 @@
   parameter Integer nBui = datDes.nBui
     "Number of buildings connected to DHC system"
     annotation (Evaluate=true);
   inner parameter
     Buildings.Experimental.DHC.Examples.Combined.BaseClasses.DesignDataSeries
     datDes(final mCon_flow_nominal=bui.ets.mSerWat_flow_nominal) "Design data"
     annotation (Placement(transformation(extent={{-340,220},{-320,240}})));
+  parameter Integer nBor = 300
+    "Number of boreholes";
+  parameter Integer hBor = 350
+    "Total height of borehole, meters";
+  parameter Real rTub = 0.02
+    "Outer radius of the tube, meters";
+  parameter Real rBor = 0.095
+    "Radius of the borehole, meters";
+  parameter Real xC = 0.05
+    "Shank spacing between the pipes and center of boreholes, meters";
+  parameter Real dxyBor = 10
+    "Distance between boreholes, meters";
+  final parameter Modelica.Units.SI.Length cooBor[nBor,2]={dxyBor*{mod(i - 1,
+      10),floor((i - 1)/10)} for i in 1:nBor}
+    "Cartesian coordinates of the boreholes in meters";
   // COMPONENTS
   Buildings.Experimental.DHC.Plants.Reservoir.BoreField
-    borFie(redeclare final package Medium = Medium) "Bore field" annotation (
+    borFie(redeclare final package Medium = Medium, borFieDat(conDat=
+          Buildings.Fluid.Geothermal.Borefields.Data.Configuration.Example(
+          borCon=Buildings.Fluid.Geothermal.Borefields.Types.BoreholeConfiguration.DoubleUTubeParallel,
+          dp_nominal=35000,
+          hBor=hBor,
+          rBor=rBor,
+          dBor=1,
+          nBor=nBor,
+          cooBor=cooBor,
+          rTub=rTub,
+          kTub=0.5,
+          eTub=0.0037,
+          xC=xC))) "Bore field" annotation (
       Placement(transformation(
         extent={{-10,-10},{10,10}},
         rotation=0,
         origin={-130,-80})));
   Buildings.Experimental.DHC.EnergyTransferStations.BaseClasses.Pump_m_flow pumDis(
     redeclare final package Medium = Medium,
     final m_flow_nominal=datDes.mPumDis_flow_nominal,
@@ -139,27 +166,27 @@
     redeclare each final package MediumSer = Medium,
     each final allowFlowReversalBui=allowFlowReversalBui,
     each final allowFlowReversalSer=allowFlowReversalSer) "Building and ETS"
     annotation (Placement(transformation(extent={{-10,170},{10,190}})));
   Modelica.Blocks.Sources.Constant TSewWat(k=273.15 + 17)
     "Sewage water temperature"
     annotation (Placement(transformation(extent={{-280,30},{-260,50}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THeaWatSupMaxSet[nBui](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant THeaWatSupMaxSet[nBui](
     k=bui.THeaWatSup_nominal)
     "Heating water supply temperature set point - Maximum value"
     annotation (Placement(transformation(extent={{-250,210},{-230,230}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant TChiWatSupSet[nBui](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant TChiWatSupSet[nBui](
     k=bui.TChiWatSup_nominal)
     "Chilled water supply temperature set point"
     annotation (Placement(transformation(extent={{-220,190},{-200,210}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THeaWatSupMinSet[nBui](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant THeaWatSupMinSet[nBui](
     each k=28 + 273.15)
     "Heating water supply temperature set point - Minimum value"
     annotation (Placement(transformation(extent={{-280,230},{-260,250}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum PPumETS(
+  Buildings.Controls.OBC.CDL.Reals.MultiSum PPumETS(
     final nin=nBui)
     "ETS pump power"
     annotation (Placement(transformation(extent={{140,190},{160,210}})));
   Modelica.Blocks.Continuous.Integrator EPumETS(
     initType=Modelica.Blocks.Types.Init.InitialState)
     "ETS pump electric energy"
     annotation (Placement(transformation(extent={{220,190},{240,210}})));
@@ -170,26 +197,26 @@
   Modelica.Blocks.Continuous.Integrator EPumSto(
     initType=Modelica.Blocks.Types.Init.InitialState)
     "Storage pump electric energy"
     annotation (Placement(transformation(extent={{220,-150},{240,-130}})));
   Modelica.Blocks.Continuous.Integrator EPumPla(initType=Modelica.Blocks.Types.Init.InitialState)
     "Plant pump electric energy"
     annotation (Placement(transformation(extent={{220,30},{240,50}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum EPum(nin=4)
+  Buildings.Controls.OBC.CDL.Reals.MultiSum EPum(nin=4)
     "Total pump electric energy"
     annotation (Placement(transformation(extent={{280,110},{300,130}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum PHeaPump(
+  Buildings.Controls.OBC.CDL.Reals.MultiSum PHeaPump(
     final nin=nBui)
     "Heat pump power"
     annotation (Placement(transformation(extent={{140,150},{160,170}})));
   Modelica.Blocks.Continuous.Integrator EHeaPum(
     initType=Modelica.Blocks.Types.Init.InitialState)
     "Heat pump electric energy"
     annotation (Placement(transformation(extent={{220,150},{240,170}})));
-  Buildings.Controls.OBC.CDL.Continuous.MultiSum ETot(nin=2) "Total electric energy"
+  Buildings.Controls.OBC.CDL.Reals.MultiSum ETot(nin=2) "Total electric energy"
     annotation (Placement(transformation(extent={{320,150},{340,170}})));
   Buildings.Experimental.DHC.Loads.BaseClasses.ConstraintViolation conVio(
     final uMin=datDes.TLooMin,
     final uMax=datDes.TLooMax,
     final nu=3+nBui)
     "Check if loop temperatures are within given range"
     annotation (Placement(transformation(extent={{320,10},{340,30}})));
@@ -273,17 +300,27 @@
   connect(TDisWatRet.T, conVio.u[3]) annotation (Line(points={{69,6.66134e-16},{
           60,6.66134e-16},{60,20},{318,20}},           color={0,0,127}));
   annotation (Diagram(
     coordinateSystem(preserveAspectRatio=false, extent={{-360,-260},{360,260}})),
       Documentation(revisions="<html>
 <ul>
 <li>
+March 3, 2024, by Nicholas Long:<br/>
+Exposed underlying borehole field data for easy access within
+Modelica Builder.
+</li>
+<li>
+November 16, 2023, by Nicholas Long:<br/>
+Default the facMul to 1. The loads for the GMT are coming from real buildings
+and we do not need to multiply the QHea/QCoo.
+</li>
+<li>
 April 12, 2023, by Nicholas Long:<br/>
 Templatized for direct use in GMT with n-building connectors.
-<li>
+</li>
 <li>
 November 16, 2022, by Michael Wetter:<br/>
 Set correct nominal pressure for distribution pump.
 </li>
 <li>
 February 23, 2021, by Antoine Gautier:<br/>
 Refactored with base classes from the <code>DHC</code> package.<br/>
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.mot`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,26 @@
-within {{ data['project_name'] }}.Districts;{% raw %}
+within {{ data['project_name'] }}.Districts;
 model district
   "Series connection with constant district water mass flow rate"
   extends
     PartialSeries(redeclare
       Buildings.Experimental.DHC.Loads.Combined.BuildingTimeSeriesWithETS
       bui[nBui](final filNam=filNam), datDes(
-      {% endraw %}nBui={{ data['building_load_files'] | count }},
+      nBui={{ data['building_load_files'] | count }},
       mPumDis_flow_nominal={{ data['max_flow_rate'] }},
       mPla_flow_nominal={{ data['max_flow_rate'] }},
       mSto_flow_nominal={{ data['max_flow_rate'] / 10 }},
-      dp_length_nominal=250,{% raw %}
-      epsPla=0.935));
+      dp_length_nominal=250,
+      epsPla=0.935,
+      {{ data['lDis'] }},
+      {{ data['lCon'] }}
+      )
+      );
   parameter String filNam[nBui]={
-    {% endraw %}{% for building in data['building_load_files'] %}
+    {% for building in data['building_load_files'] %}
     "{{ building }}"{% if not loop.last %},{% endif %}
     {% endfor %}{% raw %}}
     "Library paths of the files with thermal loads as time series";
   Modelica.Blocks.Sources.Constant masFloMaiPum(
     k=datDes.mPumDis_flow_nominal)
     "Distribution pump mass flow rate"
     annotation (Placement(transformation(extent={{-300,-70},{-280,-50}})));
@@ -24,19 +28,19 @@
     k=datDes.mPla_flow_nominal)
     "District water flow rate to plant"
     annotation (Placement(transformation(extent={{-300,-6},{-280,14}})));
   Modelica.Blocks.Sources.Constant masFloStoPum(
     k=datDes.mSto_flow_nominal)
     "Storage/GHX pump mass flow rate"
     annotation (Placement(transformation(extent={{-300,-108},{-280,-88}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THotWatSupSet[nBui](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant THotWatSupSet[nBui](
     k=fill(63 + 273.15, nBui))
     "Hot water supply temperature set point"
     annotation (Placement(transformation(extent={{-190,170},{-170,190}})));
-  Buildings.Controls.OBC.CDL.Continuous.Sources.Constant TColWat[nBui](
+  Buildings.Controls.OBC.CDL.Reals.Sources.Constant TColWat[nBui](
     k=fill(15 + 273.15, nBui))
     "Cold water temperature"
     annotation (Placement(transformation(extent={{-160,150},{-140,170}})));
 equation
   connect(masFloMaiPum.y, pumDis.m_flow_in) annotation (Line(points={{-279,-60},
           {-106,-60},{68,-60}}, color={0,0,127}));
   connect(masFloStoPum.y, pumSto.m_flow_in) annotation (Line(points={{-279,-98},
@@ -71,22 +75,23 @@
 <h4>References</h4>
 <p>
 Sommer T., Sulzer M., Wetter M., Sotnikov A., Mennel S., Stettler C.
 <i>The reservoir network: A new network topology for district heating
 and cooling.</i>
 Energy, Volume 199, 15 May 2020, 117418.
 </p>
-</html>",   revisions="<html>
+</html>", revisions="<html>
 <ul>
 <li>
 April 12, 2023, by Nicholas Long:<br/>
 Templatized for direct use in GMT with n-building connectors.<br/>
 Changes include: removing dymola run command tied to MBL path, adding
 a constant for borehole field mass flow rate (no longer tied to main
 distribution loop).
+</li>
 <li>
 February 23, 2021, by Antoine Gautier:<br/>
 Refactored with base classes from the <code>DHC</code> package.<br/>
 This is for
 <a href=\"https://github.com/lbl-srg/modelica-buildings/issues/1769\">
 issue 1769</a>.
 </li>
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-within {{ data['project_name'] }}.Districts;{% raw %} model district "Series
-connection with constant district water mass flow rate" extends PartialSeries
-(redeclare Buildings.Experimental.DHC.Loads.Combined.BuildingTimeSeriesWithETS
-bui[nBui](final filNam=filNam), datDes( {% endraw %}nBui={{ data
-['building_load_files'] | count }}, mPumDis_flow_nominal={{ data
-['max_flow_rate'] }}, mPla_flow_nominal={{ data['max_flow_rate'] }},
-mSto_flow_nominal={{ data['max_flow_rate'] / 10 }}, dp_length_nominal=250,{%
-raw %} epsPla=0.935)); parameter String filNam[nBui]={ {% endraw %}{% for
-building in data['building_load_files'] %} "{{ building }}"{% if not loop.last
-%},{% endif %} {% endfor %}{% raw %}} "Library paths of the files with thermal
-loads as time series"; Modelica.Blocks.Sources.Constant masFloMaiPum
+within {{ data['project_name'] }}.Districts; model district "Series connection
+with constant district water mass flow rate" extends PartialSeries(redeclare
+Buildings.Experimental.DHC.Loads.Combined.BuildingTimeSeriesWithETS bui[nBui]
+(final filNam=filNam), datDes( nBui={{ data['building_load_files'] | count }},
+mPumDis_flow_nominal={{ data['max_flow_rate'] }}, mPla_flow_nominal={{ data
+['max_flow_rate'] }}, mSto_flow_nominal={{ data['max_flow_rate'] / 10 }},
+dp_length_nominal=250, epsPla=0.935, {{ data['lDis'] }}, {{ data['lCon'] }} )
+); parameter String filNam[nBui]={ {% for building in data
+['building_load_files'] %} "{{ building }}"{% if not loop.last %},{% endif %}
+{% endfor %}{% raw %}} "Library paths of the files with thermal loads as time
+series"; Modelica.Blocks.Sources.Constant masFloMaiPum
 ( k=datDes.mPumDis_flow_nominal) "Distribution pump mass flow rate" annotation
 (Placement(transformation(extent={{-300,-70},{-280,-50}})));
 Modelica.Blocks.Sources.Constant masFloDisPla( k=datDes.mPla_flow_nominal)
 "District water flow rate to plant" annotation (Placement(transformation
 (extent={{-300,-6},{-280,14}}))); Modelica.Blocks.Sources.Constant masFloStoPum
 ( k=datDes.mSto_flow_nominal) "Storage/GHX pump mass flow rate" annotation
 (Placement(transformation(extent={{-300,-108},{-280,-88}})));
-Buildings.Controls.OBC.CDL.Continuous.Sources.Constant THotWatSupSet[nBui]
-( k=fill(63 + 273.15, nBui)) "Hot water supply temperature set point"
-annotation (Placement(transformation(extent={{-190,170},{-170,190}})));
-Buildings.Controls.OBC.CDL.Continuous.Sources.Constant TColWat[nBui]( k=fill(15
-+ 273.15, nBui)) "Cold water temperature" annotation (Placement(transformation
+Buildings.Controls.OBC.CDL.Reals.Sources.Constant THotWatSupSet[nBui]( k=fill
+(63 + 273.15, nBui)) "Hot water supply temperature set point" annotation
+(Placement(transformation(extent={{-190,170},{-170,190}})));
+Buildings.Controls.OBC.CDL.Reals.Sources.Constant TColWat[nBui]( k=fill(15 +
+273.15, nBui)) "Cold water temperature" annotation (Placement(transformation
 (extent={{-160,150},{-140,170}}))); equation connect(masFloMaiPum.y,
 pumDis.m_flow_in) annotation (Line(points={{-279,-60}, {-106,-60},{68,-60}},
 color={0,0,127})); connect(masFloStoPum.y, pumSto.m_flow_in) annotation (Line
 (points={{-279,-98}, {-238,-98},{-238,-66},{-180,-66}}, color={0,0,127}));
 connect(masFloDisPla.y, pla.mPum_flow) annotation (Line(points={{-279,4},{ -
 161.333,4},{-161.333,4.66667}}, color={0,0,127})); connect(THotWatSupSet.y,
 bui.THotWatSupSet) annotation (Line(points={{-168, 180},{-24,180},{-24,183},{-
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/DHC/DHC_5G_waste_heat_GHX_variable.py`

 * *Files 15% similar despite different names*

```diff
@@ -4,98 +4,120 @@
 from modelica_builder.modelica_mos_file import ModelicaMOS
 from modelica_builder.package_parser import PackageParser
 
 from geojson_modelica_translator.modelica.simple_gmt_base import SimpleGMTBase
 from geojson_modelica_translator.scaffold import Scaffold
 
 
-class DHC5GWasteHeatAndGHX(SimpleGMTBase):
-    """Generates a full Modelica package with the DHC 5G waste heat and GHX model."""
+class DHC5GWasteHeatAndGHXVariable(SimpleGMTBase):
+    """Generates a full Modelica package with the DHC 5G waste heat and GHX model with a
+    controlled variable speed distribution pump.
+    """
 
     def __init__(self, system_parameters):
         self.system_parameters = system_parameters
         self.template_dir = Path(__file__).parent
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path, project_name: str) -> None:
         """This is a bit past being a simple template as it is exporting an entire scaffolded package
         that can be loaded and simulated in Modelica. The scaffold is very specific to DES.
 
         Args:
             output_dir (Path): directory to save the package to (without the project name)
             project_name (str, optional): The name of the project which is used in the Scaffold object.
         """
-        template_data = {
-            'project_name': project_name,
-            'save_file_name': 'district',
-            'building_load_files': []
-        }
+        template_data = {"project_name": project_name, "save_file_name": "district", "building_load_files": []}
 
         # create the directory structure
         scaffold = Scaffold(output_dir, project_name=project_name)
-        scaffold.create(ignore_paths=['Loads', 'Networks', 'Plants', 'Substations'])
+        scaffold.create(ignore_paths=["Loads", "Networks", "Plants", "Substations"])
 
         # create the root package
         package = PackageParser.new_from_template(scaffold.project_path, project_name, order=[])
-        package.add_model('Districts')
+        package.add_model("Districts")
 
         # create the district package with the template_data from above
         files_to_copy = []
 
         # 1: grab all of the time series files and place them in the proper location
         for building in self.system_parameters.get_param("$.buildings[?load_model=time_series]"):
-            building_load_file = Path(building['load_model_parameters']['time_series']['filepath'])
-            files_to_copy.append({
-                "orig_file": building_load_file,
-                "geojson_id": building['geojson_id'],
-                "save_path": f"{scaffold.districts_path.resources_dir}/{building['geojson_id']}",
-                "save_filename": building_load_file.name
-            })
+            building_load_file = Path(building["load_model_parameters"]["time_series"]["filepath"])
+            files_to_copy.append(
+                {
+                    "orig_file": building_load_file,
+                    "geojson_id": building["geojson_id"],
+                    "save_path": f"{scaffold.districts_path.resources_dir}/{building['geojson_id']}",
+                    "save_filename": building_load_file.name,
+                }
+            )
 
         # 2: Copy the files to the appropriate location and ensure uniqueness by putting into a unique directory
         #    (since OpenStudio creates all files with modelica.mos)
         total_heating_load = 0
         total_cooling_load = 0
         total_swh_load = 0
         for file_to_copy in files_to_copy:
             # create the path if it doesn't exist
-            Path(file_to_copy['save_path']).mkdir(parents=True, exist_ok=True)
+            Path(file_to_copy["save_path"]).mkdir(parents=True, exist_ok=True)
             save_filename = f"{file_to_copy['save_path']}/{file_to_copy['save_filename']}"
-            shutil.copy(file_to_copy['orig_file'], save_filename)
+            shutil.copy(file_to_copy["orig_file"], save_filename)
 
-            # 3: If the file is an MOS file, and it has the Peak water heating load set to zero, then set it to a minimum value
+            # 3: If the file is an MOS file and Peak water heating load is set to zero, then set it to a minimum value
             #    Also, store the total heating, cooling, and water loads which will be used for sizing.
             mos_file = ModelicaMOS(save_filename)
-            total_heating_load += mos_file.retrieve_header_variable_value('Peak space heating load', cast_type=float)
-            total_cooling_load += mos_file.retrieve_header_variable_value('Peak space cooling load', cast_type=float)
-            peak_water = mos_file.retrieve_header_variable_value('Peak water heating load', cast_type=float)
+            total_heating_load += mos_file.retrieve_header_variable_value("Peak space heating load", cast_type=float)
+            total_cooling_load += mos_file.retrieve_header_variable_value("Peak space cooling load", cast_type=float)
+            peak_water = mos_file.retrieve_header_variable_value("Peak water heating load", cast_type=float)
             total_swh_load += peak_water
             if peak_water == 0:
-                peak_heat = mos_file.retrieve_header_variable_value('Peak space heating load', cast_type=float)
+                peak_heat = mos_file.retrieve_header_variable_value("Peak space heating load", cast_type=float)
                 peak_swh = max(peak_heat / 10, 5000)
 
-                mos_file.replace_header_variable_value('Peak water heating load', peak_swh)
+                mos_file.replace_header_variable_value("Peak water heating load", peak_swh)
                 mos_file.save()
 
             # 4: Add the path to the param data with Modelica friendly path names
-            rel_path_name = f"{project_name}/{scaffold.districts_path.resources_relative_dir}/{file_to_copy['geojson_id']}/{file_to_copy['save_filename']}"
-            template_data['building_load_files'].append(f"modelica://{rel_path_name}")  # type: ignore
+            rel_path_name = f"{project_name}/{scaffold.districts_path.resources_relative_dir}/{file_to_copy['geojson_id']}/{file_to_copy['save_filename']}"  # noqa: E501
+            template_data["building_load_files"].append(f"modelica://{rel_path_name}")  # type: ignore[attr-defined]
 
         # 5: Calculate the mass flow rates (kg/s) for the heating and cooling networks peak load (in Watts)
         #    (assuming 5C delta T [since 5G] and 4.18 Cp (kJ/kgK)). Add 1.5x the peak for oversizing
         delta_t = 5
         heating_flow_rate = 1.5 * total_heating_load / (1000 * delta_t * 4.18)
         cooling_flow_rate = 1.5 * total_cooling_load / (1000 * delta_t * 4.18)
         swh_flow_rate = 1.5 * total_swh_load / (1000 * delta_t * 4.18)
 
-        template_data['max_flow_rate'] = round(max(heating_flow_rate, cooling_flow_rate, swh_flow_rate), 3)  # type: ignore
+        template_data["max_flow_rate"] = round(max(heating_flow_rate, cooling_flow_rate, swh_flow_rate), 3)  # type: ignore[arg-type]
+
+        nbuildings = len(template_data["building_load_files"])
+        template_data["lDis"] = self.build_string("lDis = {", "0.5, ", nbuildings)
+        template_data["lCon"] = self.build_string("lCon = {", "0.5, ", nbuildings)
 
         # 6: generate the modelica files from the template
-        self.to_modelica(output_dir=Path(scaffold.districts_path.files_dir),
-                         model_name='DHC_5G_waste_heat_GHX',
-                         param_data=template_data,
-                         save_file_name='district.mo',
-                         generate_package=True,
-                         partial_files={'DHC_5G_partial': 'PartialSeries'})
+        self.to_modelica(
+            output_dir=Path(scaffold.districts_path.files_dir),
+            model_name="DHC_5G_waste_heat_GHX_variable",
+            param_data=template_data,
+            save_file_name="district.mo",
+            generate_package=True,
+            partial_files={"DHC_5G_partial": "PartialSeries"},
+        )
 
         # 7: save the root package.mo
         package.save()
+
+    def build_string(self, base_text: str, value: str, iterations: int) -> str:
+        """Builds a string with a comma separated list of values.
+
+        This is used to build 5G districts with arbitrary number of buildings.
+        It's ugly because of the Jinja/Modelica templating system.
+        This is a bit of a hack but it works.
+
+        Example output: lDis = { 0.5, 0.5, 0.5 }
+
+        Args:
+            base_text (str): The text to start the string with.
+            value (str): The value to add multiple times.
+            iterations (int): The number of values to add to the string."""
+        text = f"{base_text} {value * iterations}"
+        return text.removesuffix(", ") + " }"
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Conversion/ACACTransformer.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,15 +10,17 @@
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         transformer_params = self.system_parameters.get_param("$.transformers")
         # There can be multiple capacitors so we need to loop over them
         for index, transformer in enumerate(transformer_params):
             cap_params = {
-                'nominal_capacity': transformer["nominal_capacity"],
+                "nominal_capacity": transformer["nominal_capacity"],
                 "reactance_resistance_ratio": transformer["reactance_resistance_ratio"],
                 "tx_incoming_voltage": transformer["tx_incoming_voltage"],
                 "tx_outgoing_voltage": transformer["tx_outgoing_voltage"],
-                'model_name': f"Transformer{index}",
+                "model_name": f"Transformer{index}",
             }
             # render template to final modelica file
-            self.to_modelica(output_dir=output_dir, model_name='ACACTransformer', param_data=cap_params, iteration=index)
+            self.to_modelica(
+                output_dir=output_dir, model_name="ACACTransformer", param_data=cap_params, iteration=index
+            )
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/ACLine.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Lines/Lines.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,23 +12,23 @@
     def build_from_template(self, output_dir: Path):
         distribution_line_params = self.system_parameters.get_param("$.distribution_lines")
         # Each segment of cable gets its own mofile, numbered with 'iteration'
         for index, line in enumerate(distribution_line_params):
             # This is how we map from ditto-reader to mbl. It's pretty brittle, and will need updating in this state
             # https://github.com/urbanopt/urbanopt-ditto-reader/blob/develop/example/extended_catalog.json
             for wire in line["commercial_line_type"]:
-                if '477kcmil' in wire:
-                    mbl_wire = 'Buildings.Electrical.Transmission.MediumVoltageCables.Annealed_Al_500'
-                if '750kcmil' in wire:
+                if "477kcmil" in wire:
+                    mbl_wire = "Buildings.Electrical.Transmission.MediumVoltageCables.Annealed_Al_500"
+                if "750kcmil" in wire:
                     # FIXME: This mapping from 750kcmil to 1000kcmil is not ideal
                     # A 750kcmil has been proposed for the MBL
                     # The temporary alternative is to map to 500 kcmil, which didn't seem right to me
-                    mbl_wire = 'Buildings.Electrical.Transmission.MediumVoltageCables.Annealed_Al_1000'
+                    mbl_wire = "Buildings.Electrical.Transmission.MediumVoltageCables.Annealed_Al_1000"
             line_params = {
-                'length': line["length"],
-                'ampacity': line["ampacity"],
-                'nominal_voltage': line["nominal_voltage"],
-                'commercial_line_type': mbl_wire,
-                'model_name': f"Line{index}",
+                "length": line["length"],
+                "ampacity": line["ampacity"],
+                "nominal_voltage": line["nominal_voltage"],
+                "commercial_line_type": mbl_wire,
+                "model_name": f"Line{index}",
             }
             # render template to final modelica file
-            self.to_modelica(output_dir=output_dir, model_name='ACLine', param_data=line_params, iteration=index)
+            self.to_modelica(output_dir=output_dir, model_name="ACLine", param_data=line_params, iteration=index)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Capacitive.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Capacitive.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/Inductive.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import logging
 from pathlib import Path
 
 from geojson_modelica_translator.modelica.simple_gmt_base import SimpleGMTBase
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
-class Inductive_load(SimpleGMTBase):
+class InductiveLoad(SimpleGMTBase):
     def __init__(self, system_parameters):
         self.system_parameters = system_parameters
         self.template_dir = Path(__file__).parent
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         for building_index, building in enumerate(self.system_parameters.get_param("$.buildings")):
             inductive_params = {
-                'nominal_power_consumption': building["load"]["max_power_kw"],
-                'nominal_voltage': building["load"]["nominal_voltage"],
-                'model_name': f"Inductive{building_index}",
+                "nominal_power_consumption": building["load"]["max_power_kw"],
+                "nominal_voltage": building["load"]["nominal_voltage"],
+                "model_name": f"Inductive{building_index}",
             }
             # render template to final modelica file
             self.to_modelica(
-                output_dir=output_dir,
-                model_name='Inductive',
-                param_data=inductive_params,
-                iteration=building_index
+                output_dir=output_dir, model_name="Inductive", param_data=inductive_params, iteration=building_index
             )
             # If the sys-param file is missing an entry, it will show up as a jinja2.exceptions.UndefinedError
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitive.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Loads/capacitive.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,34 +1,26 @@
 import logging
 from pathlib import Path
 
 from geojson_modelica_translator.modelica.simple_gmt_base import SimpleGMTBase
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
-class Capacitive_load(SimpleGMTBase):
+class CapacitiveLoad(SimpleGMTBase):
     def __init__(self, system_parameters):
         self.system_parameters = system_parameters
         self.template_dir = Path(__file__).parent
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         for building_index, building in enumerate(self.system_parameters.get_param("$.buildings")):
             capacitive_params = {
-                'nominal_power_consumption': building["load"]["max_power_kw"],
-                'nominal_voltage': building["load"]["nominal_voltage"],
-                'model_name': f"Capacitive{building_index}",
+                "nominal_power_consumption": building["load"]["max_power_kw"],
+                "nominal_voltage": building["load"]["nominal_voltage"],
+                "model_name": f"Capacitive{building_index}",
             }
             # render template to final modelica file
             self.to_modelica(
-                output_dir=output_dir,
-                model_name='Capacitive',
-                param_data=capacitive_params,
-                iteration=building_index
+                output_dir=output_dir, model_name="Capacitive", param_data=capacitive_params, iteration=building_index
             )
             # If the sys-param file is missing an entry, it will show up as a jinja2.exceptions.UndefinedError
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Generator.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Generator.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Grid.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/Grid.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/PVPanels.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/WindTurbine.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/community_pv.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         community_pv_params = self.system_parameters.get_param("$.photovoltaic_panels")
         # There can be multiple community pv arrays so we need to loop over them
         for index, pvarray in enumerate(community_pv_params):
             pv_params = {
-                'net_surface_area_m2': pvarray["net_surface_area"],
-                'nominal_voltage_V': pvarray["nominal_voltage"],
-                'surface_azimuth_deg': pvarray["surface_azimuth"],
-                'surface_tilt_deg': pvarray["surface_tilt"],
-                'model_name': f"PVPanels{index}",
+                "net_surface_area_m2": pvarray["net_surface_area"],
+                "nominal_voltage_V": pvarray["nominal_voltage"],
+                "surface_azimuth_deg": pvarray["surface_azimuth"],
+                "surface_tilt_deg": pvarray["surface_tilt"],
+                "model_name": f"PVPanels{index}",
             }
             # render template to final modelica file
-            self.to_modelica(output_dir=output_dir, model_name='PVPanels', param_data=pv_params, iteration=index)
+            self.to_modelica(output_dir=output_dir, model_name="PVPanels", param_data=pv_params, iteration=index)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/generators.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,13 @@
 import logging
 from pathlib import Path
 
 from geojson_modelica_translator.modelica.simple_gmt_base import SimpleGMTBase
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
 class Generator(SimpleGMTBase):
     def __init__(self, system_parameters):
         self.system_parameters = system_parameters
         self.template_dir = Path(__file__).parent
         super().__init__(self.system_parameters, self.template_dir)
@@ -21,18 +16,15 @@
         for building_index, building in enumerate(self.system_parameters.get_param("$.buildings")):
             building_generator_params = building["diesel_generators"]
             # There can be multiple generators attached to each building so we need to loop over them
             # FIXME: This code doesn't currently support multiple generators per building
             # If multiple generators are attached to one building, only the last one will be used
             for generator_index, generator in enumerate(building_generator_params):
                 generator_params = {
-                    'source_phase_shift': generator["source_phase_shift"],
-                    'nominal_power_generation': generator["nominal_power_generation"],
-                    'model_name': f"Generator{building_index}",
+                    "source_phase_shift": generator["source_phase_shift"],
+                    "nominal_power_generation": generator["nominal_power_generation"],
+                    "model_name": f"Generator{building_index}",
                 }
             # render template to final modelica file
             self.to_modelica(
-                output_dir=output_dir,
-                model_name='Generator',
-                param_data=generator_params,
-                iteration=building_index
+                output_dir=output_dir, model_name="Generator", param_data=generator_params, iteration=building_index
             )
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/wind_turbines.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,24 +10,25 @@
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         wind_turbine_params = self.system_parameters.get_param("$.wind_turbines")
         # There can be multiple wind turbines so we need to loop over them
         for index, turbine in enumerate(wind_turbine_params):
             turbine_params = {
-                'scaling_factor': turbine["scaling_factor"],
-                'height_over_ground': turbine["height_over_ground"],
-                'nominal_voltage': turbine["nominal_voltage"],
-                'power_curve': turbine["power_curve"],
-                'model_name': f"WindTurbine{index}",
+                "scaling_factor": turbine["scaling_factor"],
+                "height_over_ground": turbine["height_over_ground"],
+                "nominal_voltage": turbine["nominal_voltage"],
+                "power_curve": turbine["power_curve"],
+                "model_name": f"WindTurbine{index}",
             }
             # FIXME: "power_curve" is a list of lists in the sys-param file.
-            # This whole string shenanigans is to format it into something that will make modelica happy.
-            # TODO: confirm that modelica chokes on a list of lists - ie comment this whole block out and see if the model will run.
-            power_curve_string = '['
+            # This whole power_curve_string shenanigans is to format it into something that will make Modelica happy.
+            power_curve_string = "["
             for point in turbine_params["power_curve"]:
-                power_curve_string += f'{point[0]}, {point[1]}; '
-            power_curve_string = power_curve_string.rstrip('; ')
-            power_curve_string += ']'
+                power_curve_string += f"{point[0]}, {point[1]}; "
+            power_curve_string = power_curve_string.rstrip("; ")
+            power_curve_string += "]"
             turbine_params["power_curve"] = power_curve_string
             # render template to final modelica file
-            self.to_modelica(output_dir=output_dir, model_name='WindTurbine', param_data=turbine_params, iteration=index)
+            self.to_modelica(
+                output_dir=output_dir, model_name="WindTurbine", param_data=turbine_params, iteration=index
+            )
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/AcBattery.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/AcBattery.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/Battery.py`

 * *Files 4% similar despite different names*

```diff
@@ -11,18 +11,15 @@
 
     def build_from_template(self, output_dir: Path):
         # TODO: add support for batteries attached to each building
         district_battery_params = self.system_parameters.get_param("$.battery_banks")
         # There can be multiple batteries so we need to loop over them
         for index, battery in enumerate(district_battery_params):
             district_battery_params = {
-                'nominal_capacity': battery["capacity"],
-                'nominal_voltage': battery["nominal_voltage"],
-                'model_name': f"AcBattery{index}",
+                "nominal_capacity": battery["capacity"],
+                "nominal_voltage": battery["nominal_voltage"],
+                "model_name": f"AcBattery{index}",
             }
             # render template to final modelica file
             self.to_modelica(
-                output_dir=output_dir,
-                model_name='AcBattery',
-                param_data=district_battery_params,
-                iteration=index
+                output_dir=output_dir, model_name="AcBattery", param_data=district_battery_params, iteration=index
             )
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/capacitor.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Storage/capacitor.py`

 * *Files 4% similar despite different names*

```diff
@@ -10,12 +10,12 @@
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
         cap_params = self.system_parameters.get_param("$.capacitor_banks")
         # There can be multiple capacitors so we need to loop over them
         for index, capacitor in enumerate(cap_params):
             cap_params = {
-                'nominal_capacity': capacitor["nominal_capacity"],
-                'model_name': f"Capacitor{index}",
+                "nominal_capacity": capacitor["nominal_capacity"],
+                "model_name": f"Capacitor{index}",
             }
             # render template to final modelica file
-            self.to_modelica(output_dir=output_dir, model_name='Capacitor', param_data=cap_params, iteration=index)
+            self.to_modelica(output_dir=output_dir, model_name="Capacitor", param_data=cap_params, iteration=index)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/PVsubsystem.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/PVsubsystem.mot`

 * *Files 0% similar despite different names*

```diff
@@ -91,9 +91,9 @@
   annotation (
     Icon(coordinateSystem(preserveAspectRatio=false, extent={{-160,-80},{140,
             140}})),
     Diagram(coordinateSystem(preserveAspectRatio=false, extent={{-160,-80},{140,
             140}})),
     uses(                            Modelica(version="4.0.0"),
       ModelicaServices(version="4.0.0"),
-      Buildings(version="9.1.0")));
+      Buildings(version="10.0.0")));
 {% endraw %}end PVsubsystem;
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/RenewableSources.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/GMT_Lib/Electrical/Examples/pv_subsystem.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/GMT_Lib/Electrical/AC/ThreePhasesBalanced/Sources/grid.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,23 @@
+import logging
 from pathlib import Path
 
 from geojson_modelica_translator.modelica.simple_gmt_base import SimpleGMTBase
 
+logger = logging.getLogger(__name__)
 
-class PVSubsystem(SimpleGMTBase):
+
+class Grid(SimpleGMTBase):
     def __init__(self, system_parameters):
         self.system_parameters = system_parameters
         self.template_dir = Path(__file__).parent
         super().__init__(self.system_parameters, self.template_dir)
 
     def build_from_template(self, output_dir: Path):
-        pv_subsystem_params = self.system_parameters.get_param("$")
-        self.to_modelica(output_dir=output_dir, model_name='PVsubsystem', param_data=pv_subsystem_params)
+        grid_params = self.system_parameters.get_param("$.electrical_grid")
+        # render template to final modelica file
+        self.to_modelica(
+            output_dir=output_dir,
+            model_name="Grid",
+            param_data=grid_params,
+        )
+        # If the sys-param file is missing an entry, it will show up as a jinja2.exceptions.UndefinedError
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/csv_modelica.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/csv_modelica.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,19 +2,17 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 from pathlib import Path
 
 import pandas as pd
 
 
-class CSVModelica(object):
-
+class CSVModelica:
     def __init__(self, input_csv_file_path, sig_fig=3):
-        """
-        Convert a CSV file into the format required by Modelica. Expects a file resulting from
+        """Convert a CSV file into the format required by Modelica. Expects a file resulting from
         https://github.com/urbanopt/DES_HVAC/tree/develop/Measures/export_time_series_modelica, which is included
         in the URBANopt SDK (potentially via common-measures-gem).
         FIXME: this is in process as of 2020-11-18
         If providing a csv file not from the DES_HVAC measure, ensure it contains the following headers in this order:
 
         0: Date/Time, string, date time. This column isn't used and will be removed upon writing out.
         1: NODE 62:System Node Temperature[C], double, Temperature hot water return, degC
@@ -30,84 +28,96 @@
         """
 
         if not Path(input_csv_file_path).exists():
             raise Exception(f"Unable to convert CSV file because this path does not exist: {input_csv_file_path}")
 
         # read the data set
         columns_to_use = [
-            'SecondsFromStart',
-            'heatingReturnTemperature[C]',
-            'heatingSupplyTemperature[C]',
-            'massFlowRateHeating',
-            'ChilledWaterReturnTemperature[C]',
-            'ChilledWaterSupplyTemperature[C]',
-            'massFlowRateCooling']
+            "SecondsFromStart",
+            "heatingReturnTemperature[C]",
+            "heatingSupplyTemperature[C]",
+            "massFlowRateHeating",
+            "ChilledWaterReturnTemperature[C]",
+            "ChilledWaterSupplyTemperature[C]",
+            "massFlowRateCooling",
+        ]
         try:
             self.timeseries_output = pd.read_csv(input_csv_file_path, usecols=columns_to_use).round(sig_fig)
         except ValueError:
             self.timeseries_output = pd.read_csv(input_csv_file_path).round(sig_fig)
 
-        if 'massFlowRateHeating' not in self.timeseries_output.columns \
-                or 'massFlowRateCooling' not in self.timeseries_output.columns:
-            raise Exception(f'Columns are missing or misspelled in your file: {input_csv_file_path}')
-
-        if 'SecondsFromStart' in self.timeseries_output.columns:
-            self.timeseries_output['heatingReturnTemperature[C]'] = self.timeseries_output[
-                'heatingReturnTemperature[C]'].round(1)
-            self.timeseries_output['heatingSupplyTemperature[C]'] = self.timeseries_output[
-                'heatingSupplyTemperature[C]'].round(1)
-            self.timeseries_output['ChilledWaterReturnTemperature[C]'] = self.timeseries_output[
-                'ChilledWaterReturnTemperature[C]'].round(1)
-            self.timeseries_output['ChilledWaterSupplyTemperature[C]'] = self.timeseries_output[
-                'ChilledWaterSupplyTemperature[C]'].round(1)
-        elif 'NODE 62:System Node Temperature[C]' in self.timeseries_output.columns:
-            self.timeseries_output['NODE 62:System Node Temperature[C]'] = self.timeseries_output[
-                'NODE 62:System Node Temperature[C]'].round(1)
-            self.timeseries_output['NODE 67:System Node Temperature[C]'] = self.timeseries_output[
-                'NODE 67:System Node Temperature[C]'].round(1)
-            self.timeseries_output['NODE 70:System Node Temperature[C]'] = self.timeseries_output[
-                'NODE 70:System Node Temperature[C]'].round(1)
-            self.timeseries_output['NODE 98:System Node Temperature[C]'] = self.timeseries_output[
-                'NODE 98:System Node Temperature[C]'].round(1)
+        if (
+            "massFlowRateHeating" not in self.timeseries_output.columns
+            or "massFlowRateCooling" not in self.timeseries_output.columns
+        ):
+            raise Exception(f"Columns are missing or misspelled in your file: {input_csv_file_path}")
+
+        if "SecondsFromStart" in self.timeseries_output.columns:
+            self.timeseries_output["heatingReturnTemperature[C]"] = self.timeseries_output[
+                "heatingReturnTemperature[C]"
+            ].round(1)
+            self.timeseries_output["heatingSupplyTemperature[C]"] = self.timeseries_output[
+                "heatingSupplyTemperature[C]"
+            ].round(1)
+            self.timeseries_output["ChilledWaterReturnTemperature[C]"] = self.timeseries_output[
+                "ChilledWaterReturnTemperature[C]"
+            ].round(1)
+            self.timeseries_output["ChilledWaterSupplyTemperature[C]"] = self.timeseries_output[
+                "ChilledWaterSupplyTemperature[C]"
+            ].round(1)
+        elif "NODE 62:System Node Temperature[C]" in self.timeseries_output.columns:
+            self.timeseries_output["NODE 62:System Node Temperature[C]"] = self.timeseries_output[
+                "NODE 62:System Node Temperature[C]"
+            ].round(1)
+            self.timeseries_output["NODE 67:System Node Temperature[C]"] = self.timeseries_output[
+                "NODE 67:System Node Temperature[C]"
+            ].round(1)
+            self.timeseries_output["NODE 70:System Node Temperature[C]"] = self.timeseries_output[
+                "NODE 70:System Node Temperature[C]"
+            ].round(1)
+            self.timeseries_output["NODE 98:System Node Temperature[C]"] = self.timeseries_output[
+                "NODE 98:System Node Temperature[C]"
+            ].round(1)
         else:
-            raise Exception(f'Columns are missing or misspelled in your file: {input_csv_file_path}')
+            raise Exception(f"Columns are missing or misspelled in your file: {input_csv_file_path}")
 
         # Dymola wants time to start at zero.
         # If time doesn't start at zero, copy the first line and set time column to zero.
-        if (self.timeseries_output.loc[0][0] != 0):
+        if self.timeseries_output.loc[0][0] != 0:
             self.timeseries_timestep = self.timeseries_output.loc[[0], :]
-            if 'SecondsFromStart' in self.timeseries_output.columns:
-                self.timeseries_timestep['SecondsFromStart'] = 0
+            if "SecondsFromStart" in self.timeseries_output.columns:
+                self.timeseries_timestep["SecondsFromStart"] = 0
             # Putting timeseries_timestep first in the concat puts the copied row at the top
             # reset_index() makes the index unique again, while keeping the duplicated row at the top
-            self.timeseries_output = pd.concat(
-                [self.timeseries_timestep, self.timeseries_output]).reset_index(drop=True)
+            self.timeseries_output = pd.concat([self.timeseries_timestep, self.timeseries_output]).reset_index(
+                drop=True
+            )
 
         # Extract the nominal flow rates from the file
         self.nominal_heating_mass_flow_rate = pd.DataFrame(
-            {'#heating': ['#Nominal heating water mass flow rate (kg/s)'],
-             '#value': [self.timeseries_output['massFlowRateHeating'].max()],
-             '#units': ['kg/s']},
-            columns=['#heating', '#value', '#units']
+            {
+                "#heating": ["#Nominal heating water mass flow rate (kg/s)"],
+                "#value": [self.timeseries_output["massFlowRateHeating"].max()],
+                "#units": ["kg/s"],
+            },
+            columns=["#heating", "#value", "#units"],
         )
         self.nominal_cooling_mass_flow_rate = pd.DataFrame(
-            {'#cooling': ['#Nominal chilled water mass flow rate (kg/s)'],
-             '#value': [self.timeseries_output['massFlowRateCooling'].max()],
-             '#units': ['kg/s']},
-            columns=['#cooling', '#value', '#units']
+            {
+                "#cooling": ["#Nominal chilled water mass flow rate (kg/s)"],
+                "#value": [self.timeseries_output["massFlowRateCooling"].max()],
+                "#units": ["kg/s"],
+            },
+            columns=["#cooling", "#value", "#units"],
         )
 
     def timeseries_to_modelica_data(
-            self,
-            output_modelica_file_name,
-            energyplus_timesteps_per_hour=4,
-            data_type='double',
-            overwrite=True):
-        """
-        Convert the loaded data to the format needed for Modelica by adding in the nominal heating water mass flow
+        self, output_modelica_file_name, energyplus_timesteps_per_hour=4, data_type="double", overwrite=True
+    ):
+        """Convert the loaded data to the format needed for Modelica by adding in the nominal heating water mass flow
         rate and the nominal cooling water mass flow rate into the header.
 
         :param output_modelica_file_name: string, The path to the desired output file name.
         :param data_type: string, data type being converted, defaults to double
         :param overwrite: boolean, if the resulting file exists, then overwrite, defaults to True.
         :return: file created to be ingested into Modelica
         """
@@ -116,28 +126,28 @@
 
         minutes_per_hour = 60
         seconds_per_minute = 60
         seconds_in_timestep = int(minutes_per_hour / energyplus_timesteps_per_hour * seconds_per_minute)
 
         # Check if output is from DES_HVAC measure or straight from E+
         # The # symbol is needed to tell Dymola this line is a comment in the output file.
-        if 'SecondsFromStart' in self.timeseries_output.columns:
-            self.timeseries_output = self.timeseries_output.rename(columns={'SecondsFromStart': '#time'})
+        if "SecondsFromStart" in self.timeseries_output.columns:
+            self.timeseries_output = self.timeseries_output.rename(columns={"SecondsFromStart": "#time"})
         else:
             self.timeseries_output.index = self.timeseries_output.index * seconds_in_timestep
-            self.timeseries_output.index.name = '#time'
-            self.timeseries_output.drop(self.timeseries_output.columns[0], axis=1, inplace=True)
+            self.timeseries_output.index.name = "#time"
+            self.timeseries_output = self.timeseries_output.drop(self.timeseries_output.columns[0], axis=1)
 
         # write to csv for modelica
         if Path(output_modelica_file_name).exists() and not overwrite:
             raise Exception(f"Output file already exists and overwrite is False: {output_modelica_file_name}")
 
-        with open(Path(output_modelica_file_name), 'w') as f:
-            line1 = '#1'
+        with open(Path(output_modelica_file_name), "w") as f:
+            line1 = "#1"
             line2 = f"{data_type} {output_modelica_file_name}({size[0]}, {size[1]})"
-            line3 = '#Nominal heating water mass flow rate=' + str(self.nominal_heating_mass_flow_rate.loc[0, '#value'])
-            line4 = '#Nominal chilled water mass flow rate=' + str(self.nominal_cooling_mass_flow_rate.loc[0, '#value'])
-            f.write('{}\n' '{}\n' '{}\n' '{}\n'.format(line1, line2, line3, line4))
-            if 'SecondsFromStart' in self.timeseries_output.columns:
+            line3 = "#Nominal heating water mass flow rate=" + str(self.nominal_heating_mass_flow_rate.loc[0, "#value"])
+            line4 = "#Nominal chilled water mass flow rate=" + str(self.nominal_cooling_mass_flow_rate.loc[0, "#value"])
+            f.write(f"{line1}\n" f"{line2}\n" f"{line3}\n" f"{line4}\n")
+            if "SecondsFromStart" in self.timeseries_output.columns:
                 self.timeseries_output.to_csv(f, header=True, index=False)
             else:
                 self.timeseries_output.to_csv(f, header=True)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/input_parser.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/input_parser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
-import os
 from pathlib import Path
 from typing import Any, List, Tuple, Union
 
 
 # TODO: This needs to be removed. It is not used anywhere in the codebase.
-class InputParser(object):
+class InputParser:
     """Class to read in Modelica files (.mo) and provide basic operations.
 
     This class is not recommended to be used and ModelicaBuilder should be used
     instead which is syntax-aware of the Modelica language.
     """
 
     def __init__(self, modelica_filename: Union[str, Path]) -> None:
@@ -21,15 +20,15 @@
             modelica_filename (Union[str, Path]): Path to the modelica file (.mo) to parse
 
         Raises:
             Exception: SyntaxError, more than one within
             Exception: SyntaxError, unknown token
 
         """
-        if not os.path.exists(modelica_filename):
+        if not Path(modelica_filename).exists():
             raise Exception(f"Modelica file does not exist: {modelica_filename}")
 
         self.modelica_filename = modelica_filename
         self.init_vars()
         self.parse_mo()
 
     def init_vars(self):
@@ -60,15 +59,15 @@
             "extends",
             "initial equation",
             "end",
         ]
         current_block = None
         obj_data = ""
         connect_data = ""
-        with open(self.modelica_filename, "r") as f:
+        with open(self.modelica_filename) as f:
             for line in f.readlines():
                 if line == "\n":
                     # Skip blank lines (for now?
                     continue
                 elif line.startswith("within"):
                     # these lines typically only have a single line, so just persist it
                     if not self.within:
@@ -95,19 +94,15 @@
                                 f"Found other token '{t}' in '{self.modelica_filename}' that is not supported... \
                                 cannot continue"
                             )
 
                 # now store data that is in between these other blocks
                 if current_block == "model":
                     # grab the lines that are comments:
-                    if (
-                        not obj_data
-                        and line.strip().startswith('"')
-                        and line.strip().endswith('"')
-                    ):
+                    if not obj_data and line.strip().startswith('"') and line.strip().endswith('"'):
                         self.model["comment"] = line.rstrip()
                         continue
 
                     # determine if this is a new object or a new object (look for ';')
                     obj_data += line
                     if line.endswith(";\n"):
                         self.model["objects"].append(obj_data)
@@ -126,16 +121,15 @@
                 elif current_block == "end":
                     pass
                 else:
                     # there is nothing to do here
                     pass
 
     def save(self) -> None:
-        """Save the resulting file to the same file from which it was initialized
-        """
+        """Save the resulting file to the same file from which it was initialized"""
         return self.save_as(self.modelica_filename)
 
     def save_as(self, new_filename: Union[str, Path]) -> None:
         """Save the resulting file with a new filename
 
         Args:
             new_filename (Union[str, Path]): name of the new file to save as
@@ -173,16 +167,15 @@
         for index, o in enumerate(self.model["objects"]):
             if obj_name in o:
                 return index, self.model["objects"][index]
 
         return None, None
 
     def reload(self):
-        """Reparse the data. This will remove any unsaved changes.
-        """
+        """Reparse the data. This will remove any unsaved changes."""
         self.init_vars()
         self.parse_mo()
 
     def replace_model_string(self, model_name: str, model_instance: str, old_string: str, new_string: str):
         """Go through the models and find the model_name with a model_instance and change the value in the field to
         the new_value. This will replace the entire value of the model field.
 
@@ -192,30 +185,28 @@
             model_name (str): name of the model
             model_instance (str): instance of the model
             old_string (str): name of the old string to replace
             new_string (str): new string
         """
         index, _ = self.find_model_object(f"{model_name} {model_instance}")
         if index is not None:
-            self.model["objects"][index] = self.model["objects"][index].replace(
-                old_string, new_string
-            )
+            self.model["objects"][index] = self.model["objects"][index].replace(old_string, new_string)
 
     def add_model_object(self, model_name: str, model_instance: str, data: List[str]) -> None:
         """Add a new model object to the model
 
         Args:
             model_name (str): name of the model
             model_instance (str): model instance name
             data (List[str]): list of data to add
         """
-        str = f"  {model_name} {model_instance}\n"
+        model_obj_str = f"  {model_name} {model_instance}\n"
         for d in data:
-            str += f"    {d}\n"
-        self.model["objects"].append(str)
+            model_obj_str += f"    {d}\n"
+        self.model["objects"].append(model_obj_str)
 
     def add_parameter(self, var_type: str, var_name: str, value: Any, description: str) -> None:
         """Add a new parameter. Will be prepended to the top of the models list
 
         Args:
             var_type (str): type of Modelica variable, Real, Integer, String, Modelica.Units.SI.Area, etc.
             var_name (str): name of the variable. Note that this does not check for conflicts.
@@ -223,15 +214,15 @@
             description (str): description of the parameter
         """
         # is the value is a string, then wrap in quotes
         if isinstance(value, str):
             value = f'"{value}"'
 
         # parameter Real fraLat= 0.8 "Fraction latent of sensible persons load = 0.8 for home, 1.25 for office.";
-        new_str = f"  parameter {var_type} {var_name}={value} \"{description}\";\n"
+        new_str = f'  parameter {var_type} {var_name}={value} "{description}";\n'
         self.model["objects"].insert(0, new_str)
 
     def add_connect(self, a: str, b: str, annotation: str) -> None:
         """Add a new connection of port a to port b. The annotation will be appended on a new line.
 
         Args:
             a (str): port a
@@ -253,24 +244,24 @@
 
         Returns:
             Tuple[Union[int, None], Union[str, None]]: index and connection tuple
         """
         for index, c in enumerate(self.connections):
             if not port_a:
                 raise Exception("Unable to replace string in connect if unknown port A")
-            if not port_b:
-                if f"({port_a}, " in c:
-                    return index, c
-            if port_a and port_b:
-                if f"({port_a}, {port_b})" in c:
-                    return index, c
+            if not port_b and f"({port_a}, " in c:
+                return index, c
+            if port_a and port_b and (f"({port_a}, {port_b})" in c):
+                return index, c
 
         return None, None
 
-    def replace_connect_string(self, a: str, b: str, new_a: Union[str, None], new_b: Union[str, None], replace_all: bool = False) -> None:
+    def replace_connect_string(
+        self, a: str, b: str, new_a: Union[str, None], new_b: Union[str, None], replace_all: bool = False
+    ) -> None:
         """Replace content of the connect string with new_a and/or new_b
 
         Args:
             a (str): existing port a
             b (str): existing port b
             new_a (str): new port (or none)
             new_b (str): new port b (or none)
@@ -303,22 +294,22 @@
         if index:
             del self.connections[index]
 
     def serialize(self) -> str:
         """Serialize the modelica object to a string with line feeds
 
         Returns:
-            str: string representation of the data
+            string_data: string representation of the data
         """
-        str = f"within {self.within};\n"
-        str += f"model {self.model['name']}\n"
-        str += f"{self.model['comment']}\n\n"
+        string_data = f"within {self.within};\n"
+        string_data += f"model {self.model['name']}\n"
+        string_data += f"{self.model['comment']}\n\n"
         for o in self.model["objects"]:
             for lx in o:
-                str += lx
-        str += "equation\n"
+                string_data += lx
+        string_data += "equation\n"
         for c in self.connections:
-            str += c
+            string_data += c
         for e in self.equations:
-            str += e
-        str += f"end {self.model['name']};\n"
-        return str
+            string_data += e
+        string_data += f"end {self.model['name']};\n"
+        return string_data
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/lib/runner/simulate.most` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/lib/runner/simulate.most`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/model_connectors/templates/RunSpawnBuilding.mot`

 * *Files 11% similar despite different names*

```diff
@@ -1,2 +1,7 @@
-simulateModel("{{project_name}}.Loads.{{model_name}}",stopTime=604800, method="Cvode", tolerance=1e-06, resultFile="{{model_name}}");
-createPlot(id=1, position={55, 50, 1783, 995}, y={% raw %}{{% endraw %}{% for zone in data['thermal_zones']%}"{{zone['modelica_object_name']}}.TAir", {% endfor %} {% raw %} "weaDat.weaBus.TDryBul", "datRea.y[1]", "datRea.y[2]", "datRea.y[3]", "datRea.y[4]", "datRea.y[5]", "datRea.y[6]", "datRea.y[7]"}, range={0.0, 620000.0, -30.0, 25.0}, grid=true, colors={{28,108,200}, {238,46,47}, {0,140,72}, {217,67,180}, {0,0,0}, {162,29,33}, {244,125,35}, {102,44,145}, {28,108,200}, {238,46,47}, {0,140,72}, {217,67,180}, {0,0,0}, {162,29,33}}, patterns={LinePattern.Solid, LinePattern.Solid, LinePattern.Solid, LinePattern.Solid,  LinePattern.Solid, LinePattern.Solid, LinePattern.Solid, LinePattern.Solid,  LinePattern.Dash, LinePattern.Dash, LinePattern.Dash, LinePattern.Dash,  LinePattern.Dash, LinePattern.Dash});{% endraw %}
+simulateModel(
+  "{{project_name}}.Loads.{{model_name}}",
+  stopTime=604800,
+  tolerance=1e-06,
+  resultFile="{{model_name}}"
+);
+createPlot(id=1, position={55, 50, 1783, 995}, y={ {% for zone in data['thermal_zones']%}"{{zone['modelica_object_name']}}.TAir", {% endfor %} {% raw %} "weaDat.weaBus.TDryBul", "datRea.y[1]", "datRea.y[2]", "datRea.y[3]", "datRea.y[4]", "datRea.y[5]", "datRea.y[6]", "datRea.y[7]"}, range={0.0, 620000.0, -30.0, 25.0}, grid=true, colors={{28,108,200}, {238,46,47}, {0,140,72}, {217,67,180}, {0,0,0}, {162,29,33}, {244,125,35}, {102,44,145}, {28,108,200}, {238,46,47}, {0,140,72}, {217,67,180}, {0,0,0}, {162,29,33}}, patterns={LinePattern.Solid, LinePattern.Solid, LinePattern.Solid, LinePattern.Solid,  LinePattern.Solid, LinePattern.Solid, LinePattern.Solid, LinePattern.Solid,  LinePattern.Dash, LinePattern.Dash, LinePattern.Dash, LinePattern.Dash,  LinePattern.Dash, LinePattern.Dash});{% endraw %}
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/model_connectors/templates/spawn_fmu.mot`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/modelica_runner.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/modelica_runner.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,79 +1,63 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
+# from __future__ import annotations
 import logging
 import os
 import shutil
 import subprocess
 from pathlib import Path
 from typing import Union
 
 from buildingspy.simulate.Dymola import Simulator
 from jinja2 import Environment, FileSystemLoader, StrictUndefined
 
 from geojson_modelica_translator.jinja_filters import ALL_CUSTOM_FILTERS
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
-class ModelicaRunner(object):
-    """
-    Class to run Modelica models.
-    """
-    ACTION_LOG_MAP = {
-        'compile': 'Compiling mo file',  # creates an FMU
-        'compile_and_run': 'Compile and run the mo file',
-        'run': 'Running FMU',
+class ModelicaRunner:
+    """Class to run Modelica models."""
+
+    ACTION_LOG_MAP = {  # noqa: RUF012
+        "compile": "Compiling mo file",  # creates an FMU
+        "compile_and_run": "Compile and run the mo file",
+        "run": "Running FMU",
     }
 
-    def __init__(self, modelica_lib_path=None):
-        """
-        Initialize the runner with data needed for simulation
-
-        :param modelica_lib_path: string, Path to the MBL to run against
-        """
-        # check if the user has defined a MODELICAPATH, is so, then use that.
-        if os.environ.get('MODELICAPATH', None):
-            print('Using predefined MODELICAPATH')
-            self.modelica_lib_path = os.environ['MODELICAPATH']
-            logger.debug(f'MODELICAPATH: {self.modelica_lib_path}')
-        else:
-            self.modelica_lib_path = modelica_lib_path
-        local_path = Path(__file__).parent.resolve()
-        self.om_docker_path = local_path / 'lib' / 'runner' / 'om_docker.sh'
+    def __init__(self):
+        """Initialize the runner with data needed for simulation"""
 
         # Verify that docker is up and running, if needed.
-        r = subprocess.call(['docker', 'ps'], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
+        r = subprocess.call(["docker", "ps"], stdout=subprocess.DEVNULL, stderr=subprocess.DEVNULL)
         self.docker_configured = r == 0
 
     def _verify_docker_run_capability(self, file_to_load: Union[str, Path, None]):
         """Verify that docker is configured on the host computer correctly before running
 
         Args:
             file_to_load (Union[str, Path]): Can be a file path or a modelica path
 
         Raises:
             SystemExit: _description_
             SystemExit: _description_
         """
         if not self.docker_configured:
-            raise SystemExit('Docker not configured on host computer, unable to run')
+            raise SystemExit("Docker not configured on host computer, unable to run")
 
         # If there is a file to load (meaning that we aren't loading from the library),
         # then check that it exists
         if file_to_load and not Path(file_to_load).exists():
-            raise SystemExit(f'File not found to run {file_to_load}')
+            raise SystemExit(f"File not found to run {file_to_load}")
 
-    def _verify_run_path_for_docker(self, run_path: Union[str, Path, None], file_to_run: Union[str, Path, None]) -> Path:
+    def _verify_run_path_for_docker(
+        self, run_path: Union[str, Path, None], file_to_run: Union[str, Path, None]
+    ) -> Path:
         """If there is no run_path, then run it in the same directory as the
         file being run. This works fine for simple Modelica projects but typically
         the run_path needs to be a few levels higher in order to include other
         project dependencies (e.g., multiple mo files).
 
         Args:
             run_path (str): directory of where to run the simulation
@@ -83,26 +67,29 @@
         Raises:
             SystemExit: Throw an exception if the run_path or file_to_run has spaces in it
 
         Returns:
             Path: Return the run_path as a Path object
         """
         if not run_path:
-            run_path = Path(file_to_run).parent  # type: ignore
+            run_path = Path(file_to_run).parent  # type: ignore[arg-type]
         new_run_path = Path(run_path)
 
         # Modelica can't handle spaces in project name or path
         if (len(str(new_run_path).split()) > 1) or (len(str(file_to_run).split()) > 1):
             raise SystemExit(
                 f"\nModelica does not support spaces in project names or paths. "
                 f"You used '{new_run_path}' for run path and {file_to_run} for model project name. "
-                "Please update your directory path or model name to not include spaces anywhere.")
+                "Please update your directory path or model name to not include spaces anywhere."
+            )
         return new_run_path
 
-    def _copy_over_docker_resources(self, run_path: Path, filename: Union[str, Path, None], model_name: str, **kwargs) -> None:
+    def _copy_over_docker_resources(
+        self, run_path: Path, filename: Union[str, Path, None], model_name: str, **kwargs
+    ) -> None:
         """Copy over files needed to run the simulation, this includes
         the generation of the OpenModelica scripts to load and compile/run
         the simulation.
 
         Must pass start_time, stop_time, and either step_size or number_of_intervals.
 
         Args:
@@ -114,110 +101,123 @@
                                              on the local file system.
                 start_time (int): start time of the simulation, in seconds
                 stop_time (int): stop time of the simulation, in seconds
                 step_size (int): step size of the simulation, in seconds
                 number_of_intervals (int): number of intervals to run the simulation
         """
         # read in the start, stop, and step times
-        project_in_library = kwargs.get('project_in_library', False)
-        start_time = kwargs.get('start_time', None)
-        stop_time = kwargs.get('stop_time', None)
-        step_size = kwargs.get('step_size', None)
-        number_of_intervals = kwargs.get('number_of_intervals', None)
+        project_in_library = kwargs.get("project_in_library", False)
+        start_time = kwargs.get("start_time", None)
+        stop_time = kwargs.get("stop_time", None)
+        step_size = kwargs.get("step_size", None)
+        number_of_intervals = kwargs.get("number_of_intervals", None)
 
         # initialize the templating framework (Jinja2)
         template_env = Environment(
-            loader=FileSystemLoader(searchpath=Path(__file__).parent.resolve() / 'lib' / 'runner'),
-            undefined=StrictUndefined
+            loader=FileSystemLoader(searchpath=Path(__file__).parent.resolve() / "lib" / "runner"),
+            undefined=StrictUndefined,
         )
         template_env.filters.update(ALL_CUSTOM_FILTERS)
-        template = template_env.get_template('simulate.most')
+        template = template_env.get_template("simulate.most")
         model_data = {
             "project_in_library": project_in_library,
             "file_to_load": Path(filename).name if filename else None,
             "model_name": model_name,
-            "use_default_time_params": False if start_time is not None and stop_time is not None else True,
+            "use_default_time_params": not start_time
+            and not stop_time,  # https://docs.astral.sh/ruff/rules/if-expr-with-false-true/#flake8-simplify-sim
             "start_time": start_time,
             "stop_time": stop_time,
             "step_size": step_size,
             "number_of_intervals": number_of_intervals,
         }
-        with open(run_path / 'simulate.mos', 'w') as f:
+        with open(run_path / "simulate.mos", "w") as f:
             f.write(template.render(**model_data))
-        template = template_env.get_template('compile_fmu.most')
-        with open(run_path / 'compile_fmu.mos', 'w') as f:
+        template = template_env.get_template("compile_fmu.most")
+        with open(run_path / "compile_fmu.mos", "w") as f:
             f.write(template.render(**model_data))
 
-        # new om_docker.sh file name
-        new_om_docker = run_path / self.om_docker_path.name
-        shutil.copyfile(self.om_docker_path, new_om_docker)
-        Path.chmod(new_om_docker, 0o775)
-
-    def _subprocess_call_to_docker(self, run_path: Union[str, Path], action: str) -> int:
+    def _subprocess_call_to_docker(self, run_path: Path, action: str) -> int:
         """Call out to a subprocess to run the command in docker
 
         Args:
             run_path (Path): local path where the Modelica simulation or compilation will start
             action (str):  action to run either compile_and_run, compile, or run
 
         Returns:
             int: exit code of the subprocess
         """
         # Set up the run content
         curdir = Path.cwd()
         os.chdir(run_path)
-        stdout_log = open('stdout.log', 'w')
+        stdout_log = open("stdout.log", "w")  # noqa: SIM115
+        model_name = run_path.parts[-1]
+        image_name = "nrel/gmt-om-runner:v2.0.1"
+        mo_script = "compile_fmu" if action == "compile" else "simulate"
         try:
-            # get the relative difference between the file to run and the path which everything is running in.
-            # make sure to simulate at a directory above the project directory!
-
-            # Use slashes for the location of the model to run. We can make these periods `.replace(os.sep, '.')`
-            # but must strip off the .mo extension on the model to run
-            # run_model = Path(file_to_run).relative_to(run_path)
-            exec_call = ['./om_docker.sh', action]
+            # create the command to call the open modelica compiler inside the docker image
+            exec_call = [
+                "docker",
+                "run",
+                "-v",
+                f"{run_path}:/mnt/shared/{model_name}",
+                f"{image_name}",
+                "/bin/bash",
+                "-c",
+                f"cd mnt/shared/{model_name} && omc {mo_script}.mos",
+            ]
+            # execute the command that calls docker
             logger.debug(f"Calling {exec_call}")
-            p = subprocess.Popen(
-                exec_call,  # type: ignore
+            completed_process = subprocess.run(
+                exec_call,
                 stdout=stdout_log,
                 stderr=subprocess.STDOUT,
-                cwd=run_path
+                cwd=run_path,
+                check=False,
             )
             # Uncomment this section and rebuild the container in order to pause the container
             # to inspect the container and test commands.
             # import time
             # time.sleep(10000)  # wait for the subprocess to start
-            logger.debug(f"Subprocess command executed, waiting for completion... \nArgs used: {p.args}")
-            exitcode = p.wait()
+            logger.debug(
+                f"Subprocess command executed, waiting for completion... \nArgs used: {completed_process.args}"
+            )
         except KeyboardInterrupt:
             # List all containers and their images
-            docker_containers_cmd = ['docker', 'ps', '--format', '{{.ID}} {{.Image}}']
-            containers_list = subprocess.check_output(docker_containers_cmd, text=True).rstrip().split('\n')
+            docker_containers_cmd = ["docker", "ps", "--format", "{{.ID}} {{.Image}}"]
+            containers_list = subprocess.check_output(docker_containers_cmd, text=True).rstrip().split("\n")
 
             # Find containers from our image
-            image_name = 'nrel/gmt-om-runner'
             for container_line in containers_list:
                 container_id, container_image = container_line.split()
                 if container_image == image_name:
                     logger.debug(f"Killing container: {container_id} (Image: {container_image})")
                     # Kill the container
                     kill_command = f"docker kill {container_id}"
                     subprocess.run(kill_command.split(), check=True, text=True)
             # Remind user why the simulation didn't complete
             raise SystemExit("Simulation stopped by user KeyboardInterrupt")
         finally:
             os.chdir(curdir)
             stdout_log.close()
-            logger.debug('Closed stdout.log')
+            logger.debug("Closed stdout.log")
 
-        return exitcode
+        return completed_process.returncode
 
-    def run_in_docker(self, action: str, model_name: str, file_to_load: Union[str, Path, None] = None,
-                      run_path: Union[str, Path, None] = None, **kwargs) -> tuple[bool, Union[str, Path]]:
-        """Run the Modelica project in a docker-based environment. The action will determine
-        what type of run will be conducted. This method supports either a file path pointing to the package to load, or a modelica path which is a period separated path. Results are saved into run_path.
+    def run_in_docker(
+        self,
+        action: str,
+        model_name: str,
+        file_to_load: Union[str, Path, None] = None,
+        run_path: Union[str, Path, None] = None,
+        **kwargs,
+    ) -> tuple[bool, Union[str, Path]]:
+        """Run the Modelica project in a docker-based environment.
+        The action will determine what type of run will be conducted.
+        This method supports either a file path pointing to the package to load, or a modelica path which is a
+        period separated path. Results are saved into run_path.
 
         stdout.log will store both stdout and stderr of the simulations
 
         Args:
             action (str): The action to run, must be one of compile_and_run, compile, or run
             model_name (str): The name of the model to be simulated (this is the name within Modelica)
             file_to_load (str, Path): The file path or a modelica path to be simulated
@@ -231,59 +231,79 @@
                 debug (bool): whether to run in debug mode or not, prevents files from being deleted.
 
         Returns:
             tuple[bool, str]: success status and path to the results directory
         """
         # Verify that the action is in the list of valid actions
         if action not in ModelicaRunner.ACTION_LOG_MAP:
-            raise SystemExit(f'Invalid action {action}, must be one of {list(ModelicaRunner.ACTION_LOG_MAP.keys())}')
+            raise SystemExit(f"Invalid action {action}, must be one of {list(ModelicaRunner.ACTION_LOG_MAP.keys())}")
 
         self._verify_docker_run_capability(file_to_load)
         verified_run_path = self._verify_run_path_for_docker(run_path, file_to_load)
 
-        self._copy_over_docker_resources(
-            verified_run_path, file_to_load, model_name, **kwargs
-        )
+        self._copy_over_docker_resources(verified_run_path, file_to_load, model_name, **kwargs)
 
         exitcode = self._subprocess_call_to_docker(verified_run_path, action)
 
-        logger.debug('checking stdout.log for errors')
-        # Check the stdout.log file for errors
-        with open(verified_run_path / 'stdout.log', 'r') as f:
+        logger.debug("Checking stdout.log for errors")
+        with open(verified_run_path / "stdout.log") as f:
             stdout_log = f.read()
-            if 'Failed to build model' in stdout_log:
-                logger.error('Model failed to build')
+            if "Failed to build model" in stdout_log:
+                logger.error("Model failed to build")
                 exitcode = 1
-            elif 'The simulation finished successfully' in stdout_log:
-                logger.info('Model ran successfully')
+            elif "Killed" in stdout_log:
+                logger.error(
+                    "Model is too large for the Docker resources available."
+                    " Increase Docker resources, decrease number of buildings simulated, or both"
+                )
+            elif "division by zero at time" and "Simulation execution failed for model:" in stdout_log:
+                logger.error("Model failed to run due to division by zero")
+                exitcode = 1
+            elif "The simulation finished successfully" in stdout_log:
+                logger.info("Model ran successfully")
                 exitcode = 0
-            elif action == 'compile':
-                logger.info('Model compiled successfully -- no errors')
+            elif action == "compile":
+                logger.info("Model compiled successfully -- no errors")
                 exitcode = 0
             else:
-                logger.error('Model failed to run -- unknown error')
+                logger.error("Model failed to run -- unknown error")
                 exitcode = 1
 
-        logger.debug('removing temporary files')
         # Cleanup all of the temporary files that get created
-        self.cleanup_path(verified_run_path, model_name, debug=kwargs.get('debug', False))
+        self.cleanup_path(verified_run_path, model_name, debug=kwargs.get("debug", False))
 
-        logger.debug('moving results to results directory')
+        logger.debug("Moving results to results directory")
         # get the location of the results path
-        results_path = Path(verified_run_path / f'{model_name}_results')
+        results_path = Path(verified_run_path / f"{model_name}_results")
         self.move_results(verified_run_path, results_path, model_name)
         return (exitcode == 0, results_path)
 
-    def run_in_dymola(self, action: str, model_name: str, file_to_load: Union[str, Path], run_path: Union[str, Path], **kwargs) -> tuple[bool, Union[str, Path]]:
+    def run_in_dymola(
+        self, action: str, model_name: str, file_to_load: Union[str, Path], run_path: Union[str, Path], **kwargs
+    ) -> tuple[bool, Union[str, Path]]:
         """If running on Windows or Linux, you can run Dymola (assuming you have a license),
         using the BuildingsPy library. This is not supported on Mac.
 
         For using Dymola with the GMT, you need to ensure that MSL v4.0 are loaded correctly and that the
         Buildings library is in the MODELICAPATH. I added the MSL openModel via appending it to the Dymola's
-        /opt/<install>/install/dymola.mos file on Linux.
+        /opt/<install>/insert/dymola.mos file on Linux. The additions to the dymola.mos will look like the following:
+
+            ```modelica
+            // If using Dymola 2024, then the MSL v4.0.0 is already loaded
+            // If needed, install the patch of the Modelica Standard Library v4.0.0 (Services)
+            openModel("/home/username/Dymola/MSL_v4_ServicesPatch/ModelicaServices/package.mo", changeDirectory=false);
+            // If needed, install MSL v4
+            openModel("/home/username/Dymola/config/Modelica 4.0.0/package.mo", changeDirectory=false);
+
+            // Open MBL
+            openModel("/home/username/working/modelica-buildings/Buildings/package.mo", changeDirectory=false);
+
+            // Set the home directory
+            cd("/home/username/working")
+            ```
 
         Args:
             action (str): compile (translate) or simulate
             model_name (str): Name of the model to translate or simulate
             package_path (Union[str, Path]): Name of the package to also load
             kwargs: additional arguments to pass to the runner which can include
                 start_time (float): start time of the simulation
@@ -314,46 +334,46 @@
                     packagePath=file_to_load,
                 )
 
             # TODO: add in passing of parameters
             # dymola_simulator.addParameters({'PI.k': 10.0, 'PI.Ti': 0.1})
             dymola_simulator.setSolver("dassl")
 
-            start_time = kwargs.get('start_time', 0)
-            stop_time = kwargs.get('stop_time', 300)
-            step_size = kwargs.get('step_size', 5)
+            start_time = kwargs.get("start_time", 0)
+            stop_time = kwargs.get("stop_time", 300)
+            step_size = kwargs.get("step_size", 5)
 
             # calculate the number of intervals based on the step size
             number_of_intervals = int((stop_time - start_time) / step_size)
 
             dymola_simulator.setStartTime(start_time)
             dymola_simulator.setStopTime(stop_time)
             dymola_simulator.setNumberOfIntervals(number_of_intervals)
 
             # Do not show progressbar! -- It will cause an "elapsed time used before assigned" error.
             # dymola_simulator.showProgressBar(show=True)
 
-            if kwargs.get('debug', False):
+            if kwargs.get("debug", False):
                 dymola_simulator.showGUI(show=True)
                 dymola_simulator.exitSimulator(False)
 
             # BuildingPy throws an exception if the model errs
             try:
-                if action == 'compile':
+                if action == "compile":
                     dymola_simulator.translate()
                     # the results of this does not create an FMU, just
                     # the status of the translation/compilation.
-                elif action == 'simulate':
+                elif action == "simulate":
                     dymola_simulator.simulate()
-            except Exception as e:
+            except Exception as e:  # noqa: BLE001
                 logger.error(f"Exception running Dymola: {e}")
                 return False, run_path
 
             # remove some of the unneeded results
-            self.cleanup_path(Path(run_path), model_name, debug=kwargs.get('debug', False))
+            self.cleanup_path(Path(run_path), model_name, debug=kwargs.get("debug", False))
         finally:
             os.chdir(current_dir)
 
         return True, run_path
 
     def move_results(self, from_path: Path, to_path: Path, model_name: Union[str, None] = None) -> None:
         """This method moves the results of the simulation that are known for now.
@@ -366,75 +386,85 @@
             from_path (Path): where the files will move from
             to_path (Path): where the files will be saved. Will be created if does not exist.
             model_name (Union[str, None], optional): name of the project ran in run_in_docker method. Defaults to None.
         """
         to_path.mkdir(parents=True, exist_ok=True)
 
         files_to_move = [
-            'stdout.log',
+            "stdout.log",
         ]
         if model_name is not None:
-            files_to_move.append(f'{model_name}.log',)
-            files_to_move.append(f'{model_name}.fmu',)
-            files_to_move.append(f"{model_name.replace('.', '_')}.log",)
-            files_to_move.append(f"{model_name.replace('.', '_')}_FMU.log",)
+            files_to_move.append(
+                f"{model_name}.log",
+            )
+            files_to_move.append(
+                f"{model_name}.fmu",
+            )
+            files_to_move.append(
+                f"{model_name.replace('.', '_')}.log",
+            )
+            files_to_move.append(
+                f"{model_name.replace('.', '_')}_FMU.log",
+            )
 
         for to_move in from_path.iterdir():
-            if not to_move == to_path:
-                if (to_move.name in files_to_move) or to_move.name.startswith(f'{model_name}_'):
-                    # typecast back to strings for the shutil method.
-                    shutil.move(str(to_move), str(to_path / to_move.name))
+            if to_move != to_path and ((to_move.name in files_to_move) or to_move.name.startswith(f"{model_name}_")):
+                # typecast back to strings for the shutil method.
+                shutil.move(str(to_move), str(to_path / to_move.name))
 
     def cleanup_path(self, path: Path, model_name: str, **kwargs: dict) -> None:
         """Clean up the files in the path that was presumably used to run the simulation.
         If debug is passed, then simulation running files will not be removed, but the
         intermediate simulation files will be removed (e.g., .c, .h, .o, .bin)
 
         Args:
             path (Path): Path of the folder to clean
             model_name (str): Name of the model, used to remove model-specific intermediate files
             kwargs: additional arguments to pass to the runner which can include
                 debug (bool): whether to remove all files or not
         """
         # list of files to always remove
         files_to_remove = [
-            'dsin.txt',
-            'dsmodel.c',
-            'dymosim',
-            'request.',
-            f'{model_name}',
-            f'{model_name}.makefile',
-            f'{model_name}.libs',
+            "dsin.txt",
+            "dsmodel.c",
+            "dymosim",
+            "request.",
+            f"{model_name}",
+            f"{model_name}.makefile",
+            f"{model_name}.libs",
             f"{model_name.replace('.', '_')}_info.json",
             f"{model_name.replace('.', '_')}_FMU.makefile",
             f"{model_name.replace('.', '_')}_FMU.libs",
         ]
 
         conditional_remove_files = [
-            'om_docker.sh',
-            'compile_fmu.mos',
-            'simulate.mos',
-            'run.mos',
-            'run_translate.mos',
+            "compile_fmu.mos",
+            "simulate.mos",
+            "run.mos",
+            "run_translate.mos",
         ]
 
-        if not kwargs.get('debug', False):
+        logger.debug("Removing temporary files")
+
+        if not kwargs.get("debug", False):
+            logger.debug("...and removing intermediate files")
             files_to_remove.extend(conditional_remove_files)
 
         for f in files_to_remove:
             (path / f).unlink(missing_ok=True)
 
         # The other files below will always be removed, debug or not
 
         # glob for the .c, .h, .o, .bin files to remove
         remove_files_glob = [
-            f'{model_name}*.c',
-            f'{model_name}*.h',
-            f'{model_name}*.o',
-            f'{model_name}*.bin',
+            f"{model_name}*.c",
+            f"{model_name}*.h",
+            f"{model_name}*.o",
+            f"{model_name}*.bin",
         ]
         for pattern in remove_files_glob:
-            for f in path.glob(pattern):  # type: ignore
+            for f in path.glob(pattern):  # type: ignore[assignment]
                 Path(f).unlink(missing_ok=True)
 
-        # Note that the om.py script that runs within the container does cleanup
-        # the 'tmp' folder including the 'tmp/temperatureResponseMatrix' folder
+        # Remove the 'tmp' folder that was created by 5G simulations
+        # Dir won't exist for 4G simulations, so ignoring errors
+        shutil.rmtree(path / "tmp", ignore_errors=True)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/modelica/simple_gmt_base.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/modelica/simple_gmt_base.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,82 +1,85 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
+# https://docs.astral.sh/ruff/rules/implicit-optional/ for to_modelica arg: partial_files
+from __future__ import annotations
+
 from pathlib import Path
 
 from modelica_builder.package_parser import PackageParser
 
 from geojson_modelica_translator.model_connectors.model_base import ModelBase
 
 
 class SimpleGMTBase(ModelBase):
     """Base class for simple GMT models."""
 
     def __init__(self, system_parameters, template_dir):
-        """
-        Initialize the SimpleGMT object.
-        """
+        """Initialize the SimpleGMT object."""
         super().__init__(system_parameters, template_dir)
 
-    def to_modelica(self, output_dir: Path, model_name: str, param_data: dict, iteration=None,
-                    save_file_name=None, generate_package=False, partial_files: dict = None) -> None:
+    def to_modelica(
+        self,
+        output_dir: Path,
+        model_name: str,
+        param_data: dict,
+        iteration=None,
+        save_file_name=None,
+        generate_package=False,
+        partial_files: dict | None = None,
+    ) -> None:
         """Render the template to a Modelica file.
 
         Args:
-            output_dir (Path): Directory to save the resulting template (modelica file) to.
-            model_name (str): Model to render and also the name of the saved file (if save_file_name is None).
-            param_data (dict): Data to pass to the rendering template.
-            iteration (Int, optional): If dynamically creating filenames, then this is the iteration to
-                                       be appended to the filename. Defaults to None.
-            save_file_name (Str, optional): Name that the file will be saved as, if None, then will default.
-                                            Do not include the directory, only the filename (with extension).
-                                            Defaults to None.
-            generate_package (bool, optional): If True, then a package.mo and package.order file will be created
-                                               alongside the rendered template (Modelica) file. Defaults to False.
-            partial_files (dict, optional): If the model has partial files, then this is a dictionary of the
-                                            partial file name and the Modelica file name to save it as. Defaults to None.
+        - output_dir (Path): Directory to save the resulting template (modelica file) to.
+        - model_name (str): Model to render and also the name of the saved file (if save_file_name is None).
+        - param_data (dict): Data to pass to the rendering template.
+        - iteration (Int, optional): If dynamically creating filenames, then this is the iteration to
+                                    be appended to the filename. Defaults to None.
+        - save_file_name (Str, optional): Name that the file will be saved as, if None, then will default.
+                                        Do not include the directory, only the filename (with extension).
+                                        Defaults to None.
+        - generate_package (bool, optional): If True, then a package.mo and package.order file will be created
+                                            alongside the rendered template (Modelica) file. Defaults to False.
+        - partial_files (dict, optional): If the model has partial files, then this is a dictionary of the
+                                        partial file name and the Modelica file name to save it as. Defaults to None.
         """
         # render template to final modelica file
         model_template = self.template_env.get_template(f"{model_name}.mot")
 
         # If the user passes in save_file_name, then use that name instead of trying
         # to figure out the name.
         if not save_file_name:
-            if iteration is not None or iteration == '':
+            if iteration is not None or iteration == "":
                 save_file_name = output_dir / f"{model_name}{iteration}.mo"
             else:
                 save_file_name = output_dir / f"{model_name}.mo"
         else:
             save_file_name = output_dir / save_file_name
 
         self.run_template(
-            template=model_template,
-            save_file_name=save_file_name,
-            project_name=output_dir.stem,
-            data=param_data
+            template=model_template, save_file_name=save_file_name, project_name=output_dir.stem, data=param_data
         )
 
         # store the order of the models that will be in the package (if requested)
         package_order = []
         package_order.append(save_file_name.stem)
 
         # Check if there are partial models (or other templated data) to be evaluated / saved.
         if partial_files:
             for template, filename in partial_files.items():
                 self.run_template(
                     template=self.template_env.get_template(f"{template}.mot"),
                     save_file_name=output_dir / f"{filename}.mo",
                     project_name=output_dir.stem,
-                    data=param_data
+                    data=param_data,
                 )
                 package_order.insert(0, filename)
 
         # include package.mo and package.order files if requested.
         # TODO: This will need to be updated to support multiple models in the "order".
         if generate_package:
             package = PackageParser.new_from_template(
-                str(output_dir),
-                output_dir.stem,
-                order=package_order,
-                within=output_dir.parent.stem
+                str(output_dir), output_dir.stem, order=package_order, within=output_dir.parent.stem
             )
             package.save()
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/scaffold.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/scaffold.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import shutil
 
 from geojson_modelica_translator.utils import ModelicaPath
 
 _log = logging.getLogger(__name__)
 
 
-class Scaffold(object):
+class Scaffold:
     """Scaffold to hold the entire directory structure for the project. The purpose of this class is to
     allow a developer/user to easily access the various paths of the project without having to
     manually strip/replace strings/filenames/paths/etc.
 
     The project structure where an URBANopt-Modelica analysis will occur follows a well
     defined structure and includes multiple levels of nested directories, data files, and scripts.
 
@@ -49,37 +49,38 @@
             else:
                 shutil.rmtree(self.project_path)
 
     def create(self, ignore_paths=[]):
         """run the scaffolding to create the directory structure for DES systems
 
         Args:
-            ignore_paths (list, optional): List of paths NOT to create. Choose from Loads, Substations, Plants, Districts, Networks. Defaults to [].
+            ignore_paths (list, optional): List of paths NOT to create.
+                Choose from Loads, Substations, Plants, Districts, Networks. Defaults to [].
         """
         # initialize all of path objects
         self.loads_path = None
         self.substations_path = None
         self.plants_path = None
         self.districts_path = None
         self.networks_path = None
 
         # leverage the ModelicaPath function
-        if 'Loads' not in ignore_paths:
+        if "Loads" not in ignore_paths:
             self.loads_path = ModelicaPath("Loads", root_dir=self.project_path, overwrite=self.overwrite)
 
-        if 'Substations' not in ignore_paths:
+        if "Substations" not in ignore_paths:
             self.substations_path = ModelicaPath("Substations", root_dir=self.project_path, overwrite=self.overwrite)
 
-        if 'Plants' not in ignore_paths:
+        if "Plants" not in ignore_paths:
             self.plants_path = ModelicaPath("Plants", root_dir=self.project_path, overwrite=self.overwrite)
 
-        if 'Districts' not in ignore_paths:
+        if "Districts" not in ignore_paths:
             self.districts_path = ModelicaPath("Districts", root_dir=self.project_path, overwrite=self.overwrite)
 
-        if 'Networks' not in ignore_paths:
+        if "Networks" not in ignore_paths:
             self.networks_path = ModelicaPath("Networks", root_dir=self.project_path, overwrite=self.overwrite)
 
     def clear_or_create_path(self, path, overwrite=False):
         if os.path.exists(path):
             if not overwrite:
                 raise Exception("Directory already exists and overwrite is false for %s" % path)
             else:
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/schema.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/schema.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999870207004253%*

 * *Differences: {"'definitions'": "{'fourth_generation_def': {'properties': {'fourth_generation': {'properties': "*

 * *                  "{'central_pump_parameters': OrderedDict([('description', 'Parameters for "*

 * *                  "central pump'), ('type', 'object'), ('properties', "*

 * *                  "OrderedDict([('pump_design_head', OrderedDict([('description', 'Measured in "*

 * *                  "Pa'), ('type', 'number')]))]))])}}}}, 'fifth_generation_def': {'properties': "*

 * *                  "{'fifth_generation': {'properties […]*

```diff
@@ -380,21 +380,21 @@
             "type": "object"
         },
         "design_def": {
             "description": "Design parameters used for GHE sizing.",
             "properties": {
                 "flow_rate": {
                     "default": 0.3,
-                    "description": "Nominal design mass flow rate. Depending on whether the flow_type attribute is set to 'borehole' or 'system', this will be the nominal flow rate for either each borehole or the entire ground heat exchanger.",
+                    "description": "Nominal design mass flow rate, in l/s. Depending on whether the flow_type attribute is set to 'borehole' or 'system', this will be the nominal flow rate for either each borehole or the entire ground heat exchanger.",
                     "minimum": 0,
                     "type": "number"
                 },
                 "flow_type": {
                     "default": "borehole",
-                    "description": "Flow type for ground heat exchanger sizing, in l/s.",
+                    "description": "Flow type for ground heat exchanger sizing",
                     "enum": [
                         "borehole",
                         "system"
                     ],
                     "type": "string"
                 },
                 "max_eft": {
@@ -683,26 +683,37 @@
                 }
             },
             "required": [
                 "supply_water_temperature_building",
                 "chilled_water_supply_temp",
                 "hot_water_supply_temp",
                 "cop_heat_pump_heating",
+                "cop_heat_pump_cooling",
                 "pump_flow_rate",
                 "pump_design_head",
                 "ets_pump_flow_rate",
                 "ets_pump_head",
                 "fan_design_flow_rate",
                 "fan_design_head"
             ]
         },
         "fifth_generation_def": {
             "properties": {
                 "fifth_generation": {
                     "properties": {
+                        "central_pump_parameters": {
+                            "description": "Parameters for central pump",
+                            "properties": {
+                                "pump_design_head": {
+                                    "description": "Measured in Pa.",
+                                    "type": "number"
+                                }
+                            },
+                            "type": "object"
+                        },
                         "connected_buildings": {
                             "items": [
                                 {
                                     "properties": {
                                         "building_id": {
                                             "description": "This is the geojson_id that is defined in the building object."
                                         }
@@ -761,14 +772,24 @@
                     "properties": {
                         "central_cooling_plant_parameters": {
                             "$ref": "#/definitions/central_cooling_plant_parameters"
                         },
                         "central_heating_plant_parameters": {
                             "$ref": "#/definitions/central_heating_plant_parameters"
                         },
+                        "central_pump_parameters": {
+                            "description": "Parameters for central pump",
+                            "properties": {
+                                "pump_design_head": {
+                                    "description": "Measured in Pa",
+                                    "type": "number"
+                                }
+                            },
+                            "type": "object"
+                        },
                         "combined_heat_and_power_parameters": {
                             "$ref": "#/definitions/combined_heat_and_power_parameters"
                         },
                         "connected_buildings": {
                             "items": [
                                 {
                                     "properties": {
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/system_parameters.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/system_parameters.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,88 +1,83 @@
 # :copyright (c) URBANopt, Alliance for Sustainable Energy, LLC, and other contributors.
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 import json
 import logging
 import math
+from contextlib import suppress
 from copy import deepcopy
 from pathlib import Path
 from typing import Union
 
 import pandas as pd
 import requests
 from jsonpath_ng.ext import parse
 from jsonschema.validators import Draft202012Validator as LatestValidator
 
 logger = logging.getLogger(__name__)
-logging.basicConfig(
-    level=logging.INFO,
-    format='%(asctime)s - %(levelname)s: %(message)s',
-    datefmt='%d-%b-%y %H:%M:%S',
-)
 
 
-class SystemParameters(object):
-    """
-    Object to hold the system parameter data (and schema).
-    """
+class SystemParameters:
+    """Object to hold the system parameter data and schema"""
 
-    PATH_ELEMENTS = [
+    PATH_ELEMENTS = (  # immutable tuple of dicts
         {"json_path": "$.buildings[?load_model=spawn].load_model_parameters.spawn.idf_filename"},
         {"json_path": "$.buildings[?load_model=spawn].load_model_parameters.spawn.epw_filename"},
         {"json_path": "$.buildings[?load_model=spawn].load_model_parameters.spawn.mos_weather_filename"},
         {"json_path": "$.buildings[?load_model=rc].load_model_parameters.rc.mos_weather_filename"},
         {"json_path": "$.buildings[?load_model=time_series].load_model_parameters.time_series.filepath"},
-        {"json_path": "$.buildings[?load_model=time_series_massflow_temperature].load_model_parameters.time_series.filepath"},
+        {
+            "json_path": "$.buildings[?load_model=time_series_massflow_temperature].load_model_parameters.time_series.filepath"  # noqa: E501
+        },
         {"json_path": "$.weather"},
-        {"json_path": "$.combined_heat_and_power_systems.[*].performance_data_path"}
-    ]
+        {"json_path": "$.combined_heat_and_power_systems.[*].performance_data_path"},
+    )
 
     def __init__(self, filename=None):
-        """
-        Read in the system design parameter file
+        """Read in the system design parameter file
 
         :param filename: string, (optional) path to file to load
         """
         # load the schema for validation
         schema = Path(__file__).parent / "schema.json"
         self.schema = json.loads(schema.read_text())
         self.param_template = {}
         self.filename = filename
 
         if self.filename:
             if Path(self.filename).is_file():
-                with open(self.filename, "r") as f:
+                with open(self.filename) as f:
                     self.param_template = json.load(f)
             else:
-                raise Exception(f"System design parameters file does not exist: {self.filename}")
+                raise FileNotFoundError(f"System design parameters file does not exist: {self.filename}")
 
             errors = self.validate()
             if len(errors) != 0:
-                raise Exception(f"Invalid system parameter file. Errors: {errors}")
+                raise ValueError(f"Invalid system parameter file. Errors: {errors}")
 
             self.resolve_paths()
 
         self.sys_param_filename = None
 
     @classmethod
     def loadd(cls, d, validate_on_load=True):
-        """
-        Create a system parameters instance from a dictionary
+        """Create a system parameters instance from a dictionary
+
         :param d: dict, system parameter data
 
         :return: object, SystemParameters
         """
         sp = cls()
         sp.param_template = d
 
         if validate_on_load:
             errors = sp.validate()
             if len(errors) != 0:
-                raise Exception(f"Invalid system parameter file. Errors: {errors}")
+                raise ValueError(f"Invalid system parameter file. Errors: {errors}")
 
         return sp
 
     def resolve_paths(self):
         """Resolve the paths in the file to be absolute if they were defined as relative. This method uses
         the JSONPath (with ext) to find if the value exists in the self.param_template object. If so, it then uses
         the set_param which navigates the JSON tree to set the value as needed."""
@@ -145,36 +140,42 @@
             results = results[0]
         elif len(results) == 0:
             return default_value
 
         # otherwise return the list of values
         return results
 
-    def get_param_by_building_id(self, building_id, jsonpath):
-        """
-        return a parameter for a specific building_id. This is similar to get_param but allows the user
-        to constrain the data based on the building id.
+    def get_param_by_id(self, param_id, jsonpath):
+        """Return a parameter for a specific id. This is similar to get_param but allows the user
+        to constrain the data based on the id.
 
-        :param building_id: string, id of the building to look up in the custom section of the system parameters
+        :param param_id: string, id of the object to look up in the system parameters file
         :param jsonpath: string, jsonpath formatted string to return
-        :param default: variant, (optional) value to return if can't find the result
         :return: variant, the value from the data
         """
 
+        # TODO: check that ids are unique in the system parameters file, i.e., a building_id doesn't match a ghe_id
         for b in self.param_template.get("buildings", []):
-            if b.get("geojson_id", None) == building_id:
+            if b.get("geojson_id") == param_id:
                 return self.get_param(jsonpath, data=b)
-        else:
-            raise SystemExit("No building_id submitted. Please retry and include the feature_id")
+        with suppress(KeyError):
+            # If this dict key doesn't exist then either this is a 4G district, no id was passed, or it wasn't a ghe_id
+            # Don't crash or quit, just keep a stiff upper lip and carry on.
+            district = self.param_template.get("district_system")
+            for ghe in district["fifth_generation"]["ghe_parameters"]["ghe_specific_params"]:
+                if ghe.get("ghe_id") == param_id:
+                    return self.get_param(jsonpath, data=ghe)
+        if param_id is None:
+            raise SystemExit("No id submitted. Please retry and include the appropriate id")
 
     def validate(self):
-        """
-        Validate an instance against a loaded schema
+        """Validate an instance against a loaded schema
 
         :param instance: dict, json instance to validate
+
         :return: validation results
         """
         results = []
         v = LatestValidator(self.schema)
         for error in sorted(v.iter_errors(self.param_template), key=str):
             results.append(error.message)
 
@@ -182,734 +183,757 @@
 
     def download_weatherfile(self, filename, save_directory: str) -> Union[str, Path]:
         """Download the MOS or EPW weather file from energyplus.net
 
         This routine downloads the weather file, either an MOS or EPW, which is selected based
         on the file extension.
 
-            filename, str: Name of weather file to download, e.g., USA_NY_Buffalo-Greater.Buffalo.Intl.AP.725280_TMY3.mos
-            save_directory, str: Location where to save the downloaded content. The path must exist before downloading.
+        filename, str: Name of weather file to download, e.g., USA_NY_Buffalo-Greater.Buffalo.Intl.AP.725280_TMY3.mos
+        save_directory, str: Location where to save the downloaded content. The path must exist before downloading.
         """
         p_download = Path(filename)
         p_save = Path(save_directory)
 
         if not p_save.is_dir():
-            print(f"Creating directory to save weather file, {str(p_save)}")
+            print(f"Creating directory to save weather file, {p_save!s}")
             p_save.mkdir(parents=True, exist_ok=True)
 
         # get country & state from weather file name
         try:
             weatherfile_location_info = p_download.parts[-1].split("_")
             weatherfile_country = weatherfile_location_info[0]
             weatherfile_state = weatherfile_location_info[1]
         except IndexError:
-            raise Exception(
-                "Malformed location, needs underscores of location (e.g., USA_NY_Buffalo-Greater.Buffalo.Intl.AP.725280_TMY3.mos)"
+            raise IndexError(
+                "Malformed location, needs underscores of location "
+                "(e.g., USA_NY_Buffalo-Greater.Buffalo.Intl.AP.725280_TMY3.mos)"
             )
 
         # download file from energyplus website
-        weatherfile_url = 'https://energyplus-weather.s3.amazonaws.com/north_and_central_america_wmo_region_4/' \
-            f'{weatherfile_country}/{weatherfile_state}/{p_download.stem}/{p_download.name}'
+        weatherfile_url = (
+            "https://energyplus-weather.s3.amazonaws.com/north_and_central_america_wmo_region_4/"
+            f"{weatherfile_country}/{weatherfile_state}/{p_download.stem}/{p_download.name}"
+        )
         outputname = p_save / p_download.name
         logger.debug(f"Downloading weather file from {weatherfile_url}")
         try:
-            weatherfile_data = requests.get(weatherfile_url)
+            weatherfile_data = requests.get(weatherfile_url, timeout=(5, 5))
             if weatherfile_data.status_code == 200:
-                with open(outputname, 'wb') as f:
+                with open(outputname, "wb") as f:
                     f.write(weatherfile_data.content)
             else:
-                raise Exception(f"Returned non 200 status code trying to download weather file: {weatherfile_data.status_code}")
+                raise requests.exceptions.RequestException(
+                    f"Returned non 200 status code trying to download weather file: {weatherfile_data.status_code}"
+                )
         except requests.exceptions.RequestException as e:
-            raise Exception(
+            raise requests.exceptions.RequestException(
                 f"Could not download weather file: {weatherfile_url}"
                 "\nAt this time we only support USA weather stations"
                 f"\n{e}"
             )
 
         if not outputname.exists():
-            raise Exception(f"Could not find or download weather file for {str(p_download)}")
+            raise FileNotFoundError(f"Could not find or download weather file for {p_download!s}")
 
         return outputname
 
     def make_list(self, inputs):
-        """ Ensure that format of inputs is a list
+        """Ensure that format of inputs is a list
         :param inputs: object, inputs (list or dict)
         :return: list of inputs
         """
         list_inputs = []
         if isinstance(inputs, dict) and len(inputs) != 0:
             list_inputs.append(inputs)
         else:
             list_inputs = inputs
 
         return list_inputs
 
     def process_wind(self, inputs):
-        """
-        Processes wind inputs and insert into template
+        """Processes wind inputs and insert into template
+
         :param inputs: object, wind inputs
         """
         wind_turbines = []
-        for item in inputs['scenario_report']['distributed_generation']['wind']:
+        for item in inputs["scenario_report"]["distributed_generation"]["wind"]:
             # nominal voltage - Default
             wt = {}
-            wt['nominal_voltage'] = 480
+            wt["nominal_voltage"] = 480
 
             # scaling factor: parameter used by the wind turbine model
             # from Modelica Buildings Library, to scale the power output
             # without changing other parameters. Multiplies "Power curve"
             # value to get a scaled up power output.
             # add default = 1
-            wt['scaling_factor'] = 1
+            wt["scaling_factor"] = 1
 
             # calculate height_over_ground and power curve from REopt
             #  "size_class" (defaults to commercial) res = 2.5kW, com = 100kW, mid = 250kW, large = 2000kW
-            heights = {'residential': 20, 'commercial': 40, 'midsize': 50, 'large': 80}
+            heights = {"residential": 20, "commercial": 40, "midsize": 50, "large": 80}
             size_class = None
-            if item['size_class']:
-                size_class = item['size_class']
+            if item["size_class"]:
+                size_class = item["size_class"]
 
             if size_class is None:
-                size_class = 'commercial'
+                size_class = "commercial"
 
             # height over ground. default 10m
-            wt['height_over_ground'] = heights[size_class]
+            wt["height_over_ground"] = heights[size_class]
 
             # add power curve
             curves = self.get_wind_power_curves()
-            wt['power_curve'] = curves[size_class]
+            wt["power_curve"] = curves[size_class]
 
             # capture size_kw just in case
-            wt['rated_power'] = item['size_kw']
+            wt["rated_power"] = item["size_kw"]
             # and yearly energy produced
-            wt['annual_energy_produced'] = item['average_yearly_energy_produced_kwh']
+            wt["annual_energy_produced"] = item["average_yearly_energy_produced_kwh"]
 
             # append to results array
             wind_turbines.append(wt)
 
-        self.param_template['wind_turbines'] = wind_turbines
+        self.param_template["wind_turbines"] = wind_turbines
 
     def get_wind_power_curves(self):
         # from: https://reopt.nrel.gov/tool/REopt%20Lite%20Web%20Tool%20User%20Manual.pdf#page=61
         # curves given in Watts (W)
         power_curves = {}
-        power_curves['residential'] = [[2, 0],
-                                       [3, 70.542773],
-                                       [4, 167.2125],
-                                       [5, 326.586914],
-                                       [6, 564.342188],
-                                       [7, 896.154492],
-                                       [8, 1337.7],
-                                       [9, 1904.654883],
-                                       [10, 2500]]
-        power_curves['commercial'] = [[2, 0],
-                                      [3, 3505.95],
-                                      [4, 8310.4],
-                                      [5, 16231.25],
-                                      [6, 28047.6],
-                                      [7, 44538.55],
-                                      [8, 66483.2],
-                                      [9, 94660.65],
-                                      [10, 100000]]
-        power_curves['midsize'] = [[2, 0],
-                                   [3, 8764.875],
-                                   [4, 20776],
-                                   [5, 40578.125],
-                                   [6, 70119],
-                                   [7, 111346.375],
-                                   [8, 166208],
-                                   [9, 236651.625],
-                                   [10, 250000]]
-
-        power_curves['large'] = [[2, 0],
-                                 [3, 70119],
-                                 [4, 166208],
-                                 [5, 324625],
-                                 [6, 560952],
-                                 [7, 890771],
-                                 [8, 1329664],
-                                 [9, 1893213],
-                                 [10, 2000000]]
+        power_curves["residential"] = [
+            [2, 0],
+            [3, 70.542773],
+            [4, 167.2125],
+            [5, 326.586914],
+            [6, 564.342188],
+            [7, 896.154492],
+            [8, 1337.7],
+            [9, 1904.654883],
+            [10, 2500],
+        ]
+        power_curves["commercial"] = [
+            [2, 0],
+            [3, 3505.95],
+            [4, 8310.4],
+            [5, 16231.25],
+            [6, 28047.6],
+            [7, 44538.55],
+            [8, 66483.2],
+            [9, 94660.65],
+            [10, 100000],
+        ]
+        power_curves["midsize"] = [
+            [2, 0],
+            [3, 8764.875],
+            [4, 20776],
+            [5, 40578.125],
+            [6, 70119],
+            [7, 111346.375],
+            [8, 166208],
+            [9, 236651.625],
+            [10, 250000],
+        ]
+
+        power_curves["large"] = [
+            [2, 0],
+            [3, 70119],
+            [4, 166208],
+            [5, 324625],
+            [6, 560952],
+            [7, 890771],
+            [8, 1329664],
+            [9, 1893213],
+            [10, 2000000],
+        ]
         return power_curves
 
     def process_pv(self, inputs, latitude):
-        """
-        Processes pv inputs
+        """Processes PV inputs
+
         :param inputs: object, pv inputs
         :return photovoltaic_panels section to be inserted per-building or globally
         """
 
         items = self.make_list(inputs)
         pvs = []
         # hardcode nominal_system_voltage 480V
         # add latitude
         for item in items:
             pv = {}
-            pv['nominal_voltage'] = 480
-            pv['latitude'] = latitude
-            if 'tilt' in item:
-                pv['surface_tilt'] = item['tilt']
-            else:
-                pv['surface_tilt'] = 0
-            if 'azimuth' in item:
-                pv['surface_azimuth'] = item['azimuth']
-            else:
-                pv['surface_azimuth'] = 0
+            pv["nominal_voltage"] = 480
+            pv["latitude"] = latitude
+            pv["surface_tilt"] = item.get("tilt", 0)
+            pv["surface_azimuth"] = item.get("azimuth", 0)
 
-            # Size (kW) = Array Area (m²) × 1 kW/m² × Module Efficiency (%)
+            # Size (kW) = Array Area (m²) * 1 kW/m² * Module Efficiency (%)
             # area = size (kW) / 1 kW/m2 / module efficiency (%)
             # module efficiency tied to module type: 0 -> standard: 15%, 1-> premium: 19%, 2-> thin film: 10%
             # defaults to standard
             efficiencies = {0: 15, 1: 19, 2: 10}
             module_type = 0
-            if 'module_type' in item:
-                module_type = item['module_type']
+            if "module_type" in item:
+                module_type = item["module_type"]
 
             eff = efficiencies[module_type]
-            pv['net_surface_area'] = item['size_kw'] / eff
+            pv["net_surface_area"] = item["size_kw"] / eff
 
             pvs.append(pv)
 
         return pvs
 
     def process_chp(self, inputs):
-        """
-        Processes global chp inputs and insert into template
+        """Processes global CHP inputs and insert into template
+
         :param inputs: object, raw inputs
         """
         # this uses the raw inputs
-        items = self.make_list(inputs['outputs']['Scenario']['Site']['CHP'])
+        items = self.make_list(inputs["outputs"]["Scenario"]["Site"]["CHP"])
         chps = []
         for item in items:
             # fuel type. options are: natural_gas (default), landfill_bio_gas, propane, diesel_oil
             chp = {}
-            chp['fuel_type'] = 'natural_gas'
-            if inputs['inputs']['Scenario']['Site']['FuelTariff']["chp_fuel_type"]:
-                chp['fuel_type'] = inputs['inputs']['Scenario']['Site']['FuelTariff']["chp_fuel_type"]
+            chp["fuel_type"] = "natural_gas"
+            if inputs["inputs"]["Scenario"]["Site"]["FuelTariff"]["chp_fuel_type"]:
+                chp["fuel_type"] = inputs["inputs"]["Scenario"]["Site"]["FuelTariff"]["chp_fuel_type"]
 
             # single_electricity_generation_capacity
-            chp['single_electricity_generation_capacity'] = item['size_kw']
+            chp["single_electricity_generation_capacity"] = item["size_kw"]
 
             # performance data filename
             # TODO: not sure how to pass this in
             # how to default this? retrieve from the template, or right here in code?
-            chp['performance_data_path'] = ''
+            chp["performance_data_path"] = ""
 
             # number of machines
             # TODO: not in REopt...default?
-            chp['number_of_machines'] = 1
+            chp["number_of_machines"] = 1
 
             chps.append(chp)
 
-        self.param_template['combined_heat_and_power_systems'] = chps
+        self.param_template["combined_heat_and_power_systems"] = chps
 
     def process_storage(self, inputs):
-        """
-        Processes global battery bank outputs and insert into template
+        """Processes global battery bank outputs and insert into template
+
         :param inputs: object, raw inputs
         """
         # this uses the raw inputs
         items = []
-        try:
-            items = self.make_list(inputs['scenario_report']['distributed_generation']['storage'])
-        except KeyError:
-            pass
+        with suppress(KeyError):
+            items = self.make_list(inputs["scenario_report"]["distributed_generation"]["storage"])
 
         batts = []
         for item in items:
-
             batt = {}
 
             # energy capacity 'size_kwh' % 1000 to convert to MWh
-            batt['capacity'] = item['size_kwh'] / 1000
+            batt["capacity"] = item["size_kwh"] / 1000
 
             # Nominal Voltage - DEFAULT
-            batt['nominal_voltage'] = 480
+            batt["nominal_voltage"] = 480
 
             batts.append(batt)
 
-        self.param_template['battery_banks'] = batts
+        self.param_template["battery_banks"] = batts
 
     def process_generators(self, inputs):
-        """
-        Processes generators outputs and insert into template
+        """Processes generators outputs and insert into template
+
         :param inputs: object, raw inputs
         """
         # this uses the raw inputs
         items = []
-        try:
-            items = self.make_list(inputs['scenario_report']['distributed_generation']['generators'])
-        except KeyError:
-            pass
+        with suppress(KeyError):
+            items = self.make_list(inputs["scenario_report"]["distributed_generation"]["generators"])
 
         generators = []
         for item in items:
-
             generator = {}
 
             # size_kw, then convert to W
-            generator['nominal_power_generation'] = item['size_kw'] * 1000
+            generator["nominal_power_generation"] = item["size_kw"] * 1000
 
             # source phase shift
             # TODO: Not in REopt
-            generator['source_phase_shift'] = 0
+            generator["source_phase_shift"] = 0
 
             generators.append(generator)
 
-        self.param_template['diesel_generators'] = generators
+        self.param_template["diesel_generators"] = generators
 
     def process_grid(self):
         grid = {}
 
         # frequency - default
-        grid['frequency'] = 60
+        grid["frequency"] = 60
         # TODO: RMS voltage source - default
         # grid['source_rms_voltage'] = 0
 
         # TODO: phase shift (degrees) - default
         # grid['source_phase_shift'] = 0
 
-        self.param_template['electrical_grid'] = grid
+        self.param_template["electrical_grid"] = grid
 
     def process_electrical_components(self, scenario_dir: Path):
-        """ process electrical results from OpenDSS
-            electrical grid
-            substations
-            transformers
-            distribution lines
-            capacitor banks (todo)
+        """Process electrical results from OpenDSS, including electrical grid, substations,
+        transformers, distribution lines, and capacitor banks (todo)
         """
         dss_data = {}
-        opendss_json_file = Path(scenario_dir) / 'scenario_report_opendss.json'
+        opendss_json_file = Path(scenario_dir) / "scenario_report_opendss.json"
         if opendss_json_file.exists():
-            with open(opendss_json_file, "r") as f:
+            with open(opendss_json_file) as f:
                 dss_data = json.load(f)
 
         if dss_data:
             # ELECTRICAL GRID: completely defaulted for now
             self.process_grid()
 
             # SUBSTATIONS
             substations = []
-            try:
-                data = dss_data['scenario_report']['scenario_power_distribution']['substations']
+            with suppress(KeyError):
+                data = dss_data["scenario_report"]["scenario_power_distribution"]["substations"]
                 for item in data:
-                    try:
+                    with suppress(KeyError):
                         s = {}
                         # TODO: default RNM Voltage (high side?)
 
                         # RMS Voltage (low side)
-                        s['RMS_voltage_low_side'] = item['nominal_voltage']
+                        s["RMS_voltage_low_side"] = item["nominal_voltage"]
                         substations.append(s)
-                    except KeyError:
-                        pass
-            except KeyError:
-                pass
 
-            self.param_template['substations'] = substations
+            self.param_template["substations"] = substations
 
             # DISTRIBUTION LINES
             lines = []
-            try:
-                data = dss_data['scenario_report']['scenario_power_distribution']['distribution_lines']
+            with suppress(KeyError):
+                data = dss_data["scenario_report"]["scenario_power_distribution"]["distribution_lines"]
                 for item in data:
-                    try:
+                    with suppress(KeyError):
                         line = {}
-                        line['length'] = item['length']
-                        line['ampacity'] = item['ampacity']
+                        line["length"] = item["length"]
+                        line["ampacity"] = item["ampacity"]
 
                         # nominal voltage is defaulted (data not available in OpenDSS)
-                        line['nominal_voltage'] = 480
+                        line["nominal_voltage"] = 480
 
-                        line['commercial_line_type'] = item['commercial_line_type']
+                        line["commercial_line_type"] = item["commercial_line_type"]
 
                         lines.append(line)
-                    except KeyError:
-                        pass
-            except KeyError:
-                pass
 
-            self.param_template['distribution_lines'] = lines
+            self.param_template["distribution_lines"] = lines
 
             # CAPACITOR BANKS
             caps = []
-            try:
-                data = dss_data['scenario_report']['scenario_power_distribution']['capacitors']
+            with suppress(KeyError):
+                data = dss_data["scenario_report"]["scenario_power_distribution"]["capacitors"]
                 for item in data:
-                    try:
+                    with suppress(KeyError):
                         cap = {}
                         # nominal capacity (var)
-                        cap['nominal_capacity'] = item['nominal_capacity']
+                        cap["nominal_capacity"] = item["nominal_capacity"]
 
                         caps.append(cap)
-                    except KeyError:
-                        pass
-            except KeyError:
-                pass
 
-            self.param_template['capacitor_banks'] = caps
+            self.param_template["capacitor_banks"] = caps
 
             # TRANSFORMERS
             transformers = []
-            data = [d for d in dss_data['feature_reports'] if d['id'].startswith('Transformer')]
+            data = [d for d in dss_data["feature_reports"] if d["id"].startswith("Transformer")]
             for item in data:
                 t = {}
-                t['id'] = item['id']
-                t['nominal_capacity'] = item['power_distribution'].get('nominal_capacity', None)
-                t['reactance_resistance_ratio'] = item['power_distribution'].get('reactance_resistance_ratio', None)
-                t['tx_incoming_voltage'] = item['power_distribution'].get('tx_incoming_voltage', None)
-                t['tx_outgoing_voltage'] = item['power_distribution'].get('tx_outgoing_voltage', None)
+                t["id"] = item["id"]
+                t["nominal_capacity"] = item["power_distribution"].get("nominal_capacity", None)
+                t["reactance_resistance_ratio"] = item["power_distribution"].get("reactance_resistance_ratio", None)
+                t["tx_incoming_voltage"] = item["power_distribution"].get("tx_incoming_voltage", None)
+                t["tx_outgoing_voltage"] = item["power_distribution"].get("tx_outgoing_voltage", None)
 
                 # Validate transformer input voltage is same as substation output voltage
-                if t['tx_incoming_voltage'] is not None and t['tx_incoming_voltage'] != self.param_template['substations']['RMS_voltage_low_side']:
-                    raise ValueError(f"Transformer input voltage {t['tx_incoming_voltage']} does not "
-                                     f"match substation output voltage {self.param_template['substations']['RMS_voltage_low_side']}")
+                if (
+                    t["tx_incoming_voltage"] is not None
+                    and t["tx_incoming_voltage"] != self.param_template["substations"]["RMS_voltage_low_side"]
+                ):
+                    raise ValueError(
+                        f"Transformer input voltage {t['tx_incoming_voltage']} does not "
+                        f"match substation output voltage {self.param_template['substations']['RMS_voltage_low_side']}"
+                    )
 
                 transformers.append(t)
 
-            self.param_template['transformers'] = transformers
+            self.param_template["transformers"] = transformers
 
             # Loads (buildings from geojson file)
             # grab all the building loads
-            data = [d for d in dss_data['feature_reports'] if d['feature_type'] == 'Building']
+            data = [d for d in dss_data["feature_reports"] if d["feature_type"] == "Building"]
 
             # grab records to modify
-            for bldg in self.param_template['buildings']:
+            for bldg in self.param_template["buildings"]:
                 # find match in data
-                match = [d for d in data if d['id'] == bldg['geojson_id']]
+                match = [d for d in data if d["id"] == bldg["geojson_id"]]
                 if match:
                     # add data
-                    bldg['load'] = {}
+                    bldg["load"] = {}
                     # print(f"Found match for {bldg['geojson_id']}: {match[0]['id']}")
-                    bldg['load']['nominal_voltage'] = match[0]['power_distribution']['nominal_voltage']
-                    bldg['load']['max_power_kw'] = match[0]['power_distribution']['max_power_kw']
-                    bldg['load']['max_reactive_power_kvar'] = match[0]['power_distribution']['max_reactive_power_kvar']
+                    bldg["load"]["nominal_voltage"] = match[0]["power_distribution"]["nominal_voltage"]
+                    bldg["load"]["max_power_kw"] = match[0]["power_distribution"]["max_power_kw"]
+                    bldg["load"]["max_reactive_power_kvar"] = match[0]["power_distribution"]["max_reactive_power_kvar"]
 
     def process_building_microgrid_inputs(self, building, scenario_dir: Path):
-        """
-        Processes microgrid inputs for a single building
-        :param building: list, building
+        """Processes microgrid inputs for a single building
+
+        :param building: dict, single building being built for the sys-param file
         :param scenario_dir: Path, location/name of folder with uo_sdk results
         :return building, updated building list object
         """
-        feature_opt_file = Path(
-            scenario_dir) / building['geojson_id'] / 'feature_reports' / 'feature_optimization.json'
+        feature_opt_file = Path(scenario_dir) / building["geojson_id"] / "feature_reports" / "feature_optimization.json"
         if feature_opt_file.exists():
-            with open(feature_opt_file, "r") as f:
+            with open(feature_opt_file) as f:
                 reopt_data = json.load(f)
 
         # extract Latitude
         try:
-            latitude = reopt_data['location']['latitude_deg']
+            latitude = reopt_data["location"]["latitude_deg"]
         except KeyError:
             logger.info(f"Latitude not found in {feature_opt_file}. Skipping PV.")
         except UnboundLocalError:
             logger.info(f"REopt data not found in {feature_opt_file}. Skipping PV.")
 
         # PV
-        if reopt_data['distributed_generation'] and reopt_data['distributed_generation']['solar_pv']:
-            building['photovoltaic_panels'] = self.process_pv(
-                reopt_data['distributed_generation']['solar_pv'], latitude)
+        if reopt_data["distributed_generation"] and reopt_data["distributed_generation"]["solar_pv"]:
+            building["photovoltaic_panels"] = self.process_pv(
+                reopt_data["distributed_generation"]["solar_pv"], latitude
+            )
 
         return building
 
     def process_microgrid_inputs(self, scenario_dir: Path):
-        """
-        Processes microgrid inputs and adds them to param_template from csv_to_sys_param method
+        """Processes microgrid inputs and adds them to param_template from csv_to_sys_param method
+
         :param scenario_dir: Path, location/name of folder with uo_sdk results
         """
         reopt_data = {}
         raw_data = {}
         # look for REopt scenario_optimization.json file in scenario dir (uo report)
-        scenario_opt_file = Path(scenario_dir) / 'scenario_optimization.json'
+        scenario_opt_file = Path(scenario_dir) / "scenario_optimization.json"
         if scenario_opt_file.exists():
-            with open(scenario_opt_file, "r") as f:
+            with open(scenario_opt_file) as f:
                 reopt_data = json.load(f)
         # also look for raw REopt report with inputs and xzx for non-uo results
-        raw_scenario_file = Path(scenario_dir) / 'reopt' / f'scenario_report_{scenario_dir.name}_reopt_run.json'
+        raw_scenario_file = Path(scenario_dir) / "reopt" / f"scenario_report_{scenario_dir.name}_reopt_run.json"
         if raw_scenario_file.exists():
-            with open(raw_scenario_file, "r") as f:
+            with open(raw_scenario_file) as f:
                 raw_data = json.load(f)
 
         # PV (add if results are found in scenario_report)
         # extract latitude
         try:
-            latitude = reopt_data['scenario_report']['location']['latitude_deg']
-            if reopt_data['scenario_report']['distributed_generation']['solar_pv']:
-                self.param_template['photovoltaic_panels'] = self.process_pv(
-                    reopt_data['scenario_report']['distributed_generation']['solar_pv'],
-                    latitude
+            latitude = reopt_data["scenario_report"]["location"]["latitude_deg"]
+            if reopt_data["scenario_report"]["distributed_generation"]["solar_pv"]:
+                self.param_template["photovoltaic_panels"] = self.process_pv(
+                    reopt_data["scenario_report"]["distributed_generation"]["solar_pv"], latitude
                 )
         except KeyError:
             logger.info("Latitude not found in scenario_report. Skipping PV.")
 
         # Wind (add if results are found in scenario_report)
         # if reopt_data['scenario_report']['distributed_generation']['wind']:
         try:
             self.process_wind(reopt_data)
         except KeyError:
             logger.info("Wind data not found in scenario_report. Skipping wind.")
 
         # CHP (add if results are found in reopt results-raw_data)
         # this is the only item not in the default URBANopt report file
-        if Path(raw_scenario_file).exists() and raw_data['outputs']['Scenario']['Site']['CHP']['size_kw'] != 0.0:
+        if Path(raw_scenario_file).exists() and raw_data["outputs"]["Scenario"]["Site"]["CHP"]["size_kw"] != 0.0:
             # there is a CHP, process
             self.process_chp(raw_data)
 
         # Battery Bank
         try:
-            if reopt_data['scenario_report']['distributed_generation']['storage']:
+            if reopt_data["scenario_report"]["distributed_generation"]["storage"]:
                 # there is storage, process
                 self.process_storage(reopt_data)
         except KeyError:
             logger.info("Energy storage data not found in scenario_report. Skipping storage.")
 
         # Generators
         try:
-            if reopt_data['scenario_report']['distributed_generation']['generators']:
+            if reopt_data["scenario_report"]["distributed_generation"]["generators"]:
                 # process diesel generators
                 self.process_generators(reopt_data)
         except KeyError:
             logger.info("Generator data not found in scenario_report. Skipping generator.")
 
         # process electrical components (from OpenDSS results)
         self.process_electrical_components(scenario_dir)
 
         # Power Converters
         # TODO: not handled in UO / OpenDSS
 
-    def calculate_dimensions(self, area, perimeter):
+    def process_ghe_inputs(self, scenario_dir: Path):
+        ghe_ids = []
+        # add properties from the feature file
+        for feature in self.sdk_input["features"]:
+            if feature["properties"]["type"] == "District System":
+                district_system_type = feature["properties"]["district_system_type"]
+                if district_system_type == "Ground Heat Exchanger":
+                    length, width = self.calculate_dimensions(
+                        feature["properties"]["footprint_area"], feature["properties"]["footprint_perimeter"]
+                    )
+                    ghe_ids.append(
+                        {"ghe_id": feature["properties"]["id"], "length_of_ghe": length, "width_of_ghe": width}
+                    )
+
+        ghe_sys_param = self.param_template["district_system"]["fifth_generation"]["ghe_parameters"]
+        # Make sys_param template entries for GHE specific properties
+        ghe_list = []
+        for ghe in ghe_ids:
+            # update GHE specific properties
+            ghe_info = deepcopy(ghe_sys_param["ghe_specific_params"][0])
+            # Update GHE ID
+            ghe_info["ghe_id"] = str(ghe["ghe_id"])
+            # Add ghe geometric properties
+            ghe_info["ghe_geometric_params"]["length_of_ghe"] = ghe["length_of_ghe"]
+            ghe_info["ghe_geometric_params"]["width_of_ghe"] = ghe["width_of_ghe"]
+            ghe_list.append(ghe_info)
+
+        # Add all GHE specific properties to sys-param file
+        ghe_sys_param["ghe_specific_params"] = ghe_list
+
+        # Update ghe_dir
+        ghe_dir = scenario_dir / "ghe_dir"
+        ghe_sys_param["ghe_dir"] = str(ghe_dir)
+
+        # remove fourth generation district system type
+        del self.param_template["district_system"]["fourth_generation"]
+
+        return ghe_sys_param
+
+    def retrieve_building_data_from_sdk(
+        self, scenario_dir: Path, modelica_load_filename, model_type: str, district_type: str
+    ):
+        measure_list = []
 
-        discriminant = perimeter ** 2 - 16 * area
+        # Grab building load filepaths from sdk output
+        for thing in scenario_dir.iterdir():
+            if thing.is_dir():
+                for item in thing.iterdir():
+                    if item.is_dir():
+                        if str(item).endswith("_export_time_series_modelica"):
+                            measure_list.append(Path(item) / "building_loads.csv")  # used for mfrt
+                        elif str(item).endswith("_export_modelica_loads"):
+                            measure_list.append(
+                                Path(item) / modelica_load_filename
+                            )  # space heating/cooling & water heating
+                            measure_list.append(Path(item) / "building_loads.csv")  # used for max electricity load
+
+        # Get each building feature id from the SDK FeatureFile
+        building_ids = []
+        for feature in self.sdk_input["features"]:
+            if feature["properties"]["type"] == "Building":
+                building_ids.append(feature["properties"]["id"])
+
+        # Make sys_param template entries for each feature_id
+        building_list = []
+        for building in building_ids:
+            if "4G" in district_type:
+                building_params = deepcopy(self.param_template["buildings"][0])
+            elif "5G" in district_type:
+                building_params = deepcopy(self.param_template["buildings"][1])
+            building_params["geojson_id"] = str(building)
+            building_list.append(building_params)
+
+        # Grab the modelica file for the each Feature, and add it to the appropriate building dict
+        district_nominal_massflow_rate = 0
+        for building in building_list:
+            building_nominal_massflow_rate = 0
+            for measure_file_path in measure_list:
+                # Grab the feature name and measure folder name from the path, items -3 & -2 respectively
+                feature_name = Path(measure_file_path).parts[-3]
+                measure_folder_name = Path(measure_file_path).parts[-2]
+                if feature_name != building["geojson_id"]:
+                    continue
+                if measure_file_path.suffix == ".mos":
+                    # if there is a relative path, then set the path relative
+                    timeseries_load_file_path = measure_file_path.resolve()
+                    if self.rel_path:
+                        timeseries_load_file_path = timeseries_load_file_path.relative_to(self.rel_path)
+
+                    building["load_model_parameters"][model_type]["filepath"] = str(timeseries_load_file_path)
+                if "4G" in district_type:
+                    if (measure_file_path.suffix == ".csv") and (
+                        "_export_time_series_modelica" in str(measure_folder_name)
+                    ):
+                        massflow_rate_df = pd.read_csv(measure_file_path)
+                        try:
+                            building_nominal_massflow_rate = round(
+                                massflow_rate_df["massFlowRateHeating"].max(), 3
+                            )  # round max to 3 decimal places
+                            # Force casting to float even if building_nominal_massflow_rate == 0
+                            # FIXME: Related to building_type == `lodging` for non-zero building percentages?
+                            building["ets_indirect_parameters"]["nominal_mass_flow_building"] = float(
+                                building_nominal_massflow_rate
+                            )
+                        except KeyError:
+                            # If massFlowRateHeating is not in the export_time_series_modelica output, skip this step.
+                            # It won't be in the export for hpxml residential buildings, at least as of 2022-06-29
+                            logger.info("mass-flow-rate heating is not expected in residential buildings. Skipping.")
+                            continue
+                    district_nominal_massflow_rate += building_nominal_massflow_rate
+                if measure_file_path.suffix == ".csv" and measure_folder_name.endswith("_export_modelica_loads"):
+                    try:
+                        # only use the one column to make the df small
+                        building_loads = pd.read_csv(measure_file_path, usecols=["ElectricityFacility"])
+                    except (
+                        ValueError
+                    ):  # hack to handle the case where there is no ElectricityFacility column in the csv
+                        continue
+                    max_electricity_load = int(building_loads["ElectricityFacility"].max())
+                    building["load_model_parameters"][model_type]["max_electrical_load"] = max_electricity_load
+
+        # Remove template buildings that weren't used or don't have successful simulations with modelica outputs
+        building_list = [
+            x for x in building_list if not x["load_model_parameters"][model_type]["filepath"].endswith("populated")
+        ]
+        if len(building_list) == 0:
+            raise SystemExit(
+                "No Modelica files found. Modelica files are expected to be found within each feature in folders "
+                "with names that include '_modelica'\n"
+                f"For instance: {scenario_dir / '2' / '016_export_modelica_loads'}\n"
+                "If these files don't exist the UO SDK simulations may not have been successful"
+            )
+        return building_list, district_nominal_massflow_rate
+
+    def calculate_dimensions(self, area, perimeter):
+        discriminant = perimeter**2 - 16 * area
 
         if discriminant < 0:
             raise ValueError("No valid rectangle dimensions exist for the given area and perimeter.")
 
         length = (perimeter + math.sqrt(discriminant)) / 4
         width = (perimeter - 2 * length) / 2
 
         return length, width
 
-    def csv_to_sys_param(self,
-                         model_type: str,
-                         scenario_dir: Path,
-                         feature_file: Path,
-                         sys_param_filename: Path,
-                         ghe=False,
-                         overwrite=True,
-                         microgrid=False,
-                         **kwargs) -> None:
-        """
-        Create a system parameters file using output from URBANopt SDK
+    def csv_to_sys_param(
+        self,
+        model_type: str,
+        scenario_dir: Path,
+        feature_file: Path,
+        sys_param_filename: Path,
+        district_type: str = "4G",
+        overwrite=True,
+        microgrid=False,
+        **kwargs,
+    ) -> None:
+        """Create a system parameters file using output from URBANopt SDK
 
         :param model_type: str, model type to select which sys_param template to use
         :param scenario_dir: Path, location/name of folder with uo_sdk results
         :param feature_file: Path, location/name of uo_sdk input file
         :param sys_param_filename: Path, location/name of system parameter file to be created
+        :param district_type: str, district type to model
         :param overwrite: Boolean, whether to overwrite existing sys-param file
-        :param ghe: Boolean, flag to add Ground Heat Exchanger properties to System Parameter File
         :param microgrid: Boolean, Optional. If set to true, also process microgrid fields
 
         :kwargs (optional):
             - relative_path: Path, set the paths (time series files, weather file, etc) relate to `relative_path`
+            - skip_weather_download: Boolean, set to True to not download the weather file, defaults to False
+            - modelica_load_filename: str, name (only) of file for the modelica load file, defaults to "modelica.mos"
         :return None, file created and saved to user-specified location
-
-
         """
         self.sys_param_filename = sys_param_filename
-        self.rel_path = kwargs.get('relative_path', None)
+        self.rel_path = kwargs.get("relative_path", None)
+        skip_weather_download = kwargs.get("skip_weather_download", False)
+        modelica_load_filename = kwargs.get("modelica_load_filename", "modelica.mos")
 
-        if model_type == 'time_series':
+        if model_type == "time_series":
             # TODO: delineate between time_series and time_series_massflow_rate
-            if microgrid:
-                param_template_path = Path(__file__).parent / 'time_series_microgrid_template.json'
-            else:
-                param_template_path = Path(__file__).parent / 'time_series_template.json'
-        elif model_type == 'spawn':
+            param_template_path = Path(__file__).parent / "time_series_template.json"
+        elif model_type == "spawn":
             # TODO: We should support spawn as well
-            raise SystemExit('Spawn models are not implemented at this time.')
+            raise SystemExit("Spawn models are not implemented at this time.")
         else:
             raise SystemExit(f"No template found. {model_type} is not a valid template")
 
         if not Path(scenario_dir).is_dir():
             raise SystemExit(f"Unable to find your scenario. The path you provided was: {scenario_dir}")
 
         if not Path(feature_file).is_file():
             raise SystemExit(f"Unable to find your feature file. The path you provided was: {feature_file}")
 
         if Path(self.sys_param_filename).is_file() and not overwrite:
             raise SystemExit(f"Output file already exists and overwrite is False: {self.sys_param_filename}")
 
-        with open(param_template_path, "r") as f:
-            self.param_template = json.load(f)
+        if district_type not in ["steam", "4G", "5G", "5G_ghe"]:
+            raise SystemExit(
+                f"{district_type} is not a valid district type. Available options are: ['steam', '4G', '5G', '5G_ghe']"
+            )
 
-        measure_list = []
+        self.param_template = json.loads(param_template_path.read_text())
 
-        # Grab building load filepaths from sdk output
-        for thing in scenario_dir.iterdir():
-            if thing.is_dir():
-                for item in thing.iterdir():
-                    if item.is_dir():
-                        if str(item).endswith('_export_time_series_modelica'):
-                            measure_list.append(Path(item) / "building_loads.csv")  # used for mfrt
-                        elif str(item).endswith('_export_modelica_loads'):
-                            measure_list.append(Path(item) / "modelica.mos")  # space heating/cooling & water heating
-                            measure_list.append(Path(item) / "building_loads.csv")  # used for max electricity load
+        self.sdk_input = json.loads(feature_file.read_text())
 
-        # Get each building feature id from the SDK FeatureFile
-        building_ids = []
-        with open(feature_file) as json_file:
-            sdk_input = json.load(json_file)
-        weather_filename = sdk_input['project']['weather_filename']
+        # Get weather data
+        weather_filename = self.sdk_input["project"]["weather_filename"]
         weather_path = self.sys_param_filename.parent / weather_filename
-        for feature in sdk_input['features']:
-            if feature['properties']['type'] == 'Building':
-                building_ids.append(feature['properties']['id'])
-
         # Check if the EPW weatherfile exists, if not, try to download
-        if not weather_path.exists():
+        if not skip_weather_download and not weather_path.exists():
             self.download_weatherfile(weather_path.name, weather_path.parent)
 
         # also download the MOS weatherfile -- this is the file that will be set in the sys param file
-        mos_weather_path = weather_path.with_suffix('.mos')
-        if not mos_weather_path.exists():
+        mos_weather_path = weather_path.with_suffix(".mos")
+        if not skip_weather_download and not mos_weather_path.exists():
             self.download_weatherfile(mos_weather_path.name, mos_weather_path.parent)
 
-        # Make sys_param template entries for each feature_id
-        building_list = []
-        for building in building_ids:
-            feature_info = deepcopy(self.param_template['buildings'][0])
-            feature_info['geojson_id'] = str(building)
-            building_list.append(feature_info)
-
-        # Grab the modelica file for the each Feature, and add it to the appropriate building dict
-        district_nominal_massflow_rate = 0
-        for building in building_list:
-            building_nominal_massflow_rate = 0
-            for measure_file_path in measure_list:
-                # Grab the relevant 2 components of the path: feature name and measure folder name, items -3 & -2 respectively
-                feature_name = Path(measure_file_path).parts[-3]
-                measure_folder_name = Path(measure_file_path).parts[-2]
-                if feature_name != building['geojson_id']:
-                    continue
-                if (measure_file_path.suffix == '.mos'):
-                    # if there is a relative path, then set the path relative
-                    to_file_path = measure_file_path.resolve()
-                    if self.rel_path:
-                        to_file_path = to_file_path.relative_to(self.rel_path)
-
-                    building['load_model_parameters']['time_series']['filepath'] = str(to_file_path)
-                if (measure_file_path.suffix == '.csv') and ('_export_time_series_modelica' in str(measure_folder_name)):
-                    massflow_rate_df = pd.read_csv(measure_file_path)
-                    try:
-                        building_nominal_massflow_rate = round(massflow_rate_df['massFlowRateHeating'].max(), 3)  # round max to 3 decimal places
-                        # Force casting to float even if building_nominal_massflow_rate == 0
-                        # FIXME: This might be related to building_type == `lodging` for non-zero building percentages
-                        building['ets_indirect_parameters']['nominal_mass_flow_building'] = float(building_nominal_massflow_rate)
-                    except KeyError:
-                        # If massFlowRateHeating is not in the export_time_series_modelica output, just skip this step.
-                        # It probably won't be in the export for hpxml residential buildings, at least as of 2022-06-29
-                        logger.info("mass-flow-rate heating is not present. It is not expected in residential buildings. Skipping.")
-                        continue
-                district_nominal_massflow_rate += building_nominal_massflow_rate
-                if measure_file_path.suffix == '.csv' and measure_folder_name.endswith('_export_modelica_loads'):
-                    try:
-                        building_loads = pd.read_csv(measure_file_path, usecols=['ElectricityFacility'])  # only use the one column to make the df small
-                    except ValueError:  # hack to handle the case where there is no ElectricityFacility column in the csv
-                        continue
-                    max_electricity_load = int(building_loads['ElectricityFacility'].max())
-                    building['load_model_parameters']['time_series']['max_electrical_load'] = max_electricity_load
-
-        # Remove template buildings that weren't used or don't have successful simulations with modelica outputs
-        # TODO: Another place where we only support time series for now.
-        building_list = [x for x in building_list if not x['load_model_parameters']
-                         ['time_series']['filepath'].endswith("populated")]
-        if len(building_list) == 0:
-            raise SystemExit("No Modelica files found. Modelica files are expected to be found within each feature in folders "
-                             "with names that include '_modelica'\n"
-                             f"For instance: {scenario_dir / '2' / '016_export_modelica_loads'}\n"
-                             "If these files don't exist the UO SDK simulations may not have been successful")
+        # Use building data from URBANopt SDK
+        building_list, district_nominal_massflow_rate = self.retrieve_building_data_from_sdk(
+            scenario_dir, modelica_load_filename, model_type, district_type
+        )
 
         # Update specific sys-param settings for each building
         for building in building_list:
-            building['ets_indirect_parameters']['nominal_mass_flow_district'] = district_nominal_massflow_rate
-            feature_opt_file = scenario_dir / building['geojson_id'] / 'feature_reports' / 'feature_optimization.json'
+            if "4G" in district_type:
+                building["ets_indirect_parameters"]["nominal_mass_flow_district"] = district_nominal_massflow_rate
+            feature_opt_file = scenario_dir / building["geojson_id"] / "feature_reports" / "feature_optimization.json"
             if microgrid and not feature_opt_file.exists():
-                logger.debug(f"No feature optimization file found for {building['geojson_id']}. Skipping REopt for this building")
+                logger.debug(
+                    f"No feature optimization file found for {building['geojson_id']}. Skipping REopt for this building"
+                )
             elif microgrid and feature_opt_file.exists():
-                building = self.process_building_microgrid_inputs(building, scenario_dir)
+                self.process_building_microgrid_inputs(building, scenario_dir)
 
         # Add all buildings to the sys-param file
-        self.param_template['buildings'] = building_list
+        self.param_template["buildings"] = building_list
 
         # Update district sys-param settings
-        # Parens are to allow the line break
-        to_file_path = mos_weather_path
         if self.rel_path:
-            to_file_path = to_file_path.relative_to(self.rel_path)
-        self.param_template['weather'] = str(to_file_path)
+            mos_weather_path = mos_weather_path.relative_to(self.rel_path)
+        self.param_template["weather"] = str(mos_weather_path)
+        # Process community microgrid inputs
         if microgrid and not feature_opt_file.exists():
-            logger.warn("Microgrid requires OpenDSS and REopt feature optimization for full functionality.\n"
-                        "Run opendss and reopt-feature post-processing in the UO SDK for a full-featured microgrid.")
-        try:
-            self.process_microgrid_inputs(scenario_dir)
-        except UnboundLocalError:
-            raise SystemExit(f"\nError: No scenario_optimization.json file found in {scenario_dir}\n"
-                             "Perhaps you haven't run REopt post-processing step in the UO sdk?")
+            logger.warn(
+                "Microgrid requires OpenDSS and REopt feature optimization for full functionality.\n"
+                "Run opendss and reopt-feature post-processing in the UO SDK for a full-featured microgrid."
+            )
+        elif microgrid and feature_opt_file.exists():
+            try:
+                self.process_microgrid_inputs(scenario_dir)
+            except UnboundLocalError:
+                raise SystemExit(
+                    f"\nError: No scenario_optimization.json file found in {scenario_dir}\n"
+                    "Perhaps you haven't run REopt post-processing step in the UO sdk?"
+                )
 
         # Update ground heat exchanger properties if true
-        if ghe:
-            ghe_ids = []
-            # add properties from the feature file
-            with open(feature_file) as json_file:
-                sdk_input = json.load(json_file)
-            for feature in sdk_input['features']:
-                if feature['properties']['type'] == 'District System':
-                    try:
-                        district_system_type = feature['properties']['district_system_type']
-                    except KeyError:
-                        pass
-                    if district_system_type == 'Ground Heat Exchanger':
-                        length, width = self.calculate_dimensions(feature['properties']['footprint_area'], feature['properties']['footprint_perimeter'])
-                        ghe_ids.append({'ghe_id': feature['properties']['id'],
-                                        'length_of_ghe': length,
-                                        'width_of_ghe': width})
-
-            ghe_sys_param = self.param_template['district_system']['fifth_generation']['ghe_parameters']
-            # Make sys_param template entries for GHE specific properties
-            ghe_list = []
-            for ghe in ghe_ids:
-                # update GHE specific properties
-                ghe_info = deepcopy(ghe_sys_param['ghe_specific_params'][0])
-                # Update GHE ID
-                ghe_info['ghe_id'] = str(ghe['ghe_id'])
-                # Add ghe geometric properties
-                ghe_info['ghe_geometric_params']['length_of_ghe'] = ghe['length_of_ghe']
-                ghe_info['ghe_geometric_params']['width_of_ghe'] = ghe['width_of_ghe']
-                ghe_list.append(ghe_info)
-
-            # Add all GHE specific properties to sys-param file
-            ghe_sys_param['ghe_specific_params'] = ghe_list
-
-            # Update ghe_dir
-            ghe_dir = scenario_dir / 'ghe_dir'
-            ghe_sys_param['ghe_dir'] = str(ghe_dir)
-
-            # remove fourth generation district system type
-            del self.param_template['district_system']['fourth_generation']
-
-        else:
+        if "5G_ghe" in district_type:
+            self.process_ghe_inputs(scenario_dir)
+        elif "4G" in district_type or "steam" in district_type:
             # remove fifth generation district system type if it exists in template and ghe is not true
-            try:
-                del self.param_template['district_system']['fifth_generation']
-            except KeyError:
-                pass
+            with suppress(KeyError):
+                del self.param_template["district_system"]["fifth_generation"]
 
         # save the file to disk
         self.save()
 
     def save(self):
-        """
-        Write the system parameters file with param_template and save
-        """
-        with open(self.sys_param_filename, 'w') as outfile:
+        """Write the system parameters file with param_template and save"""
+        with open(self.sys_param_filename, "w") as outfile:
             json.dump(self.param_template, outfile, indent=2)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/time_series_microgrid_template.json` & `geojson_modelica_translator-0.7.0/management/data/baseline_sys_params.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.15773545944187392%*

 * *Differences: {"'buildings'": "{1: {'geojson_id': 'abcdefghijklmnopqrstuvwx', 'load_model_parameters': "*

 * *                "{'time_series': {'filepath': './baseline_time_series.mos', delete: "*

 * *                "['max_electrical_load']}}, 'ets_indirect_parameters': {'heat_flow_nominal': "*

 * *                "10000, 'heat_exchanger_efficiency': 0.9, 'cooling_controller_y_max': 0.6, "*

 * *                "'heating_controller_y_max': 0.7, 'booster_heater': False, 'ets_generation': "*

 * *                "'Fourth Generation'}, delete: ['pho […]*

```diff
@@ -1,59 +1,96 @@
 {
-    "battery_banks": [],
     "buildings": [
         {
-            "battery_banks": [],
-            "diesel_generators": [],
             "ets_indirect_parameters": {
-                "cooling_controller_y_max": 1,
+                "booster_heater": false,
+                "cooling_controller_y_max": 0.6,
                 "cooling_controller_y_min": 0,
                 "cooling_supply_water_temperature_building": 7,
                 "delta_temp_chw_building": 5,
                 "delta_temp_chw_district": 8,
                 "delta_temp_hw_building": 15,
                 "delta_temp_hw_district": 20,
-                "heat_exchanger_efficiency": 0.8,
+                "ets_generation": "Fourth Generation",
+                "heat_exchanger_efficiency": 0.9,
                 "heat_exchanger_primary_pressure_drop": 500,
                 "heat_exchanger_secondary_pressure_drop": 500,
-                "heat_flow_nominal": 8000,
-                "heating_controller_y_max": 1,
+                "heat_flow_nominal": 10000,
+                "heating_controller_y_max": 0.7,
                 "heating_controller_y_min": 0,
                 "heating_supply_water_temperature_building": 50,
                 "nominal_mass_flow_building": 0.5,
                 "nominal_mass_flow_district": 0.5,
                 "valve_pressure_drop": 6000
             },
             "ets_model": "Indirect Heating and Cooling",
-            "geojson_id": "0",
+            "geojson_id": "5a6b99ec37f4de7f94020090",
             "load_model": "time_series",
             "load_model_parameters": {
                 "time_series": {
                     "delta_temp_air_cooling": 10,
                     "delta_temp_air_heating": 18,
-                    "filepath": "To be populated",
+                    "filepath": "./baseline_time_series.mos",
                     "has_electric_cooling": false,
                     "has_electric_heating": false,
                     "has_liquid_cooling": true,
                     "has_liquid_heating": true,
-                    "max_electrical_load": 0,
                     "temp_chw_return": 12,
                     "temp_chw_supply": 7,
                     "temp_hw_return": 35,
                     "temp_hw_supply": 40,
                     "temp_setpoint_cooling": 24,
                     "temp_setpoint_heating": 20
                 }
+            }
+        },
+        {
+            "ets_indirect_parameters": {
+                "booster_heater": false,
+                "cooling_controller_y_max": 0.6,
+                "cooling_controller_y_min": 0,
+                "cooling_supply_water_temperature_building": 7,
+                "delta_temp_chw_building": 5,
+                "delta_temp_chw_district": 8,
+                "delta_temp_hw_building": 15,
+                "delta_temp_hw_district": 20,
+                "ets_generation": "Fourth Generation",
+                "heat_exchanger_efficiency": 0.9,
+                "heat_exchanger_primary_pressure_drop": 500,
+                "heat_exchanger_secondary_pressure_drop": 500,
+                "heat_flow_nominal": 10000,
+                "heating_controller_y_max": 0.7,
+                "heating_controller_y_min": 0,
+                "heating_supply_water_temperature_building": 50,
+                "nominal_mass_flow_building": 0.5,
+                "nominal_mass_flow_district": 0.5,
+                "valve_pressure_drop": 6000
             },
-            "photovoltaic_panels": []
+            "ets_model": "Indirect Heating and Cooling",
+            "geojson_id": "abcdefghijklmnopqrstuvwx",
+            "load_model": "time_series",
+            "load_model_parameters": {
+                "time_series": {
+                    "delta_temp_air_cooling": 10,
+                    "delta_temp_air_heating": 18,
+                    "filepath": "./baseline_time_series.mos",
+                    "has_electric_cooling": false,
+                    "has_electric_heating": false,
+                    "has_liquid_cooling": true,
+                    "has_liquid_heating": true,
+                    "temp_chw_return": 12,
+                    "temp_chw_supply": 7,
+                    "temp_hw_return": 35,
+                    "temp_hw_supply": 40,
+                    "temp_setpoint_cooling": 24,
+                    "temp_setpoint_heating": 20
+                }
+            }
         }
     ],
-    "capacitor_banks": [],
-    "combined_heat_and_power_systems": [],
-    "distribution_lines": [],
     "district_system": {
         "fourth_generation": {
             "central_cooling_plant_parameters": {
                 "chiller_water_flow_minimum": 9.9,
                 "chw_pump_head": 300000,
                 "cooling_tower_fan_power_nominal": 4999,
                 "cooling_tower_water_temperature_difference_nominal": 6.56,
@@ -76,19 +113,16 @@
                 "boiler_water_flow_minimum": 0.1,
                 "chp_installed": false,
                 "heat_flow_nominal": 8001,
                 "mass_hhw_flow_nominal": 1,
                 "pressure_drop_hhw_nominal": 55001,
                 "pressure_drop_hhw_valve_nominal": 6001,
                 "pressure_drop_setpoint": 50000,
-                "temp_setpoint_hhw": 54
+                "temp_setpoint_hhw": 68
+            },
+            "central_pump_parameters": {
+                "pump_design_head": 60000
             }
         }
     },
-    "electrical_grid": {},
-    "photovoltaic_panels": [],
-    "power_converters": [],
-    "substations": [],
-    "transformers": [],
-    "weather": "../../data_shared/USA_CA_San.Francisco.Intl.AP.724940_TMY3.mos",
-    "wind_turbines": []
+    "weather": "./baseline_weather.mos"
 }
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/system_parameters/time_series_template.json` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/system_parameters/time_series_template.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.19509214743589742%*

 * *Differences: {"'battery_banks'": '[]',*

 * * "'buildings'": "{0: {'geojson_id': '4G', 'photovoltaic_panels': [], 'diesel_generators': [], "*

 * *                "'battery_banks': []}, insert: [(1, OrderedDict([('geojson_id', '5G'), "*

 * *                "('load_model', 'time_series'), ('load_model_parameters', "*

 * *                "OrderedDict([('time_series', OrderedDict([('filepath', 'To be populated'), "*

 * *                "('delta_temp_air_cooling', 10), ('delta_temp_air_heating', 18), "*

 * *                "('has_liquid_cooling', True), ( […]*

```diff
@@ -1,10 +1,13 @@
 {
+    "battery_banks": [],
     "buildings": [
         {
+            "battery_banks": [],
+            "diesel_generators": [],
             "ets_indirect_parameters": {
                 "cooling_controller_y_max": 1,
                 "cooling_controller_y_min": 0,
                 "cooling_supply_water_temperature_building": 7,
                 "delta_temp_chw_building": 5,
                 "delta_temp_chw_district": 8,
                 "delta_temp_hw_building": 15,
@@ -17,15 +20,15 @@
                 "heating_controller_y_min": 0,
                 "heating_supply_water_temperature_building": 50,
                 "nominal_mass_flow_building": 0.5,
                 "nominal_mass_flow_district": 0.5,
                 "valve_pressure_drop": 6000
             },
             "ets_model": "Indirect Heating and Cooling",
-            "geojson_id": "0",
+            "geojson_id": "4G",
             "load_model": "time_series",
             "load_model_parameters": {
                 "time_series": {
                     "delta_temp_air_cooling": 10,
                     "delta_temp_air_heating": 18,
                     "filepath": "To be populated",
                     "has_electric_cooling": false,
@@ -36,19 +39,65 @@
                     "temp_chw_return": 12,
                     "temp_chw_supply": 7,
                     "temp_hw_return": 35,
                     "temp_hw_supply": 40,
                     "temp_setpoint_cooling": 24,
                     "temp_setpoint_heating": 20
                 }
-            }
+            },
+            "photovoltaic_panels": []
+        },
+        {
+            "battery_banks": [],
+            "diesel_generators": [],
+            "ets_model": "Fifth Gen Heat Pump",
+            "fifth_gen_ets_parameters": {
+                "chilled_water_supply_temp": 5,
+                "cop_heat_pump_cooling": 3.5,
+                "cop_heat_pump_heating": 2.5,
+                "ets_pump_flow_rate": 0.0005,
+                "ets_pump_head": 10000,
+                "fan_design_flow_rate": 0.25,
+                "fan_design_head": 150,
+                "hot_water_supply_temp": 50,
+                "pump_design_head": 150000,
+                "pump_flow_rate": 0.01,
+                "supply_water_temperature_building": 15
+            },
+            "geojson_id": "5G",
+            "load_model": "time_series",
+            "load_model_parameters": {
+                "time_series": {
+                    "delta_temp_air_cooling": 10,
+                    "delta_temp_air_heating": 18,
+                    "filepath": "To be populated",
+                    "has_electric_cooling": false,
+                    "has_electric_heating": false,
+                    "has_liquid_cooling": true,
+                    "has_liquid_heating": true,
+                    "max_electrical_load": 0,
+                    "temp_chw_return": 12,
+                    "temp_chw_supply": 7,
+                    "temp_hw_return": 35,
+                    "temp_hw_supply": 40,
+                    "temp_setpoint_cooling": 24,
+                    "temp_setpoint_heating": 20
+                }
+            },
+            "photovoltaic_panels": []
         }
     ],
+    "capacitor_banks": [],
+    "combined_heat_and_power_systems": [],
+    "distribution_lines": [],
     "district_system": {
         "fifth_generation": {
+            "central_pump_parameters": {
+                "pump_design_head": 60000
+            },
             "ghe_parameters": {
                 "design": {
                     "flow_rate": 0.2,
                     "flow_type": "borehole",
                     "max_eft": 35.0,
                     "method": "AREAPROPORTIONAL",
                     "min_eft": 5.0
@@ -74,15 +123,15 @@
                             "length_of_boreholes": 1.0,
                             "number_of_boreholes": 5
                         },
                         "ghe_geometric_params": {
                             "length_of_ghe": 100,
                             "width_of_ghe": 100
                         },
-                        "ghe_id": "c432cb11-4813-40df-8dd4-e88f5de40033"
+                        "ghe_id": "0b575a8f-97d1-47e6-b329-7ef7566d26f2"
                     }
                 ],
                 "grout": {
                     "conductivity": 1.0,
                     "rho_cp": 3901000
                 },
                 "pipe": {
@@ -131,12 +180,21 @@
                 "chp_installed": false,
                 "heat_flow_nominal": 8001,
                 "mass_hhw_flow_nominal": 1,
                 "pressure_drop_hhw_nominal": 55001,
                 "pressure_drop_hhw_valve_nominal": 6001,
                 "pressure_drop_setpoint": 50000,
                 "temp_setpoint_hhw": 54
+            },
+            "central_pump_parameters": {
+                "pump_design_head": 60000
             }
         }
     },
-    "weather": "../../data_shared/USA_CA_San.Francisco.Intl.AP.724940_TMY3.mos"
+    "electrical_grid": {},
+    "photovoltaic_panels": [],
+    "power_converters": [],
+    "substations": [],
+    "transformers": [],
+    "weather": "../../data_shared/USA_CA_San.Francisco.Intl.AP.724940_TMY3.mos",
+    "wind_turbines": []
 }
```

### Comparing `geojson_modelica_translator-0.6.0rc2/geojson_modelica_translator/utils.py` & `geojson_modelica_translator-0.7.0/geojson_modelica_translator/utils.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,21 +3,19 @@
 
 import logging
 import os
 import shutil
 from pathlib import Path
 from uuid import uuid4
 
-_log = logging.getLogger(__name__)
+logger = logging.getLogger(__name__)
 
 
 def copytree(src, dst, symlinks=False, ignore=None):
-    """
-    Alternate version of copytree that will work if the directory already exists (use instead of shutil)
-    """
+    """Alternate version of copytree that will work if the directory already exists (use instead of shutil)"""
     for item in os.listdir(src):
         s = os.path.join(src, item)
         d = os.path.join(dst, item)
         if os.path.isdir(s):
             shutil.copytree(s, d, symlinks, ignore)
         else:
             shutil.copy2(s, d)
@@ -32,26 +30,33 @@
     return c + 273.15
 
 
 def linecount(filename: Path) -> int:
     """Counts the number of lines in a file
     Probably not the most efficient way to do this, but it works
     """
-    return len(open(filename).readlines())
+    with open(filename) as f:
+        filelength = len(f.readlines())
+    return filelength
 
 
-class ModelicaPath(object):
+def mbl_version():
+    """Returns the version of the Modelica Buildings Library (MBL) used by the
+    geojson-modelica-translator.
     """
-    Class for storing Modelica paths. This allows the path to point to
+    return "10.0.0"
+
+
+class ModelicaPath:
+    """Class for storing Modelica paths. This allows the path to point to
     the model directory, resources, and scripts directory.
     """
 
     def __init__(self, name, root_dir, overwrite=False):
-        """
-        Create a new modelica-based path with name of 'name'
+        """Create a new modelica-based path with name of 'name'
 
         :param name: Name to create
         """
         self.name = name
         self.root_dir = root_dir
         self.overwrite = overwrite
 
@@ -70,88 +75,85 @@
                 raise Exception("Directory already exists and overwrite is false for %s" % path)
             else:
                 shutil.rmtree(path)
         os.makedirs(path, exist_ok=True)
 
     @property
     def files_dir(self):
-        """
-        Return the path to the files (models) for the specified ModelicaPath. This path does not include the
+        """Return the path to the files (models) for the specified ModelicaPath. This path does not include the
         trailing slash.
 
         :return: string, path to where files (models) are stored, without trailing slash
         """
         if self.root_dir is None:
             return self.files_relative_dir
         else:
             return f"{self.root_dir}/{self.name}"
 
     @property
     def resources_relative_dir(self):
-        """
-        Return the relative resource directory instead of the full path. This is useful when replacing
+        """Return the relative resource directory instead of the full path. This is useful when replacing
         strings within modelica files which are relative to the package.
 
         :return: string, relative resource's data path
         """
         return f"Resources/Data/{self.name}"
 
     @property
-    def scripts_relative_dir(self, platform='Dymola'):
+    def scripts_relative_dir(self, platform="Dymola"):  # noqa: PLR0206
+        # FIXME: https://docs.astral.sh/ruff/rules/property-with-parameters/
         """Return the scripts directory that is in the resources directory. This only returns the
         relative directory and is useful when replacing string values within Modelica files.
 
         :return: string, relative scripts path
         """
         return f"Resources/Scripts/{self.name}/{platform}"
 
     @property
     def files_relative_dir(self):
         """Return the path to the files relative to the project name."""
         return os.path.join(self.name)
 
     @property
     def resources_dir(self):
-        """
-        Return the path to the resources directory for the specified ModelicaPath. This path does not include
+        """Return the path to the resources directory for the specified ModelicaPath. This path does not include
         the trailing slash.
 
         :return: string, path to where resources are stored, without trailing slash.
         """
         if self.root_dir is None:
             return self.resources_relative_dir
         else:
             return f"{self.root_dir}/{self.resources_relative_dir}"
 
     @property
     def scripts_dir(self):
-        """
-        Return the path to the scripts directory (in the resources dir) for the specified ModelicaPath.
+        """Return the path to the scripts directory (in the resources dir) for the specified ModelicaPath.
         This path does not include the trailing slash.
 
         :return: string, path to where scripts are stored, without trailing slash.
         """
         if self.root_dir is None:
             return self.scripts_relative_dir
         else:
             return f"{self.root_dir}/{self.scripts_relative_dir}"
 
 
 # This is used for some test cases where we need deterministic IDs to be generated
-USE_DETERMINISTIC_ID = bool(os.environ.get('GMT_DETERMINISTIC_ID', False))
+USE_DETERMINISTIC_ID = bool(os.environ.get("GMT_DETERMINISTIC_ID", False))
 
 counter = 0
 
 
 def simple_uuid():
     """Generates a simple string uuid
 
     :return: string, uuid
     """
-    global counter
+    global counter  # noqa: PLW0603
 
     if not USE_DETERMINISTIC_ID:
         return str(uuid4()).split("-")[0]
     else:
-        id = str(counter)
+        string_id = str(counter)
         counter += 1
-        return id
+        return string_id
```

### Comparing `geojson_modelica_translator-0.6.0rc2/management/check_sys_params.py` & `geojson_modelica_translator-0.7.0/management/check_sys_params.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,101 +14,104 @@
 from pathlib import Path
 
 import click
 from jsonpath_ng.ext import parse
 
 logger = logging.getLogger(__name__)
 
-DATA_DIR = Path(__file__).parent / 'data'
+DATA_DIR = Path(__file__).parent / "data"
 
-BASELINE_PACKAGE = 'baseline_package'
-BASELINE_GEOJSON = 'baseline_geojson.json'
-BASELINE_SYS_PARAMS = 'baseline_sys_params.json'
-BASELINE_TIME_SERIES = 'baseline_time_series.mos'
-BASELINE_WEATHER_FILE = 'baseline_weather.mos'
+BASELINE_PACKAGE = "baseline_package"
+BASELINE_GEOJSON = "baseline_geojson.json"
+BASELINE_SYS_PARAMS = "baseline_sys_params.json"
+BASELINE_TIME_SERIES = "baseline_time_series.mos"
+BASELINE_WEATHER_FILE = "baseline_weather.mos"
 
-SYS_PARAMS_SCHEMA_PATH = Path(__file__).parent.parent / 'geojson_modelica_translator' / 'system_parameters' / 'schema.json'
+SYS_PARAMS_SCHEMA_PATH = (
+    Path(__file__).parent.parent / "geojson_modelica_translator" / "system_parameters" / "schema.json"
+)
 
 
 def create_package(package_path, geojson_path, sys_params_path):
     """Creates a package using the uo_des CLI.
     Raises an exception if it fails to create the package.
 
     :param package_path: Path | str, where to create the package
     :param geojson_path: Path | str, where the geojson file is located
     :param sys_params_path: Path | str, where the system parameters file is located
     :return None:
     """
     process = subprocess.Popen(
-        ['poetry', 'run', 'uo_des', 'create-model', sys_params_path, geojson_path, package_path],
+        ["poetry", "run", "uo_des", "create-model", sys_params_path, geojson_path, package_path],
         stdout=subprocess.PIPE,
-        stderr=subprocess.PIPE)
+        stderr=subprocess.PIPE,
+    )
 
     stdout, stderr = process.communicate()
 
     if process.returncode != 0:
         logger.error(stdout.decode())
         logger.error(stderr.decode())
-        raise Exception('Failed to create model')
+        raise Exception("Failed to create model")
 
 
 def get_terminal_paths(obj, current_path):
     """Find all paths to terminal values in the object (recursively).
     Each path object contains a type (number, string, bool, etc) and a list
     of keys to reach that point.
 
     :param obj: dict
     :param current_path: list[str], list of keys that got us to this point
     :return: list[dict]
     """
     paths = []
     for key, value in obj.items():
         if type(value) in [int, float]:
-            paths.append({'type': 'number', 'path': current_path + [key]})
-        elif type(value) is str:
-            paths.append({'type': 'string', 'path': current_path + [key]})
-        elif type(value) is bool:
-            paths.append({'type': 'bool', 'path': current_path + [key]})
-        elif type(value) is list:
-            if len(value) > 0 and type(value[0]) is dict:
+            paths.append({"type": "number", "path": [*current_path, key]})
+        elif isinstance(value, str) is str:
+            paths.append({"type": "string", "path": [*current_path, key]})
+        elif isinstance(value, bool):
+            paths.append({"type": "bool", "path": [*current_path, key]})
+        elif isinstance(value, list):
+            if len(value) > 0 and isinstance(value[0], dict):
                 for idx, item in enumerate(value):
-                    paths += get_terminal_paths(item, current_path + [f'{key}[{idx}]'])
+                    paths += get_terminal_paths(item, [*current_path, f"{key}[{idx}]"])
             else:
                 # skip lists that aren't dicts for now
                 continue
-        elif type(value) is dict:
-            paths += get_terminal_paths(value, current_path + [key])
+        elif isinstance(value, dict):
+            paths += get_terminal_paths(value, [*current_path, key])
         else:
             raise Exception(f'Unhandled type: "{type(value)}"')
 
     return paths
 
 
 def get_all_terminal_paths(obj):
     """Construct JSON paths to all terminal values in obj
 
     :param obj: dict
     :return: list[dict]
     """
-    terminal_paths = get_terminal_paths(obj, ['$'])
+    terminal_paths = get_terminal_paths(obj, ["$"])
 
     # reformat path arrays into jsonpaths
     for terminal_path in terminal_paths:
-        terminal_path['path'] = ".".join(terminal_path["path"])
+        terminal_path["path"] = ".".join(terminal_path["path"])
 
     # deduplicate array objects
     # flag duplicates with "skip"
     registered_paths = set()
     for terminal_path in terminal_paths:
-        standardized_path = re.sub(r'\[\d+\]', '[*]', terminal_path['path'])
+        standardized_path = re.sub(r"\[\d+\]", "[*]", terminal_path["path"])
         if standardized_path not in registered_paths:
             registered_paths.add(standardized_path)
-            terminal_path['skip'] = False
+            terminal_path["skip"] = False
         else:
-            terminal_path['skip'] = True
+            terminal_path["skip"] = True
 
     return terminal_paths
 
 
 def print_diffs(p1, p2, output_file):
     """Print the diffs between modelica packages p1 and p2
 
@@ -121,76 +124,65 @@
     package_2_name = Path(p2).name
 
     found_any_diffs = False
 
     # for each file in p1, compare it to the same file in p2
     for root, _, filenames in os.walk(p1):
         for filename in filenames:
-
-            f1 = f'{root}/{filename}'
-            f2 = f'{root.replace(p1, p2)}/{filename}'
+            f1 = f"{root}/{filename}"
+            f2 = f"{root.replace(p1, p2)}/{filename}"
 
             with open(f1) as f:
                 f1_text = f.readlines()
             with open(f2) as f:
                 f2_text_orig = f.readlines()
                 f2_text = []
                 for line in f2_text_orig:
                     # replace the package names in the files
                     f2_text.append(line.replace(package_2_name, package_1_name))
 
             # remove annotations (placements might get moved around)
             f1_used_lines = []
             for line in f1_text:
-                if not line.strip().startswith('annotation'):
+                if not line.strip().startswith("annotation"):
                     f1_used_lines.append(line)
 
             f2_used_lines = []
             for line in f2_text:
-                if not line.strip().startswith('annotation'):
+                if not line.strip().startswith("annotation"):
                     f2_used_lines.append(line)
 
             file_diffs = difflib.unified_diff(
                 f1_used_lines,
                 f2_used_lines,
                 fromfile=f1,
                 tofile=f2,
-                lineterm='',
+                lineterm="",
             )
             for diff in file_diffs:
                 found_any_diffs = True
                 print(diff, file=output_file)
 
     if not found_any_diffs:
-        print('No diff', file=output_file)
+        print("No diff", file=output_file)
 
 
 @click.command()
+@click.option("-v", is_flag=True, help="Verbose logging", default=False)
+@click.option("-vv", is_flag=True, help="Very verbose logging", default=False)
 @click.option(
-    '-v',
-    is_flag=True,
-    help="Verbose logging",
-    default=False
-)
-@click.option(
-    '-vv',
-    is_flag=True,
-    help="Very verbose logging",
-    default=False
-)
-@click.option(
-    '-o',
-    '--output-file',
+    "-o",
+    "--output-file",
     help="Output file name. Defaults to STDOUT",
     type=click.Path(exists=False, file_okay=True, dir_okay=False),
     default=None,
 )
 @click.option(
-    '-l',
-    '--log-file',
+    "-l",
+    "--log-file",
     help="Log file name. Defaults to STDERR",
     type=click.Path(exists=False, file_okay=True, dir_okay=False),
     default=None,
 )
 def check_sys_params(v, vv, output_file, log_file):
     """Given a baseline systems parameters file, this function generates a package
     from the sys params. Then, for each system parameter, it tweaks the parameter
@@ -208,75 +200,75 @@
     log_level = logging.WARNING
     if v:
         log_level = logging.INFO
     if vv:
         log_level = logging.DEBUG
     logging.basicConfig(level=log_level, filename=log_file)
 
-    output_file_handle = open(output_file, 'w') if output_file else sys.stdout
+    output_file_handle = open(output_file, "w") if output_file else sys.stdout  # noqa: SIM115
 
     # use deterministic IDs for models so that we can diff packages without worrying
     # about different IDs
-    os.environ["GMT_DETERMINISTIC_ID"] = 'True'
+    os.environ["GMT_DETERMINISTIC_ID"] = "True"
 
-    DELIMITER = '=' * 50
+    delimiter = "=" * 50
 
     with tempfile.TemporaryDirectory() as tmpdirname:
-        logger.debug(f'Saving temporary models in {tmpdirname}')
+        logger.debug(f"Saving temporary models in {tmpdirname}")
 
         # some setup in the temp-dir
-        BASELINE_GEOJSON_PATH = f'{tmpdirname}/{BASELINE_GEOJSON}'
-        BASELINE_SYS_PARAMS_PATH = f'{tmpdirname}/{BASELINE_SYS_PARAMS}'
+        baseline_geojson_path = f"{tmpdirname}/{BASELINE_GEOJSON}"
+        baseline_sys_params_path = f"{tmpdirname}/{BASELINE_SYS_PARAMS}"
         for baseline_file_name in [BASELINE_SYS_PARAMS, BASELINE_GEOJSON, BASELINE_TIME_SERIES, BASELINE_WEATHER_FILE]:
             source_path = DATA_DIR / baseline_file_name
-            destination_path = f'{tmpdirname}/{baseline_file_name}'
-            logger.debug(f'Copying {source_path} to {destination_path}')
+            destination_path = f"{tmpdirname}/{baseline_file_name}"
+            logger.debug(f"Copying {source_path} to {destination_path}")
             shutil.copyfile(source_path, destination_path)
 
         # create the baseline package
-        BASELINE_PACKAGE_PATH = f'{tmpdirname}/{BASELINE_PACKAGE}'
-        create_package(BASELINE_PACKAGE_PATH, BASELINE_GEOJSON_PATH, BASELINE_SYS_PARAMS_PATH)
+        baseline_package_path = f"{tmpdirname}/{BASELINE_PACKAGE}"
+        create_package(baseline_package_path, baseline_geojson_path, baseline_sys_params_path)
 
-        with open(BASELINE_SYS_PARAMS_PATH) as f:
+        with open(baseline_sys_params_path) as f:
             base_sys_params = json.loads(f.read())
 
         params = get_all_terminal_paths(base_sys_params)
 
         # for each param, see what happens to the package when we modify it
         for idx, param in enumerate(params):
-            print(DELIMITER, file=output_file_handle)
-            if param['skip']:
+            print(delimiter, file=output_file_handle)
+            if param["skip"]:
                 print(f'{param["path"]} Skipped (duplicate)', file=output_file_handle)
                 continue
 
-            if param['type'] == 'string':
+            if param["type"] == "string":
                 print(f'{param["path"]} Skipped (string)', file=output_file_handle)
                 continue
 
-            jsonpath = parse(param['path'])
+            jsonpath = parse(param["path"])
             original_value = jsonpath.find(base_sys_params)[0].value
 
-            if param['type'] == 'number':
+            if param["type"] == "number":
                 value = 1337000
-            elif param['type'] == 'bool':
+            elif param["type"] == "bool":
                 value = not original_value
             else:
                 raise Exception(f'Unhandled parameter type "{param["type"]}"')
 
             test_sys_params = copy.deepcopy(base_sys_params)
             jsonpath.update(test_sys_params, value)
-            test_package_name = f'test_package_{idx}'
-            test_package_path = f'{tmpdirname}/{test_package_name}'
+            test_package_name = f"test_package_{idx}"
+            test_package_path = f"{tmpdirname}/{test_package_name}"
 
             # generate the package
-            with open(f'{tmpdirname}/test_sys_params.json', 'w') as fp:
+            with open(f"{tmpdirname}/test_sys_params.json", "w") as fp:
                 fp.write(json.dumps(test_sys_params))
                 fp.seek(0)
                 test_sys_params_path = fp.name
-                create_package(test_package_path, BASELINE_GEOJSON_PATH, test_sys_params_path)
+                create_package(test_package_path, baseline_geojson_path, test_sys_params_path)
 
             print(f'{param["path"]}   Testing    Original: {original_value}; New: {value}', file=output_file_handle)
 
             # compare the package to baseline (find diffs)
-            print_diffs(BASELINE_PACKAGE_PATH, test_package_path, output_file_handle)
+            print_diffs(baseline_package_path, test_package_path, output_file_handle)
 
     output_file_handle.close()
```

### Comparing `geojson_modelica_translator-0.6.0rc2/management/data/baseline_geojson.json` & `geojson_modelica_translator-0.7.0/management/data/baseline_geojson.json`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/management/data/baseline_weather.mos` & `geojson_modelica_translator-0.7.0/management/data/baseline_weather.mos`

 * *Files identical despite different names*

### Comparing `geojson_modelica_translator-0.6.0rc2/management/format_modelica_files.py` & `geojson_modelica_translator-0.7.0/management/format_modelica_files.py`

 * *Files 9% similar despite different names*

```diff
@@ -5,205 +5,199 @@
 import re
 import subprocess
 from pathlib import Path
 from tempfile import mkstemp
 
 import click
 
-SKIP_FILES = ['DistrictEnergySystem.mot', 'DistrictEnergySystem5G.mot']
-TEMPLATE_FILES = Path('geojson_modelica_translator/model_connectors').glob('**/templates/*')
+SKIP_FILES = ["DistrictEnergySystem.mot", "DistrictEnergySystem5G.mot"]
+TEMPLATE_FILES = Path("geojson_modelica_translator/model_connectors").glob("**/templates/*")
 
 
 @click.command()
-@click.argument('mofile', required=False)
+@click.argument("mofile", required=False)
 def fmt_modelica_files(mofile):
     if mofile is not None:
         files = [mofile]
     else:
         files = TEMPLATE_FILES
 
     for filepath in files:
         if os.path.basename(filepath) in SKIP_FILES:
             continue
         try:
             if filepath.suffix == ".mot":
                 preprocess_and_format(str(filepath))
             elif filepath.suffix == ".mo":
                 apply_formatter(str(filepath))
-        except FormattingException as e:
-            click.echo(f'Error processing file {filepath}:\n    {e}', err=True)
+        except FormattingError as e:
+            click.echo(f"Error processing file {filepath}:\n    {e}", err=True)
 
 
-class FormattingException(Exception):
+class FormattingError(Exception):
     pass
 
 
-def apply_formatter(filepath):
-    """
-    Run modelicafmt on a file
+def apply_formatter(filepath: str):
+    """Run modelicafmt on a file
 
     :param filepath: str, path to file
     """
     try:
         subprocess.run(["modelicafmt", "-w", filepath], stdout=subprocess.PIPE, check=True)
     except FileNotFoundError:
-        raise FormattingException('Failed to run modelicafmt; ensure it can be found in $PATH')
+        raise FormattingError("Failed to run modelicafmt; ensure it can be found in $PATH")
     except subprocess.CalledProcessError as e:
-        raise FormattingException(f'Failed to format filename: {e.stdout}')
+        raise FormattingError(f"Failed to format filename: {e.stdout}")
 
 
 class SubMap:
-    """
-    Class for managing substitutions into modelica template files (ie Jinja templates)
-    """
+    """Class for managing substitutions into modelica template files (i.e., Jinja templates)"""
 
     def __init__(self):
         self._cur_id = 1
         self._map = {}
 
     def add_sub(self, text):
-        """
-        Registers a substitution and returns the substitution name
+        """Registers a substitution and returns the substitution name
 
         :param text: str, text to substitute
         :returns: str, substitution name/id
         """
-        sub_id = f'JINJA_SUB_{self._cur_id:03}'
+        sub_id = f"JINJA_SUB_{self._cur_id:03}"
         self._map[sub_id] = text
         self._cur_id += 1
 
         return sub_id
 
     def get_text(self, sub):
-        """
-        Get original text for a substitution
+        """Get original text for a substitution
 
         :param sub: str, substitution name
         :returns: str, text corresponding to that substitution name
         """
         try:
             return self._map[sub]
         except KeyError:
-            raise FormattingException(f'Key "{sub}" was not found in the substitution map, this should never happen... '
-                                      f'Perhaps the substitution name was a false positive match?')
+            raise FormattingError(
+                f'Key "{sub}" was not found in the substitution map, this should never happen... '
+                f"Perhaps the substitution name was a false positive match?"
+            )
 
 
-GENERIC_CONTROL_REGEX = re.compile('({%.*?%})')
+GENERIC_CONTROL_REGEX = re.compile("({%.*?%})")
 
 
 def sub_generic(text, sub_map):
-    """
-    Substitutes all Jinja control statements, those that look like {% ... %}
+    """Substitutes all Jinja control statements, those that look like {% ... %}
 
     :param text: str, text to make substitutions in
     :param sub_map: SubMap
     :returns: str, text post substitutions
     """
     matches = reversed([m.span() for m in GENERIC_CONTROL_REGEX.finditer(text)])
     for span in matches:
-        sub_id = sub_map.add_sub(text[span[0]:span[1]])
-        text = f'{text[:span[0]]}/*{sub_id}*/{text[span[1]:]}'
+        sub_id = sub_map.add_sub(text[span[0] : span[1]])
+        text = f"{text[:span[0]]}/*{sub_id}*/{text[span[1]:]}"
 
     return text
 
 
-EXPRESSION_REGEX = re.compile('({{.*?}})')
+EXPRESSION_REGEX = re.compile("({{.*?}})")
 
 
 def sub_expression(text, sub_map):
-    """
-    Substitutes all Jinja expression statements, those that look like {{ ... }}
+    """Substitutes all Jinja expression statements, those that look like {{ ... }}
 
     :param text: str, text to make substitutions in
     :param sub_map: SubMap
     :returns: str, text post substitutions
     """
     matches = reversed([m.span() for m in EXPRESSION_REGEX.finditer(text)])
     for span in matches:
-        sub_id = sub_map.add_sub(text[span[0]:span[1]])
-        text = f'{text[:span[0]]}{sub_id}{text[span[1]:]}'
+        sub_id = sub_map.add_sub(text[span[0] : span[1]])
+        text = f"{text[:span[0]]}{sub_id}{text[span[1]:]}"
 
     return text
 
 
-COMMENTED_SUB = re.compile(r'/\*(JINJA_SUB_\d\d\d)\*/')
-NORMAL_SUB = re.compile(r'JINJA_SUB_\d\d\d')
+COMMENTED_SUB = re.compile(r"/\*(JINJA_SUB_\d\d\d)\*/")
+NORMAL_SUB = re.compile(r"JINJA_SUB_\d\d\d")
 
 
 def reverse_sub(text, sub_map):
-    """
-    Reverses Jinja substitutions, ie replaces the JINJA_SUB_XXX texts with their
+    """Reverses Jinja substitutions, ie replaces the JINJA_SUB_XXX texts with their
     original texts
 
     :param text: str, text to reverse substitutions
     :param sub_map: SubMap, the submap used for making substitutions
     :returns: str, text with substitutions reversed
     """
     # remove the comments around commented substitutions
-    text = COMMENTED_SUB.sub(r'\1', text)
+    text = COMMENTED_SUB.sub(r"\1", text)
 
     # replace all substitutions with their original values
     def _replace(matchobj):
         return sub_map.get_text(matchobj.group(0))
+
     text = NORMAL_SUB.sub(_replace, text)
 
     return text
 
 
 def preprocess_and_format(filename, outfilename=None):
-    """
-    Formats modelica files that include Jinja templating.
+    """Formats modelica files that include Jinja templating.
 
     :param filename: str, template file to format
     """
     try:
         with open(filename) as f:
             contents = f.read()
     except FileNotFoundError:
-        raise FormattingException(f'File "{filename}" not found.')
+        raise FormattingError(f'File "{filename}" not found.')
 
     tmp_fd, tmp_filepath = mkstemp()
     try:
         # General strategy:
         #   1. replace all Jinja templating stuff with unique IDs, additionally
         #      commenting out any IDs that would result in invalid modelica
         #      syntax (those that are flow control, ie {% ... %}). After this
         #      step the file should be "valid" from the modelica lexer's perspective
         #   2. apply modelica formatter to format the file
         #   3. reverse the substitutions, replacing IDs with their original text
         sub_map = SubMap()
         previous_span = (0, 0)
-        raw_regex = re.compile(r'{% raw %}[\s\S]*?{% endraw %}')
+        raw_regex = re.compile(r"{% raw %}[\s\S]*?{% endraw %}")
         raw_groups = [m.span() for m in raw_regex.finditer(contents)]
-        with open(tmp_fd, 'w') as f:
+        with open(tmp_fd, "w") as f:
             for span in raw_groups:
                 # format from previous end to new start
-                text = contents[previous_span[1]:span[0]]
+                text = contents[previous_span[1] : span[0]]
                 text = sub_generic(text, sub_map)
                 text = sub_expression(text, sub_map)
                 f.write(text)
 
                 # format current span (should be raw)
-                text = contents[span[0]:span[1]]
+                text = contents[span[0] : span[1]]
                 text = sub_generic(text, sub_map)
                 f.write(text)
 
                 previous_span = span
 
             # finish from end of last span to end of file
-            text = contents[previous_span[1]:]
+            text = contents[previous_span[1] :]
             text = sub_generic(text, sub_map)
             text = sub_expression(text, sub_map)
             f.write(text)
 
         apply_formatter(tmp_filepath)
 
         # substitute original values back in
-        with open(tmp_filepath, 'r') as f:
+        with open(tmp_filepath) as f:
             formatted_result = reverse_sub(f.read(), sub_map)
 
         if outfilename is None:
             outfilename = filename
-        with open(outfilename, 'w') as f:
+        with open(outfilename, "w") as f:
             f.write(formatted_result)
     finally:
         os.remove(tmp_filepath)
```

### Comparing `geojson_modelica_translator-0.6.0rc2/management/uo_des.py` & `geojson_modelica_translator-0.7.0/management/uo_des.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,23 +2,19 @@
 # See also https://github.com/urbanopt/geojson-modelica-translator/blob/develop/LICENSE.md
 
 from pathlib import Path
 from shutil import rmtree
 
 import click
 
-from geojson_modelica_translator.geojson_modelica_translator import (
-    GeoJsonModelicaTranslator
-)
+from geojson_modelica_translator.geojson_modelica_translator import GeoJsonModelicaTranslator
 from geojson_modelica_translator.modelica.modelica_runner import ModelicaRunner
-from geojson_modelica_translator.system_parameters.system_parameters import (
-    SystemParameters
-)
+from geojson_modelica_translator.system_parameters.system_parameters import SystemParameters
 
-CONTEXT_SETTINGS = dict(help_option_names=['-h', '--help'])
+CONTEXT_SETTINGS = {"help_option_names": ["-h", "--help"]}
 
 
 @click.group(context_settings=CONTEXT_SETTINGS)
 def cli():
     """URBANopt District Energy Systems"""
 
 
@@ -32,81 +28,81 @@
     type=click.Path(exists=True, file_okay=True, dir_okay=False),
 )
 @click.argument(
     "feature_file",
     type=click.Path(exists=True, file_okay=True, dir_okay=False),
 )
 @click.argument(
+    "district_type",
+    default="4G",
+)
+@click.argument(
     "model_type",
-    default='time_series',
+    default="time_series",
 )
 @click.option(
-    '-o',
-    '--overwrite',
+    "-o",
+    "--overwrite",
     is_flag=True,
     help="Delete and replace any existing file of the same name & location",
-    default=False
+    default=False,
 )
 @click.option(
-    '-m',
-    '--microgrid',
+    "-m",
+    "--microgrid",
     is_flag=True,
     help="If specified, microgrid inputs will be added to system parameters file",
-    default=False
+    default=False,
 )
-@click.option(
-    '-g',
-    '--ghe',
-    is_flag=True,
-    help="If specified, Ground Heat Exchanger properties will be added to System Parameters File",
-    default=False
-)
-def build_sys_param(model_type: str,
-                    sys_param_filename: Path,
-                    scenario_file: Path,
-                    feature_file: Path,
-                    ghe: bool,
-                    overwrite: bool,
-                    microgrid: bool
-                    ):
-    """
-    Create system parameters file using uo_sdk output
+def build_sys_param(
+    model_type: str,
+    sys_param_filename: Path,
+    scenario_file: Path,
+    feature_file: Path,
+    district_type: str,
+    overwrite: bool,
+    microgrid: bool,
+):
+    """Create system parameters file using uo_sdk output
+    #FIXME: Formatting of the args...
 
     SYS_PARAM_FILENAME: Path/name to sys-param file be created. Be sure to include the ".json" suffix.
 
     SCENARIO_FILE: Path to sdk scenario file.
 
     FEATURE_FILE: Path to sdk json feature file with data about the buildings.
 
+    DISTRICT_TYPE: selection for which kind of simulation this sys-param file will support.
+
     \b
     MODEL_TYPE: selection for which kind of simulation this sys-param file will support.
         Valid choices for MODEL_TYPE: "time_series"
 
     \f
     :param model_type: string, selection of which model type to use in the GMT
     :param sys_param_filename: Path, location & name of json output file to save
     :param scenario_file: Path, location of SDK scenario_file
     :param feature_file: Path, location of SDK feature_file
-    :param ghe: Boolean, flag to add Ground Heat Exchanger properties to System Parameter File
+    :param district_type: string, district type to model
     :param overwrite: Boolean, flag to overwrite an existing file of the same name/location
     :param microgrid: Boolean, flag to add Microgrid properties to System Parameter File
     """
 
     # Use scenario_file to be consistent with sdk
     scenario_name = Path(scenario_file).stem
-    scenario_dir = Path(scenario_file).parent / 'run' / scenario_name
+    scenario_dir = Path(scenario_file).parent / "run" / scenario_name
     sp = SystemParameters()
     sp.csv_to_sys_param(
         model_type=model_type,
         sys_param_filename=Path(sys_param_filename),
         scenario_dir=Path(scenario_dir),
         feature_file=Path(feature_file),
-        ghe=ghe,
+        district_type=district_type,
         overwrite=overwrite,
-        microgrid=microgrid
+        microgrid=microgrid,
     )
 
     if Path(sys_param_filename).exists():
         print(f"\nSystem parameters file {sys_param_filename} successfully created.")
     else:
         raise SystemExit(f"{sys_param_filename} failed. Please check your inputs and try again.")
 
@@ -122,112 +118,125 @@
 )
 @click.argument(
     "project_path",
     default="model_from_sdk",
     type=click.Path(exists=False, file_okay=False, dir_okay=True),
 )
 @click.option(
-    '-o',
-    '--overwrite',
+    "-o",
+    "--overwrite",
     is_flag=True,
     help="Delete and replace any existing folder of the same name & location",
-    default=False
+    default=False,
 )
 def create_model(sys_param_file: Path, geojson_feature_file: Path, project_path: Path, overwrite: bool):
     """Build Modelica model from user data
 
     SYS_PARAM_FILE: Path/name to sys-param file, possibly created with this CLI.
 
     GEOJSON_FEATURE_FILE: Path to sdk json feature file with data about the buildings.
 
     PROJECT_PATH: Path for Modelica project directory created with this command
 
     \f
-    :param model_type: String, type of model to create
     :param sys_param_file: Path, location and name of file created with this cli
     :param geojson_feature_file: Path, location and name of sdk feature_file
     :param project_path: Path, location and name of Modelica model dir to be created
     :param overwrite: Boolean, flag to overwrite an existing file of the same name/location
     """
     project_path = Path(project_path)
     if project_path.exists():
         if overwrite:
             rmtree(project_path, ignore_errors=True)
         else:
             raise SystemExit(f"Output dir '{project_path}' already exists and overwrite flag is not given")
     if len(project_path.name.split()) > 1:  # Modelica can't handle spaces in project name
         raise SystemExit(
             f"\n'{project_path}' failed. Modelica does not support spaces in project names or paths. "
-            "Please choose a different 'project_path'")
+            "Please choose a different 'project_path'"
+        )
 
-    gmt = GeoJsonModelicaTranslator(
-        geojson_feature_file,
-        sys_param_file,
-        project_path.parent,
-        project_path.name
-    )
+    gmt = GeoJsonModelicaTranslator(geojson_feature_file, sys_param_file, project_path.parent, project_path.name)
 
     gmt.to_modelica()
 
 
 @cli.command(short_help="Run Modelica model")
 @click.argument(
     "modelica_project",
     default="./model_from_sdk",
     required=True,
     type=click.Path(exists=True, file_okay=False, dir_okay=True),
 )
-@click.argument(
-    "start_time",
+@click.option(
+    "-a",
+    "--start_time",
     default=17280000,
+    help="Start time of the simulation (seconds of a year)",
     type=int,
-    required=False,
 )
-@click.argument(
-    "stop_time",
+@click.option(
+    "-z",
+    "--stop_time",
     default=17366400,
+    help="Stop time of the simulation (seconds of a year)",
     type=int,
-    required=False,
 )
-@click.argument(
-    "step_size",
+@click.option(
+    "-x",
+    "--step_size",
     default=90,
+    help="Step size of the simulation (seconds)",
     type=int,
-    required=False,
 )
-def run_model(modelica_project: Path, start_time: int, stop_time: int, step_size: int):
-    """
+@click.option(
+    "-i",
+    "--intervals",
+    default=100,
+    help="Number of intervals to divide the simulation into (alternative to step_size)",
+    type=int,
+)
+def run_model(modelica_project: Path, start_time: int, stop_time: int, step_size: int, intervals: int):
+    """Run the model
     \b
     Run the Modelica project in a docker-based environment.
     Results are saved at the same level as the project path that is passed.
     The model that runs is hard coded to be the Districts/DistrictEnergySystem.mo within the package.
 
     \b
     MODELICA_PROJECT: Path to the Modelica project, possibly created by this cli
         default = ./model_from_sdk
 
     \f
     :param modelica_project: Path, name & location of modelica project, possibly created with this cli
+    :param start_time (int): start time of the simulation (seconds of a year)
+    :param stop_time (int): stop time of the simulation (seconds of a year)
+    :param step_size (int): step size of the simulation (seconds)
+    :param number_of_intervals (int): number of intervals to run the simulation
     """
     run_path = Path(modelica_project).resolve()
     project_name = run_path.stem
 
     if len(str(run_path).split()) > 1:  # Modelica can't handle spaces in project name or path
         raise SystemExit(
             f"\n'{run_path}' failed. Modelica does not support spaces in project names or paths. "
-            "Please update your directory tree to not include spaces in any name")
+            "Please update your directory tree to not include spaces in any name"
+        )
 
     # setup modelica runner
     mr = ModelicaRunner()
-    mr.run_in_docker('compile_and_run',
-                     f'{project_name}.Districts.DistrictEnergySystem',
-                     file_to_load=run_path / 'package.mo',
-                     run_path=run_path,
-                     start_time=start_time,
-                     stop_time=stop_time,
-                     step_size=step_size
-                     )
+    mr.run_in_docker(
+        "compile_and_run",
+        f"{project_name}.Districts.DistrictEnergySystem",
+        file_to_load=run_path / "package.mo",
+        run_path=run_path,
+        start_time=start_time,
+        stop_time=stop_time,
+        step_size=step_size,
+        number_of_intervals=intervals,
+    )
 
-    if (run_path.parent / f'{project_name}/{project_name}.Districts.DistrictEnergySystem_results' / f'{project_name}_Districts_DistrictEnergySystem_res.mat').exists():
-        print(f"\nModelica model {project_name} ran successfully")
+    run_location = run_path.parent / project_name / f"{project_name}.Districts.DistrictEnergySystem_results"
+    if (run_location / f"{project_name}.Districts.DistrictEnergySystem_res.mat").exists():
+        print(f"\nModelica model {project_name} ran successfully and can be found in {run_location}")
     else:
-        raise SystemExit(f"\n{project_name} failed. Check the error log at {project_name}_results/stdout.log for more info.")
+        raise SystemExit(f"\n{project_name} failed. Check the error log at {run_location}/stdout.log for more info.")
```

### Comparing `geojson_modelica_translator-0.6.0rc2/management/update_schemas.py` & `geojson_modelica_translator-0.7.0/management/update_schemas.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,22 +13,25 @@
     "electrical_junction_properties.json",
     "region_properties.json",
     "site_properties.json",
     "thermal_connector_properties.json",
     "thermal_junction_properties.json",
 ]
 
-baseurl = "https://raw.githubusercontent.com/urbanopt/urbanopt-geojson-gem/develop/lib/urbanopt/geojson/schema/"  # noqa
+baseurl = "https://raw.githubusercontent.com/urbanopt/urbanopt-geojson-gem/develop/lib/urbanopt/geojson/schema/"
 
 
 @click.command()
-@click.argument('schema', required=False)
+@click.argument("schema", required=False)
 def update_schemas(schema):
+    files_to_download.append(schema)
     for f in files_to_download:
         click.echo(f"Downloading schema: {f}")
-        response = requests.get(f"{baseurl}/{f}")
+        response = requests.get(f"{baseurl}/{f}", timeout=(5, 5))
         save_path = f"geojson_modelica_translator/geojson/data/schemas/{f}"
         with open(save_path, "w") as outf:
             json.dump(response.json(), outf, indent=2)
 
-        print("Note that the [unused] fields will have been overwritten by this operation. It is recommended to "
-              "open the previous version and new version in a diff tool to copy over the [unused] tags.")
+        print(
+            "Note that the [unused] fields will have been overwritten by this operation. It is recommended to "
+            "open the previous version and new version in a diff tool to copy over the [unused] tags."
+        )
```

### Comparing `geojson_modelica_translator-0.6.0rc2/PKG-INFO` & `geojson_modelica_translator-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,115 +1,99 @@
 Metadata-Version: 2.1
 Name: geojson-modelica-translator
-Version: 0.6.0rc2
+Version: 0.7.0
 Summary: Package for converting GeoJSON to Modelica models for Urban Scale Analyses.
 Home-page: https://docs.urbanopt.net
 License: BSD-4-Clause
 Keywords: URBANopt,Modelica,GeoJSON,Physics-based Modeling
 Author: URBANopt DES Team
 Author-email: nicholas.long@nrel.gov
-Requires-Python: >=3.9,<3.12
+Requires-Python: >=3.9,<3.13
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering
 Requires-Dist: BuildingsPy (==4.0.0)
-Requires-Dist: click (==8.1.3)
-Requires-Dist: geojson (>=3.0.0,<4.0.0)
+Requires-Dist: click (>=8.1,<9.0)
+Requires-Dist: geojson (>=3.1,<4.0)
 Requires-Dist: jinja2 (==3.1.2)
 Requires-Dist: jsonpath-ng (>=1.6,<1.7)
-Requires-Dist: jsonschema (>=4.19,<4.20)
-Requires-Dist: modelica-builder (>=0.4.0,<0.5.0)
-Requires-Dist: pandas (==2.0.2)
+Requires-Dist: jsonschema (>=4.20,<4.21)
+Requires-Dist: modelica-builder (>=0.5.1,<0.6.0)
+Requires-Dist: pandas (>=2,<3)
 Requires-Dist: requests (>=2.28,<3.0)
 Requires-Dist: teaser (==0.7.5)
 Project-URL: Documentation, https://docs.urbanopt.net/geojson-modelica-translator/
 Project-URL: Repository, https://github.com/urbanopt/geojson-modelica-translator
-Description-Content-Type: text/x-rst
+Description-Content-Type: text/markdown
 
-GeoJSON Modelica Translator (GMT)
----------------------------------
+# GeoJSON Modelica Translator (GMT)
 
-.. image:: https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml/badge.svg?branch=develop
-    :target: https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml
+[![image](https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml/badge.svg?branch=develop)](https://github.com/urbanopt/geojson-modelica-translator/actions/workflows/ci.yml)
+[![image](https://coveralls.io/repos/github/urbanopt/geojson-modelica-translator/badge.svg?branch=develop)](https://coveralls.io/github/urbanopt/geojson-modelica-translator?branch=develop)
+[![image](https://badge.fury.io/py/geojson-modelica-translator.svg)](https://badge.fury.io/py/geojson-modelica-translator)
 
-.. image:: https://coveralls.io/repos/github/urbanopt/geojson-modelica-translator/badge.svg?branch=develop
-    :target: https://coveralls.io/github/urbanopt/geojson-modelica-translator?branch=develop
-
-.. image:: https://badge.fury.io/py/geojson-modelica-translator.svg
-    :target: https://badge.fury.io/py/geojson-modelica-translator
-
-Description
------------
-
-The GeoJSON Modelica Translator (GMT) is a one-way trip from GeoJSON in combination with a well-defined instance of the system parameters schema to a Modelica package with multiple buildings loads, energy transfer stations, distribution networks, and central plants. The project will eventually allow multiple paths to build up different district heating and cooling system topologies; however, the initial implementation is limited to 1GDH and 4GDHC.
+The GeoJSON Modelica Translator (GMT) is a one-way trip from GeoJSON in combination with a well-defined instance of the system parameters schema to a Modelica package with multiple buildings loads, energy transfer stations, distribution networks, and central plants. The project will eventually allow multiple paths to build up different district heating and cooling system topologies; however, the initial implementation is limited to 4GDHC and 5GDHC.
 
 The project is motivated by the need to easily evaluate district energy systems. The goal is to eventually cover the various generations of heating and cooling systems as shown in the figure below. The need to move towards 5GDHC systems results in higher efficiencies and greater access to additional waste-heat sources.
 
-.. image:: https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-generations.png
-
-Getting Started
----------------
+![image](https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-generations.png)
 
-It is possible to test the GeoJSON to Modelica Translator (GMT) by simply installing the Python package and running the
-command line interface (CLI) with results from and URBANopt SDK set of results. However, to fully leverage the
-functionality of this package (e.g., running simulations), then you must also install the Modelica Buildings
-library (MBL) and Docker. Instructions for installing and configuring the MBL and Docker are available
-`here <docs/getting_started.rst>`_.
+## Getting Started
 
-To simply scaffold out a Modelica package that can be inspected in a Modelica environment (e.g., Dymola) then
-run the following code below up to the point of run-model. The example generates a complete 4th Generation District
-Heating and Cooling (4GDHC) system with time series loads that were generated from the URBANopt SDK using
-OpenStudio/EnergyPlus simulations.
+It is possible to test the GeoJSON to Modelica Translator (GMT) by simply installing the Python package and running the command line interface (CLI) with results from and URBANopt SDK set of results. However, to fully leverage the functionality of this package (e.g., running simulations), then you must also install the Modelica Buildings library (MBL) and Docker. Instructions for installing and configuring the MBL and Docker are available [here](docs/getting_started.rst).
 
-.. code-block:: bash
+To simply scaffold out a Modelica package that can be inspected in a Modelica environment (e.g., Dymola, OpenModelica) then run the following code below up to the point of run-model. The example generates a complete 4th Generation District Heating and Cooling (4GDHC) system with time series loads that were generated from the URBANopt SDK using OpenStudio/EnergyPlus simulations.
 
-    pip install geojson-modelica-translator
+``` bash
+pip install geojson-modelica-translator
 
-    # from the simulation results within a checkout of this repository
-    # in the ./tests/management/data/sdk_project_scraps path.
+# from the simulation results within a checkout of this repository
+# in the ./tests/management/data/sdk_project_scraps path.
 
-    # generate the system parameter from the results of the URBANopt SDK and OpenStudio Simulations
-    uo_des build-sys-param sys_param.json baseline_scenario.csv example_project.json
+# generate the system parameter from the results of the URBANopt SDK and OpenStudio Simulations
+uo_des build-sys-param sys_param.json baseline_scenario.csv example_project.json
 
-    # create the modelica package (requires installation of the MBL)
-    uo_des create-model sys_param.json example_project.json model_from_sdk
+# create the modelica package (requires installation of the MBL)
+uo_des create-model sys_param.json example_project.json model_from_sdk
 
-    # test running the new Modelica package (requires installation of Docker)
-    uo_des run-model model_from_sdk
+# test running the new Modelica package (requires installation of Docker)
+uo_des run-model model_from_sdk
+```
 
-More example projects are available in an accompanying
-`example repository <https://github.com/urbanopt/geojson-modelica-translator-examples>`_.
+More example projects are available in an accompanying [example repository](https://github.com/urbanopt/geojson-modelica-translator-examples).
 
-Architecture Overview
----------------------
+## Architecture Overview
 
-The GMT is designed to enable "easy" swapping of building loads, district systems, and network topologies. Some
-of these functionalities are more developed than others, for instance swapping building loads between Spawn and
-RC models (using TEASER) is fleshed out; however, swapping between a first and fifth generation heating system has
-yet to be fully implemented.
+The GMT is designed to enable "easy" swapping of building loads, district systems, and network topologies. Some of these functionalities are more developed than others, for instance swapping building loads between Spawn and RC models (using TEASER) is fleshed out; however, swapping between a first and fifth generation heating system has yet to be fully implemented.
 
-The diagram below is meant to illustrate the future proposed interconnectivity and functionality of the
-GMT project.
+The diagram below is meant to illustrate the future proposed interconnectivity and functionality of the GMT project.
 
-.. image:: https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-connections.png
+![image](https://raw.githubusercontent.com/urbanopt/geojson-modelica-translator/develop/docs/images/des-connections.png)
 
-As shown in the image, there are multiple building loads that can be deployed with the GMT and are described in the `Building Load Models`_ section below. These models, and the associated design parameters, are required to create a fully runnable Modelica model. The GMT leverages two file formats for generating the Modelica project and are the GeoJSON feature file and a System Parameter JSON file. See the more `comprehensive
-documentation on the GMT <https://docs.urbanopt.net/geojson-modelica-translator/>`_ or the `documentation on
-URBANopt SDK  <https://docs.urbanopt.net/>`_.
+As shown in the image, there are multiple building loads that can be deployed with the GMT and are described in the [Building Load Models](#building-load-models) section below. These models, and the associated design parameters, are required to create a fully runnable Modelica model. The GMT leverages two file formats for generating the Modelica project and are the GeoJSON feature file and a System Parameter JSON file. See the more [comprehensive documentation on the GMT](https://docs.urbanopt.net/geojson-modelica-translator/) or the [documentation on URBANopt SDK](https://docs.urbanopt.net/).
 
-Building Load Models
-++++++++++++++++++++
+### Building Load Models
 
 The building loads can be defined multiple ways depending on the fidelity of the required models. Each of the building load models are easily replaced using configuration settings within the System Parameters file. The 4 different building load models include:
 
-#. Time Series in Watts: This building load is the total heating, cooling, and domestic hot water loads represented in a CSV type file (MOS file). The units are Watts and should be reported at an hour interval; however, finer resolution is possible. The load is defined as the load seen by the ETS.
-#. Time Series as mass flow rate and delta temperature: This building load is similar to the other Time Series model but uses the load as seen by the ETS in the form of mass flow rate and delta temperature. The file format is similar to the other Time Series model but the columns are mass flow rate and delta temperature for heating and cooling separately.
-#. RC Model: This model leverages the TEASER framework to generate an RC model with the correct coefficients based on high level parameters that are extracted from the GeoJSON file including building area and building type.
-#. Spawn of EnergyPlus: This model uses EnergyPlus models to represent the thermal zone heat balance portion of the models while using Modelica for the remaining components. Spawn of EnergyPlus is still under development and currently only works on Linux-based systems.
+1. **Time Series in Watts**: This building load is the total heating, cooling, and domestic hot water loads represented in a CSV type file (MOS file). The units are Watts and should be reported at an hour interval; however, finer resolution is possible. The load is defined as the load seen by the ETS.
+2. **Time Series as mass flow rate and delta temperature**: This building load is similar to the other Time Series model but uses the load as seen by the ETS in the form of mass flow rate and delta temperature. The file format is similar to the other Time Series model but the columns are mass flow rate and delta temperature for heating and cooling separately.
+3. **RC Model**: This model leverages the TEASER framework to generate an RC model with the correct coefficients based on high level parameters that are extracted from the GeoJSON file including building area and building type.
+4. **Spawn of EnergyPlus**: This model uses EnergyPlus models to represent the thermal zone heat balance portion of the models while using Modelica for the remaining components. Spawn of EnergyPlus is still under development and currently only works on Linux-based systems.
+
+## Release Instructions
+
+1. Create a branch named `prep-0.x.y Release`
+2. Update CHANGELOG using GitHub's "Autogenerate Change Log" feature
+3. After tests pass, merge branch into develop
+4. Create new PR from develop into main named `Release 0.x.y`
+5. Using GitHub squash-merge into main
+6. From local repo, immediately merge main into develop (as a merge commit) and push. This can only be done with users that have bypass privileges on GitHub.
```

