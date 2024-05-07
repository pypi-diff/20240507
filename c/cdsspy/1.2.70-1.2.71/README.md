# Comparing `tmp/cdsspy-1.2.70.tar.gz` & `tmp/cdsspy-1.2.71.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdsspy-1.2.70.tar", last modified: Thu May 25 12:18:57 2023, max compression
+gzip compressed data, was "cdsspy-1.2.71.tar", last modified: Tue May  7 15:55:54 2024, max compression
```

## Comparing `cdsspy-1.2.70.tar` & `cdsspy-1.2.71.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:57.536836 cdsspy-1.2.70/
--rw-rw-rw-   0        0        0     1059 2023-01-10 16:17:56.000000 cdsspy-1.2.70/LICENSE
--rw-rw-rw-   0        0        0    19401 2023-05-25 12:18:57.536836 cdsspy-1.2.70/PKG-INFO
--rw-rw-rw-   0        0        0    18980 2023-01-12 17:46:31.000000 cdsspy-1.2.70/README.md
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:57.519837 cdsspy-1.2.70/cdsspy/
--rw-rw-rw-   0        0        0      275 2023-05-25 12:18:35.000000 cdsspy-1.2.70/cdsspy/__init__.py
--rw-rw-rw-   0        0        0     5075 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/admin_calls.py
--rw-rw-rw-   0        0        0    34256 2023-05-25 12:16:52.000000 cdsspy-1.2.70/cdsspy/analysis_services.py
--rw-rw-rw-   0        0        0    23253 2023-05-25 12:18:49.000000 cdsspy-1.2.70/cdsspy/climate.py
--rw-rw-rw-   0        0        0    15842 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/gw.py
--rw-rw-rw-   0        0        0    25370 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/reference_tbl.py
--rw-rw-rw-   0        0        0    34631 2023-05-25 12:16:28.000000 cdsspy-1.2.70/cdsspy/structures.py
--rw-rw-rw-   0        0        0    24836 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/sw.py
--rw-rw-rw-   0        0        0    11244 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/telemetry.py
--rw-rw-rw-   0        0        0    33575 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/utils.py
--rw-rw-rw-   0        0        0     9956 2023-05-25 12:10:29.000000 cdsspy-1.2.70/cdsspy/water_rights.py
-drwxrwxrwx   0        0        0        0 2023-05-25 12:18:57.534838 cdsspy-1.2.70/cdsspy.egg-info/
--rw-rw-rw-   0        0        0    19401 2023-05-25 12:18:57.000000 cdsspy-1.2.70/cdsspy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      392 2023-05-25 12:18:57.000000 cdsspy-1.2.70/cdsspy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-25 12:18:57.000000 cdsspy-1.2.70/cdsspy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-25 12:18:57.000000 cdsspy-1.2.70/cdsspy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-25 12:18:57.000000 cdsspy-1.2.70/cdsspy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-25 12:18:57.536836 cdsspy-1.2.70/setup.cfg
--rw-rw-rw-   0        0        0     1356 2023-05-25 12:18:44.000000 cdsspy-1.2.70/setup.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 15:55:54.801221 cdsspy-1.2.71/
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1053 2024-05-07 15:37:35.000000 cdsspy-1.2.71/LICENSE
+-rw-r--r--   0 anguswatters   (501) staff       (20)    18892 2024-05-07 15:55:54.800933 cdsspy-1.2.71/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)    18352 2024-05-07 15:48:26.000000 cdsspy-1.2.71/README.md
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 15:55:54.799152 cdsspy-1.2.71/cdsspy/
+-rw-r--r--   0 anguswatters   (501) staff       (20)      265 2024-05-07 15:50:01.000000 cdsspy-1.2.71/cdsspy/__init__.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     4941 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/admin_calls.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    33365 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/analysis_services.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    22661 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/climate.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    15410 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/gw.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24621 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/reference_tbl.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    33729 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/structures.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    24200 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/sw.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    10959 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/telemetry.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)    32661 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/utils.py
+-rw-r--r--   0 anguswatters   (501) staff       (20)     9699 2024-05-07 15:37:35.000000 cdsspy-1.2.71/cdsspy/water_rights.py
+drwxr-xr-x   0 anguswatters   (501) staff       (20)        0 2024-05-07 15:55:54.800600 cdsspy-1.2.71/cdsspy.egg-info/
+-rw-r--r--   0 anguswatters   (501) staff       (20)    18892 2024-05-07 15:55:54.000000 cdsspy-1.2.71/cdsspy.egg-info/PKG-INFO
+-rw-r--r--   0 anguswatters   (501) staff       (20)      392 2024-05-07 15:55:54.000000 cdsspy-1.2.71/cdsspy.egg-info/SOURCES.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        1 2024-05-07 15:55:54.000000 cdsspy-1.2.71/cdsspy.egg-info/dependency_links.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       50 2024-05-07 15:55:54.000000 cdsspy-1.2.71/cdsspy.egg-info/requires.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)        7 2024-05-07 15:55:54.000000 cdsspy-1.2.71/cdsspy.egg-info/top_level.txt
+-rw-r--r--   0 anguswatters   (501) staff       (20)       38 2024-05-07 15:55:54.801270 cdsspy-1.2.71/setup.cfg
+-rw-r--r--   0 anguswatters   (501) staff       (20)     1333 2024-05-07 15:55:49.000000 cdsspy-1.2.71/setup.py
```

### Comparing `cdsspy-1.2.70/LICENSE` & `cdsspy-1.2.71/LICENSE`

 * *Ordering differences only*

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,7 @@
-Copyright 2023 cdsspy authors
-
-Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
-
+Copyright 2023 cdsspy authors
+
+Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.
+
 THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
```

### Comparing `cdsspy-1.2.70/PKG-INFO` & `cdsspy-1.2.71/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,290 +1,297 @@
-Metadata-Version: 2.1
-Name: cdsspy
-Version: 1.2.70
-Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
-Author: Angus Watters
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **cdsspy** <img src="https://cdsspy-images.s3.us-west-1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
-
-<!-- badges: start -->
-
-[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-<!-- badges: end -->
-
-<div align="left">
-
-<p align="left">
-<a href="https://dwr.state.co.us/Tools"><strong>Â« CDSS Â»</strong></a>
-<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
-Services</a>
-</p>
-
-</div>
-
-<hr>
-
-The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
-
-The Coloradoâ€™s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
-
-Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
-
-<br>
-
-> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
-
----
-
-- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
-
-- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
-
-- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
-
-- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
-
----
-
-<br> 
-
-## **Installation**
-Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
-
-``` 
-pip install cdsspy
-```
-<br>
-
-## **Available endpoints**
-
-Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
-|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
-|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
-|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
-|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
-|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
-|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
-|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-<br>
-
-## **Identify query inputs using reference tables**
-
-The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
-
-<br>
-
-```python
-# available parameters for telemetry stations
-telemetry_params = cdsspy.get_reference_tbl(
-    table_name = "telemetryparams"
-    )
-```
-
-|    | Parameter   |
-|---:|:------------|
-|  0 | AIRTEMP     |
-|  1 | BAR_P       |
-|  2 | BATTERY     |
-|  3 | COND        |
-|  4 | D1          |
-|  5 | D2          |
-|  6 | DISCHRG     |
-|  7 | DISCHRG1    |
-|  8 | DISCHRG2    |
-|  9 | DISCHRG3    |
-| 10 | DISCHRG4    |
-| 11 | ELEV        |
-
-<br>
-<br>
-<br>
-
-## **Locate structures**
-
-**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
-|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
-
-<br>
-
-### **Example: Locating telemetry stations by county:**
-
-```python
-# identify telemetry stations in Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    county = "Boulder"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/county_telem_stations2.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations around a point**
-
-```python
-# identify telemetry stations within a 15 mile radius of the center point of Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = [-105.358164, 40.092608],
-    radius = 15
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/poi_telem_stations.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations within a spatial extent**
-A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
-
-```python
-# identify telemetry stations 15 miles around the centroid of a polygon
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_county.gpkg")
-    radius = 15
-    )
-```
-
-This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve time series data** 
-
-The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-
-#### **Example: Daily discharge at a telemetry station**
-We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
-
-<br>
-
-The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
-
-```python
-# Daily discharge at "ANDDITCO" telemetry station
-discharge_ts   = cdsspy.get_telemetry_ts(
-    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
-    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
-    start_date     = "2015-01-01",   # Starting date
-    end_date       = "2022-01-01",   # Ending date
-    timescale      = "day"           # select daily timescale
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
-
-<br>
-<br>
-
-#### **Example: Retrieve Diversion records for multiple structures**
-Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
-
-
-1. Executing a spatial search using **`get_structures()`** 
-2. Selecting the WDIDs of interest from the search results
-3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
-
-
-```python 
-# 1. Executing a spatial search
-structures = cdsspy.get_structures(
-    aoi    = [-105.3578, 40.09244],
-    radius = 5
-    )
-
-# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
-ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
-ditch_wdids = list(ditch_wdids['wdid'])
-
-# 3. Providing the WDID's as a list to get_structures_divrec_ts()
-diversion_rec  = cdsspy.get_structures_divrec_ts(
-    wdid           = ditch_wdids,
-    wc_identifier  = "diversion",
-    timescale      = "month"
-    )
-```
-**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve groundwater data**
-The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
-
-| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
-|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
-| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
-| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
-| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
-| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
-
-<br>
-
-Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
-
-```python
-# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
-well_measure = cdsspy.get_gw_wl_wellmeasures(
-    wellid     = "1274",
-    start_date = "1990-01-01",
-    end_date   = "2022-01-01"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/gw_depth_to_water_plot2.png)
+Metadata-Version: 2.1
+Name: cdsspy
+Version: 1.2.71
+Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
+Author: Angus Watters
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: datetime
+Requires-Dist: requests
+Requires-Dist: geopandas
+Requires-Dist: shapely
+Requires-Dist: pyproj
+
+# **cdsspy** <img src="img/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
+
+<!-- badges: start -->
+
+[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+<!-- badges: end -->
+
+<div align="left">
+
+<p align="left">
+<a href="https://dwr.state.co.us/Tools"><strong>« CDSS »</strong></a>
+<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
+Services</a>
+</p>
+
+</div>
+
+<hr>
+
+The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
+
+The Colorado’s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
+
+Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
+
+<br>
+
+> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
+
+---
+
+- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
+
+- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
+
+- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
+
+- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
+
+---
+
+<br> 
+
+## **Installation**
+Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
+
+``` 
+pip install cdsspy
+```
+<br>
+
+## **Available endpoints**
+
+Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
+|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
+|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
+|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
+|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
+|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
+|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
+|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+<br>
+
+## **Identify query inputs using reference tables**
+
+The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
+
+<br>
+
+```python
+# available parameters for telemetry stations
+telemetry_params = cdsspy.get_reference_tbl(
+    table_name = "telemetryparams"
+    )
+```
+
+|    | Parameter   |
+|---:|:------------|
+|  0 | AIRTEMP     |
+|  1 | BAR_P       |
+|  2 | BATTERY     |
+|  3 | COND        |
+|  4 | D1          |
+|  5 | D2          |
+|  6 | DISCHRG     |
+|  7 | DISCHRG1    |
+|  8 | DISCHRG2    |
+|  9 | DISCHRG3    |
+| 10 | DISCHRG4    |
+| 11 | ELEV        |
+
+<br>
+<br>
+<br>
+
+## **Locate structures**
+
+**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
+|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
+
+<br>
+
+### **Example: Locating telemetry stations by county:**
+
+```python
+# identify telemetry stations in Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    county = "Boulder"
+    )
+```
+
+![](img/county_telem_stations2.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations around a point**
+
+```python
+# identify telemetry stations within a 15 mile radius of the center point of Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = [-105.358164, 40.092608],
+    radius = 15
+    )
+```
+
+![](img/poi_telem_stations.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations within a spatial extent**
+A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
+
+```python
+# identify telemetry stations 15 miles around the centroid of a polygon
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = geopandas.read_file("example-data/boulder_county.gpkg")
+    radius = 15
+    )
+```
+
+This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
+
+![](img/boulder_telem_stations_poly2.gif)
+
+<br>
+<br>
+<br>
+<br>
+
+
+## **Retrieve time series data** 
+
+The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+
+#### **Example: Daily discharge at a telemetry station**
+We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
+
+<br>
+
+The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
+
+```python
+# Daily discharge at "ANDDITCO" telemetry station
+discharge_ts   = cdsspy.get_telemetry_ts(
+    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
+    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
+    start_date     = "2015-01-01",   # Starting date
+    end_date       = "2022-01-01",   # Ending date
+    timescale      = "day"           # select daily timescale
+    )
+```
+
+![](img/discharge_timeseries_plot2.png)
+
+<br>
+<br>
+
+#### **Example: Retrieve Diversion records for multiple structures**
+Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
+
+
+1. Executing a spatial search using **`get_structures()`** 
+2. Selecting the WDIDs of interest from the search results
+3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
+
+
+```python 
+# 1. Executing a spatial search
+structures = cdsspy.get_structures(
+    aoi    = [-105.3578, 40.09244],
+    radius = 5
+    )
+
+# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
+ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
+ditch_wdids = list(ditch_wdids['wdid'])
+
+# 3. Providing the WDID's as a list to get_structures_divrec_ts()
+diversion_rec  = cdsspy.get_structures_divrec_ts(
+    wdid           = ditch_wdids,
+    wc_identifier  = "diversion",
+    timescale      = "month"
+    )
+```
+**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
+
+![](img/divrec_facet_plot.png)
+
+<br>
+<br>
+<br>
+<br>
+
+## **Retrieve groundwater data**
+The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
+
+| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
+|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
+| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
+| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
+| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
+| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
+
+<br>
+
+Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
+
+```python
+# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
+well_measure = cdsspy.get_gw_wl_wellmeasures(
+    wellid     = "1274",
+    start_date = "1990-01-01",
+    end_date   = "2022-01-01"
+    )
+```
+
+![](img/gw_depth_to_water_plot2.png)
```

#### html2text {}

```diff
@@ -1,24 +1,25 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.70 Summary: Provides Python
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.71 Summary: Provides Python
 functions for discovering and requesting data from the CDSS REST API. Author:
 Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
 Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
-1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png][![Dependencies](https:
-//img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
-choosealicense.com/licenses/mit/)
-_?Ã_?_?Â_?«_ _CC_DD_SS_SS_ _?Ã_?_?Â_?»
+License-File: LICENSE Requires-Dist: pandas Requires-Dist: datetime Requires-
+Dist: requests Requires-Dist: geopandas Requires-Dist: shapely Requires-Dist:
+pyproj # **cdsspy** [img/co_dnr_div_cdss_cwcbdwr_transparent.png][!
+[Dependencies](https://img.shields.io/badge/dependencies-12/01-
+orange?style=flat)](#) [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+_?Â_?«_ _CC_DD_SS_SS_ _?Â_?»
 _C_D_S_S_ _R_E_S_T_ _W_e_b_ _S_e_r_v_i_c_e_s
 ===============================================================================
 The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide
 functions that help Python users to navigate, explore, and make requests to the
-CDSS REST API web service. The ColoradoÃ¢â¬â¢s Decision Support Systems
-(CDSS) is a water management system created and developed by the Colorado Water
+CDSS REST API web service. The Coloradoâs Decision Support Systems (CDSS) is
+a water management system created and developed by the Colorado Water
 Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
 Thank you to those at CWCB and DWR for providing an accessible and well
 documented REST API!
 > See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R**
 version of this package --- - [**cdssr (R)**](https://github.com/anguswg-ucsb/
 cdssr) - [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/) -
 [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy) - [**cdsspy
@@ -146,32 +147,29 @@
 help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml) | |6 |
 **get_telemetry_stations()** | Returns telemetry stations and their most recent
 parameter reading | [telemetrystations/telemetrystation](https://
 dwr.state.co.us/rest/get/
 help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml) |
 ### **Example: Locating telemetry stations by county:** ```python # identify
 telemetry stations in Boulder County stations = cdsspy.get_telemetry_stations
-( county = "Boulder" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/county_telem_stations2.png)
+( county = "Boulder" ) ``` ![](img/county_telem_stations2.png)
 
 ### **Example: Locating telemetry stations around a point** ```python #
 identify telemetry stations within a 15 mile radius of the center point of
 Boulder County stations = cdsspy.get_telemetry_stations( aoi = [-105.358164,
-40.092608], radius = 15 ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/poi_telem_stations.png)
+40.092608], radius = 15 ) ``` ![](img/poi_telem_stations.png)
 
 ### **Example: Locating telemetry stations within a spatial extent** A masking
 operation is performed when a location search is done using a **polygon**. This
 ensures that the function only returns points that are ***within*** the given
 polygon. ```python # identify telemetry stations 15 miles around the centroid
 of a polygon stations = cdsspy.get_telemetry_stations( aoi =
-geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/
-boulder_county.gpkg") radius = 15 ) ``` This gif highlights the masking process
-that happens when the **`aoi`** argument is given a **polygon** ![](https://
-cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
+geopandas.read_file("example-data/boulder_county.gpkg") radius = 15 ) ``` This
+gif highlights the masking process that happens when the **`aoi`** argument is
+given a **polygon** ![](img/boulder_telem_stations_poly2.gif)
 
 
 
 ## **Retrieve time series data** The functions in the table below retrieve time
 series data from the various time series related CDSS API endpoints. |**-**
 |**Function** | **Description** | **Endpoint** | |------|----------------------
 ----------| -------------------------------------------------------------------
@@ -205,16 +203,16 @@
 into the **`get_telemetry_ts()`** function.
 The function below returns a dataframe of daily discharge for the "ANDDITCO"
 site between 2015-2022. ```python # Daily discharge at "ANDDITCO" telemetry
 station discharge_ts = cdsspy.get_telemetry_ts( abbrev = "ANDDITCO", # Site
 abbreviation from the outputs of get_telemetry_stations() parameter =
 "DISCHRG", # Desired parameter, identified by the get_reference_tbl()
 start_date = "2015-01-01", # Starting date end_date = "2022-01-01", # Ending
-date timescale = "day" # select daily timescale ) ``` ![](https://cdsspy-
-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
+date timescale = "day" # select daily timescale ) ``` ![](img/
+discharge_timeseries_plot2.png)
 
 #### **Example: Retrieve Diversion records for multiple structures** Some of
 the CDSS API endpoints allow users to request data from multiple structures if
 you provide a list of IDs. If we want to get diversion data from multiple
 structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs
 within a given area by: 1. Executing a spatial search using **`get_structures
 ()`** 2. Selecting the WDIDs of interest from the search results 3. Providing
@@ -224,15 +222,15 @@
 search results and putting WDIDs into a list ditch_wdids = structures[
 (structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
 ditch_wdids = list(ditch_wdids['wdid']) # 3. Providing the WDID's as a list to
 get_structures_divrec_ts() diversion_rec = cdsspy.get_structures_divrec_ts
 ( wdid = ditch_wdids, wc_identifier = "diversion", timescale = "month" ) ```
 **Note:** Data availability can vary between structures (i.e. Missing data, not
 all structures have every data type/temporal resolution available, etc.) ![]
-(https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
+(img/divrec_facet_plot.png)
 
 
 
 ## **Retrieve groundwater data** The **`get_gw_()`** set of functions lets
 users retrieve data from the various groundwater related API endpoints shown in
 the table below: | **-** | **Function** | **Endpoint** | |-------|-------------
 --------------------|----------------------------------------------------------
@@ -247,9 +245,8 @@
 **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/
 geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-
 geophysicallogs-geoplogpicks) |
 Here we will retrieve groundwater well measurement data for Well ID 1274
 between 2021-2022. ```python # Request wellmeasurements endpoint (api/v2/
 groundwater/waterlevels/wellmeasurements) well_measure =
 cdsspy.get_gw_wl_wellmeasures( wellid = "1274", start_date = "1990-01-01",
-end_date = "2022-01-01" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/gw_depth_to_water_plot2.png)
+end_date = "2022-01-01" ) ``` ![](img/gw_depth_to_water_plot2.png)
```

### Comparing `cdsspy-1.2.70/README.md` & `cdsspy-1.2.71/cdsspy.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,278 +1,297 @@
-# **cdsspy** <img src="https://cdsspy-images.s3.us-west-1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
-
-<!-- badges: start -->
-
-[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-<!-- badges: end -->
-
-<div align="left">
-
-<p align="left">
-<a href="https://dwr.state.co.us/Tools"><strong>« CDSS »</strong></a>
-<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
-Services</a>
-</p>
-
-</div>
-
-<hr>
-
-The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
-
-The Colorado’s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
-
-Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
-
-<br>
-
-> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
-
----
-
-- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
-
-- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
-
-- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
-
-- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
-
----
-
-<br> 
-
-## **Installation**
-Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
-
-``` 
-pip install cdsspy
-```
-<br>
-
-## **Available endpoints**
-
-Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
-|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
-|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
-|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
-|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
-|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
-|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
-|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-<br>
-
-## **Identify query inputs using reference tables**
-
-The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
-
-<br>
-
-```python
-# available parameters for telemetry stations
-telemetry_params = cdsspy.get_reference_tbl(
-    table_name = "telemetryparams"
-    )
-```
-
-|    | Parameter   |
-|---:|:------------|
-|  0 | AIRTEMP     |
-|  1 | BAR_P       |
-|  2 | BATTERY     |
-|  3 | COND        |
-|  4 | D1          |
-|  5 | D2          |
-|  6 | DISCHRG     |
-|  7 | DISCHRG1    |
-|  8 | DISCHRG2    |
-|  9 | DISCHRG3    |
-| 10 | DISCHRG4    |
-| 11 | ELEV        |
-
-<br>
-<br>
-<br>
-
-## **Locate structures**
-
-**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
-|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
-
-<br>
-
-### **Example: Locating telemetry stations by county:**
-
-```python
-# identify telemetry stations in Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    county = "Boulder"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/county_telem_stations2.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations around a point**
-
-```python
-# identify telemetry stations within a 15 mile radius of the center point of Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = [-105.358164, 40.092608],
-    radius = 15
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/poi_telem_stations.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations within a spatial extent**
-A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
-
-```python
-# identify telemetry stations 15 miles around the centroid of a polygon
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_county.gpkg")
-    radius = 15
-    )
-```
-
-This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve time series data** 
-
-The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-
-#### **Example: Daily discharge at a telemetry station**
-We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
-
-<br>
-
-The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
-
-```python
-# Daily discharge at "ANDDITCO" telemetry station
-discharge_ts   = cdsspy.get_telemetry_ts(
-    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
-    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
-    start_date     = "2015-01-01",   # Starting date
-    end_date       = "2022-01-01",   # Ending date
-    timescale      = "day"           # select daily timescale
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
-
-<br>
-<br>
-
-#### **Example: Retrieve Diversion records for multiple structures**
-Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
-
-
-1. Executing a spatial search using **`get_structures()`** 
-2. Selecting the WDIDs of interest from the search results
-3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
-
-
-```python 
-# 1. Executing a spatial search
-structures = cdsspy.get_structures(
-    aoi    = [-105.3578, 40.09244],
-    radius = 5
-    )
-
-# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
-ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
-ditch_wdids = list(ditch_wdids['wdid'])
-
-# 3. Providing the WDID's as a list to get_structures_divrec_ts()
-diversion_rec  = cdsspy.get_structures_divrec_ts(
-    wdid           = ditch_wdids,
-    wc_identifier  = "diversion",
-    timescale      = "month"
-    )
-```
-**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve groundwater data**
-The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
-
-| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
-|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
-| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
-| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
-| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
-| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
-
-<br>
-
-Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
-
-```python
-# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
-well_measure = cdsspy.get_gw_wl_wellmeasures(
-    wellid     = "1274",
-    start_date = "1990-01-01",
-    end_date   = "2022-01-01"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/gw_depth_to_water_plot2.png)
+Metadata-Version: 2.1
+Name: cdsspy
+Version: 1.2.71
+Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
+Author: Angus Watters
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: pandas
+Requires-Dist: datetime
+Requires-Dist: requests
+Requires-Dist: geopandas
+Requires-Dist: shapely
+Requires-Dist: pyproj
+
+# **cdsspy** <img src="img/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
+
+<!-- badges: start -->
+
+[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+<!-- badges: end -->
+
+<div align="left">
+
+<p align="left">
+<a href="https://dwr.state.co.us/Tools"><strong>« CDSS »</strong></a>
+<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
+Services</a>
+</p>
+
+</div>
+
+<hr>
+
+The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
+
+The Colorado’s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
+
+Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
+
+<br>
+
+> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
+
+---
+
+- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
+
+- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
+
+- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
+
+- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
+
+---
+
+<br> 
+
+## **Installation**
+Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
+
+``` 
+pip install cdsspy
+```
+<br>
+
+## **Available endpoints**
+
+Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
+|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
+|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
+|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
+|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
+|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
+|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
+|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+<br>
+
+## **Identify query inputs using reference tables**
+
+The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
+
+<br>
+
+```python
+# available parameters for telemetry stations
+telemetry_params = cdsspy.get_reference_tbl(
+    table_name = "telemetryparams"
+    )
+```
+
+|    | Parameter   |
+|---:|:------------|
+|  0 | AIRTEMP     |
+|  1 | BAR_P       |
+|  2 | BATTERY     |
+|  3 | COND        |
+|  4 | D1          |
+|  5 | D2          |
+|  6 | DISCHRG     |
+|  7 | DISCHRG1    |
+|  8 | DISCHRG2    |
+|  9 | DISCHRG3    |
+| 10 | DISCHRG4    |
+| 11 | ELEV        |
+
+<br>
+<br>
+<br>
+
+## **Locate structures**
+
+**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
+|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
+
+<br>
+
+### **Example: Locating telemetry stations by county:**
+
+```python
+# identify telemetry stations in Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    county = "Boulder"
+    )
+```
+
+![](img/county_telem_stations2.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations around a point**
+
+```python
+# identify telemetry stations within a 15 mile radius of the center point of Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = [-105.358164, 40.092608],
+    radius = 15
+    )
+```
+
+![](img/poi_telem_stations.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations within a spatial extent**
+A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
+
+```python
+# identify telemetry stations 15 miles around the centroid of a polygon
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = geopandas.read_file("example-data/boulder_county.gpkg")
+    radius = 15
+    )
+```
+
+This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
+
+![](img/boulder_telem_stations_poly2.gif)
+
+<br>
+<br>
+<br>
+<br>
+
+
+## **Retrieve time series data** 
+
+The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+
+#### **Example: Daily discharge at a telemetry station**
+We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
+
+<br>
+
+The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
+
+```python
+# Daily discharge at "ANDDITCO" telemetry station
+discharge_ts   = cdsspy.get_telemetry_ts(
+    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
+    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
+    start_date     = "2015-01-01",   # Starting date
+    end_date       = "2022-01-01",   # Ending date
+    timescale      = "day"           # select daily timescale
+    )
+```
+
+![](img/discharge_timeseries_plot2.png)
+
+<br>
+<br>
+
+#### **Example: Retrieve Diversion records for multiple structures**
+Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
+
+
+1. Executing a spatial search using **`get_structures()`** 
+2. Selecting the WDIDs of interest from the search results
+3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
+
+
+```python 
+# 1. Executing a spatial search
+structures = cdsspy.get_structures(
+    aoi    = [-105.3578, 40.09244],
+    radius = 5
+    )
+
+# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
+ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
+ditch_wdids = list(ditch_wdids['wdid'])
+
+# 3. Providing the WDID's as a list to get_structures_divrec_ts()
+diversion_rec  = cdsspy.get_structures_divrec_ts(
+    wdid           = ditch_wdids,
+    wc_identifier  = "diversion",
+    timescale      = "month"
+    )
+```
+**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
+
+![](img/divrec_facet_plot.png)
+
+<br>
+<br>
+<br>
+<br>
+
+## **Retrieve groundwater data**
+The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
+
+| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
+|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
+| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
+| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
+| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
+| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
+
+<br>
+
+Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
+
+```python
+# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
+well_measure = cdsspy.get_gw_wl_wellmeasures(
+    wellid     = "1274",
+    start_date = "1990-01-01",
+    end_date   = "2022-01-01"
+    )
+```
+
+![](img/gw_depth_to_water_plot2.png)
```

#### html2text {}

```diff
@@ -1,12 +1,18 @@
-# **cdsspy** [https://cdsspy-images.s3.us-west-1.amazonaws.com/
-co_dnr_div_cdss_cwcbdwr_transparent.png][![Dependencies](https://
-img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [![License: MIT]
-(https://img.shields.io/badge/License-MIT-yellow.svg)](https://
-choosealicense.com/licenses/mit/)
+Metadata-Version: 2.1 Name: cdsspy Version: 1.2.71 Summary: Provides Python
+functions for discovering and requesting data from the CDSS REST API. Author:
+Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
+License :: OSI Approved :: MIT License Classifier: Operating System :: OS
+Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
+License-File: LICENSE Requires-Dist: pandas Requires-Dist: datetime Requires-
+Dist: requests Requires-Dist: geopandas Requires-Dist: shapely Requires-Dist:
+pyproj # **cdsspy** [img/co_dnr_div_cdss_cwcbdwr_transparent.png][!
+[Dependencies](https://img.shields.io/badge/dependencies-12/01-
+orange?style=flat)](#) [![License: MIT](https://img.shields.io/badge/License-
+MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
 _?Â_?«_ _CC_DD_SS_SS_ _?Â_?»
 _C_D_S_S_ _R_E_S_T_ _W_e_b_ _S_e_r_v_i_c_e_s
 ===============================================================================
 The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide
 functions that help Python users to navigate, explore, and make requests to the
 CDSS REST API web service. The Coloradoâs Decision Support Systems (CDSS) is
 a water management system created and developed by the Colorado Water
@@ -141,32 +147,29 @@
 help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml) | |6 |
 **get_telemetry_stations()** | Returns telemetry stations and their most recent
 parameter reading | [telemetrystations/telemetrystation](https://
 dwr.state.co.us/rest/get/
 help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml) |
 ### **Example: Locating telemetry stations by county:** ```python # identify
 telemetry stations in Boulder County stations = cdsspy.get_telemetry_stations
-( county = "Boulder" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/county_telem_stations2.png)
+( county = "Boulder" ) ``` ![](img/county_telem_stations2.png)
 
 ### **Example: Locating telemetry stations around a point** ```python #
 identify telemetry stations within a 15 mile radius of the center point of
 Boulder County stations = cdsspy.get_telemetry_stations( aoi = [-105.358164,
-40.092608], radius = 15 ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/poi_telem_stations.png)
+40.092608], radius = 15 ) ``` ![](img/poi_telem_stations.png)
 
 ### **Example: Locating telemetry stations within a spatial extent** A masking
 operation is performed when a location search is done using a **polygon**. This
 ensures that the function only returns points that are ***within*** the given
 polygon. ```python # identify telemetry stations 15 miles around the centroid
 of a polygon stations = cdsspy.get_telemetry_stations( aoi =
-geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/
-boulder_county.gpkg") radius = 15 ) ``` This gif highlights the masking process
-that happens when the **`aoi`** argument is given a **polygon** ![](https://
-cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
+geopandas.read_file("example-data/boulder_county.gpkg") radius = 15 ) ``` This
+gif highlights the masking process that happens when the **`aoi`** argument is
+given a **polygon** ![](img/boulder_telem_stations_poly2.gif)
 
 
 
 ## **Retrieve time series data** The functions in the table below retrieve time
 series data from the various time series related CDSS API endpoints. |**-**
 |**Function** | **Description** | **Endpoint** | |------|----------------------
 ----------| -------------------------------------------------------------------
@@ -200,16 +203,16 @@
 into the **`get_telemetry_ts()`** function.
 The function below returns a dataframe of daily discharge for the "ANDDITCO"
 site between 2015-2022. ```python # Daily discharge at "ANDDITCO" telemetry
 station discharge_ts = cdsspy.get_telemetry_ts( abbrev = "ANDDITCO", # Site
 abbreviation from the outputs of get_telemetry_stations() parameter =
 "DISCHRG", # Desired parameter, identified by the get_reference_tbl()
 start_date = "2015-01-01", # Starting date end_date = "2022-01-01", # Ending
-date timescale = "day" # select daily timescale ) ``` ![](https://cdsspy-
-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
+date timescale = "day" # select daily timescale ) ``` ![](img/
+discharge_timeseries_plot2.png)
 
 #### **Example: Retrieve Diversion records for multiple structures** Some of
 the CDSS API endpoints allow users to request data from multiple structures if
 you provide a list of IDs. If we want to get diversion data from multiple
 structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs
 within a given area by: 1. Executing a spatial search using **`get_structures
 ()`** 2. Selecting the WDIDs of interest from the search results 3. Providing
@@ -219,15 +222,15 @@
 search results and putting WDIDs into a list ditch_wdids = structures[
 (structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
 ditch_wdids = list(ditch_wdids['wdid']) # 3. Providing the WDID's as a list to
 get_structures_divrec_ts() diversion_rec = cdsspy.get_structures_divrec_ts
 ( wdid = ditch_wdids, wc_identifier = "diversion", timescale = "month" ) ```
 **Note:** Data availability can vary between structures (i.e. Missing data, not
 all structures have every data type/temporal resolution available, etc.) ![]
-(https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
+(img/divrec_facet_plot.png)
 
 
 
 ## **Retrieve groundwater data** The **`get_gw_()`** set of functions lets
 users retrieve data from the various groundwater related API endpoints shown in
 the table below: | **-** | **Function** | **Endpoint** | |-------|-------------
 --------------------|----------------------------------------------------------
@@ -242,9 +245,8 @@
 **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/
 geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-
 geophysicallogs-geoplogpicks) |
 Here we will retrieve groundwater well measurement data for Well ID 1274
 between 2021-2022. ```python # Request wellmeasurements endpoint (api/v2/
 groundwater/waterlevels/wellmeasurements) well_measure =
 cdsspy.get_gw_wl_wellmeasures( wellid = "1274", start_date = "1990-01-01",
-end_date = "2022-01-01" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/gw_depth_to_water_plot2.png)
+end_date = "2022-01-01" ) ``` ![](img/gw_depth_to_water_plot2.png)
```

### Comparing `cdsspy-1.2.70/cdsspy/admin_calls.py` & `cdsspy-1.2.71/cdsspy/admin_calls.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,135 +1,135 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_admin_calls(
-    division            = None,
-    location_wdid       = None,
-    call_number         = None,
-    start_date          = None,
-    end_date            = None,
-    active              = True,
-    api_key             = None
-    ):
-    """Return active/historic administrative calls data
-
-    Make a request to the api/v2/administrativecalls endpoints to locate active or historical administrative calls by division, location WDID, or call number within a specified date range.
-
-    Args:
-        division (int, str, optional): Water division to query for administrative calls. Defaults to None.
-        location_wdid (str, optional): call location structure WDID to query for administrative calls. Defaults to None.
-        call_number (int, str, optional): unique call identifier to query. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        active (bool, optional): whether to get active or historical administrative calls. Defaults to True which returns active administrative calls.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of active/historical administrative calls data
-    """
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date", "active"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # collapse location_wdid list, tuple, vector of site_id into query formatted string
-    location_wdid = utils._collapse_vector(
-        vect = location_wdid, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    #  base API URL and print statements
-    if active == True:
-        print("Retrieving active administrative calls data")
-        base = "https://dwr.state.co.us/Rest/GET/api/v2/administrativecalls/active/?"
-    else:
-        print("Retrieving historical administrative calls data")
-        base = "https://dwr.state.co.us/Rest/GET/api/v2/administrativecalls/historical/?"
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving surface water station data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-        
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-dateTimeSet={start_date or ""}' 
-            f'&max-dateTimeSet={end_date or ""}'
-            f'&division={division or ""}' 
-            f'&callNumber={call_number or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # Construct query URL w/ location WDID
-        if location_wdid is not None:
-            url = url + "&locationWdid=" + str(location_wdid)
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-        
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_admin_calls(
+    division            = None,
+    location_wdid       = None,
+    call_number         = None,
+    start_date          = None,
+    end_date            = None,
+    active              = True,
+    api_key             = None
+    ):
+    """Return active/historic administrative calls data
+
+    Make a request to the api/v2/administrativecalls endpoints to locate active or historical administrative calls by division, location WDID, or call number within a specified date range.
+
+    Args:
+        division (int, str, optional): Water division to query for administrative calls. Defaults to None.
+        location_wdid (str, optional): call location structure WDID to query for administrative calls. Defaults to None.
+        call_number (int, str, optional): unique call identifier to query. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        active (bool, optional): whether to get active or historical administrative calls. Defaults to True which returns active administrative calls.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of active/historical administrative calls data
+    """
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date", "active"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # collapse location_wdid list, tuple, vector of site_id into query formatted string
+    location_wdid = utils._collapse_vector(
+        vect = location_wdid, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    #  base API URL and print statements
+    if active == True:
+        print("Retrieving active administrative calls data")
+        base = "https://dwr.state.co.us/Rest/GET/api/v2/administrativecalls/active/?"
+    else:
+        print("Retrieving historical administrative calls data")
+        base = "https://dwr.state.co.us/Rest/GET/api/v2/administrativecalls/historical/?"
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving surface water station data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+        
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-dateTimeSet={start_date or ""}' 
+            f'&max-dateTimeSet={end_date or ""}'
+            f'&division={division or ""}' 
+            f'&callNumber={call_number or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # Construct query URL w/ location WDID
+        if location_wdid is not None:
+            url = url + "&locationWdid=" + str(location_wdid)
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+        
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy/analysis_services.py` & `cdsspy-1.2.71/cdsspy/analysis_services.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,892 +1,892 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_call_analysis_wdid(
-    wdid                = None,
-    admin_no            = None,
-    start_date          = None,
-    end_date            = None,
-    batch               = False,
-    api_key             = None
-    ):
-    """Return call analysis by WDID from analysis services API
-    
-    Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
-    
-    Args:
-        wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
-        admin_no (str, int optional): Water Right Administration Number. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        batch (bool, optional): Boolean, whether to break date range calls into batches of 1 year. This can speed up data retrieval for date ranges greater than a year. A date range of 5 years would be batched into 5 separate API calls for each year. Default is False, will run a single query for the entire date range.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-    Returns:
-        pandas dataframe object: dataframe of call services by WDID
-    """
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # convert int admin_no to str
-    if(isinstance(admin_no, (int))):
-        admin_no = str(admin_no)
-    
-    # if function should be run in batch mode
-    if(batch == True):
-
-        # final output dataframe to append query results to
-        out_df = pd.DataFrame()
-        
-        # make a list of date ranges to issue GET requests in smaller batches
-        date_lst = utils._batch_dates(
-            start_date = start_date,
-            end_date   = end_date
-            )
-        
-        # print message 
-        print("Retrieving call analysis data by WDID")
-
-        # go through range of dates in date_df and make batch GET requests
-        for idx, val in enumerate(date_lst):
-
-            print("Batch: ", idx+1, "/", len(date_lst))
-            
-            cdss_df = _inner_call_analysis_wdid(
-                wdid       = wdid,
-                admin_no   = admin_no,
-                start_date = val[0],
-                end_date   = val[1],
-                api_key    = api_key
-                )
-            
-            # bind data from this page
-            out_df = pd.concat([out_df, cdss_df])
-        
-        return out_df
-    
-    else:
-
-        # print message 
-        print("Retrieving call analysis data by WDID")
-
-        out_df = _inner_call_analysis_wdid(
-            wdid       = wdid,
-            admin_no   = admin_no,
-            start_date = start_date,
-            end_date   = end_date,
-            api_key    = api_key
-            )
-        
-        return out_df
-
-def _inner_call_analysis_wdid(
-    wdid                = None,
-    admin_no            = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return call analysis by WDID from analysis services API
-    
-    Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
-    
-    Args:
-        wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
-        admin_no (str, int optional): Water Right Administration Number. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of call services by WDID
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [wdid, admin_no]):
-    #     raise TypeError("Invalid 'wdid' and 'admin_no' parameters.\nPlease enter a 'wdid' and 'admin_no' to retrieve call analysis data")
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # convert int admin_no to str
-    if(isinstance(admin_no, (int))):
-        admin_no = str(admin_no)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
-    
-    # parse start_date into query string format
-    start = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-        )
-
-    # parse end_date into query string format
-    end = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&adminNo={admin_no or ""}'
-            f'&endDate={end or ""}'
-            f'&startDate={start or ""}'
-            f'&wdid={wdid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-        
-        # # make API call w/ error handling
-        # cdss_req = _get_error_handler(
-        #     url      = url
-        #     )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _inner_call_analysis_gnisid(
-    gnis_id             = None,
-    admin_no            = None,
-    stream_mile         = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return call analysis by GNIS ID from analysis services API
-    
-    Makes a request to the analysisservices/callanalysisbygnisid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified stream/stream mile and priority was out of priority and the downstream call in priority. 
-    This can be used when there is not an existing WDID to be analyzed.
-
-    Args:
-        gnis_id(str): GNIS ID to query. Defaults to None.
-        admin_no (str, int): Water Right Administration Number. Defaults to None.
-        stream_mile (str, int, float): stream mile for call analysis. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of call services by GNIS ID
-    """
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # convert int admin_no to str
-    if(isinstance(admin_no, (int))):
-        admin_no = str(admin_no)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbygnisid/?"
-    
-    # parse start_date into query string format
-    start = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-        )
-
-    # parse end_date into query string format
-    end = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&adminNo={admin_no or ""}'
-            f'&endDate={end or ""}'
-            f'&gnisId={gnis_id or ""}'
-            f'&startDate={start or ""}'
-            f'&streamMile={stream_mile or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-        
-        # # make API call w/ error handling
-        # cdss_req = _get_error_handler(
-        #     url      = url
-        #     )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def get_call_analysis_gnisid(
-    gnis_id             = None,
-    admin_no            = None,
-    stream_mile         = None,
-    start_date          = None,
-    end_date            = None,
-    batch               = False,
-    api_key             = None
-    ):
-    """Return call analysis by GNIS ID from analysis services API
-    
-    Makes a request to the analysisservices/callanalysisbygnisid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified stream/stream mile and priority was out of priority and the downstream call in priority. 
-    This can be used when there is not an existing WDID to be analyzed.
-
-    Args:
-        gnis_id(str): GNIS ID to query. Defaults to None.
-        admin_no (str, int): Water Right Administration Number. Defaults to None.
-        stream_mile (str, int, float): stream mile for call analysis. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        batch (bool, optional): Boolean, whether to break date range calls into batches of 1 year. This can speed up data retrieval for date ranges greater than a year. A date range of 5 years would be batched into 5 separate API calls for each year. Default is False, will run a single query for the entire date range.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-    Returns:
-        pandas dataframe object: dataframe of call services by GNIS ID
-    """
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # convert int admin_no to str
-    if(isinstance(admin_no, (int))):
-        admin_no = str(admin_no)
-    
-    # if function should be run in batch mode
-    if(batch == True):
-
-        # final output dataframe to append query results to
-        out_df = pd.DataFrame()
-        
-        # make a list of date ranges to issue GET requests in smaller batches
-        date_lst = utils._batch_dates(
-            start_date = start_date,
-            end_date   = end_date
-            )
-        
-        # print message 
-        print("Retrieving call analysis data by GNIS ID")
-
-        # go through range of dates in date_df and make batch GET requests
-        for idx, val in enumerate(date_lst):
-
-            print("Batch: ", idx+1, "/", len(date_lst))
-
-            cdss_df = _inner_call_analysis_gnisid(
-                gnis_id      = gnis_id,
-                admin_no     = admin_no,
-                stream_mile  = stream_mile,
-                start_date   = val[0],
-                end_date     = val[1],
-                api_key      = api_key
-                )
-            
-            # bind data from this page
-            out_df = pd.concat([out_df, cdss_df])
-        
-        return out_df
-    
-    else:
-
-        # print message 
-        print("Retrieving call analysis data by GNIS ID")
-
-        out_df = _inner_call_analysis_gnisid(
-            gnis_id      = gnis_id,
-            admin_no     = admin_no,
-            stream_mile  = stream_mile,
-            start_date   = start_date,
-            end_date     = end_date,
-            api_key      = api_key
-            )
-        
-        return out_df
-    
-
-def get_source_route_framework(
-    division            = None,
-    gnis_name           = None,
-    water_district      = None,
-    api_key             = None
-    ):
-    """Return call analysis by WDID from analysis services API
-
-    Makes a request to the analysisservices/watersourcerouteframework/ endpoint to retrieve the DWR source route framework reference table for the criteria specified.
-
-    Args:
-        division (int, str, optional):  Water division to query for water rights. Defaults to None.
-        gnis_name (str, optional): GNIS Name to query and retrieve DWR source route frameworks. Defaults to None.
-        water_district (str, optional): Water district to query for water rights. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of source route framework
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [division, gnis_name, water_district]):
-    #     raise TypeError("Invalid 'division', 'gnis_name' or 'water_district' parameters.\nPlease enter a 'division', 'gnis_name' or 'water_district' to retrieve  DWR source route framework data")
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/watersourcerouteframework/?"
-    
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving DWR source route frameworks")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&division={division or ""}'
-            f'&gnisName={gnis_name or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def get_source_route_analysis(
-    lt_gnis_id          = None,
-    lt_stream_mile      = None,
-    ut_gnis_id          = None,
-    ut_stream_mile      = None,
-    api_key             = None
-    ):
-    """Returns all WDID(s), and their stream mile, located between two different stream locations on the DWR Water Source Framework
-
-    Makes a request to the analysisservices/watersourcerouteanalysis/ endpoint to retrieve the DWR source route framework analysis data.
-    Args:
-        lt_gnis_id (str, int):  lower terminus GNIS ID. Defaults to None.
-        lt_stream_mile (str, int): lower terminus stream mile. Defaults to None.
-        ut_gnis_id (str, int):  upper terminus GNIS ID. Defaults to None.
-        ut_stream_mile (str, int): upper terminus stream mile. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of water source route framework analysis
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/watersourcerouteanalysis/?"
-    
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving DWR source route analysis")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&ltGnisId={lt_gnis_id or ""}'
-            f'&ltStreamMile={lt_stream_mile or ""}'
-            f'&utGnisId={ut_gnis_id or ""}'
-            f'&utStreamMile={ut_stream_mile or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-# def get_call_analysis_wdid(
-#     wdid                = None,
-#     admin_no            = None,
-#     start_date          = None,
-#     end_date            = None,
-#     api_key             = None
-#     ):
-#     """Return call analysis by WDID from analysis services API
-    
-#     Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
-    
-#     Args:
-#         wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
-#         admin_no (str, int optional): Water Right Administration Number. Defaults to None.
-#         start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-#         end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-#         api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-#     Returns:
-#         pandas dataframe object: dataframe of call services by WDID
-#     """
-    
-#     # list of function inputs
-#     input_args = locals()
-
-#     # check function arguments for missing/invalid inputs
-#     arg_lst = utils._check_args(
-#         arg_dict = input_args,
-#         ignore   = ["api_key", "start_date", "end_date"],
-#         f        = any
-#         )
-    
-#     # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-#     if arg_lst is not None:
-#         raise Exception(arg_lst)
-    
-#     # convert int admin_no to str
-#     if(isinstance(admin_no, (int))):
-#         admin_no = str(admin_no)
-
-#     #  base API URL
-#     base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
-
-#     # make a list of date ranges to issue GET requests in smaller batches
-#     date_lst = utils._batch_dates(
-#         start_date = start_date,
-#         end_date   = end_date
-#         )
-
-#     # final output dataframe to append query results to
-#     out_df = pd.DataFrame()
-
-#     # print message 
-#     print("Retrieving call analysis data by WDID")
-
-#     # go through range of dates in date_df and make batch GET requests
-#     for idx, val in enumerate(date_lst):
-
-#         print("index: ", idx, " | value: ", val)
-#         # print("START: ", val[0], " | END: ", val[1])
-
-#         # parse start_date into query string format
-#         start = utils._parse_date(
-#             date   = val[0],
-#             start  = True,
-#             format = "%m-%d-%Y"
-#             )
-
-#         # parse end_date into query string format
-#         end = utils._parse_date(
-#             date   = val[1],
-#             start  = False,
-#             format = "%m-%d-%Y"
-#             )
-
-#         # maximum records per page
-#         page_size = 50000
-
-#         # initialize empty dataframe to store data from multiple pages
-#         data_df = pd.DataFrame()
-
-#         # initialize first page index
-#         page_index = 1
-
-#         # Loop through pages until there are no more pages to get
-#         more_pages = True
-
-#         # Loop through pages until last page of data is found, binding each response dataframe together
-#         while more_pages == True:
-
-#             # create query URL string
-#             url = (
-#                 f'{base}format=json&dateFormat=spaceSepToSeconds'
-#                 f'&adminNo={admin_no or ""}'
-#                 f'&endDate={end or ""}'
-#                 f'&startDate={start or ""}'
-#                 f'&wdid={wdid or ""}'
-#                 f'&pageSize={page_size}&pageIndex={page_index}'
-#                 )
-
-#             # If an API key is provided, add it to query URL
-#             if api_key is not None:
-#                 # Construct query URL w/ API key
-#                 url = url + "&apiKey=" + str(api_key)
-
-#             # make API call w/ error handling
-#             cdss_req = utils._parse_gets(
-#                 url      = url, 
-#                 arg_dict = input_args,
-#                 ignore   = None
-#                 )
-            
-#             # # make API call w/ error handling
-#             # cdss_req = _get_error_handler(
-#             #     url      = url
-#             #     )
-
-#             # extract dataframe from list column
-#             cdss_df = cdss_req.json()
-#             cdss_df = pd.DataFrame(cdss_df)
-#             cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-#             # bind data from this page
-#             data_df = pd.concat([data_df, cdss_df])
-
-#             # Check if more pages to get to continue/stop while loop
-#             if len(cdss_df.index) < page_size:
-#                 more_pages = False
-#             else:
-#                 page_index += 1
-
-#         # bind data from this page
-#         out_df = pd.concat([out_df, data_df])
-
-#     return out_df
-
-
-# def get_call_analysis_wdid(
-#     wdid                = None,
-#     admin_no            = None,
-#     start_date          = None,
-#     end_date            = None,
-#     api_key             = None
-#     ):
-#     """Return call analysis by WDID from analysis services API
-    
-#     Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
-    
-#     Args:
-#         wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
-#         admin_no (str, int optional): Water Right Administration Number. Defaults to None.
-#         start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-#         end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-#         api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-#     Returns:
-#         pandas dataframe object: dataframe of call services by WDID
-#     """
-    
-#     # list of function inputs
-#     input_args = locals()
-
-#     # check function arguments for missing/invalid inputs
-#     arg_lst = utils._check_args(
-#         arg_dict = input_args,
-#         ignore   = ["api_key", "start_date", "end_date"],
-#         f        = any
-#         )
-    
-#     # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-#     if arg_lst is not None:
-#         raise Exception(arg_lst)
-    
-#     # convert int admin_no to str
-#     if(isinstance(admin_no, (int))):
-#         admin_no = str(admin_no)
-
-#     #  base API URL
-#     base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
-
-#     # make a list of date ranges to issue GET requests in smaller batches
-#     date_lst = utils._batch_dates(
-#         start_date = start_date,
-#         end_date   = end_date
-#         )
-
-#     # final output dataframe to append query results to
-#     out_df = pd.DataFrame()
-
-#     # print message 
-#     print("Retrieving call analysis data by WDID")
-
-#     # go through range of dates in date_df and make batch GET requests
-#     for idx, val in enumerate(date_lst):
-
-#         print("index: ", idx, " | value: ", val)
-#         # print("START: ", val[0], " | END: ", val[1])
-
-#         # parse start_date into query string format
-#         start = utils._parse_date(
-#             date   = val[0],
-#             start  = True,
-#             format = "%m-%d-%Y"
-#             )
-
-#         # parse end_date into query string format
-#         end = utils._parse_date(
-#             date   = val[1],
-#             start  = False,
-#             format = "%m-%d-%Y"
-#             )
-
-#         # maximum records per page
-#         page_size = 50000
-
-#         # initialize empty dataframe to store data from multiple pages
-#         data_df = pd.DataFrame()
-
-#         # initialize first page index
-#         page_index = 1
-
-#         # Loop through pages until there are no more pages to get
-#         more_pages = True
-
-#         # Loop through pages until last page of data is found, binding each response dataframe together
-#         while more_pages == True:
-
-#             # create query URL string
-#             url = (
-#                 f'{base}format=json&dateFormat=spaceSepToSeconds'
-#                 f'&adminNo={admin_no or ""}'
-#                 f'&endDate={end or ""}'
-#                 f'&startDate={start or ""}'
-#                 f'&wdid={wdid or ""}'
-#                 f'&pageSize={page_size}&pageIndex={page_index}'
-#                 )
-
-#             # If an API key is provided, add it to query URL
-#             if api_key is not None:
-#                 # Construct query URL w/ API key
-#                 url = url + "&apiKey=" + str(api_key)
-
-#             # make API call w/ error handling
-#             cdss_req = utils._parse_gets(
-#                 url      = url, 
-#                 arg_dict = input_args,
-#                 ignore   = None
-#                 )
-            
-#             # # make API call w/ error handling
-#             # cdss_req = _get_error_handler(
-#             #     url      = url
-#             #     )
-
-#             # extract dataframe from list column
-#             cdss_df = cdss_req.json()
-#             cdss_df = pd.DataFrame(cdss_df)
-#             cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-#             # bind data from this page
-#             data_df = pd.concat([data_df, cdss_df])
-
-#             # Check if more pages to get to continue/stop while loop
-#             if len(cdss_df.index) < page_size:
-#                 more_pages = False
-#             else:
-#                 page_index += 1
-
-#         # bind data from this page
-#         out_df = pd.concat([out_df, data_df])
-
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_call_analysis_wdid(
+    wdid                = None,
+    admin_no            = None,
+    start_date          = None,
+    end_date            = None,
+    batch               = False,
+    api_key             = None
+    ):
+    """Return call analysis by WDID from analysis services API
+    
+    Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
+    
+    Args:
+        wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
+        admin_no (str, int optional): Water Right Administration Number. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        batch (bool, optional): Boolean, whether to break date range calls into batches of 1 year. This can speed up data retrieval for date ranges greater than a year. A date range of 5 years would be batched into 5 separate API calls for each year. Default is False, will run a single query for the entire date range.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+    Returns:
+        pandas dataframe object: dataframe of call services by WDID
+    """
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # convert int admin_no to str
+    if(isinstance(admin_no, (int))):
+        admin_no = str(admin_no)
+    
+    # if function should be run in batch mode
+    if(batch == True):
+
+        # final output dataframe to append query results to
+        out_df = pd.DataFrame()
+        
+        # make a list of date ranges to issue GET requests in smaller batches
+        date_lst = utils._batch_dates(
+            start_date = start_date,
+            end_date   = end_date
+            )
+        
+        # print message 
+        print("Retrieving call analysis data by WDID")
+
+        # go through range of dates in date_df and make batch GET requests
+        for idx, val in enumerate(date_lst):
+
+            print("Batch: ", idx+1, "/", len(date_lst))
+            
+            cdss_df = _inner_call_analysis_wdid(
+                wdid       = wdid,
+                admin_no   = admin_no,
+                start_date = val[0],
+                end_date   = val[1],
+                api_key    = api_key
+                )
+            
+            # bind data from this page
+            out_df = pd.concat([out_df, cdss_df])
+        
+        return out_df
+    
+    else:
+
+        # print message 
+        print("Retrieving call analysis data by WDID")
+
+        out_df = _inner_call_analysis_wdid(
+            wdid       = wdid,
+            admin_no   = admin_no,
+            start_date = start_date,
+            end_date   = end_date,
+            api_key    = api_key
+            )
+        
+        return out_df
+
+def _inner_call_analysis_wdid(
+    wdid                = None,
+    admin_no            = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return call analysis by WDID from analysis services API
+    
+    Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
+    
+    Args:
+        wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
+        admin_no (str, int optional): Water Right Administration Number. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of call services by WDID
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [wdid, admin_no]):
+    #     raise TypeError("Invalid 'wdid' and 'admin_no' parameters.\nPlease enter a 'wdid' and 'admin_no' to retrieve call analysis data")
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # convert int admin_no to str
+    if(isinstance(admin_no, (int))):
+        admin_no = str(admin_no)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
+    
+    # parse start_date into query string format
+    start = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+        )
+
+    # parse end_date into query string format
+    end = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&adminNo={admin_no or ""}'
+            f'&endDate={end or ""}'
+            f'&startDate={start or ""}'
+            f'&wdid={wdid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+        
+        # # make API call w/ error handling
+        # cdss_req = _get_error_handler(
+        #     url      = url
+        #     )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _inner_call_analysis_gnisid(
+    gnis_id             = None,
+    admin_no            = None,
+    stream_mile         = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return call analysis by GNIS ID from analysis services API
+    
+    Makes a request to the analysisservices/callanalysisbygnisid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified stream/stream mile and priority was out of priority and the downstream call in priority. 
+    This can be used when there is not an existing WDID to be analyzed.
+
+    Args:
+        gnis_id(str): GNIS ID to query. Defaults to None.
+        admin_no (str, int): Water Right Administration Number. Defaults to None.
+        stream_mile (str, int, float): stream mile for call analysis. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of call services by GNIS ID
+    """
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # convert int admin_no to str
+    if(isinstance(admin_no, (int))):
+        admin_no = str(admin_no)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbygnisid/?"
+    
+    # parse start_date into query string format
+    start = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+        )
+
+    # parse end_date into query string format
+    end = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&adminNo={admin_no or ""}'
+            f'&endDate={end or ""}'
+            f'&gnisId={gnis_id or ""}'
+            f'&startDate={start or ""}'
+            f'&streamMile={stream_mile or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+        
+        # # make API call w/ error handling
+        # cdss_req = _get_error_handler(
+        #     url      = url
+        #     )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def get_call_analysis_gnisid(
+    gnis_id             = None,
+    admin_no            = None,
+    stream_mile         = None,
+    start_date          = None,
+    end_date            = None,
+    batch               = False,
+    api_key             = None
+    ):
+    """Return call analysis by GNIS ID from analysis services API
+    
+    Makes a request to the analysisservices/callanalysisbygnisid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified stream/stream mile and priority was out of priority and the downstream call in priority. 
+    This can be used when there is not an existing WDID to be analyzed.
+
+    Args:
+        gnis_id(str): GNIS ID to query. Defaults to None.
+        admin_no (str, int): Water Right Administration Number. Defaults to None.
+        stream_mile (str, int, float): stream mile for call analysis. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        batch (bool, optional): Boolean, whether to break date range calls into batches of 1 year. This can speed up data retrieval for date ranges greater than a year. A date range of 5 years would be batched into 5 separate API calls for each year. Default is False, will run a single query for the entire date range.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+    Returns:
+        pandas dataframe object: dataframe of call services by GNIS ID
+    """
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # convert int admin_no to str
+    if(isinstance(admin_no, (int))):
+        admin_no = str(admin_no)
+    
+    # if function should be run in batch mode
+    if(batch == True):
+
+        # final output dataframe to append query results to
+        out_df = pd.DataFrame()
+        
+        # make a list of date ranges to issue GET requests in smaller batches
+        date_lst = utils._batch_dates(
+            start_date = start_date,
+            end_date   = end_date
+            )
+        
+        # print message 
+        print("Retrieving call analysis data by GNIS ID")
+
+        # go through range of dates in date_df and make batch GET requests
+        for idx, val in enumerate(date_lst):
+
+            print("Batch: ", idx+1, "/", len(date_lst))
+
+            cdss_df = _inner_call_analysis_gnisid(
+                gnis_id      = gnis_id,
+                admin_no     = admin_no,
+                stream_mile  = stream_mile,
+                start_date   = val[0],
+                end_date     = val[1],
+                api_key      = api_key
+                )
+            
+            # bind data from this page
+            out_df = pd.concat([out_df, cdss_df])
+        
+        return out_df
+    
+    else:
+
+        # print message 
+        print("Retrieving call analysis data by GNIS ID")
+
+        out_df = _inner_call_analysis_gnisid(
+            gnis_id      = gnis_id,
+            admin_no     = admin_no,
+            stream_mile  = stream_mile,
+            start_date   = start_date,
+            end_date     = end_date,
+            api_key      = api_key
+            )
+        
+        return out_df
+    
+
+def get_source_route_framework(
+    division            = None,
+    gnis_name           = None,
+    water_district      = None,
+    api_key             = None
+    ):
+    """Return call analysis by WDID from analysis services API
+
+    Makes a request to the analysisservices/watersourcerouteframework/ endpoint to retrieve the DWR source route framework reference table for the criteria specified.
+
+    Args:
+        division (int, str, optional):  Water division to query for water rights. Defaults to None.
+        gnis_name (str, optional): GNIS Name to query and retrieve DWR source route frameworks. Defaults to None.
+        water_district (str, optional): Water district to query for water rights. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of source route framework
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [division, gnis_name, water_district]):
+    #     raise TypeError("Invalid 'division', 'gnis_name' or 'water_district' parameters.\nPlease enter a 'division', 'gnis_name' or 'water_district' to retrieve  DWR source route framework data")
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/watersourcerouteframework/?"
+    
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving DWR source route frameworks")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&division={division or ""}'
+            f'&gnisName={gnis_name or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def get_source_route_analysis(
+    lt_gnis_id          = None,
+    lt_stream_mile      = None,
+    ut_gnis_id          = None,
+    ut_stream_mile      = None,
+    api_key             = None
+    ):
+    """Returns all WDID(s), and their stream mile, located between two different stream locations on the DWR Water Source Framework
+
+    Makes a request to the analysisservices/watersourcerouteanalysis/ endpoint to retrieve the DWR source route framework analysis data.
+    Args:
+        lt_gnis_id (str, int):  lower terminus GNIS ID. Defaults to None.
+        lt_stream_mile (str, int): lower terminus stream mile. Defaults to None.
+        ut_gnis_id (str, int):  upper terminus GNIS ID. Defaults to None.
+        ut_stream_mile (str, int): upper terminus stream mile. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of water source route framework analysis
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/watersourcerouteanalysis/?"
+    
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving DWR source route analysis")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&ltGnisId={lt_gnis_id or ""}'
+            f'&ltStreamMile={lt_stream_mile or ""}'
+            f'&utGnisId={ut_gnis_id or ""}'
+            f'&utStreamMile={ut_stream_mile or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+# def get_call_analysis_wdid(
+#     wdid                = None,
+#     admin_no            = None,
+#     start_date          = None,
+#     end_date            = None,
+#     api_key             = None
+#     ):
+#     """Return call analysis by WDID from analysis services API
+    
+#     Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
+    
+#     Args:
+#         wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
+#         admin_no (str, int optional): Water Right Administration Number. Defaults to None.
+#         start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+#         end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+#         api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+#     Returns:
+#         pandas dataframe object: dataframe of call services by WDID
+#     """
+    
+#     # list of function inputs
+#     input_args = locals()
+
+#     # check function arguments for missing/invalid inputs
+#     arg_lst = utils._check_args(
+#         arg_dict = input_args,
+#         ignore   = ["api_key", "start_date", "end_date"],
+#         f        = any
+#         )
+    
+#     # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+#     if arg_lst is not None:
+#         raise Exception(arg_lst)
+    
+#     # convert int admin_no to str
+#     if(isinstance(admin_no, (int))):
+#         admin_no = str(admin_no)
+
+#     #  base API URL
+#     base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
+
+#     # make a list of date ranges to issue GET requests in smaller batches
+#     date_lst = utils._batch_dates(
+#         start_date = start_date,
+#         end_date   = end_date
+#         )
+
+#     # final output dataframe to append query results to
+#     out_df = pd.DataFrame()
+
+#     # print message 
+#     print("Retrieving call analysis data by WDID")
+
+#     # go through range of dates in date_df and make batch GET requests
+#     for idx, val in enumerate(date_lst):
+
+#         print("index: ", idx, " | value: ", val)
+#         # print("START: ", val[0], " | END: ", val[1])
+
+#         # parse start_date into query string format
+#         start = utils._parse_date(
+#             date   = val[0],
+#             start  = True,
+#             format = "%m-%d-%Y"
+#             )
+
+#         # parse end_date into query string format
+#         end = utils._parse_date(
+#             date   = val[1],
+#             start  = False,
+#             format = "%m-%d-%Y"
+#             )
+
+#         # maximum records per page
+#         page_size = 50000
+
+#         # initialize empty dataframe to store data from multiple pages
+#         data_df = pd.DataFrame()
+
+#         # initialize first page index
+#         page_index = 1
+
+#         # Loop through pages until there are no more pages to get
+#         more_pages = True
+
+#         # Loop through pages until last page of data is found, binding each response dataframe together
+#         while more_pages == True:
+
+#             # create query URL string
+#             url = (
+#                 f'{base}format=json&dateFormat=spaceSepToSeconds'
+#                 f'&adminNo={admin_no or ""}'
+#                 f'&endDate={end or ""}'
+#                 f'&startDate={start or ""}'
+#                 f'&wdid={wdid or ""}'
+#                 f'&pageSize={page_size}&pageIndex={page_index}'
+#                 )
+
+#             # If an API key is provided, add it to query URL
+#             if api_key is not None:
+#                 # Construct query URL w/ API key
+#                 url = url + "&apiKey=" + str(api_key)
+
+#             # make API call w/ error handling
+#             cdss_req = utils._parse_gets(
+#                 url      = url, 
+#                 arg_dict = input_args,
+#                 ignore   = None
+#                 )
+            
+#             # # make API call w/ error handling
+#             # cdss_req = _get_error_handler(
+#             #     url      = url
+#             #     )
+
+#             # extract dataframe from list column
+#             cdss_df = cdss_req.json()
+#             cdss_df = pd.DataFrame(cdss_df)
+#             cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+#             # bind data from this page
+#             data_df = pd.concat([data_df, cdss_df])
+
+#             # Check if more pages to get to continue/stop while loop
+#             if len(cdss_df.index) < page_size:
+#                 more_pages = False
+#             else:
+#                 page_index += 1
+
+#         # bind data from this page
+#         out_df = pd.concat([out_df, data_df])
+
+#     return out_df
+
+
+# def get_call_analysis_wdid(
+#     wdid                = None,
+#     admin_no            = None,
+#     start_date          = None,
+#     end_date            = None,
+#     api_key             = None
+#     ):
+#     """Return call analysis by WDID from analysis services API
+    
+#     Makes a request to the analysisservices/callanalysisbywdid/ endpoint that performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority.
+    
+#     Args:
+#         wdid (str, optional): DWR WDID unique structure identifier code. Defaults to None.
+#         admin_no (str, int optional): Water Right Administration Number. Defaults to None.
+#         start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+#         end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+#         api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+#     Returns:
+#         pandas dataframe object: dataframe of call services by WDID
+#     """
+    
+#     # list of function inputs
+#     input_args = locals()
+
+#     # check function arguments for missing/invalid inputs
+#     arg_lst = utils._check_args(
+#         arg_dict = input_args,
+#         ignore   = ["api_key", "start_date", "end_date"],
+#         f        = any
+#         )
+    
+#     # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+#     if arg_lst is not None:
+#         raise Exception(arg_lst)
+    
+#     # convert int admin_no to str
+#     if(isinstance(admin_no, (int))):
+#         admin_no = str(admin_no)
+
+#     #  base API URL
+#     base = "https://dwr.state.co.us/Rest/GET/api/v2/analysisservices/callanalysisbywdid/?"
+
+#     # make a list of date ranges to issue GET requests in smaller batches
+#     date_lst = utils._batch_dates(
+#         start_date = start_date,
+#         end_date   = end_date
+#         )
+
+#     # final output dataframe to append query results to
+#     out_df = pd.DataFrame()
+
+#     # print message 
+#     print("Retrieving call analysis data by WDID")
+
+#     # go through range of dates in date_df and make batch GET requests
+#     for idx, val in enumerate(date_lst):
+
+#         print("index: ", idx, " | value: ", val)
+#         # print("START: ", val[0], " | END: ", val[1])
+
+#         # parse start_date into query string format
+#         start = utils._parse_date(
+#             date   = val[0],
+#             start  = True,
+#             format = "%m-%d-%Y"
+#             )
+
+#         # parse end_date into query string format
+#         end = utils._parse_date(
+#             date   = val[1],
+#             start  = False,
+#             format = "%m-%d-%Y"
+#             )
+
+#         # maximum records per page
+#         page_size = 50000
+
+#         # initialize empty dataframe to store data from multiple pages
+#         data_df = pd.DataFrame()
+
+#         # initialize first page index
+#         page_index = 1
+
+#         # Loop through pages until there are no more pages to get
+#         more_pages = True
+
+#         # Loop through pages until last page of data is found, binding each response dataframe together
+#         while more_pages == True:
+
+#             # create query URL string
+#             url = (
+#                 f'{base}format=json&dateFormat=spaceSepToSeconds'
+#                 f'&adminNo={admin_no or ""}'
+#                 f'&endDate={end or ""}'
+#                 f'&startDate={start or ""}'
+#                 f'&wdid={wdid or ""}'
+#                 f'&pageSize={page_size}&pageIndex={page_index}'
+#                 )
+
+#             # If an API key is provided, add it to query URL
+#             if api_key is not None:
+#                 # Construct query URL w/ API key
+#                 url = url + "&apiKey=" + str(api_key)
+
+#             # make API call w/ error handling
+#             cdss_req = utils._parse_gets(
+#                 url      = url, 
+#                 arg_dict = input_args,
+#                 ignore   = None
+#                 )
+            
+#             # # make API call w/ error handling
+#             # cdss_req = _get_error_handler(
+#             #     url      = url
+#             #     )
+
+#             # extract dataframe from list column
+#             cdss_df = cdss_req.json()
+#             cdss_df = pd.DataFrame(cdss_df)
+#             cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+#             # bind data from this page
+#             data_df = pd.concat([data_df, cdss_df])
+
+#             # Check if more pages to get to continue/stop while loop
+#             if len(cdss_df.index) < page_size:
+#                 more_pages = False
+#             else:
+#                 page_index += 1
+
+#         # bind data from this page
+#         out_df = pd.concat([out_df, data_df])
+
 #     return out_df
```

### Comparing `cdsspy-1.2.70/cdsspy/climate.py` & `cdsspy-1.2.71/cdsspy/climate.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,593 +1,593 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-# from .utils import shared_function
-from cdsspy import utils
-
-def get_climate_stations(
-    aoi                 = None,
-    radius              = None,
-    county              = None,
-    division            = None,
-    station_name        = None,
-    site_id             = None,
-    water_district      = None,
-    api_key             = None
-    ):
-    """Return Climate Station information
-
-    Make a request to the climatedata/climatestations/ endpoint to locate climate stations via a spatial search, or by county, division, station name, Site ID or water district.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        county (str, optional): County to query for climate stations. Defaults to None.
-        division (int, str, optional):  Water division to query for climate stations. Defaults to None.
-        station_name (str, optional):  climate station name. Defaults to None.
-        site_id (str, tuple, list, optional): string, tuple or list of site IDs. Defaults to None.
-        water_district (int, str, optional): Water district to query for climate stations. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of climate station data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # collapse site_id list, tuple, vector of site_id into query formatted string
-    site_id = utils._collapse_vector(
-        vect = site_id, 
-        sep  = "%2C+"
-        )
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestations/?"
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving climate station data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}' 
-            f'&division={division or ""}'
-            f'&stationName={station_name or ""}' 
-            f'&siteId={site_id or ""}'
-            f'&waterDistrict={water_district or ""}' 
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-
-    return data_df
-
-def get_climate_frostdates(
-    station_number      = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return climate stations frost dates 
-
-    Make a request to the /climatedata/climatestationfrostdates endpoint to retrieve climate stations frost dates data by station number within a given date range (start and end dates)
-
-    Args:
-        station_number (str, optional): climate data station number. Defaults to None.
-        start_date (str, optional): date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of climate station frost dates data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationfrostdates/?"
-    
-    # parse start_date into query string format
-    start_year = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%Y"
-    )
-
-    # parse end_date into query string format
-    end_year = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving climate station frost dates data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-calYear={start_year or ""}' 
-            f'&max-calYear={end_year or ""}'
-            f'&stationNum={station_number or ""}' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-
-def _get_climate_ts_day(
-    station_number      = None,
-    site_id             = None,
-    param               = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return daily climate data
-    
-    Make a request to the /climatedata/climatestationtsday endpoint to retrieve climate stations daily time series data by station number, or Site IDs within a given date range (start and end dates)
-    
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        site_id (str, tuple, list, optional): string, tuple or list of climate station site IDs. Defaults to None.
-        param (str):  climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of climate station daily time series data
-    """
-
-    # list of valid parameters
-    param_lst = ["Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow","SnowDepth", "SnowSWE", "Solar","VP", "Wind"]
-
-    # if parameter is not in list of valid parameters
-    if param not in param_lst:
-        raise ValueError("Invalid `param` argument \nPlease enter one of the following valid parameters: \nEvap, FrostDate, MaxTemp, MeanTemp, MinTemp, Precip, Snow, SnowDepth, SnowSWE, Solar, VP, Wind")
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [site_id, station_number]):
-    #     raise TypeError("Invalid 'site_id' or 'station_number' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_dict)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationtsday/?"
-
-    # collapse list, tuple, vector of site_id into query formatted string
-    site_id = utils._collapse_vector(
-        vect = site_id, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print(f"Retrieving daily climate time series data ({param})")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-measDate={start_date or ""}' 
-            f'&max-measDate={end_date or ""}'
-            f'&stationNum={station_number or ""}' 
-            f'&siteId={site_id or ""}'
-            f'&measType={param or ""}' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # convert measDate columns to 'date' and pd datetime type
-        cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def _get_climate_ts_month(
-    station_number      = None,
-    site_id             = None,
-    param               = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return monthly climate data
-    
-    Make a request to the /climatedata/climatestationtsmonth endpoint to retrieve climate stations monthly time series data by station number, or Site IDs within a given date range (start and end dates)
-    
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        site_id (str, optional):  tuple or list of climate station site IDs. Defaults to None.
-        param (str, optional):  climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of climate station monthly time series data
-    """
-    # list of valid parameters
-    param_lst = ["Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow","SnowDepth", "SnowSWE", "Solar","VP", "Wind"]
-
-    # if parameter is not in list of valid parameters
-    if param not in param_lst:
-        raise ValueError("Invalid `param` argument \nPlease enter one of the following valid parameters: \nEvap, FrostDate, MaxTemp, MeanTemp, MinTemp, Precip, Snow, SnowDepth, SnowSWE, Solar, VP, Wind")
-    
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationtsmonth/?"
-
-    # collapse list, tuple, vector of site_id into query formatted string
-    site_id = utils._collapse_vector(
-        vect = site_id, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%Y"
-        )
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print(f"Retrieving monthly climate time series data ({param})")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-calYear={start_date or ""}'
-            f'&max-calYear={end_date or ""}'
-            f'&stationNum={station_number or ""}' 
-            f'&siteId={site_id or ""}' 
-            f'&measType={param or ""}' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # convert string month to have leading 0 if month < 10
-        cdss_df['month_str'] = cdss_df["calMonthNum"]
-
-        # add month w/ leading 0 column
-        cdss_df.loc[(cdss_df['calMonthNum'] < 10), 'month_str'] = "0" + cdss_df["calMonthNum"].astype(str)
-
-        # create datetime column w/ calYear and month_str columns, and convert to pd datetime type
-        cdss_df["datetime"] = pd.to_datetime(cdss_df['calYear'].astype(str) + "-" + cdss_df["month_str"].astype(str) + "-01")
-    
-        # drop month_str column
-        cdss_df = cdss_df.drop('month_str', axis = 1)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def get_climate_ts(
-    station_number      = None,
-    site_id             = None,
-    param               = None,
-    start_date          = None,
-    end_date            = None,
-    timescale           = None,
-    api_key             = None
-    ):
-
-    """Return climate station time series data
-
-    Make a request to the /climatedata/climatestationts endpoints to retrieve daily or monthly (climatestationtsday or climatestationtsmonth)climate station time series data by station number or Site IDs within a given date range (start and end dates)
-    
-    Args:
-        station_number (str, optional): climate data station number. Defaults to None.
-        site_id (str, optional): string, tuple or list of climate station site IDs. Defaults to None.
-        param (str, optional): climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        timescale (str, optional): timestep of the time series data to return, either "day" or "month". Defaults to None and will request daily time series.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of climate station time series data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore  = ["api_key", "start_date", "end_date", "timescale"],
-        f       = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    # lists of valid timesteps
-    day_lst       = ['day', 'days', 'daily', 'd']
-    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
-    timescale_lst = day_lst + month_lst
-
-    # if timescale is None, then defaults to "day"
-    if timescale is None: 
-        timescale = "day"
-        
-    # if parameter is NOT in list of valid parameters
-    if timescale not in timescale_lst:
-        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}")
-
-    # request daily climate time series data
-    if timescale in day_lst:    
-        clim_data = _get_climate_ts_day(
-            station_number      = station_number,
-            site_id             = site_id,
-            param               = param,
-            start_date          = start_date,
-            end_date            = end_date,
-            api_key             = api_key
-            )
-
-        # return daily climate time series data
-        return clim_data
-
-    # request monthly climate time series data
-    if timescale in month_lst:    
-
-        clim_data = _get_climate_ts_month(
-            station_number      = station_number,
-            site_id             = site_id,
-            param               = param,
-            start_date          = start_date,
-            end_date            = end_date,
-            api_key             = api_key
-            )
-
-        # return monthly climate time series data
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+# from .utils import shared_function
+from cdsspy import utils
+
+def get_climate_stations(
+    aoi                 = None,
+    radius              = None,
+    county              = None,
+    division            = None,
+    station_name        = None,
+    site_id             = None,
+    water_district      = None,
+    api_key             = None
+    ):
+    """Return Climate Station information
+
+    Make a request to the climatedata/climatestations/ endpoint to locate climate stations via a spatial search, or by county, division, station name, Site ID or water district.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        county (str, optional): County to query for climate stations. Defaults to None.
+        division (int, str, optional):  Water division to query for climate stations. Defaults to None.
+        station_name (str, optional):  climate station name. Defaults to None.
+        site_id (str, tuple, list, optional): string, tuple or list of site IDs. Defaults to None.
+        water_district (int, str, optional): Water district to query for climate stations. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of climate station data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # collapse site_id list, tuple, vector of site_id into query formatted string
+    site_id = utils._collapse_vector(
+        vect = site_id, 
+        sep  = "%2C+"
+        )
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestations/?"
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving climate station data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}' 
+            f'&division={division or ""}'
+            f'&stationName={station_name or ""}' 
+            f'&siteId={site_id or ""}'
+            f'&waterDistrict={water_district or ""}' 
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+
+    return data_df
+
+def get_climate_frostdates(
+    station_number      = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return climate stations frost dates 
+
+    Make a request to the /climatedata/climatestationfrostdates endpoint to retrieve climate stations frost dates data by station number within a given date range (start and end dates)
+
+    Args:
+        station_number (str, optional): climate data station number. Defaults to None.
+        start_date (str, optional): date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of climate station frost dates data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationfrostdates/?"
+    
+    # parse start_date into query string format
+    start_year = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%Y"
+    )
+
+    # parse end_date into query string format
+    end_year = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving climate station frost dates data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-calYear={start_year or ""}' 
+            f'&max-calYear={end_year or ""}'
+            f'&stationNum={station_number or ""}' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+
+def _get_climate_ts_day(
+    station_number      = None,
+    site_id             = None,
+    param               = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return daily climate data
+    
+    Make a request to the /climatedata/climatestationtsday endpoint to retrieve climate stations daily time series data by station number, or Site IDs within a given date range (start and end dates)
+    
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        site_id (str, tuple, list, optional): string, tuple or list of climate station site IDs. Defaults to None.
+        param (str):  climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of climate station daily time series data
+    """
+
+    # list of valid parameters
+    param_lst = ["Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow","SnowDepth", "SnowSWE", "Solar","VP", "Wind"]
+
+    # if parameter is not in list of valid parameters
+    if param not in param_lst:
+        raise ValueError("Invalid `param` argument \nPlease enter one of the following valid parameters: \nEvap, FrostDate, MaxTemp, MeanTemp, MinTemp, Precip, Snow, SnowDepth, SnowSWE, Solar, VP, Wind")
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [site_id, station_number]):
+    #     raise TypeError("Invalid 'site_id' or 'station_number' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_dict)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationtsday/?"
+
+    # collapse list, tuple, vector of site_id into query formatted string
+    site_id = utils._collapse_vector(
+        vect = site_id, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print(f"Retrieving daily climate time series data ({param})")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-measDate={start_date or ""}' 
+            f'&max-measDate={end_date or ""}'
+            f'&stationNum={station_number or ""}' 
+            f'&siteId={site_id or ""}'
+            f'&measType={param or ""}' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # convert measDate columns to 'date' and pd datetime type
+        cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def _get_climate_ts_month(
+    station_number      = None,
+    site_id             = None,
+    param               = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return monthly climate data
+    
+    Make a request to the /climatedata/climatestationtsmonth endpoint to retrieve climate stations monthly time series data by station number, or Site IDs within a given date range (start and end dates)
+    
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        site_id (str, optional):  tuple or list of climate station site IDs. Defaults to None.
+        param (str, optional):  climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of climate station monthly time series data
+    """
+    # list of valid parameters
+    param_lst = ["Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow","SnowDepth", "SnowSWE", "Solar","VP", "Wind"]
+
+    # if parameter is not in list of valid parameters
+    if param not in param_lst:
+        raise ValueError("Invalid `param` argument \nPlease enter one of the following valid parameters: \nEvap, FrostDate, MaxTemp, MeanTemp, MinTemp, Precip, Snow, SnowDepth, SnowSWE, Solar, VP, Wind")
+    
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/climatedata/climatestationtsmonth/?"
+
+    # collapse list, tuple, vector of site_id into query formatted string
+    site_id = utils._collapse_vector(
+        vect = site_id, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%Y"
+        )
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print(f"Retrieving monthly climate time series data ({param})")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-calYear={start_date or ""}'
+            f'&max-calYear={end_date or ""}'
+            f'&stationNum={station_number or ""}' 
+            f'&siteId={site_id or ""}' 
+            f'&measType={param or ""}' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # convert string month to have leading 0 if month < 10
+        cdss_df['month_str'] = cdss_df["calMonthNum"]
+
+        # add month w/ leading 0 column
+        cdss_df.loc[(cdss_df['calMonthNum'] < 10), 'month_str'] = "0" + cdss_df["calMonthNum"].astype(str)
+
+        # create datetime column w/ calYear and month_str columns, and convert to pd datetime type
+        cdss_df["datetime"] = pd.to_datetime(cdss_df['calYear'].astype(str) + "-" + cdss_df["month_str"].astype(str) + "-01")
+    
+        # drop month_str column
+        cdss_df = cdss_df.drop('month_str', axis = 1)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def get_climate_ts(
+    station_number      = None,
+    site_id             = None,
+    param               = None,
+    start_date          = None,
+    end_date            = None,
+    timescale           = None,
+    api_key             = None
+    ):
+
+    """Return climate station time series data
+
+    Make a request to the /climatedata/climatestationts endpoints to retrieve daily or monthly (climatestationtsday or climatestationtsmonth)climate station time series data by station number or Site IDs within a given date range (start and end dates)
+    
+    Args:
+        station_number (str, optional): climate data station number. Defaults to None.
+        site_id (str, optional): string, tuple or list of climate station site IDs. Defaults to None.
+        param (str, optional): climate variable. One of: "Evap", "FrostDate",  "MaxTemp", "MeanTemp", "MinTemp", "Precip", "Snow", "SnowDepth", "SnowSWE", "Solar","VP", "Wind". Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        timescale (str, optional): timestep of the time series data to return, either "day" or "month". Defaults to None and will request daily time series.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of climate station time series data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore  = ["api_key", "start_date", "end_date", "timescale"],
+        f       = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    # lists of valid timesteps
+    day_lst       = ['day', 'days', 'daily', 'd']
+    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
+    timescale_lst = day_lst + month_lst
+
+    # if timescale is None, then defaults to "day"
+    if timescale is None: 
+        timescale = "day"
+        
+    # if parameter is NOT in list of valid parameters
+    if timescale not in timescale_lst:
+        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}")
+
+    # request daily climate time series data
+    if timescale in day_lst:    
+        clim_data = _get_climate_ts_day(
+            station_number      = station_number,
+            site_id             = site_id,
+            param               = param,
+            start_date          = start_date,
+            end_date            = end_date,
+            api_key             = api_key
+            )
+
+        # return daily climate time series data
+        return clim_data
+
+    # request monthly climate time series data
+    if timescale in month_lst:    
+
+        clim_data = _get_climate_ts_month(
+            station_number      = station_number,
+            site_id             = site_id,
+            param               = param,
+            start_date          = start_date,
+            end_date            = end_date,
+            api_key             = api_key
+            )
+
+        # return monthly climate time series data
         return clim_data
```

### Comparing `cdsspy-1.2.70/cdsspy/gw.py` & `cdsspy-1.2.71/cdsspy/gw.py`

 * *Ordering differences only*

 * *Files 23% similar despite different names*

```diff
@@ -1,433 +1,433 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_gw_wl_wells(
-    county              = None,
-    designated_basin    = None,
-    division            = None,
-    management_district = None,
-    water_district      = None,
-    wellid              = None,
-    api_key             = None
-    ):
-    """Search for groundwater water level wells
-    
-    Make a request to the groundwater/waterlevels/wells endpoint to retrieve groundwater water level wells data.
-
-    Args:
-        county (str, optional): County to query for groundwater water level wells. Defaults to None.
-        designated_basin (str, optional): Designated basin to query for groundwater water level wells. Defaults to None.
-        division (str, optional): Division to query for groundwater water level wells. Defaults to None.
-        management_district (str, optional): Management district to query for groundwater water level wells. Defaults to None.
-        water_district (str, optional): Water district to query for groundwater water level wells. Defaults to None.
-        wellid (str, optional): Well ID of a groundwater water level well. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
-
-    Returns:
-        pandas dataframe object: dataframe of groundwater water level wells
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore  = ["api_key"],
-        f       = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/waterlevels/wells/?"
-
-    # if county is given, make sure it is separated by "+" and all uppercase 
-    if county is not None:
-        county = county.replace(" ", "+")
-        county = county.upper()
-
-    # if management_district is given, make sure it is separated by "+" and all uppercase 
-    if management_district is not None:
-        management_district = management_district.replace(" ", "+")
-        management_district = management_district.upper()
-
-    # if designated_basin is given, make sure it is separated by "+" and all uppercase 
-    if designated_basin is not None:
-        designated_basin = designated_basin.replace(" ", "+")
-        designated_basin = designated_basin.upper()
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving groundwater water level data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}' 
-            f'&wellId={wellid or ""}'
-            f'&division={division or ""}' 
-            f'&waterDistrict={water_district or ""}' 
-            f'&designatedBasin={designated_basin or ""}' 
-            f'&managementDistrict={management_district or ""}' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def get_gw_wl_wellmeasures(
-    wellid        = None,
-    start_date    = None,
-    end_date      = None,
-    api_key       = None
-    ):
-    """Return groundwater water level well measurements
-
-    Make a request to the groundwater/waterlevels/wellmeasurements endpoint to retrieve groundwater water level well measurement data.
-
-    Args:
-        wellid (str): Well ID to query for groundwater water level measurements. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
-
-    Returns:
-        pandas dataframe object: dataframe of groundwater well measurements
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/waterlevels/wellmeasurements/?"
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving groundwater water level measurements")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-measurementDate={start_date or ""}' 
-            f'&min-measurementDate={end_date or ""}'
-            f'&wellId={wellid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def get_gw_gplogs_wells(
-    county              = None,
-    designated_basin    = None,
-    division            = None,
-    management_district = None,
-    water_district      = None,
-    wellid              = None,
-    api_key             = None
-    ):
-    """Search for groundwater geophysicallog wells
-    
-    Make a request to the groundwater/geophysicallogs/wells endpoint to retrieve groundwater geophysicallog wells data.
-    
-    Args:
-        county (str, optional): County to query for groundwater geophysicallog wells. Defaults to None.
-        designated_basin (str, optional): Designated basin to query for groundwater geophysicallog wells. Defaults to None.
-        division (str, optional): Division to query for groundwater geophysicallog wells. Defaults to None.
-        management_district (str, optional): Management district to query for groundwater geophysicallog wells. Defaults to None.
-        water_district (str, optional): Water district to query for groundwater geophysicallog wells. Defaults to None.
-        wellid (str, optional): Well ID of a groundwater geophysicallog wells. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
-
-    Returns:
-        pandas dataframe object: dataframe of groundwater geophysicallog wells
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/geophysicallogs/wells/?"
-
-    # if county is given, make sure it is separated by "+" and all uppercase 
-    if county is not None:
-        county = county.replace(" ", "+")
-        county = county.upper()
-
-    # if management_district is given, make sure it is separated by "+" and all uppercase 
-    if management_district is not None:
-        management_district = management_district.replace(" ", "+")
-        management_district = management_district.upper()
-
-    # if designated_basin is given, make sure it is separated by "+" and all uppercase 
-    if designated_basin is not None:
-        designated_basin = designated_basin.replace(" ", "+")
-        designated_basin = designated_basin.upper()
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving groundwater geophysicallog wells data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-        
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}' 
-            f'&wellId={wellid or ""}'
-            f'&division={division or ""}' 
-            f'&waterDistrict={water_district or ""}' 
-            f'&designatedBasin={designated_basin or ""}' 
-            f'&managementDistrict={management_district or ""}' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def get_gw_gplogs_geologpicks(
-    wellid              = None,
-    api_key             = None
-    ):
-    """Return Groundwater Geophysical Log picks by well ID
-
-    Make a request to the groundwater/geophysicallogs/wells endpoint to retrieve groundwater geophysical log picks for the given well ID.
-    
-    Args:
-        wellid (str, optional): Well ID of a groundwater geophysicallog wells. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
-
-    Returns:
-        pandas dataframe object: dataframe of groundwater geophysical log picks
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/geophysicallogs/geoplogpicks/?"
-
-    # If no well ID is provided
-    if wellid is None:
-        return print("Invalid 'wellid' parameter")
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving groundwater geophysical log picks data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&wellId={wellid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_gw_wl_wells(
+    county              = None,
+    designated_basin    = None,
+    division            = None,
+    management_district = None,
+    water_district      = None,
+    wellid              = None,
+    api_key             = None
+    ):
+    """Search for groundwater water level wells
+    
+    Make a request to the groundwater/waterlevels/wells endpoint to retrieve groundwater water level wells data.
+
+    Args:
+        county (str, optional): County to query for groundwater water level wells. Defaults to None.
+        designated_basin (str, optional): Designated basin to query for groundwater water level wells. Defaults to None.
+        division (str, optional): Division to query for groundwater water level wells. Defaults to None.
+        management_district (str, optional): Management district to query for groundwater water level wells. Defaults to None.
+        water_district (str, optional): Water district to query for groundwater water level wells. Defaults to None.
+        wellid (str, optional): Well ID of a groundwater water level well. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
+
+    Returns:
+        pandas dataframe object: dataframe of groundwater water level wells
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore  = ["api_key"],
+        f       = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/waterlevels/wells/?"
+
+    # if county is given, make sure it is separated by "+" and all uppercase 
+    if county is not None:
+        county = county.replace(" ", "+")
+        county = county.upper()
+
+    # if management_district is given, make sure it is separated by "+" and all uppercase 
+    if management_district is not None:
+        management_district = management_district.replace(" ", "+")
+        management_district = management_district.upper()
+
+    # if designated_basin is given, make sure it is separated by "+" and all uppercase 
+    if designated_basin is not None:
+        designated_basin = designated_basin.replace(" ", "+")
+        designated_basin = designated_basin.upper()
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving groundwater water level data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}' 
+            f'&wellId={wellid or ""}'
+            f'&division={division or ""}' 
+            f'&waterDistrict={water_district or ""}' 
+            f'&designatedBasin={designated_basin or ""}' 
+            f'&managementDistrict={management_district or ""}' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def get_gw_wl_wellmeasures(
+    wellid        = None,
+    start_date    = None,
+    end_date      = None,
+    api_key       = None
+    ):
+    """Return groundwater water level well measurements
+
+    Make a request to the groundwater/waterlevels/wellmeasurements endpoint to retrieve groundwater water level well measurement data.
+
+    Args:
+        wellid (str): Well ID to query for groundwater water level measurements. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
+
+    Returns:
+        pandas dataframe object: dataframe of groundwater well measurements
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/waterlevels/wellmeasurements/?"
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving groundwater water level measurements")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-measurementDate={start_date or ""}' 
+            f'&min-measurementDate={end_date or ""}'
+            f'&wellId={wellid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def get_gw_gplogs_wells(
+    county              = None,
+    designated_basin    = None,
+    division            = None,
+    management_district = None,
+    water_district      = None,
+    wellid              = None,
+    api_key             = None
+    ):
+    """Search for groundwater geophysicallog wells
+    
+    Make a request to the groundwater/geophysicallogs/wells endpoint to retrieve groundwater geophysicallog wells data.
+    
+    Args:
+        county (str, optional): County to query for groundwater geophysicallog wells. Defaults to None.
+        designated_basin (str, optional): Designated basin to query for groundwater geophysicallog wells. Defaults to None.
+        division (str, optional): Division to query for groundwater geophysicallog wells. Defaults to None.
+        management_district (str, optional): Management district to query for groundwater geophysicallog wells. Defaults to None.
+        water_district (str, optional): Water district to query for groundwater geophysicallog wells. Defaults to None.
+        wellid (str, optional): Well ID of a groundwater geophysicallog wells. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
+
+    Returns:
+        pandas dataframe object: dataframe of groundwater geophysicallog wells
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/geophysicallogs/wells/?"
+
+    # if county is given, make sure it is separated by "+" and all uppercase 
+    if county is not None:
+        county = county.replace(" ", "+")
+        county = county.upper()
+
+    # if management_district is given, make sure it is separated by "+" and all uppercase 
+    if management_district is not None:
+        management_district = management_district.replace(" ", "+")
+        management_district = management_district.upper()
+
+    # if designated_basin is given, make sure it is separated by "+" and all uppercase 
+    if designated_basin is not None:
+        designated_basin = designated_basin.replace(" ", "+")
+        designated_basin = designated_basin.upper()
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving groundwater geophysicallog wells data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+        
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}' 
+            f'&wellId={wellid or ""}'
+            f'&division={division or ""}' 
+            f'&waterDistrict={water_district or ""}' 
+            f'&designatedBasin={designated_basin or ""}' 
+            f'&managementDistrict={management_district or ""}' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def get_gw_gplogs_geologpicks(
+    wellid              = None,
+    api_key             = None
+    ):
+    """Return Groundwater Geophysical Log picks by well ID
+
+    Make a request to the groundwater/geophysicallogs/wells endpoint to retrieve groundwater geophysical log picks for the given well ID.
+    
+    Args:
+        wellid (str, optional): Well ID of a groundwater geophysicallog wells. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS.
+
+    Returns:
+        pandas dataframe object: dataframe of groundwater geophysical log picks
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/groundwater/geophysicallogs/geoplogpicks/?"
+
+    # If no well ID is provided
+    if wellid is None:
+        return print("Invalid 'wellid' parameter")
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving groundwater geophysical log picks data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&wellId={wellid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy/reference_tbl.py` & `cdsspy-1.2.71/cdsspy/reference_tbl.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,750 +1,750 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_reference_tbl(
-    table_name = None,
-    api_key    = None
-    ):
-    """Return Reference Table reference table
-    
-    Makes requests to the /referencetables/ endpoints and returns helpful reference tables. Reference tables can help identify valid inputs for querying CDSS API resources using cdsspy.  
-    For more detailed information visit: https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml.
-    
-    Args:
-        table_name (str, optional): name of the reference table to return. Must be one of:
-            ("county", "waterdistricts", "waterdivisions", "designatedbasins", "managementdistricts", "telemetryparams", "climateparams", "divrectypes", "flags"). Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-    
-    Returns:
-        pandas dataframe: dataframe of CDSS reference tables
-    """
-    # list of valid parameters
-    tbl_lst = ["county", "waterdistricts", "waterdivisions", "designatedbasins", "managementdistricts", "telemetryparams", "climateparams", "divrectypes", "flags"]
-
-    # if parameter is not in list of valid parameters
-    if table_name not in tbl_lst:
-        raise ValueError("Invalid `table_name` argument \nPlease enter one of the following valid table names: \ncounty\nwaterdistricts\nwaterdivisions\ndesignatedbasins\nmanagementdistricts\ntelemetryparams\nclimateparams\ndivrectypes\nflags")
-
-    # retrieve county reference table
-    if table_name == "county":
-        ref_table = _get_ref_county(
-            api_key = api_key
-            )
-        return ref_table
-    
-    # retrieve water districts reference table
-    if table_name == "waterdistricts":
-        ref_table = _get_ref_waterdistricts(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve water divisions reference table
-    if table_name == "waterdivisions":
-        ref_table = _get_ref_waterdivisions(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve management districts reference table
-    if table_name == "managementdistricts":
-        ref_table = _get_ref_managementdistricts(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve designated basins reference table
-    if table_name == "designatedbasins":
-        ref_table = _get_ref_designatedbasins(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve telemetry station parameters reference table
-    if table_name == "telemetryparams":
-        ref_table = _get_ref_telemetry_params(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve climate station parameters reference table
-    if table_name == "climateparams":
-        ref_table = _get_ref_climate_params(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve diversion record types reference table
-    if table_name == "divrectypes":
-        ref_table = _get_ref_divrectypes(
-            api_key = api_key
-            )
-        return ref_table
-
-    # retrieve station flags reference table
-    if table_name == "flags":
-        ref_table = _get_ref_stationflags(
-            api_key = api_key
-            )
-        return ref_table
-        
-def _get_ref_county(
-    county  = None, 
-    api_key = None
-    ):
-    """Return county reference table
-
-    Args:
-        county (str, optional): County to query, if no county is given, entire county dataframe is returned. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of Colorado counties
-    """
-    
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/county/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving reference table: Counties")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-# _get_ref_county()
-# get_reference_tbl("county")
-
-def _get_ref_waterdistricts(
-    division       = None, 
-    water_district = None,
-    api_key        = None
-    ):
-    """Return water districts reference table
-
-    Args:
-        division (str, optional):  (optional) indicating the division to query, if no division is given, dataframe of all water districts is returned. Defaults to None.
-        water_district (str, optional):  (optional) indicating the water district to query, if no water district is given, dataframe of all water districts is returned. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of Colorado water_districts
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/waterdistrict/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving reference table: Water districts")
-    
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&division={division or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_waterdivisions(
-    division       = None, 
-    api_key        = None
-    ):
-    """Return water divisions reference table
-
-    Args:
-        division (str, optional): Division to query, if no division is given, dataframe of all water divisions is returned. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of Colorado water divisions
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/waterdivision/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving reference table: Water divisions")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&division={division or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_managementdistricts(
-    management_district   = None, 
-    api_key               = None
-    ):
-    """Return management districts reference table
-    
-    Args:
-        management_district (str, optional): Indicating the management district to query, if no management district is given, dataframe of all management districts is returned Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of Colorado management districts
-    """
-
-    # get input args
-    input_args = locals()
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/managementdistrict/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving reference table: Management districts")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&managementDistrictName={management_district or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_designatedbasins(
-    designated_basin   = None, 
-    api_key            = None
-    ):
-    """Return designated basin reference table
-    
-    Args:
-        designated_basin (str, optional): Indicating the  designated basin to query character, if no designated basin is given, all designated basins dataframe is returned. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of Colorado designated basins
-    """
-
-    # get input args
-    input_args = locals()
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/designatedbasin/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving reference table: Designated basins")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&designatedBasinName={designated_basin or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_telemetry_params(
-    param    = None, 
-    api_key  = None
-    ):
-    """Return telemetry station parameter reference table
-    
-    Args:
-        param (str, optional): Indicating the parameter to query character, if no parameter is given, all parameter dataframe is returned Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of telemetry station parameter reference table
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/telemetryparams/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print("Retrieving reference table: Telemetry station parameters")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json'
-            f'&parameter={param or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_climate_params(
-    param      = None, 
-    api_key    = None
-    ):
-    """Return climate station parameter reference table
-    
-    Args:
-        param (str, optional): Indicating the climate station parameter to query, if no parameter is given, all parameter dataframe is returned. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of climate station parameter reference table
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/climatestationmeastype/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print("Retrieving reference table: Climate station parameters")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json'
-            f'&measType={param or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_divrectypes(
-    divrectype   = None, 
-    api_key      = None
-    ):
-    """Return Diversion Record Types reference table
-    
-    Args:
-        divrectype (str, optional): Diversion record type to query, if no divrectype is given, a dataframe with all diversion record types is returned. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of diversion record types reference table
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/divrectypes/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print("Retrieving reference table: Diversion record types")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json'
-            f'&divRecType={divrectype or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_ref_stationflags(
-    flag    = None, 
-    api_key = None
-    ):
-    """Return Station Flag reference table
-    
-    Args:
-        flag (str, optional): short code for the flag to query, if no flag is given, a dataframe with all flags is returned. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe: dataframe of diversion record types reference table
-    """
-
-    # get input args
-    input_args = locals()
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/stationflags/?"
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print("Retrieving reference table: Station flags")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json'
-            f'&flag={flag or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_reference_tbl(
+    table_name = None,
+    api_key    = None
+    ):
+    """Return Reference Table reference table
+    
+    Makes requests to the /referencetables/ endpoints and returns helpful reference tables. Reference tables can help identify valid inputs for querying CDSS API resources using cdsspy.  
+    For more detailed information visit: https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml.
+    
+    Args:
+        table_name (str, optional): name of the reference table to return. Must be one of:
+            ("county", "waterdistricts", "waterdivisions", "designatedbasins", "managementdistricts", "telemetryparams", "climateparams", "divrectypes", "flags"). Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+    
+    Returns:
+        pandas dataframe: dataframe of CDSS reference tables
+    """
+    # list of valid parameters
+    tbl_lst = ["county", "waterdistricts", "waterdivisions", "designatedbasins", "managementdistricts", "telemetryparams", "climateparams", "divrectypes", "flags"]
+
+    # if parameter is not in list of valid parameters
+    if table_name not in tbl_lst:
+        raise ValueError("Invalid `table_name` argument \nPlease enter one of the following valid table names: \ncounty\nwaterdistricts\nwaterdivisions\ndesignatedbasins\nmanagementdistricts\ntelemetryparams\nclimateparams\ndivrectypes\nflags")
+
+    # retrieve county reference table
+    if table_name == "county":
+        ref_table = _get_ref_county(
+            api_key = api_key
+            )
+        return ref_table
+    
+    # retrieve water districts reference table
+    if table_name == "waterdistricts":
+        ref_table = _get_ref_waterdistricts(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve water divisions reference table
+    if table_name == "waterdivisions":
+        ref_table = _get_ref_waterdivisions(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve management districts reference table
+    if table_name == "managementdistricts":
+        ref_table = _get_ref_managementdistricts(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve designated basins reference table
+    if table_name == "designatedbasins":
+        ref_table = _get_ref_designatedbasins(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve telemetry station parameters reference table
+    if table_name == "telemetryparams":
+        ref_table = _get_ref_telemetry_params(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve climate station parameters reference table
+    if table_name == "climateparams":
+        ref_table = _get_ref_climate_params(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve diversion record types reference table
+    if table_name == "divrectypes":
+        ref_table = _get_ref_divrectypes(
+            api_key = api_key
+            )
+        return ref_table
+
+    # retrieve station flags reference table
+    if table_name == "flags":
+        ref_table = _get_ref_stationflags(
+            api_key = api_key
+            )
+        return ref_table
+        
+def _get_ref_county(
+    county  = None, 
+    api_key = None
+    ):
+    """Return county reference table
+
+    Args:
+        county (str, optional): County to query, if no county is given, entire county dataframe is returned. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of Colorado counties
+    """
+    
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/county/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving reference table: Counties")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+# _get_ref_county()
+# get_reference_tbl("county")
+
+def _get_ref_waterdistricts(
+    division       = None, 
+    water_district = None,
+    api_key        = None
+    ):
+    """Return water districts reference table
+
+    Args:
+        division (str, optional):  (optional) indicating the division to query, if no division is given, dataframe of all water districts is returned. Defaults to None.
+        water_district (str, optional):  (optional) indicating the water district to query, if no water district is given, dataframe of all water districts is returned. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of Colorado water_districts
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/waterdistrict/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving reference table: Water districts")
+    
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&division={division or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_waterdivisions(
+    division       = None, 
+    api_key        = None
+    ):
+    """Return water divisions reference table
+
+    Args:
+        division (str, optional): Division to query, if no division is given, dataframe of all water divisions is returned. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of Colorado water divisions
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/waterdivision/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving reference table: Water divisions")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&division={division or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_managementdistricts(
+    management_district   = None, 
+    api_key               = None
+    ):
+    """Return management districts reference table
+    
+    Args:
+        management_district (str, optional): Indicating the management district to query, if no management district is given, dataframe of all management districts is returned Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of Colorado management districts
+    """
+
+    # get input args
+    input_args = locals()
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/managementdistrict/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving reference table: Management districts")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&managementDistrictName={management_district or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_designatedbasins(
+    designated_basin   = None, 
+    api_key            = None
+    ):
+    """Return designated basin reference table
+    
+    Args:
+        designated_basin (str, optional): Indicating the  designated basin to query character, if no designated basin is given, all designated basins dataframe is returned. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of Colorado designated basins
+    """
+
+    # get input args
+    input_args = locals()
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/designatedbasin/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving reference table: Designated basins")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&designatedBasinName={designated_basin or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_telemetry_params(
+    param    = None, 
+    api_key  = None
+    ):
+    """Return telemetry station parameter reference table
+    
+    Args:
+        param (str, optional): Indicating the parameter to query character, if no parameter is given, all parameter dataframe is returned Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of telemetry station parameter reference table
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/telemetryparams/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print("Retrieving reference table: Telemetry station parameters")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json'
+            f'&parameter={param or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_climate_params(
+    param      = None, 
+    api_key    = None
+    ):
+    """Return climate station parameter reference table
+    
+    Args:
+        param (str, optional): Indicating the climate station parameter to query, if no parameter is given, all parameter dataframe is returned. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of climate station parameter reference table
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/climatestationmeastype/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print("Retrieving reference table: Climate station parameters")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json'
+            f'&measType={param or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_divrectypes(
+    divrectype   = None, 
+    api_key      = None
+    ):
+    """Return Diversion Record Types reference table
+    
+    Args:
+        divrectype (str, optional): Diversion record type to query, if no divrectype is given, a dataframe with all diversion record types is returned. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of diversion record types reference table
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/divrectypes/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print("Retrieving reference table: Diversion record types")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json'
+            f'&divRecType={divrectype or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_ref_stationflags(
+    flag    = None, 
+    api_key = None
+    ):
+    """Return Station Flag reference table
+    
+    Args:
+        flag (str, optional): short code for the flag to query, if no flag is given, a dataframe with all flags is returned. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe: dataframe of diversion record types reference table
+    """
+
+    # get input args
+    input_args = locals()
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/referencetables/stationflags/?"
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print("Retrieving reference table: Station flags")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json'
+            f'&flag={flag or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy/structures.py` & `cdsspy-1.2.71/cdsspy/structures.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,903 +1,903 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def _get_structures_divrecday(
-    wdid          = None,
-    wc_identifier = None,
-    start_date    = None,
-    end_date      = None,
-    api_key       = None
-    ):
-    """Return Structure Daily Diversion/Release Records
-
-    Make a request to the api/v2/structures/divrec/divrecday/ endpoint to retrieve daily structure diversion/release data for a specified WDID within a specified date range.
-
-    Args:
-        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
-        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of daily structure diversion/releases records 
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecday/?"
-
-    # correctly format wc_identifier, if NULL, return "*diversion*"
-    wc_id = utils._align_wcid(
-        x       = wc_identifier,
-        default = "*diversion*"
-        )
-    
-    # collapse list, tuple, vector of wdid into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # print message
-    if wc_identifier is None: 
-        print(f'Retrieving daily divrec data (diversion)')
-    else:
-        print(f'Retrieving daily divrec data ({wc_identifier})')
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&wcIdentifier={wc_id or ""}'
-            f'&min-dataMeasDate={start_date or ""}'
-            f'&max-dataMeasDate={end_date or ""}'
-            f'&wdid={wdid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-
-def _get_structures_divrecmonth(
-    wdid          = None,
-    wc_identifier = None,
-    start_date    = None,
-    end_date      = None,
-    api_key       = None
-    ):
-    """Return Structure Monthly Diversion/Release Records
-
-    Make a request to the api/v2/structures/divrec/divrecmonth/ endpoint to retrieve monthly structure diversion/release data for a specified WDID within a specified date range.
-
-    Args:
-        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
-        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of monthly structure diversion/releases records 
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecmonth/?"
-
-    # correctly format wc_identifier, if NULL, return "*diversion*"
-    wc_id = utils._align_wcid(
-        x       = wc_identifier,
-        default = "*diversion*"
-        )
-    
-    # collapse list, tuple, vector of wdid into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # print message
-    if wc_identifier is None: 
-        print(f'Retrieving monthly divrec data (diversion)')
-    else:
-        print(f'Retrieving monthly divrec data ({wc_identifier})')
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&wcIdentifier={wc_id or ""}'
-            f'&min-dataMeasDate={start_date or ""}'
-            f'&max-dataMeasDate={end_date or ""}'
-            f'&wdid={wdid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-
-    return data_df
-
-def _get_structures_divrecyear(
-    wdid          = None,
-    wc_identifier = None,
-    start_date    = None,
-    end_date      = None,
-    api_key       = None
-    ):
-    """Return Structure Annual Diversion/Release Records
-
-    Make a request to the structures/divrec/divrecyear/ endpoint to retrieve annual structure diversion/release data for a specified WDID within a specified date range.
-
-    Args:
-        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
-        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of annual structure diversion/releases records 
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecyear/?"
-
-    # correctly format wc_identifier, if NULL, return "*diversion*"
-    wc_id = utils._align_wcid(
-        x       = wc_identifier,
-        default = "*diversion*"
-        )
-
-    # collapse list, tuple, vector of wdid into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # print message
-    if wc_identifier is None: 
-        print(f'Retrieving yearly divrec data (diversion)')
-    else:
-        print(f'Retrieving yearly divrec data ({wc_identifier})')
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&wcIdentifier={wc_id or ""}'
-            f'&min-dataMeasDate={start_date or ""}'
-            f'&max-dataMeasDate={end_date or ""}'
-            f'&wdid={wdid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def get_structures_divrec_ts(
-    wdid          = None,
-    wc_identifier = None,
-    start_date    = None,
-    end_date      = None,
-    timescale     = None, 
-    api_key       = None
-    ):
-
-    """Return diversion/releases record data for administrative structures
-
-    Make a request to the CDSS API /structures/divrec endpoints to get diversion/releases time series data for administrative structures by wdid, within a given date range (start and end dates) and at a specified temporal resolution.     
-
-    Args:
-        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
-        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        timescale (str, optional): timestep of the time series data to return, either "day", "month", or "year". Defaults to None and will request daily time series.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of structure diversion/releases time series data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "wc_identifier", "start_date", "end_date", "timescale"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    # lists of valid timesteps
-    day_lst       = ['day', 'days', 'daily', 'd']
-    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
-    year_lst      = ['year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
-    timescale_lst = day_lst + month_lst + year_lst
-
-    # if timescale is None, then defaults to "day"
-    if timescale is None: 
-        timescale = "day"
-        
-    # if parameter is NOT in list of valid parameters
-    if timescale not in timescale_lst:
-        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}\n{year_lst}")
-
-    # request daily structure divrec time series data
-    if timescale in day_lst:    
-        divrec_df = _get_structures_divrecday(
-            wdid          = wdid,
-            wc_identifier = wc_identifier,
-            start_date    = start_date,
-            end_date      = end_date,
-            api_key       = api_key
-            )
-
-        # return daily climate time series data
-        return divrec_df
-
-    # request monthly structure divrec time series data
-    if timescale in month_lst:    
-
-        divrec_df = _get_structures_divrecmonth(
-            wdid          = wdid,
-            wc_identifier = wc_identifier,
-            start_date    = start_date,
-            end_date      = end_date,
-            api_key       = api_key
-            )
-
-        # return monthly structure divrec time series data  
-        return divrec_df
-
-    # request yearly structure divrec time series data
-    if timescale in year_lst:    
-
-        divrec_df = _get_structures_divrecyear(
-            wdid          = wdid,
-            wc_identifier = wc_identifier,
-            start_date    = start_date,
-            end_date      = end_date,
-            api_key       = api_key
-            )
-
-        # return yearly structure divrec time series data
-        return divrec_df
-
-def get_structures_stage_ts(
-    wdid          = None,
-    start_date    = None,
-    end_date      = None,
-    api_key       = None
-    ):
-    """Return stage/volume record data for administrative structures
-
-    Make a request to the structures/divrec/stagevolume/ endpoint to retrieve structure stage/volume data for a specified WDID within a specified date range.
-
-    Args:
-        wdid (str):  WDID code of structure. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):   optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of daily structure stage/volume records 
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/stagevolume/?"
-
-    # collapse list, tuple, vector of wdid into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&min-dataMeasDate={start_date or ""}'
-            f'&max-dataMeasDate={end_date or ""}'
-            f'&wdid={wdid or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def get_structures(
-    aoi            = None,
-    radius         = None,
-    county         = None,
-    division       = None,
-    gnis_id        = None,
-    water_district = None,
-    wdid           = None,
-    api_key        = None
-):
-    """Return list of administrative structures
-
-    Make a request to the api/v2/structures endpoint to locate administrative structures via a spatial search or by division, county, water_district, GNIS, or WDID.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        county (str, optional): Indicating the county to query. Defaults to None.
-        division (int, str, optional): Indicating the water division to query. Defaults to None.
-        gnis_id (str, optional): Water source - Geographic Name Information System ID (GNIS ID). Defaults to None.
-        water_district (int, str, optional): Indicating the water district to query. Defaults to None.
-        wdid (str, tuple or list, optional): WDID(s) code of structure. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of administrative structures
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/?"
-
-    # convert numeric division to string
-    if type(division) == int or type(division) == float:
-        division = str(division)
-
-    # convert numeric water_district to string
-    if type(water_district) == int or type(water_district) == float:
-        water_district = str(water_district)
-
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # collapse WDID list, tuple, vector of site_id into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-        
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}'
-            f'&division={division or ""}'
-            f'&gnisId={gnis_id or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&wdid={wdid or ""}'
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-        
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-    
-    return data_df
-
-def get_water_classes(
-        wdid                = None,
-        county              = None,
-        division            = None,
-        water_district      = None,
-        wc_identifier       = None,
-        aoi                 = None,
-        radius              = None,
-        gnis_id             = None,
-        start_date          = None,
-        end_date            = None,
-        divrectype          = None,
-        ciu_code            = None,
-        timestep            = None,
-        api_key             = None
-        ):
-    """Return list of waterclasses
-
-    Make a request to the /structures/divrec/waterclasses endpoint to identify water classes via a spatial search or by division, county, water_district, GNIS, or WDID.
-
-    Args:
-        wdid (str, tuple or list, optional): WDID(s) code of structure. Defaults to None.
-        county (str, optional): county to query. Defaults to None.
-        division (str, int, optional): water division to query. Defaults to None.
-        water_district (str, int, optional): water district to query. Defaults to None.
-        wc_identifier (_type_, optional): series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. The Water Class, combined with a daily, monthly or annual volume, constitutes a Diversion Record. Defaults to None.
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        gnis_id (str, optional): water source - Geographic Name Information System ID. Defaults to None.
-        start_date (str, optional): date of first measurement in the well's period of record (YYYY-MM-DD). Defaults to None.
-        end_date (str, optional): date of last measurement in the well's period of record (YYYY-MM-DD). Defaults to None.
-        divrectype (str, optional): type of record: "DivComment", "DivTotal", "RelComment", "RelTolal", "StageVolume", or "WaterClass".. Defaults to None.
-        ciu_code (str, optional): current in use code of structure. Defaults to None.
-        timestep (str, optional): timestep, one of "day", "month", "year". Defaults to None which returns a daily timestep.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of water class data for administrative structures
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date", "aoi", "radius",
-                    "ciu_code", "divrectype", "gnis_id", "timestep"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/waterclasses/?"
-
-    # correctly format wc_identifier, if NULL, return "*diversion*"
-    wc_id = utils._align_wcid(
-        x       = wc_identifier,
-        default = None
-        )
-    
-    # collapse list, tuple, vector of wdid into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-    
-    # if start_date is None, return None
-    if start_date is None:
-        start = None
-    else:
-        # parse start_date into query string format
-        start = utils._parse_date(
-            date   = start_date,
-            start  = True,
-            format = "%m-%d-%Y",
-            sep    = "%2F"
-        )
-
-    # if end_date is None, return None
-    if end_date is None:
-        end = None
-    else:
-        # parse start_date into query string format
-        end = utils._parse_date(
-            date   = end_date,
-            start  = False,
-            format = "%m-%d-%Y",
-            sep    = "%2F"
-        )
-
-    # collapse WDID list, tuple, vector of site_id into query formatted string
-    wdid = utils._collapse_vector(
-        vect = wdid, 
-        sep  = "%2C+"
-        )
-    
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # if county is given, make sure it is separated by "+" and all uppercase 
-    if county is not None:
-        county = county.replace(" ", "+")
-        county = county.upper()
-    
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df   = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    # print message
-    print("Retrieving structure water classes")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-        
-        # create query URL string
-        url = (
-            f'{base}'
-            f'timestep={timestep or ""}'
-            f'format=json&dateFormat=spaceSepToSeconds'
-            f'&ciuCode={ciu_code or ""}'
-            f'&county={county or ""}'
-            f'&division={division or ""}'
-            f'&divrectype={divrectype or ""}'
-            f'&min-porEnd={end or ""}'
-            f'&min-porStart={start or ""}'
-            f'&gnisId={gnis_id or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&wcIdentifier={wc_id or ""}'
-            f'&wdid={wdid or ""}'
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def _get_structures_divrecday(
+    wdid          = None,
+    wc_identifier = None,
+    start_date    = None,
+    end_date      = None,
+    api_key       = None
+    ):
+    """Return Structure Daily Diversion/Release Records
+
+    Make a request to the api/v2/structures/divrec/divrecday/ endpoint to retrieve daily structure diversion/release data for a specified WDID within a specified date range.
+
+    Args:
+        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
+        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of daily structure diversion/releases records 
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecday/?"
+
+    # correctly format wc_identifier, if NULL, return "*diversion*"
+    wc_id = utils._align_wcid(
+        x       = wc_identifier,
+        default = "*diversion*"
+        )
+    
+    # collapse list, tuple, vector of wdid into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # print message
+    if wc_identifier is None: 
+        print(f'Retrieving daily divrec data (diversion)')
+    else:
+        print(f'Retrieving daily divrec data ({wc_identifier})')
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&wcIdentifier={wc_id or ""}'
+            f'&min-dataMeasDate={start_date or ""}'
+            f'&max-dataMeasDate={end_date or ""}'
+            f'&wdid={wdid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+
+def _get_structures_divrecmonth(
+    wdid          = None,
+    wc_identifier = None,
+    start_date    = None,
+    end_date      = None,
+    api_key       = None
+    ):
+    """Return Structure Monthly Diversion/Release Records
+
+    Make a request to the api/v2/structures/divrec/divrecmonth/ endpoint to retrieve monthly structure diversion/release data for a specified WDID within a specified date range.
+
+    Args:
+        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
+        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of monthly structure diversion/releases records 
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecmonth/?"
+
+    # correctly format wc_identifier, if NULL, return "*diversion*"
+    wc_id = utils._align_wcid(
+        x       = wc_identifier,
+        default = "*diversion*"
+        )
+    
+    # collapse list, tuple, vector of wdid into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # print message
+    if wc_identifier is None: 
+        print(f'Retrieving monthly divrec data (diversion)')
+    else:
+        print(f'Retrieving monthly divrec data ({wc_identifier})')
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&wcIdentifier={wc_id or ""}'
+            f'&min-dataMeasDate={start_date or ""}'
+            f'&max-dataMeasDate={end_date or ""}'
+            f'&wdid={wdid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+
+    return data_df
+
+def _get_structures_divrecyear(
+    wdid          = None,
+    wc_identifier = None,
+    start_date    = None,
+    end_date      = None,
+    api_key       = None
+    ):
+    """Return Structure Annual Diversion/Release Records
+
+    Make a request to the structures/divrec/divrecyear/ endpoint to retrieve annual structure diversion/release data for a specified WDID within a specified date range.
+
+    Args:
+        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
+        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of annual structure diversion/releases records 
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "wc_identifier", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/divrecyear/?"
+
+    # correctly format wc_identifier, if NULL, return "*diversion*"
+    wc_id = utils._align_wcid(
+        x       = wc_identifier,
+        default = "*diversion*"
+        )
+
+    # collapse list, tuple, vector of wdid into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # print message
+    if wc_identifier is None: 
+        print(f'Retrieving yearly divrec data (diversion)')
+    else:
+        print(f'Retrieving yearly divrec data ({wc_identifier})')
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&wcIdentifier={wc_id or ""}'
+            f'&min-dataMeasDate={start_date or ""}'
+            f'&max-dataMeasDate={end_date or ""}'
+            f'&wdid={wdid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def get_structures_divrec_ts(
+    wdid          = None,
+    wc_identifier = None,
+    start_date    = None,
+    end_date      = None,
+    timescale     = None, 
+    api_key       = None
+    ):
+
+    """Return diversion/releases record data for administrative structures
+
+    Make a request to the CDSS API /structures/divrec endpoints to get diversion/releases time series data for administrative structures by wdid, within a given date range (start and end dates) and at a specified temporal resolution.     
+
+    Args:
+        wdid (str, optional):  tuple or list of WDIDs code of structure. Defaults to None.
+        wc_identifier (str, optional):  series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. Provide "diversion" or "release" to retrieve diversion/release records. Default is None which will return diversions records.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        timescale (str, optional): timestep of the time series data to return, either "day", "month", or "year". Defaults to None and will request daily time series.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of structure diversion/releases time series data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "wc_identifier", "start_date", "end_date", "timescale"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    # lists of valid timesteps
+    day_lst       = ['day', 'days', 'daily', 'd']
+    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
+    year_lst      = ['year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
+    timescale_lst = day_lst + month_lst + year_lst
+
+    # if timescale is None, then defaults to "day"
+    if timescale is None: 
+        timescale = "day"
+        
+    # if parameter is NOT in list of valid parameters
+    if timescale not in timescale_lst:
+        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}\n{year_lst}")
+
+    # request daily structure divrec time series data
+    if timescale in day_lst:    
+        divrec_df = _get_structures_divrecday(
+            wdid          = wdid,
+            wc_identifier = wc_identifier,
+            start_date    = start_date,
+            end_date      = end_date,
+            api_key       = api_key
+            )
+
+        # return daily climate time series data
+        return divrec_df
+
+    # request monthly structure divrec time series data
+    if timescale in month_lst:    
+
+        divrec_df = _get_structures_divrecmonth(
+            wdid          = wdid,
+            wc_identifier = wc_identifier,
+            start_date    = start_date,
+            end_date      = end_date,
+            api_key       = api_key
+            )
+
+        # return monthly structure divrec time series data  
+        return divrec_df
+
+    # request yearly structure divrec time series data
+    if timescale in year_lst:    
+
+        divrec_df = _get_structures_divrecyear(
+            wdid          = wdid,
+            wc_identifier = wc_identifier,
+            start_date    = start_date,
+            end_date      = end_date,
+            api_key       = api_key
+            )
+
+        # return yearly structure divrec time series data
+        return divrec_df
+
+def get_structures_stage_ts(
+    wdid          = None,
+    start_date    = None,
+    end_date      = None,
+    api_key       = None
+    ):
+    """Return stage/volume record data for administrative structures
+
+    Make a request to the structures/divrec/stagevolume/ endpoint to retrieve structure stage/volume data for a specified WDID within a specified date range.
+
+    Args:
+        wdid (str):  WDID code of structure. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):   optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of daily structure stage/volume records 
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/stagevolume/?"
+
+    # collapse list, tuple, vector of wdid into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&min-dataMeasDate={start_date or ""}'
+            f'&max-dataMeasDate={end_date or ""}'
+            f'&wdid={wdid or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def get_structures(
+    aoi            = None,
+    radius         = None,
+    county         = None,
+    division       = None,
+    gnis_id        = None,
+    water_district = None,
+    wdid           = None,
+    api_key        = None
+):
+    """Return list of administrative structures
+
+    Make a request to the api/v2/structures endpoint to locate administrative structures via a spatial search or by division, county, water_district, GNIS, or WDID.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        county (str, optional): Indicating the county to query. Defaults to None.
+        division (int, str, optional): Indicating the water division to query. Defaults to None.
+        gnis_id (str, optional): Water source - Geographic Name Information System ID (GNIS ID). Defaults to None.
+        water_district (int, str, optional): Indicating the water district to query. Defaults to None.
+        wdid (str, tuple or list, optional): WDID(s) code of structure. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of administrative structures
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/?"
+
+    # convert numeric division to string
+    if type(division) == int or type(division) == float:
+        division = str(division)
+
+    # convert numeric water_district to string
+    if type(water_district) == int or type(water_district) == float:
+        water_district = str(water_district)
+
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # collapse WDID list, tuple, vector of site_id into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+        
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}'
+            f'&division={division or ""}'
+            f'&gnisId={gnis_id or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&wdid={wdid or ""}'
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+        
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+    
+    return data_df
+
+def get_water_classes(
+        wdid                = None,
+        county              = None,
+        division            = None,
+        water_district      = None,
+        wc_identifier       = None,
+        aoi                 = None,
+        radius              = None,
+        gnis_id             = None,
+        start_date          = None,
+        end_date            = None,
+        divrectype          = None,
+        ciu_code            = None,
+        timestep            = None,
+        api_key             = None
+        ):
+    """Return list of waterclasses
+
+    Make a request to the /structures/divrec/waterclasses endpoint to identify water classes via a spatial search or by division, county, water_district, GNIS, or WDID.
+
+    Args:
+        wdid (str, tuple or list, optional): WDID(s) code of structure. Defaults to None.
+        county (str, optional): county to query. Defaults to None.
+        division (str, int, optional): water division to query. Defaults to None.
+        water_district (str, int, optional): water district to query. Defaults to None.
+        wc_identifier (_type_, optional): series of water class codes that provide the location of the diversion, the SOURCE of water, the USE of the water and the administrative operation required to make the diversion. The Water Class, combined with a daily, monthly or annual volume, constitutes a Diversion Record. Defaults to None.
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        gnis_id (str, optional): water source - Geographic Name Information System ID. Defaults to None.
+        start_date (str, optional): date of first measurement in the well's period of record (YYYY-MM-DD). Defaults to None.
+        end_date (str, optional): date of last measurement in the well's period of record (YYYY-MM-DD). Defaults to None.
+        divrectype (str, optional): type of record: "DivComment", "DivTotal", "RelComment", "RelTolal", "StageVolume", or "WaterClass".. Defaults to None.
+        ciu_code (str, optional): current in use code of structure. Defaults to None.
+        timestep (str, optional): timestep, one of "day", "month", "year". Defaults to None which returns a daily timestep.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of water class data for administrative structures
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date", "aoi", "radius",
+                    "ciu_code", "divrectype", "gnis_id", "timestep"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/structures/divrec/waterclasses/?"
+
+    # correctly format wc_identifier, if NULL, return "*diversion*"
+    wc_id = utils._align_wcid(
+        x       = wc_identifier,
+        default = None
+        )
+    
+    # collapse list, tuple, vector of wdid into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+    
+    # if start_date is None, return None
+    if start_date is None:
+        start = None
+    else:
+        # parse start_date into query string format
+        start = utils._parse_date(
+            date   = start_date,
+            start  = True,
+            format = "%m-%d-%Y",
+            sep    = "%2F"
+        )
+
+    # if end_date is None, return None
+    if end_date is None:
+        end = None
+    else:
+        # parse start_date into query string format
+        end = utils._parse_date(
+            date   = end_date,
+            start  = False,
+            format = "%m-%d-%Y",
+            sep    = "%2F"
+        )
+
+    # collapse WDID list, tuple, vector of site_id into query formatted string
+    wdid = utils._collapse_vector(
+        vect = wdid, 
+        sep  = "%2C+"
+        )
+    
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # if county is given, make sure it is separated by "+" and all uppercase 
+    if county is not None:
+        county = county.replace(" ", "+")
+        county = county.upper()
+    
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df   = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    # print message
+    print("Retrieving structure water classes")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+        
+        # create query URL string
+        url = (
+            f'{base}'
+            f'timestep={timestep or ""}'
+            f'format=json&dateFormat=spaceSepToSeconds'
+            f'&ciuCode={ciu_code or ""}'
+            f'&county={county or ""}'
+            f'&division={division or ""}'
+            f'&divrectype={divrectype or ""}'
+            f'&min-porEnd={end or ""}'
+            f'&min-porStart={start or ""}'
+            f'&gnisId={gnis_id or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&wcIdentifier={wc_id or ""}'
+            f'&wdid={wdid or ""}'
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy/sw.py` & `cdsspy-1.2.71/cdsspy/sw.py`

 * *Ordering differences only*

 * *Files 19% similar despite different names*

```diff
@@ -1,637 +1,637 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_sw_stations(
-    aoi                 = None,
-    radius              = None,
-    abbrev              = None,
-    county              = None,
-    division            = None,
-    station_name        = None,
-    usgs_id             = None,
-    water_district      = None,
-    api_key             = None
-    ):
-    """Return Surface Water Station information
-    
-    Make a request to the /surfacewater/surfacewaterstations endpoint to locate surface water stations via a spatial search, or by station abbreviation, county, division, station name, USGS ID or water_district.  
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        abbrev (str, list, tuple, optional): surface water station abbreviation. Defaults to None.
-        county (str, optional): County to query for surface water stations. Defaults to None.
-        division (int, str, optional):  Water division to query for surface water stations. Defaults to None.
-        station_name (str, optional): surface water station name. Defaults to None.
-        usgs_id (str, tuple or list , optional): USGS IDs. Defaults to None.
-        water_district (int, str, optional): Water district to query for surface water stations. Defaults to None.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-    
-    Returns:
-        pandas dataframe object: dataframe of surface water station data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # collapse abbrev list, tuple, vector of abbrev into query formatted string
-    abbrev = utils._collapse_vector(
-        vect = abbrev, 
-        sep  = "%2C+"
-        )
-
-    # collapse usgs_id list, tuple, vector of usgs_id into query formatted string
-    usgs_id = utils._collapse_vector(
-        vect = usgs_id, 
-        sep  = "%2C+"
-        )
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewaterstations/?"
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving surface water station data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}' 
-            f'&county={county or ""}' 
-            f'&division={division or ""}'
-            f'&stationName={station_name or ""}' 
-            f'&usgsSiteId={usgs_id or ""}'
-            f'&waterDistrict={water_district or ""}' 
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-
-    return data_df
-
-def _get_sw_ts_day(
-    abbrev              = None,
-    station_number      = None,
-    usgs_id             = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return daily surface water time series data
-    
-    Make a request to the /surfacewater/surfacewatertsday endpoint to retrieve surface water stations daily time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
-    
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
-        station_number (int, str, optional):  surface water station number. Defaults to None.
-        usgs_id (tuple, list, optional):  tuple or list of USGS ID. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: daily surface water time series data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [abbrev, station_number, usgs_id]):
-    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertsday/?"
-
-    # collapse abbreviation list, tuple, vector of site_id into query formatted string
-    abbrev = utils._collapse_vector(
-        vect = abbrev, 
-        sep  = "%2C+"
-        )
-
-    # collapse USGS ID list, tuple, vector of site_id into query formatted string
-    usgs_id = utils._collapse_vector(
-        vect = usgs_id, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-    
-    print("Retrieving daily surface water time series")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}'
-            f'&min-measDate={start_date or ""}'
-            f'&max-measDate={end_date or ""}'
-            f'&stationNum={station_number or ""}'
-            f'&usgsSiteId={usgs_id or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # convert measDate columns to 'date' and pd datetime type
-        cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def _get_sw_ts_month(
-    abbrev              = None,
-    station_number      = None,
-    usgs_id             = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return monthly surface water time series data
-    
-    Make a request to the /surfacewater/surfacewatertsmonth endpoint to retrieve surface water stations monthly time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
-    
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        abbrev (tuple, list, optional):  tuple or list of surface water station abbreviation. Defaults to None.
-        station_number (int, str, optional):  surface water station number. Defaults to None.
-        usgs_id (str, optional):  tuple or list of USGS ID. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: monthly surface water time series data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [abbrev, station_number, usgs_id]):
-    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertsmonth/?"
-
-    # collapse abbreviation list, tuple, vector of site_id into query formatted string
-    abbrev = utils._collapse_vector(
-        vect = abbrev, 
-        sep  = "%2C+"
-        )
-
-    # collapse USGS ID list, tuple, vector of site_id into query formatted string
-    usgs_id = utils._collapse_vector(
-        vect = usgs_id, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%Y"
-        )
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True 
-    
-    print("Retrieving monthly surface water time series")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}'
-            f'&min-calYear={start_date or ""}'
-            f'&max-calYear={end_date or ""}'
-            f'&stationNum={station_number or ""}'
-            f'&usgsSiteId={usgs_id or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def _get_sw_ts_wyear(
-    abbrev              = None,
-    station_number      = None,
-    usgs_id             = None,
-    start_date          = None,
-    end_date            = None,
-    api_key             = None
-    ):
-    """Return water year surface water time series data
-
-    Make a request to the /surfacewater/surfacewatertswateryear endpoint to retrieve surface water stations annual time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
-
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
-        station_number (int, str, optional):  surface water station number. Defaults to None.
-        usgs_id (str, optional):  tuple or list of USGS ID. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: annual surface water time series data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [abbrev, station_number, usgs_id]):
-    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertswateryear/?"
-
-    # collapse abbreviation list, tuple, vector of site_id into query formatted string
-    abbrev = utils._collapse_vector(
-        vect = abbrev, 
-        sep  = "%2C+"
-        )
-
-    # collapse USGS ID list, tuple, vector of site_id into query formatted string
-    usgs_id = utils._collapse_vector(
-        vect = usgs_id, 
-        sep  = "%2C+"
-        )
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%Y"
-        )
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving water year surface water time series")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}'
-            f'&min-waterYear={start_date or ""}'
-            f'&max-waterYear={end_date or ""}'
-            f'&stationNum={station_number or ""}'
-            f'&usgsSiteId={usgs_id or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-    
-    return data_df
-
-def get_sw_ts(
-    abbrev              = None,
-    station_number      = None,
-    usgs_id             = None,
-    start_date          = None,
-    end_date            = None,
-    timescale           = None,
-    api_key             = None
-    ):
-
-    """Return surface water time series data
-    
-    Make a request to the /surfacewater/surfacewaterts/ endpoints (surfacewatertsday, surfacewatertsmonth, surfacewatertswateryear) to retrieve surface water station time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates) and at a specified temporal resolution.     
-    
-    Args:
-        station_number (str, optional):  climate data station number. Defaults to None.
-        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
-        station_number (int, str, optional):  surface water station number. Defaults to None.
-        usgs_id (tuple, list, optional):  tuple or list of USGS ID. Defaults to None.
-        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        timescale (str, optional): timestep of the time series data to return, either "day", "month", or "water_year". Defaults to None and will request daily time series.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of surface water station time series data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [abbrev, station_number, usgs_id]):
-    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "start_date", "end_date", "timescale"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # lists of valid timesteps
-    day_lst       = ['day', 'days', 'daily', 'd']
-    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
-    year_lst      = ['wyear', 'water_year', 'wyears', 'water_years', 'wateryear', 'wateryears', 'wy', 'year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
-    timescale_lst = day_lst + month_lst + year_lst
-
-    # if timescale is None, then defaults to "day"
-    if timescale is None: 
-        timescale = "day"
-        
-    # if parameter is NOT in list of valid parameters
-    if timescale not in timescale_lst:
-        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}\n{year_lst}")
-
-    # request daily surface water time series data
-    if timescale in day_lst:    
-        sw_df = _get_sw_ts_day(
-            abbrev              = abbrev,
-            station_number      = station_number,
-            usgs_id             = usgs_id,
-            start_date          = start_date,
-            end_date            = end_date,
-            api_key             = api_key
-            )
-
-        # return daily surface water time series data
-        return sw_df
-
-    # request monthly surface water time series data
-    if timescale in month_lst:    
-
-        sw_df = _get_sw_ts_month(
-            abbrev              = abbrev,
-            station_number      = station_number,
-            usgs_id             = usgs_id,
-            start_date          = start_date,
-            end_date            = end_date,
-            api_key             = api_key
-            )
-
-        # return monthly surface water time series data
-        return sw_df
-
-    # request yearly surface water time series data
-    if timescale in year_lst:    
-
-        sw_df = _get_sw_ts_wyear(
-            abbrev              = abbrev,
-            station_number      = station_number,
-            usgs_id             = usgs_id,
-            start_date          = start_date,
-            end_date            = end_date,
-            api_key             = api_key
-            )
-
-        # return yearly surface water time series data
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_sw_stations(
+    aoi                 = None,
+    radius              = None,
+    abbrev              = None,
+    county              = None,
+    division            = None,
+    station_name        = None,
+    usgs_id             = None,
+    water_district      = None,
+    api_key             = None
+    ):
+    """Return Surface Water Station information
+    
+    Make a request to the /surfacewater/surfacewaterstations endpoint to locate surface water stations via a spatial search, or by station abbreviation, county, division, station name, USGS ID or water_district.  
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        abbrev (str, list, tuple, optional): surface water station abbreviation. Defaults to None.
+        county (str, optional): County to query for surface water stations. Defaults to None.
+        division (int, str, optional):  Water division to query for surface water stations. Defaults to None.
+        station_name (str, optional): surface water station name. Defaults to None.
+        usgs_id (str, tuple or list , optional): USGS IDs. Defaults to None.
+        water_district (int, str, optional): Water district to query for surface water stations. Defaults to None.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+    
+    Returns:
+        pandas dataframe object: dataframe of surface water station data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # collapse abbrev list, tuple, vector of abbrev into query formatted string
+    abbrev = utils._collapse_vector(
+        vect = abbrev, 
+        sep  = "%2C+"
+        )
+
+    # collapse usgs_id list, tuple, vector of usgs_id into query formatted string
+    usgs_id = utils._collapse_vector(
+        vect = usgs_id, 
+        sep  = "%2C+"
+        )
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewaterstations/?"
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving surface water station data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}' 
+            f'&county={county or ""}' 
+            f'&division={division or ""}'
+            f'&stationName={station_name or ""}' 
+            f'&usgsSiteId={usgs_id or ""}'
+            f'&waterDistrict={water_district or ""}' 
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+
+    return data_df
+
+def _get_sw_ts_day(
+    abbrev              = None,
+    station_number      = None,
+    usgs_id             = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return daily surface water time series data
+    
+    Make a request to the /surfacewater/surfacewatertsday endpoint to retrieve surface water stations daily time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
+    
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
+        station_number (int, str, optional):  surface water station number. Defaults to None.
+        usgs_id (tuple, list, optional):  tuple or list of USGS ID. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: daily surface water time series data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [abbrev, station_number, usgs_id]):
+    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertsday/?"
+
+    # collapse abbreviation list, tuple, vector of site_id into query formatted string
+    abbrev = utils._collapse_vector(
+        vect = abbrev, 
+        sep  = "%2C+"
+        )
+
+    # collapse USGS ID list, tuple, vector of site_id into query formatted string
+    usgs_id = utils._collapse_vector(
+        vect = usgs_id, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+    
+    print("Retrieving daily surface water time series")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}'
+            f'&min-measDate={start_date or ""}'
+            f'&max-measDate={end_date or ""}'
+            f'&stationNum={station_number or ""}'
+            f'&usgsSiteId={usgs_id or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # convert measDate columns to 'date' and pd datetime type
+        cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def _get_sw_ts_month(
+    abbrev              = None,
+    station_number      = None,
+    usgs_id             = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return monthly surface water time series data
+    
+    Make a request to the /surfacewater/surfacewatertsmonth endpoint to retrieve surface water stations monthly time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
+    
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        abbrev (tuple, list, optional):  tuple or list of surface water station abbreviation. Defaults to None.
+        station_number (int, str, optional):  surface water station number. Defaults to None.
+        usgs_id (str, optional):  tuple or list of USGS ID. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: monthly surface water time series data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [abbrev, station_number, usgs_id]):
+    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertsmonth/?"
+
+    # collapse abbreviation list, tuple, vector of site_id into query formatted string
+    abbrev = utils._collapse_vector(
+        vect = abbrev, 
+        sep  = "%2C+"
+        )
+
+    # collapse USGS ID list, tuple, vector of site_id into query formatted string
+    usgs_id = utils._collapse_vector(
+        vect = usgs_id, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%Y"
+        )
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True 
+    
+    print("Retrieving monthly surface water time series")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}'
+            f'&min-calYear={start_date or ""}'
+            f'&max-calYear={end_date or ""}'
+            f'&stationNum={station_number or ""}'
+            f'&usgsSiteId={usgs_id or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def _get_sw_ts_wyear(
+    abbrev              = None,
+    station_number      = None,
+    usgs_id             = None,
+    start_date          = None,
+    end_date            = None,
+    api_key             = None
+    ):
+    """Return water year surface water time series data
+
+    Make a request to the /surfacewater/surfacewatertswateryear endpoint to retrieve surface water stations annual time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates)
+
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
+        station_number (int, str, optional):  surface water station number. Defaults to None.
+        usgs_id (str, optional):  tuple or list of USGS ID. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        api_key (str, optional):  API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: annual surface water time series data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [abbrev, station_number, usgs_id]):
+    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base =  "https://dwr.state.co.us/Rest/GET/api/v2/surfacewater/surfacewatertswateryear/?"
+
+    # collapse abbreviation list, tuple, vector of site_id into query formatted string
+    abbrev = utils._collapse_vector(
+        vect = abbrev, 
+        sep  = "%2C+"
+        )
+
+    # collapse USGS ID list, tuple, vector of site_id into query formatted string
+    usgs_id = utils._collapse_vector(
+        vect = usgs_id, 
+        sep  = "%2C+"
+        )
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%Y"
+        )
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving water year surface water time series")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}'
+            f'&min-waterYear={start_date or ""}'
+            f'&max-waterYear={end_date or ""}'
+            f'&stationNum={station_number or ""}'
+            f'&usgsSiteId={usgs_id or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+    
+    return data_df
+
+def get_sw_ts(
+    abbrev              = None,
+    station_number      = None,
+    usgs_id             = None,
+    start_date          = None,
+    end_date            = None,
+    timescale           = None,
+    api_key             = None
+    ):
+
+    """Return surface water time series data
+    
+    Make a request to the /surfacewater/surfacewaterts/ endpoints (surfacewatertsday, surfacewatertsmonth, surfacewatertswateryear) to retrieve surface water station time series data by station abbreviations, station number, or USGS Site IDs within a given date range (start and end dates) and at a specified temporal resolution.     
+    
+    Args:
+        station_number (str, optional):  climate data station number. Defaults to None.
+        abbrev (str, optional):  tuple or list of surface water station abbreviation. Defaults to None.
+        station_number (int, str, optional):  surface water station number. Defaults to None.
+        usgs_id (tuple, list, optional):  tuple or list of USGS ID. Defaults to None.
+        start_date (str, optional): string date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): string date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        timescale (str, optional): timestep of the time series data to return, either "day", "month", or "water_year". Defaults to None and will request daily time series.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of surface water station time series data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [abbrev, station_number, usgs_id]):
+    #     raise TypeError("Invalid 'abbrev', 'station_number', or 'usgs_id' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "start_date", "end_date", "timescale"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # lists of valid timesteps
+    day_lst       = ['day', 'days', 'daily', 'd']
+    month_lst     = ['month', 'months', 'monthly', 'mon', 'm']
+    year_lst      = ['wyear', 'water_year', 'wyears', 'water_years', 'wateryear', 'wateryears', 'wy', 'year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
+    timescale_lst = day_lst + month_lst + year_lst
+
+    # if timescale is None, then defaults to "day"
+    if timescale is None: 
+        timescale = "day"
+        
+    # if parameter is NOT in list of valid parameters
+    if timescale not in timescale_lst:
+        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{day_lst}\n{month_lst}\n{year_lst}")
+
+    # request daily surface water time series data
+    if timescale in day_lst:    
+        sw_df = _get_sw_ts_day(
+            abbrev              = abbrev,
+            station_number      = station_number,
+            usgs_id             = usgs_id,
+            start_date          = start_date,
+            end_date            = end_date,
+            api_key             = api_key
+            )
+
+        # return daily surface water time series data
+        return sw_df
+
+    # request monthly surface water time series data
+    if timescale in month_lst:    
+
+        sw_df = _get_sw_ts_month(
+            abbrev              = abbrev,
+            station_number      = station_number,
+            usgs_id             = usgs_id,
+            start_date          = start_date,
+            end_date            = end_date,
+            api_key             = api_key
+            )
+
+        # return monthly surface water time series data
+        return sw_df
+
+    # request yearly surface water time series data
+    if timescale in year_lst:    
+
+        sw_df = _get_sw_ts_wyear(
+            abbrev              = abbrev,
+            station_number      = station_number,
+            usgs_id             = usgs_id,
+            start_date          = start_date,
+            end_date            = end_date,
+            api_key             = api_key
+            )
+
+        # return yearly surface water time series data
         return sw_df
```

### Comparing `cdsspy-1.2.70/cdsspy/telemetry.py` & `cdsspy-1.2.71/cdsspy/telemetry.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,286 +1,286 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-from cdsspy import utils
-
-def get_telemetry_stations(
-    aoi            = None,
-    radius         = None,
-    abbrev         = None,
-    county         = None,
-    division       = None,
-    gnis_id        = None,
-    usgs_id        = None,
-    water_district = None,
-    wdid           = None,
-    api_key        = None
-    ):
-    """Return Telemetry Station info
-
-    Make a request to the /telemetrystations/telemetrystation endpoint to locate telemetry stations via a spatial search, or by station abbreviation, county, division, GNIS ID, USGS ID, water_district or WDID.  
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        abbrev (str, tuple, list, optional): Abbreviation name (or list of abbreviations) of the telemetry station. Defaults to None.
-        county (str, optional): County to query for telemetry stations. Defaults to None.
-        division (int, str, optional):  Water division to query for telemetry stations. Defaults to None.
-        gnis_id (str, optional): GNIS ID of the telemetry station. Defaults to None.
-        usgs_id (str, optional): USGS ID of the telemetry station. Defaults to None.
-        water_district (int, str, optional): Water district to query for telemetry stations. Defaults to None.
-        wdid (str, optional): WDID of the telemetry station. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-
-    Returns:
-        pandas dataframe object: dataframe of telemetry station data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [aoi, abbrev, county, division, gnis_id, usgs_id, water_district, wdid]):
-    #     raise TypeError("Invalid 'aoi', 'abbrev', 'county', 'division', 'gnis_id', 'usgs_id', 'water_district', or 'wdid' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    # base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/telemetrystations/telemetrystation/?"
-
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # collapse site_id list, tuple, vector of site_id into query formatted string
-    abbrev = utils._collapse_vector(
-        vect = abbrev, 
-        sep  = "%2C+"
-        )
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving telemetry station data")
-    
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}'
-            f'&county={county or ""}'
-            f'&division={division or ""}'
-            f'&gnisId={gnis_id or ""}'
-            f'&includeThirdParty=true'
-            f'&usgsStationId={usgs_id or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&wdid={wdid or ""}'
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if (len(cdss_df.index) < page_size):
-            more_pages = False
-        else:
-            page_index += 1
-    
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-
-    return data_df
-
-def get_telemetry_ts(
-    abbrev              = None,
-    parameter           = "DISCHRG",
-    start_date          = None,
-    end_date            = None,
-    timescale           = None,
-    include_third_party = True,
-    api_key             = None
-    ):
-    """Return Telemetry station time series data
-
-    Make a request to the /telemetrystations/telemetrytimeseries endpoint to retrieve raw, hourly, or daily telemetry station time series data by station abbreviations, within a given date range (start and end dates).
-
-    Args:
-        abbrev (str, optional): Station abbreviation. Defaults to None.
-        parameter (str, optional): Indicating which telemetry station parameter should be retrieved. Default is "DISCHRG" (discharge), all parameters are not available at all telemetry stations. Defaults to "DISCHRG".
-        start_date (str, optional): Date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
-        end_date (str, optional): Date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
-        timescale (str, optional): Data timescale to return, either "raw", "hour", or "day". Defaults to None and will request daily time series.
-        include_third_party (bool, optional): Boolean, indicating whether to retrieve data from other third party sources if necessary. Defaults to True.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of telemetry station time series data
-    """
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key", "parameter", "start_date", "end_date", "timescale"],
-        f        = any
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-    
-    # lists of valid timesteps
-    timescale_lst = ["day", "hour", "raw"]
-
-    # if timescale is None, then defaults to "day"
-    if timescale is None: 
-        timescale = "day"
-        
-    # if parameter is NOT in list of valid parameters
-    if timescale not in timescale_lst:
-        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{timescale_lst}")
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/telemetrystations/telemetrytimeseries" + timescale + "/?"
-
-    # parse start_date into query string format
-    start_date = utils._parse_date(
-        date   = start_date,
-        start  = True,
-        format = "%m-%d-%Y"
-    )
-
-    # parse end_date into query string format
-    end_date = utils._parse_date(
-        date   = end_date,
-        start  = False,
-        format = "%m-%d-%Y"
-        )
-    
-    # Create True or False include 3rd party string
-    third_party_str = str(include_third_party).lower()
-
-    # maximum records per page
-    page_size  = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df    = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print(f"Retrieving telemetry station time series data ({timescale} - {parameter})")
-
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-        
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&abbrev={abbrev or ""}'
-            f'&endDate={end_date or ""}'
-            f'&startDate={start_date or ""}'
-            f'&includeThirdParty={third_party_str or ""}'
-            f'&parameter={parameter or ""}'
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-        
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df  = cdss_req.json() 
-        cdss_df  = pd.DataFrame(cdss_df)
-        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
-        
-        # convert measDateTime and measDate columns to 'date' and pd datetime type
-        if timescale == "raw":
-            # convert measDate column to datetime column
-            cdss_df['measDateTime'] = pd.to_datetime(cdss_df['measDateTime'])
-
-        else: 
-            # convert measDate column to datetime column
-            cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-        
-        # Check if more pages to get to continue/stop while loop
-        if(len(cdss_df.index) < page_size): 
-            more_pages = False
-        else:
-            page_index += 1
-
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+from cdsspy import utils
+
+def get_telemetry_stations(
+    aoi            = None,
+    radius         = None,
+    abbrev         = None,
+    county         = None,
+    division       = None,
+    gnis_id        = None,
+    usgs_id        = None,
+    water_district = None,
+    wdid           = None,
+    api_key        = None
+    ):
+    """Return Telemetry Station info
+
+    Make a request to the /telemetrystations/telemetrystation endpoint to locate telemetry stations via a spatial search, or by station abbreviation, county, division, GNIS ID, USGS ID, water_district or WDID.  
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        abbrev (str, tuple, list, optional): Abbreviation name (or list of abbreviations) of the telemetry station. Defaults to None.
+        county (str, optional): County to query for telemetry stations. Defaults to None.
+        division (int, str, optional):  Water division to query for telemetry stations. Defaults to None.
+        gnis_id (str, optional): GNIS ID of the telemetry station. Defaults to None.
+        usgs_id (str, optional): USGS ID of the telemetry station. Defaults to None.
+        water_district (int, str, optional): Water district to query for telemetry stations. Defaults to None.
+        wdid (str, optional): WDID of the telemetry station. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+
+    Returns:
+        pandas dataframe object: dataframe of telemetry station data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [aoi, abbrev, county, division, gnis_id, usgs_id, water_district, wdid]):
+    #     raise TypeError("Invalid 'aoi', 'abbrev', 'county', 'division', 'gnis_id', 'usgs_id', 'water_district', or 'wdid' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    # base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/telemetrystations/telemetrystation/?"
+
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # collapse site_id list, tuple, vector of site_id into query formatted string
+    abbrev = utils._collapse_vector(
+        vect = abbrev, 
+        sep  = "%2C+"
+        )
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving telemetry station data")
+    
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}'
+            f'&county={county or ""}'
+            f'&division={division or ""}'
+            f'&gnisId={gnis_id or ""}'
+            f'&includeThirdParty=true'
+            f'&usgsStationId={usgs_id or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&wdid={wdid or ""}'
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if (len(cdss_df.index) < page_size):
+            more_pages = False
+        else:
+            page_index += 1
+    
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+
+    return data_df
+
+def get_telemetry_ts(
+    abbrev              = None,
+    parameter           = "DISCHRG",
+    start_date          = None,
+    end_date            = None,
+    timescale           = None,
+    include_third_party = True,
+    api_key             = None
+    ):
+    """Return Telemetry station time series data
+
+    Make a request to the /telemetrystations/telemetrytimeseries endpoint to retrieve raw, hourly, or daily telemetry station time series data by station abbreviations, within a given date range (start and end dates).
+
+    Args:
+        abbrev (str, optional): Station abbreviation. Defaults to None.
+        parameter (str, optional): Indicating which telemetry station parameter should be retrieved. Default is "DISCHRG" (discharge), all parameters are not available at all telemetry stations. Defaults to "DISCHRG".
+        start_date (str, optional): Date to request data start point YYYY-MM-DD. Defaults to None, which will return data starting at "1900-01-01".
+        end_date (str, optional): Date to request data end point YYYY-MM-DD. Defaults to None, which will return data ending at the current date.
+        timescale (str, optional): Data timescale to return, either "raw", "hour", or "day". Defaults to None and will request daily time series.
+        include_third_party (bool, optional): Boolean, indicating whether to retrieve data from other third party sources if necessary. Defaults to True.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of telemetry station time series data
+    """
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key", "parameter", "start_date", "end_date", "timescale"],
+        f        = any
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+    
+    # lists of valid timesteps
+    timescale_lst = ["day", "hour", "raw"]
+
+    # if timescale is None, then defaults to "day"
+    if timescale is None: 
+        timescale = "day"
+        
+    # if parameter is NOT in list of valid parameters
+    if timescale not in timescale_lst:
+        raise ValueError(f"Invalid `timescale` argument: '{timescale}'\nPlease enter one of the following valid timescales: \n{timescale_lst}")
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/telemetrystations/telemetrytimeseries" + timescale + "/?"
+
+    # parse start_date into query string format
+    start_date = utils._parse_date(
+        date   = start_date,
+        start  = True,
+        format = "%m-%d-%Y"
+    )
+
+    # parse end_date into query string format
+    end_date = utils._parse_date(
+        date   = end_date,
+        start  = False,
+        format = "%m-%d-%Y"
+        )
+    
+    # Create True or False include 3rd party string
+    third_party_str = str(include_third_party).lower()
+
+    # maximum records per page
+    page_size  = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df    = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print(f"Retrieving telemetry station time series data ({timescale} - {parameter})")
+
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+        
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&abbrev={abbrev or ""}'
+            f'&endDate={end_date or ""}'
+            f'&startDate={start_date or ""}'
+            f'&includeThirdParty={third_party_str or ""}'
+            f'&parameter={parameter or ""}'
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+        
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df  = cdss_req.json() 
+        cdss_df  = pd.DataFrame(cdss_df)
+        cdss_df  = cdss_df["ResultList"].apply(pd.Series) 
+        
+        # convert measDateTime and measDate columns to 'date' and pd datetime type
+        if timescale == "raw":
+            # convert measDate column to datetime column
+            cdss_df['measDateTime'] = pd.to_datetime(cdss_df['measDateTime'])
+
+        else: 
+            # convert measDate column to datetime column
+            cdss_df['measDate'] = pd.to_datetime(cdss_df['measDate'])
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+        
+        # Check if more pages to get to continue/stop while loop
+        if(len(cdss_df.index) < page_size): 
+            more_pages = False
+        else:
+            page_index += 1
+
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy/utils.py` & `cdsspy-1.2.71/cdsspy/utils.py`

 * *Ordering differences only*

 * *Files 16% similar despite different names*

```diff
@@ -1,915 +1,915 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-def _check_args(
-        arg_dict = None, 
-        ignore   = None,
-        f        = any
-        ):
-    """Check all arguments of a function for any/all NULL values
-    
-    Internal function for checking a function arguments for any/all invalid/missing arguments necessary to the function it is called within
-    
-    Args:
-        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
-        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
-        f (built-in function): Built in function "any" or "all" to indicate whether to check for "any" or "all" None argument. 
-            If "any" then if any of the function arguments are None, then an error is thrown.
-            If "all" then all relevant arguments must be None for an error to be thrown. Defaults to any.
-
-    Returns:
-        string: error statement with any/all None arguments listed, or None if no error is thrown by None values
-    """
-
-    # if no function arguments are given, throw an error
-    if arg_dict is None:
-        raise Exception("provide a list of function arguments by calling 'locals()', within another function")
-
-    # argument dictionary key/values as lists
-    key_lst  = list(arg_dict.keys())
-    val_lst  = list(arg_dict.values())
-
-    # if certain arguments are specifically supposed to be ignored
-    if ignore is not None:
-        
-        # remove specifically ignorged arguments
-        ignored_lst = [i for i, x in enumerate(key_lst) if x not in ignore]
-
-        # keys and values of arguments to keep
-        key_args        = [key_lst[i] for i in ignored_lst]
-        val_args        = [val_lst[i] for i in ignored_lst]
-    else:
-        
-        # if no arguments are ignored, keep all argument key/values
-        key_args        = key_lst
-        val_args        = val_lst
-
-    # if any/all arguments are None, return an error statement. Otherwise return None if None check is passed
-    if(f(i is None for i in val_args)):
-        # check where in remaining arguments the value is None, and get the index of missing arguments
-        idx_miss = [i for i in range(len(val_args)) if val_args[i] == None]
-
-        # return the argument names of None arguments
-        key_miss = ", ".join(["'"+key_lst[i]+"'" for i in idx_miss])
-
-        # error print statement
-        err_msg = "Invalid or missing " + key_miss + " arguments"
-
-        return err_msg
-    else:
-        return None
-    
-def _align_wcid(
-        x       = None, 
-        default = None
-        ):
-    """Set wc_identifier name to releases or diversions
-
-    Args:
-        x (str): Water class identifier. Defaults to None 
-        default (str, int, bool, Nonetype, optional):  value to return if "x" argument is None. Defaults to None.
-
-    Returns:
-        string: wc_identifier equaling either "diversion", "release", or a properly formatted water class identifier string
-    """
-    # if x is NULL/ not given, return "default"
-    if x is None:
-        return default
-    
-    # check if x is not in any of diversion/release lists
-    if x not in ["diversion", "diversions", "div", "divs", "d", 
-                "release", "releases", "rel", "rels", "r"]:
-        
-        # format wcidentifer query
-        x = "+".join([i.replace(":", "%3A") for i in x.split(" ")])
-
-    # if x in the diversions list
-    if x in ["diversion", "diversions", "div", "divs", "d"]:
-        x = "diversion"
-
-    # if x in the releases list
-    if x in ["release", "releases", "rel", "rels", "r"]:
-        x = "release"
-
-    x = "*" + x + "*"
-
-    return x
-def _valid_divrectype(
-        divrectype = None
-        ):
-
-    # check if type is NULL, default timescale to "day"
-    if divrectype is None:
-
-        divrectype = None
-
-        return divrectype
-    
-    # list of available divrectypes
-    divrectype_lst <- ["DivComment", "DivTotal", "RelComment", "RelTolal", "StageVolume", "WaterClass"]
-
-    # if a divrectype argument is provided (not NULL)
-    if divrectype is not None:
-
-        # lowercase divrectype_lst 
-        low_lst = [i.lower() for i in divrectype_lst]
-
-        # if divrectype matches any of the list, return correctly formatted divrectype
-        if divrectype.lower() in low_lst:
-            
-            divrectype = divrectype_lst[low_lst.index(divrectype.lower())]
-        
-
-        # check if divrectype is a valid divrectype
-        if divrectype.lower() not in low_lst and divrectype not in divrectype_lst:
-            raise Exception((
-                f"Invalid `divrectype` argument: '{divrectype}'",
-                f"\nPlease enter one of the following valid 'divrectype' arguments: \n{divrectype_lst}" 
-                ))
-
-    return(divrectype)
-
-def _valid_timesteps(
-        timestep = None
-        ):
-    
-    # list of valid timescales
-    day_lst       = ["day", "days", "daily", "d"]
-    month_lst     = ["month", "months", "monthly", "mon", "mons", "m"]
-    year_lst      = ['year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
-
-    timestep_lst  = [day_lst, month_lst, year_lst]
-
-    # check if type is None, default timescale to "day"
-    if timestep is None:
-        # set timescale to "day"
-        timestep = "day"
-
-    # convert timescale to lowercase
-    timestep = timestep.lower()
-    
-    # check if type is correctly inputed
-    if timestep not in timestep_lst: 
-        raise Exception((
-            f"Invalid `timestep` argument: '{timestep}'",
-            f"\nPlease enter one of the following valid timesteps:\nDay: {day_lst}\nMonth: {month_lst}\nYear: {year_lst}" 
-            ))
-    
-    # check if given timestep is in day_lst and set timestep to "day"
-    if timestep in day_lst:
-
-        # set timescale to "day"
-        timestep = "day"
-
-    # check if given timestep is in month_lst and set timestep to "month"
-    if timestep in month_lst:
-        
-        # set timescale to "mohth"
-        timestep = "month"
-
-    # check if given timestep is in month_lst and set timestep to "month"
-    if timestep in year_lst:
-        
-        # set timescale to "year"
-        timestep = "year"
-
-    return timestep
-
-def _parse_date(
-    date   = None,
-    start  = True,
-    format =  "%m-%d-%Y"
-    ):
-
-    # if the date is the starting date
-    if start == True:
-
-        # if no start_date is given, default to 1900-01-01
-        if date is None:
-            date = "1900-01-01"
-            date = datetime.datetime.strptime(date, '%Y-%m-%d')
-            date = date.strftime(format)
-            date = date.replace("-", "%2F")
-        else:
-            date = datetime.datetime.strptime(date, '%Y-%m-%d')
-            date = date.strftime(format)
-            date = date.replace("-", "%2F") 
-
-    # if date is the ending date
-    else:
-
-        # if no end date is given, default to current date
-        if date is None: 
-            date   = datetime.date.today()
-            date   = date.strftime(format)
-            date   = date.replace("-", "%2F")
-        else:
-            date   = datetime.datetime.strptime(date, '%Y-%m-%d')
-            date   = date.strftime(format)
-            date   = date.replace("-", "%2F")
-
-    return date
-
-def _collapse_vector(
-    vect = None, 
-    sep  = "%2C+"
-    ):
-    
-    # if a list of vects, collapse list
-    if type(vect) == list or type(vect) == tuple:
-        vect = [str(x) for x in vect]
-        # join list into single string seperated by 'sep'
-        vect = sep.join(vect)
-        
-        # replace white space w/ 'sep'
-        vect = vect.replace(" ", sep)
-    else:
-        # if vect is an int or float, convert to string
-        if type(vect) == int or type(vect) == float:
-            vect = str(vect)
-        
-        if type(vect) == str:
-            # replace white space w/ plus sign
-            vect = vect.replace(" ", sep)
-    
-    return vect
-
-def _batch_dates(
-        start_date = None,
-        end_date   = None
-        ):
-    
-    """Create yearly date ranges to make batch GET requests
-
-    Internal function for extracting necessary yearly start and end dates to make a batch of smaller GET requests, instead 1 large date range. 
-    Allows for larger date ranges to be queried from the CDSS API without encountering a server side error.
-
-    Args:
-        start_date (str): starting date in YYYY-MM-DD format. Default is None which defaults start_date to "1900-01-01".
-        end_date (str): ending date in YYYY-MM-DD format. Default is None which defaults to the current date.
-    
-    Returns:
-        list: returns list of date range lists
-    """
-
-    # set default start date if None is given 
-    if start_date is None:
-        start_date = "1900-01-01"
-
-    # set default end_date if None is given 
-    if end_date is None:
-        end_date   = datetime.date.today()
-        end_date   = end_date.strftime('%Y-%m-%d')
-
-    # starting and ending years
-    start_year = int(start_date[:4])
-    end_year   = int(end_date[:4])
-
-    # empty list add date intervals to
-    lst = []
-
-    # if dates are multiple years apart, break into yearly date intervals
-    if start_year != end_year:
-
-        # start_date to end of first year
-        lst.append((start_date, f"{start_year}-12-31"))
-
-        # yearly intervals
-        for y in range(start_year + 1, end_year):
-            lst.append((f"{y}-01-01", f"{y}-12-31"))
-
-        # portion of the last year
-        lst.append((f"{end_year}-01-01", end_date))
-
-    # if dates are within the same year, just return start_date to end_date
-    else:
-        lst.append((start_date, end_date))
-
-    return(lst)
-
-def _get_error_handler(
-    url      = None
-    ):
-
-    """ Make GET requests and return the responses
-
-    Internal function for making get request and returning unsuccesful response text. 
-    Used within a try, except block within _parse_gets() function.
-
-    Args:
-        url (str, optional): URL of the request
-    
-    Returns:
-        requests.models.Response: returns results of attempted get request   
-    """
-
-    # If NO url is given
-    if(url is None):
-        raise Exception('Please provide a URL to perform a get request')
-    
-    # make API call
-
-    # attempt GET request
-    req_attempt = requests.get(url)
-
-    # if request is 200 (OK), return JSON content data
-    if req_attempt.status_code == 200:
-        # return successful response
-        return req_attempt
-    else:
-        # return req_attempt.text
-        raise Exception(req_attempt.text)
-    
-
-def _parse_gets(
-        url      = None, 
-        arg_dict = None, 
-        ignore   = None
-        ):
-    
-    """ Makes GET requests and dynamically handle errors 
-
-    Internal function for handling GET requests and associated errors.
-    Function will try to make a GET request, and if an error occurs, the function 
-    will return an error message with relevenant information detailing the error 
-    and the inputs that led to the error.
-
-    Args:
-        url (str): URL of the request
-        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
-        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
-    
-    Returns:
-        requests response: returns results of attempted get request 
-    """
-
-    # try to make GET request and error handling unsuccessful requests
-    try:
-        # attempt GET request
-        req = _get_error_handler(url = url)
-
-        return(req)
-    
-    except Exception as e:
-
-        # if an error occurred, use _query_error() to format a helpful error message to user
-        raise Exception(_query_error(
-            arg_dict = arg_dict,
-            url      = url,
-            ignore   = ignore,
-            e_msg    = e
-            )
-            )
-    
-def _query_error(
-        arg_dict = None,
-        url      = None,
-        ignore   = None,
-        e_msg    = None
-        ):
-    """GET Request Error message handler
-
-    Internal function for generating dynamic error messages for failed GET requests.
-    Designed to be called within another function and print out the functions input arguments.
-
-    Args:
-        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
-        url (str): URL of the request. Defaults to None.
-        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
-        e_msg (exception, str): exception message or string message that should be pointed to as the original error message. Defaults to None.
-
-    Returns:
-        str: error message that includes the query inputs that led to the error, the requested URL, and the original error message
-    """
-
-    # if no function arguments are given, throw an error
-    if arg_dict is None:
-        raise Exception("provide a list of function arguments by calling 'locals()', within another function")
-    
-    # argument dictionary key/values as lists
-    key_lst  = list(arg_dict.keys())
-    val_lst  = list(arg_dict.values())
-
-    # if certain arguments are specifically supposed to be ignored
-    if ignore is not None:
-        
-        # remove specifically ignorged arguments
-        ignored_lst = [i for i, x in enumerate(key_lst) if x not in ignore]
-
-        # keys and values of arguments to keep
-        key_args        = [key_lst[i] for i in ignored_lst]
-        val_args        = [val_lst[i] for i in ignored_lst]
-    else:
-        
-        # if no arguments are ignored, keep all argument key/values
-        key_args        = key_lst
-        val_args        = val_lst
-
-    # query_dict = dict(zip(key_args, val_args))
-
-    q_lst = []
-
-    for i in range(len(key_args)):
-            q_lst.append(f'{key_args[i]}: {val_args[i]}')
-
-    q_msg = ("DATA RETRIEVAL ERROR\nQuery:\n" + '\n'.join(q_lst) +
-            "\nRequested URL: " + url + 
-            "\n\n" + "Original error message: " + "\n-----------------------\n\n" + str(e_msg)
-            )
-
-    return q_msg
-
-def _get_error_handler2(
-    url     = None
-    ):
-
-    """
-    Internal function for making get request and error handling unsuccessful requests
-
-    Args:
-        url (str, optional): URL of the request
-    
-    Returns:
-        requests.models.Response: returns results of attempted get request   
-    """
-
-    # If NO url is given
-    if(url is None):
-        raise Exception('Please provide a URL to perform a get request')
-    
-    # make API call
-    try:
-        # attempt GET request
-        req_attempt = requests.get(url)
-
-        req_attempt.raise_for_status()
-
-        # return successful response
-        return req_attempt
-
-    except requests.exceptions.HTTPError as errh:
-        print("HTTP Error:\n", errh)
-        print("\nClient response:\n", errh.response.text)
-        raise
-    except requests.exceptions.ConnectionError as errc:
-        print("Connection Error:\n", errc)
-        print("\nClient response:\n", errc.response.text)
-        raise
-    except requests.exceptions.Timeout as errt:
-        print("Timeout Error:\n", errt)
-        print("\nClient response:\n", errt.response.text)
-        raise
-    except requests.exceptions.RequestException as err:
-        print("Exception raised:\n", err)
-        print("\nClient response:\n", err.response.text)
-        raise
-
-def _aoi_error_msg():
-    """
-    Function to return error message to user when aoi is not valid.
-    Returns:
-        string: print statement for aoi errors
-    """
-
-    msg = ("\nInvalid 'aoi' argument, 'aoi' must be one of the following:\n" + 
-    "1. List/Tuple of an XY coordinate pair\n" +
-    "2. Dictionary with X and Y keys\n" +
-    "3. Pandas DataFrame containing XY coordinates\n" +
-    "4. a shapely Point/Polygon/LineString\n" +
-    "5. Geopandas GeoDataFrame containing a Polygon/LineString/LinearRing/Point geometry\n" +
-    "6. Geopandas GeoSeries containing a Polygon/LineString/Point geometry\n")
-
-    return msg
-
-def _check_coord_crs(epsg_code, lng, lat):
-
-    """Function that checks if a set of longitude and latitude points are within a given EPSG space.
-
-    Returns:
-        boolean: True if the coordinates are within the provided EPSG space, False otherwise.
-    """
-    # given crs epsg code
-    crs = pyproj.CRS.from_user_input(epsg_code)
-
-    # if lng/lat fall within CRS space
-    if((crs.area_of_use.south <= lat <= crs.area_of_use.north) and (crs.area_of_use.west <= lng <= crs.area_of_use.east)):
-        crs_check = True
-    else:
-        crs_check = False
-
-    return crs_check
-
-def _extract_shapely_coords(aoi):
-    """Function for extracting coordinates from a shapely Polygon/LineString/Point
-    Internal helper function used in location search queries.
-
-    Args:
-        aoi (shapely Polygon/LineString/Point): shapely Polygon/LineString/Point object to extract coordinates from
-
-    Returns:
-        list: list of string coordinates with precision of 5 decimal places
-    """
-
-    # ensure that the shapely geometry is either a Polygon, LineString or a Point
-    if(isinstance(aoi, (shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString, shapely.geometry.point.Point))):
-
-        # if geometry is Polygon or Linestring
-        if(isinstance(aoi, (shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString))):
-            # extract lng/lat coords
-            lng = aoi.centroid.x
-            lat = aoi.centroid.y
-
-            # lng, lat coordinates
-            coord_lst = [lng, lat]
-            
-            # Valid coords in correct CRS space
-            if(_check_coord_crs(epsg_code = 4326, lng = lng, lat = lat)):
-
-                # round coordinates to 5 decimal places
-                coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                # return list of coordinates
-                return coord_lst
-
-            else:
-                raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
-
-        # if geometry is a Point
-        if(isinstance(aoi, (shapely.geometry.point.Point))):
-            # extract lng/lat coords
-            lng = aoi.x
-            lat = aoi.y
-            
-            # lng, lat coordinates
-            coord_lst = [lng, lat]
-
-            # Valid coords in correct CRS space
-            if(_check_coord_crs(epsg_code = 4326, lng = lng, lat = lat)):
-
-                # round coordinates to 5 decimal places
-                coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                # return list of coordinates
-                return coord_lst
-
-            else:
-                raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
-    else:
-        raise Exception("Invalid 'aoi' shapely geometry, must be either a shapely Polygon, LineString or Point")
-
-
-
-def _extract_coords(
-    aoi = None
-    ):
-
-    """Internal function for extracting XY coordinates from aoi arguments
-    Function takes in a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries of spatial objects,
-    and returns a list of length 2, indicating the XY coordinate pair. 
-    If the object provided is a Polygon/LineString/LinearRing, the function will return the XY coordinates of the centroid of the spatial object.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-    
-    Returns:
-        list object: list object of an XY coordinate pair
-    """
-    # if None is passed to 'aoi', return None
-    if aoi is None: 
-
-        return None
-
-    # if 'aoi' is NOT none, extract XY coordinates from object
-    else:
-
-        # make sure 'aoi' is one of supported types
-        if(isinstance(aoi, (list, tuple, dict, geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame, 
-        pd.core.frame.DataFrame, shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString, shapely.geometry.point.Point)) is False):
-            raise Exception(_aoi_error_msg())
-
-        # check if aoi is a list or tuple
-        if(isinstance(aoi, (list, tuple))):
-
-            if(len(aoi) >= 2):
-
-                # make coordinate list of XY values
-                coord_lst = [aoi[0], aoi[1]]
-
-                # round coordinates to 5 decimal places
-                coord_lst = [float(num) for num in coord_lst]
-
-                # Valid coords in correct CRS space
-                if(_check_coord_crs(epsg_code = 4326, lng = coord_lst[0], lat = coord_lst[1])):
-
-                    # round coordinates to 5 decimal places
-                    coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                    # return list of coordinates
-                    return coord_lst
-
-                else:
-                    raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
-
-            else:
-
-                # return list of coordinates
-                raise Exception(_aoi_error_msg())
-
-        # check if aoi is a shapely Polygon/LineString/Point
-        if("shapely" in str(type(aoi))):
-
-            # extract coordinates from shapely geometry objects
-            coord_lst = _extract_shapely_coords(aoi = aoi)
-
-            return coord_lst 
-
-        # check if aoi is a geopandas geoseries or geodataframe 
-        if(isinstance(aoi, (geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame))):
-            
-            if(len(aoi) > 1):
-                raise Exception(_aoi_error_msg())
-
-            # convert CRS to 5070
-            aoi = aoi.to_crs(5070)
-
-            # if aoi geometry type is polygon/line/linearRing
-            if(["Polygon", 'LineString', 'LinearRing'] in aoi.geom_type.values):
-
-                # checking if point is geopandas Geoseries
-                if(isinstance(aoi, (geopandas.geoseries.GeoSeries))):
-
-                    # get centroid of polygon, and convert to 4326 and add lng/lat as column
-                    lng = float(aoi.centroid.to_crs(4326).geometry.x)
-                    lat = float(aoi.centroid.to_crs(4326).geometry.y)
-
-                    # lng, lat coordinates
-                    coord_lst = [lng, lat]
-                    
-                    # round coordinates to 5 decimal places
-                    coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                    # return list of coordinates
-                    return coord_lst
-
-                # checking if point is geopandas GeoDataFrame
-                if(isinstance(aoi, (geopandas.geodataframe.GeoDataFrame))):
-
-                    # get centroid of polygon, and convert to 4326 and add lng/lat as column
-                    aoi["lng"] = aoi.centroid.to_crs(4326).map(lambda p: p.x)
-                    aoi["lat"] = aoi.centroid.to_crs(4326).map(lambda p: p.y)
-
-                    # subset just lng/lat cols
-                    aoi_coords = aoi.loc[ : , ['lng', 'lat']]
-
-                    # extract lat/lng from centroid of polygon
-                    lng = float(aoi_coords["lng"])
-                    lat = float(aoi_coords["lat"])
-
-                    # lng, lat coordinates
-                    coord_lst = [lng, lat]
-                    
-                    # round coordinates to 5 decimal places
-                    coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                    # return list of coordinates
-                    return coord_lst
-
-            # if aoi geometry type is point
-            if("Point" in aoi.geom_type.values):
-
-                # checking if point is geopandas Geoseries
-                if(isinstance(aoi, (geopandas.geoseries.GeoSeries))):
-
-                    # convert to 4326, and extract lat/lng from Pandas GeoSeries
-                    lng = float(aoi.to_crs(4326).x)
-                    lat = float(aoi.to_crs(4326).y)
-
-                    # lng, lat coordinates
-                    coord_lst = [lng, lat]
-                    
-                    # round coordinates to 5 decimal places
-                    coord_lst = [f'{num:.5f}' for num in coord_lst]
-                    
-                    # return list of coordinates
-                    return coord_lst
-
-                # checking if point is geopandas GeoDataFrame
-                if(isinstance(aoi, (geopandas.geodataframe.GeoDataFrame))):
-
-                    # convert to 4326, and extract lat/lng from Pandas GeoDataFrame
-                    lng = float(aoi.to_crs(4326)['geometry'].x)
-                    lat = float(aoi.to_crs(4326)['geometry'].y)
-                
-                    # lng, lat coordinates
-                    coord_lst = [lng, lat]
-
-                    # round coordinates to 5 decimal places
-                    coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-                    # return list of coordinates
-                    return coord_lst
-                    
-        # check if aoi is a Pandas dataframe
-        if(isinstance(aoi, (pd.core.frame.DataFrame))):
-            
-            # extract first and second columns
-            lng = float(aoi.iloc[:, 0])
-            lat = float(aoi.iloc[:, 1])
-
-            # lng, lat coordinates
-            coord_lst = [lng, lat]
-            
-            # round coordinates to 5 decimal places
-            coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-            # return list of coordinates
-            return coord_lst
-
-        # check if aoi is a dictionary
-        if(isinstance(aoi, (dict))):
-            
-            # extract "X" and "Y" dict keys
-            lng = float(aoi["X"])
-            lat = float(aoi["Y"])
-
-            # lng, lat coordinates
-            coord_lst = [lng, lat]
-            
-            # round coordinates to 5 decimal places
-            coord_lst = [f'{num:.5f}' for num in coord_lst]
-
-            # return list of coordinates
-            return coord_lst
-
-def _check_radius(
-    aoi    = None,
-    radius = None
-    ):
-
-    """Internal function for radius argument value is within the valid value range for location search queries. 
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None.
-
-    Returns:
-        int: radius value between 1-150 miles
-    """
-    # convert str radius value to int
-    if(isinstance(radius, (str))):
-        radius = int(radius)
-
-    # if spatial data is provided, check type and try to extract XY coordinates
-    if aoi is not None:
-        # print("AOI arg is NOT None")
-
-        # if radius is not NULL, and is larger than 150, set to max of 150. if NULL radius is provided with spatial data, default to 150 miles
-        if radius is not None:
-            # print("radius arg is NOT None")
-            
-            # if radius value is over max, set to 150
-            if(radius > 150):
-
-                # print("radius arg > 150, so set to 150")
-                radius = 150
-
-            # if radius value is under min, set to 1
-            if(radius <= 0):
-                # print("radius arg <= 0, so set to 1")
-                radius = 1
-
-        # if no radius given, set to 20 miles
-        else:
-            # print("radius arg is None, default to 20 miles")
-            radius = 20
-    else:
-        # print("AOI arg is None")
-        radius = None
-    
-    # Return radius value
-    return radius
-
-
-def _check_aoi(
-    aoi    = None, 
-    radius = None
-    ):
-
-    """Internal function for checking AOI and radius arguments are valid for use in location search queries.
-    Function takes in a list/tuple of an XY coordinate pair, a Pandas Dataframe, or a Geopandas GeoDataFrame/GeoSeries of spatial objects,
-    along with a radius value between 1-150 miles.
-    The extracts the necessary coordinates from the given aoi parameter and also makes sure the radius value is within the valid value range. 
-    The function then returns a list of length 2, indicating the XY coordinate pair. 
-    If the object provided is a Polygon/LineString/LinearRing, the function will return the XY coordinates of the centroid of the spatial object.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None.
-
-    Returns:
-        list: list containing the latitude, longitude, and radius values to use for location search queries.
-    """
-
-    # convert str radius value to int
-    if(isinstance(radius, (str))):
-        radius = int(radius)
-
-    # extract lat/long coords for query
-    if(aoi is not None):
-        # extract coordinates from matrix/dataframe/sf object
-        coord_df = _extract_coords(aoi = aoi)
-        
-        # check radius is valid and fix if necessary
-        radius = _check_radius(
-            aoi    = aoi,
-            radius = radius
-            )
-
-        # lat/long coords
-        lng = coord_df[0]
-        lat = coord_df[1]
-    
-    else:
-        # if None aoi given, set coords and radius to None
-        lng    = None
-        lat    = None
-        radius = None
-    
-    # create list to return container longitude, latitude, and radius
-    aoi_lst = [lng, lat, radius]
-    
-    # return lng, lat, radius list
-    return aoi_lst  
-
-def _aoi_mask(
-    aoi = None,
-    pts = None
-    ):
-
-    """For location search queries using a polygon, the response data from the CDSS API will be masked to the polygon area, removing any extra points.
-    Internal helper function, if aoi is None, then the function will just return the original dataset. 
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        pts (pandas dataframe): pandas dataframe of points that should be masked to the given aoi. Dataframe must contain "utmY" and "utmX" columns
-
-    Returns:
-        pandas dataframe: pandas dataframe with all points within the given aoi polygon area
-    """
-
-    # if AOI and pts are None, return None
-    if all(i is None for i in [aoi, pts]):
-        return None
-
-    # if no 'aoi' is given (None), just return original pts data. Default behavior
-    if(aoi is None):
-        return pts
-    
-    # check if aoi is a shapely geometry polygon
-    if(isinstance(aoi, (shapely.geometry.polygon.Polygon))):
-
-        # if aoi geometry type is polygon/line/linearRing
-        if("Polygon" in aoi.geom_type):
-
-            rel_pts = geopandas.overlay(
-                geopandas.GeoDataFrame(pts, geometry = geopandas.points_from_xy(pts['utmX'], pts['utmY'])).set_crs(26913).to_crs(4326), 
-                geopandas.GeoDataFrame(index = [0], crs = 'epsg:4326', geometry = [aoi]), 
-                how = 'intersection'
-                )
-
-            # convert geopandas dataframe to pandas dataframe and drop geometry column
-            rel_pts = pd.DataFrame(rel_pts.drop(columns='geometry'))
-
-            return rel_pts
-        else:
-            return pts
-    
-        
-    # check if aoi is a geopandas geoseries or geodataframe 
-    if(isinstance(aoi, (geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame))):
-
-        # if aoi geometry type is polygon/line/linearRing
-        if(["Polygon"] in aoi.geom_type.values):
-
-            # convert CRS to 4326
-            aoi = aoi.to_crs(4326)
-            
-            # get intersection of points and polygons 
-            rel_pts = geopandas.overlay(
-                geopandas.GeoDataFrame(pts, geometry = geopandas.points_from_xy(pts['utmX'], pts['utmY'])).set_crs(26913).to_crs(4326), 
-                geopandas.GeoDataFrame(aoi.geometry),
-                how = 'intersection'
-                )
-
-            # convert geopandas dataframe to pandas dataframe and drop geometry column
-            rel_pts = pd.DataFrame(rel_pts.drop(columns='geometry'))
-
-            return rel_pts
-        else:
-            return pts
-    else:
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+def _check_args(
+        arg_dict = None, 
+        ignore   = None,
+        f        = any
+        ):
+    """Check all arguments of a function for any/all NULL values
+    
+    Internal function for checking a function arguments for any/all invalid/missing arguments necessary to the function it is called within
+    
+    Args:
+        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
+        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
+        f (built-in function): Built in function "any" or "all" to indicate whether to check for "any" or "all" None argument. 
+            If "any" then if any of the function arguments are None, then an error is thrown.
+            If "all" then all relevant arguments must be None for an error to be thrown. Defaults to any.
+
+    Returns:
+        string: error statement with any/all None arguments listed, or None if no error is thrown by None values
+    """
+
+    # if no function arguments are given, throw an error
+    if arg_dict is None:
+        raise Exception("provide a list of function arguments by calling 'locals()', within another function")
+
+    # argument dictionary key/values as lists
+    key_lst  = list(arg_dict.keys())
+    val_lst  = list(arg_dict.values())
+
+    # if certain arguments are specifically supposed to be ignored
+    if ignore is not None:
+        
+        # remove specifically ignorged arguments
+        ignored_lst = [i for i, x in enumerate(key_lst) if x not in ignore]
+
+        # keys and values of arguments to keep
+        key_args        = [key_lst[i] for i in ignored_lst]
+        val_args        = [val_lst[i] for i in ignored_lst]
+    else:
+        
+        # if no arguments are ignored, keep all argument key/values
+        key_args        = key_lst
+        val_args        = val_lst
+
+    # if any/all arguments are None, return an error statement. Otherwise return None if None check is passed
+    if(f(i is None for i in val_args)):
+        # check where in remaining arguments the value is None, and get the index of missing arguments
+        idx_miss = [i for i in range(len(val_args)) if val_args[i] == None]
+
+        # return the argument names of None arguments
+        key_miss = ", ".join(["'"+key_lst[i]+"'" for i in idx_miss])
+
+        # error print statement
+        err_msg = "Invalid or missing " + key_miss + " arguments"
+
+        return err_msg
+    else:
+        return None
+    
+def _align_wcid(
+        x       = None, 
+        default = None
+        ):
+    """Set wc_identifier name to releases or diversions
+
+    Args:
+        x (str): Water class identifier. Defaults to None 
+        default (str, int, bool, Nonetype, optional):  value to return if "x" argument is None. Defaults to None.
+
+    Returns:
+        string: wc_identifier equaling either "diversion", "release", or a properly formatted water class identifier string
+    """
+    # if x is NULL/ not given, return "default"
+    if x is None:
+        return default
+    
+    # check if x is not in any of diversion/release lists
+    if x not in ["diversion", "diversions", "div", "divs", "d", 
+                "release", "releases", "rel", "rels", "r"]:
+        
+        # format wcidentifer query
+        x = "+".join([i.replace(":", "%3A") for i in x.split(" ")])
+
+    # if x in the diversions list
+    if x in ["diversion", "diversions", "div", "divs", "d"]:
+        x = "diversion"
+
+    # if x in the releases list
+    if x in ["release", "releases", "rel", "rels", "r"]:
+        x = "release"
+
+    x = "*" + x + "*"
+
+    return x
+def _valid_divrectype(
+        divrectype = None
+        ):
+
+    # check if type is NULL, default timescale to "day"
+    if divrectype is None:
+
+        divrectype = None
+
+        return divrectype
+    
+    # list of available divrectypes
+    divrectype_lst <- ["DivComment", "DivTotal", "RelComment", "RelTolal", "StageVolume", "WaterClass"]
+
+    # if a divrectype argument is provided (not NULL)
+    if divrectype is not None:
+
+        # lowercase divrectype_lst 
+        low_lst = [i.lower() for i in divrectype_lst]
+
+        # if divrectype matches any of the list, return correctly formatted divrectype
+        if divrectype.lower() in low_lst:
+            
+            divrectype = divrectype_lst[low_lst.index(divrectype.lower())]
+        
+
+        # check if divrectype is a valid divrectype
+        if divrectype.lower() not in low_lst and divrectype not in divrectype_lst:
+            raise Exception((
+                f"Invalid `divrectype` argument: '{divrectype}'",
+                f"\nPlease enter one of the following valid 'divrectype' arguments: \n{divrectype_lst}" 
+                ))
+
+    return(divrectype)
+
+def _valid_timesteps(
+        timestep = None
+        ):
+    
+    # list of valid timescales
+    day_lst       = ["day", "days", "daily", "d"]
+    month_lst     = ["month", "months", "monthly", "mon", "mons", "m"]
+    year_lst      = ['year', 'years', 'yearly', 'annual', 'annually', 'yr', 'y']
+
+    timestep_lst  = [day_lst, month_lst, year_lst]
+
+    # check if type is None, default timescale to "day"
+    if timestep is None:
+        # set timescale to "day"
+        timestep = "day"
+
+    # convert timescale to lowercase
+    timestep = timestep.lower()
+    
+    # check if type is correctly inputed
+    if timestep not in timestep_lst: 
+        raise Exception((
+            f"Invalid `timestep` argument: '{timestep}'",
+            f"\nPlease enter one of the following valid timesteps:\nDay: {day_lst}\nMonth: {month_lst}\nYear: {year_lst}" 
+            ))
+    
+    # check if given timestep is in day_lst and set timestep to "day"
+    if timestep in day_lst:
+
+        # set timescale to "day"
+        timestep = "day"
+
+    # check if given timestep is in month_lst and set timestep to "month"
+    if timestep in month_lst:
+        
+        # set timescale to "mohth"
+        timestep = "month"
+
+    # check if given timestep is in month_lst and set timestep to "month"
+    if timestep in year_lst:
+        
+        # set timescale to "year"
+        timestep = "year"
+
+    return timestep
+
+def _parse_date(
+    date   = None,
+    start  = True,
+    format =  "%m-%d-%Y"
+    ):
+
+    # if the date is the starting date
+    if start == True:
+
+        # if no start_date is given, default to 1900-01-01
+        if date is None:
+            date = "1900-01-01"
+            date = datetime.datetime.strptime(date, '%Y-%m-%d')
+            date = date.strftime(format)
+            date = date.replace("-", "%2F")
+        else:
+            date = datetime.datetime.strptime(date, '%Y-%m-%d')
+            date = date.strftime(format)
+            date = date.replace("-", "%2F") 
+
+    # if date is the ending date
+    else:
+
+        # if no end date is given, default to current date
+        if date is None: 
+            date   = datetime.date.today()
+            date   = date.strftime(format)
+            date   = date.replace("-", "%2F")
+        else:
+            date   = datetime.datetime.strptime(date, '%Y-%m-%d')
+            date   = date.strftime(format)
+            date   = date.replace("-", "%2F")
+
+    return date
+
+def _collapse_vector(
+    vect = None, 
+    sep  = "%2C+"
+    ):
+    
+    # if a list of vects, collapse list
+    if type(vect) == list or type(vect) == tuple:
+        vect = [str(x) for x in vect]
+        # join list into single string seperated by 'sep'
+        vect = sep.join(vect)
+        
+        # replace white space w/ 'sep'
+        vect = vect.replace(" ", sep)
+    else:
+        # if vect is an int or float, convert to string
+        if type(vect) == int or type(vect) == float:
+            vect = str(vect)
+        
+        if type(vect) == str:
+            # replace white space w/ plus sign
+            vect = vect.replace(" ", sep)
+    
+    return vect
+
+def _batch_dates(
+        start_date = None,
+        end_date   = None
+        ):
+    
+    """Create yearly date ranges to make batch GET requests
+
+    Internal function for extracting necessary yearly start and end dates to make a batch of smaller GET requests, instead 1 large date range. 
+    Allows for larger date ranges to be queried from the CDSS API without encountering a server side error.
+
+    Args:
+        start_date (str): starting date in YYYY-MM-DD format. Default is None which defaults start_date to "1900-01-01".
+        end_date (str): ending date in YYYY-MM-DD format. Default is None which defaults to the current date.
+    
+    Returns:
+        list: returns list of date range lists
+    """
+
+    # set default start date if None is given 
+    if start_date is None:
+        start_date = "1900-01-01"
+
+    # set default end_date if None is given 
+    if end_date is None:
+        end_date   = datetime.date.today()
+        end_date   = end_date.strftime('%Y-%m-%d')
+
+    # starting and ending years
+    start_year = int(start_date[:4])
+    end_year   = int(end_date[:4])
+
+    # empty list add date intervals to
+    lst = []
+
+    # if dates are multiple years apart, break into yearly date intervals
+    if start_year != end_year:
+
+        # start_date to end of first year
+        lst.append((start_date, f"{start_year}-12-31"))
+
+        # yearly intervals
+        for y in range(start_year + 1, end_year):
+            lst.append((f"{y}-01-01", f"{y}-12-31"))
+
+        # portion of the last year
+        lst.append((f"{end_year}-01-01", end_date))
+
+    # if dates are within the same year, just return start_date to end_date
+    else:
+        lst.append((start_date, end_date))
+
+    return(lst)
+
+def _get_error_handler(
+    url      = None
+    ):
+
+    """ Make GET requests and return the responses
+
+    Internal function for making get request and returning unsuccesful response text. 
+    Used within a try, except block within _parse_gets() function.
+
+    Args:
+        url (str, optional): URL of the request
+    
+    Returns:
+        requests.models.Response: returns results of attempted get request   
+    """
+
+    # If NO url is given
+    if(url is None):
+        raise Exception('Please provide a URL to perform a get request')
+    
+    # make API call
+
+    # attempt GET request
+    req_attempt = requests.get(url)
+
+    # if request is 200 (OK), return JSON content data
+    if req_attempt.status_code == 200:
+        # return successful response
+        return req_attempt
+    else:
+        # return req_attempt.text
+        raise Exception(req_attempt.text)
+    
+
+def _parse_gets(
+        url      = None, 
+        arg_dict = None, 
+        ignore   = None
+        ):
+    
+    """ Makes GET requests and dynamically handle errors 
+
+    Internal function for handling GET requests and associated errors.
+    Function will try to make a GET request, and if an error occurs, the function 
+    will return an error message with relevenant information detailing the error 
+    and the inputs that led to the error.
+
+    Args:
+        url (str): URL of the request
+        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
+        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
+    
+    Returns:
+        requests response: returns results of attempted get request 
+    """
+
+    # try to make GET request and error handling unsuccessful requests
+    try:
+        # attempt GET request
+        req = _get_error_handler(url = url)
+
+        return(req)
+    
+    except Exception as e:
+
+        # if an error occurred, use _query_error() to format a helpful error message to user
+        raise Exception(_query_error(
+            arg_dict = arg_dict,
+            url      = url,
+            ignore   = ignore,
+            e_msg    = e
+            )
+            )
+    
+def _query_error(
+        arg_dict = None,
+        url      = None,
+        ignore   = None,
+        e_msg    = None
+        ):
+    """GET Request Error message handler
+
+    Internal function for generating dynamic error messages for failed GET requests.
+    Designed to be called within another function and print out the functions input arguments.
+
+    Args:
+        arg_dict (dict): list of function arguments by calling locals() within a function. Defaults to None.
+        url (str): URL of the request. Defaults to None.
+        ignore (list, optional):  List of function arguments to ignore None check. Defaults to None.
+        e_msg (exception, str): exception message or string message that should be pointed to as the original error message. Defaults to None.
+
+    Returns:
+        str: error message that includes the query inputs that led to the error, the requested URL, and the original error message
+    """
+
+    # if no function arguments are given, throw an error
+    if arg_dict is None:
+        raise Exception("provide a list of function arguments by calling 'locals()', within another function")
+    
+    # argument dictionary key/values as lists
+    key_lst  = list(arg_dict.keys())
+    val_lst  = list(arg_dict.values())
+
+    # if certain arguments are specifically supposed to be ignored
+    if ignore is not None:
+        
+        # remove specifically ignorged arguments
+        ignored_lst = [i for i, x in enumerate(key_lst) if x not in ignore]
+
+        # keys and values of arguments to keep
+        key_args        = [key_lst[i] for i in ignored_lst]
+        val_args        = [val_lst[i] for i in ignored_lst]
+    else:
+        
+        # if no arguments are ignored, keep all argument key/values
+        key_args        = key_lst
+        val_args        = val_lst
+
+    # query_dict = dict(zip(key_args, val_args))
+
+    q_lst = []
+
+    for i in range(len(key_args)):
+            q_lst.append(f'{key_args[i]}: {val_args[i]}')
+
+    q_msg = ("DATA RETRIEVAL ERROR\nQuery:\n" + '\n'.join(q_lst) +
+            "\nRequested URL: " + url + 
+            "\n\n" + "Original error message: " + "\n-----------------------\n\n" + str(e_msg)
+            )
+
+    return q_msg
+
+def _get_error_handler2(
+    url     = None
+    ):
+
+    """
+    Internal function for making get request and error handling unsuccessful requests
+
+    Args:
+        url (str, optional): URL of the request
+    
+    Returns:
+        requests.models.Response: returns results of attempted get request   
+    """
+
+    # If NO url is given
+    if(url is None):
+        raise Exception('Please provide a URL to perform a get request')
+    
+    # make API call
+    try:
+        # attempt GET request
+        req_attempt = requests.get(url)
+
+        req_attempt.raise_for_status()
+
+        # return successful response
+        return req_attempt
+
+    except requests.exceptions.HTTPError as errh:
+        print("HTTP Error:\n", errh)
+        print("\nClient response:\n", errh.response.text)
+        raise
+    except requests.exceptions.ConnectionError as errc:
+        print("Connection Error:\n", errc)
+        print("\nClient response:\n", errc.response.text)
+        raise
+    except requests.exceptions.Timeout as errt:
+        print("Timeout Error:\n", errt)
+        print("\nClient response:\n", errt.response.text)
+        raise
+    except requests.exceptions.RequestException as err:
+        print("Exception raised:\n", err)
+        print("\nClient response:\n", err.response.text)
+        raise
+
+def _aoi_error_msg():
+    """
+    Function to return error message to user when aoi is not valid.
+    Returns:
+        string: print statement for aoi errors
+    """
+
+    msg = ("\nInvalid 'aoi' argument, 'aoi' must be one of the following:\n" + 
+    "1. List/Tuple of an XY coordinate pair\n" +
+    "2. Dictionary with X and Y keys\n" +
+    "3. Pandas DataFrame containing XY coordinates\n" +
+    "4. a shapely Point/Polygon/LineString\n" +
+    "5. Geopandas GeoDataFrame containing a Polygon/LineString/LinearRing/Point geometry\n" +
+    "6. Geopandas GeoSeries containing a Polygon/LineString/Point geometry\n")
+
+    return msg
+
+def _check_coord_crs(epsg_code, lng, lat):
+
+    """Function that checks if a set of longitude and latitude points are within a given EPSG space.
+
+    Returns:
+        boolean: True if the coordinates are within the provided EPSG space, False otherwise.
+    """
+    # given crs epsg code
+    crs = pyproj.CRS.from_user_input(epsg_code)
+
+    # if lng/lat fall within CRS space
+    if((crs.area_of_use.south <= lat <= crs.area_of_use.north) and (crs.area_of_use.west <= lng <= crs.area_of_use.east)):
+        crs_check = True
+    else:
+        crs_check = False
+
+    return crs_check
+
+def _extract_shapely_coords(aoi):
+    """Function for extracting coordinates from a shapely Polygon/LineString/Point
+    Internal helper function used in location search queries.
+
+    Args:
+        aoi (shapely Polygon/LineString/Point): shapely Polygon/LineString/Point object to extract coordinates from
+
+    Returns:
+        list: list of string coordinates with precision of 5 decimal places
+    """
+
+    # ensure that the shapely geometry is either a Polygon, LineString or a Point
+    if(isinstance(aoi, (shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString, shapely.geometry.point.Point))):
+
+        # if geometry is Polygon or Linestring
+        if(isinstance(aoi, (shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString))):
+            # extract lng/lat coords
+            lng = aoi.centroid.x
+            lat = aoi.centroid.y
+
+            # lng, lat coordinates
+            coord_lst = [lng, lat]
+            
+            # Valid coords in correct CRS space
+            if(_check_coord_crs(epsg_code = 4326, lng = lng, lat = lat)):
+
+                # round coordinates to 5 decimal places
+                coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                # return list of coordinates
+                return coord_lst
+
+            else:
+                raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
+
+        # if geometry is a Point
+        if(isinstance(aoi, (shapely.geometry.point.Point))):
+            # extract lng/lat coords
+            lng = aoi.x
+            lat = aoi.y
+            
+            # lng, lat coordinates
+            coord_lst = [lng, lat]
+
+            # Valid coords in correct CRS space
+            if(_check_coord_crs(epsg_code = 4326, lng = lng, lat = lat)):
+
+                # round coordinates to 5 decimal places
+                coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                # return list of coordinates
+                return coord_lst
+
+            else:
+                raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
+    else:
+        raise Exception("Invalid 'aoi' shapely geometry, must be either a shapely Polygon, LineString or Point")
+
+
+
+def _extract_coords(
+    aoi = None
+    ):
+
+    """Internal function for extracting XY coordinates from aoi arguments
+    Function takes in a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries of spatial objects,
+    and returns a list of length 2, indicating the XY coordinate pair. 
+    If the object provided is a Polygon/LineString/LinearRing, the function will return the XY coordinates of the centroid of the spatial object.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+    
+    Returns:
+        list object: list object of an XY coordinate pair
+    """
+    # if None is passed to 'aoi', return None
+    if aoi is None: 
+
+        return None
+
+    # if 'aoi' is NOT none, extract XY coordinates from object
+    else:
+
+        # make sure 'aoi' is one of supported types
+        if(isinstance(aoi, (list, tuple, dict, geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame, 
+        pd.core.frame.DataFrame, shapely.geometry.polygon.Polygon, shapely.geometry.linestring.LineString, shapely.geometry.point.Point)) is False):
+            raise Exception(_aoi_error_msg())
+
+        # check if aoi is a list or tuple
+        if(isinstance(aoi, (list, tuple))):
+
+            if(len(aoi) >= 2):
+
+                # make coordinate list of XY values
+                coord_lst = [aoi[0], aoi[1]]
+
+                # round coordinates to 5 decimal places
+                coord_lst = [float(num) for num in coord_lst]
+
+                # Valid coords in correct CRS space
+                if(_check_coord_crs(epsg_code = 4326, lng = coord_lst[0], lat = coord_lst[1])):
+
+                    # round coordinates to 5 decimal places
+                    coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                    # return list of coordinates
+                    return coord_lst
+
+                else:
+                    raise Exception("Invalid 'aoi' CRS, must convert 'aoi' CRS to epsg:4326")
+
+            else:
+
+                # return list of coordinates
+                raise Exception(_aoi_error_msg())
+
+        # check if aoi is a shapely Polygon/LineString/Point
+        if("shapely" in str(type(aoi))):
+
+            # extract coordinates from shapely geometry objects
+            coord_lst = _extract_shapely_coords(aoi = aoi)
+
+            return coord_lst 
+
+        # check if aoi is a geopandas geoseries or geodataframe 
+        if(isinstance(aoi, (geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame))):
+            
+            if(len(aoi) > 1):
+                raise Exception(_aoi_error_msg())
+
+            # convert CRS to 5070
+            aoi = aoi.to_crs(5070)
+
+            # if aoi geometry type is polygon/line/linearRing
+            if(["Polygon", 'LineString', 'LinearRing'] in aoi.geom_type.values):
+
+                # checking if point is geopandas Geoseries
+                if(isinstance(aoi, (geopandas.geoseries.GeoSeries))):
+
+                    # get centroid of polygon, and convert to 4326 and add lng/lat as column
+                    lng = float(aoi.centroid.to_crs(4326).geometry.x)
+                    lat = float(aoi.centroid.to_crs(4326).geometry.y)
+
+                    # lng, lat coordinates
+                    coord_lst = [lng, lat]
+                    
+                    # round coordinates to 5 decimal places
+                    coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                    # return list of coordinates
+                    return coord_lst
+
+                # checking if point is geopandas GeoDataFrame
+                if(isinstance(aoi, (geopandas.geodataframe.GeoDataFrame))):
+
+                    # get centroid of polygon, and convert to 4326 and add lng/lat as column
+                    aoi["lng"] = aoi.centroid.to_crs(4326).map(lambda p: p.x)
+                    aoi["lat"] = aoi.centroid.to_crs(4326).map(lambda p: p.y)
+
+                    # subset just lng/lat cols
+                    aoi_coords = aoi.loc[ : , ['lng', 'lat']]
+
+                    # extract lat/lng from centroid of polygon
+                    lng = float(aoi_coords["lng"])
+                    lat = float(aoi_coords["lat"])
+
+                    # lng, lat coordinates
+                    coord_lst = [lng, lat]
+                    
+                    # round coordinates to 5 decimal places
+                    coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                    # return list of coordinates
+                    return coord_lst
+
+            # if aoi geometry type is point
+            if("Point" in aoi.geom_type.values):
+
+                # checking if point is geopandas Geoseries
+                if(isinstance(aoi, (geopandas.geoseries.GeoSeries))):
+
+                    # convert to 4326, and extract lat/lng from Pandas GeoSeries
+                    lng = float(aoi.to_crs(4326).x)
+                    lat = float(aoi.to_crs(4326).y)
+
+                    # lng, lat coordinates
+                    coord_lst = [lng, lat]
+                    
+                    # round coordinates to 5 decimal places
+                    coord_lst = [f'{num:.5f}' for num in coord_lst]
+                    
+                    # return list of coordinates
+                    return coord_lst
+
+                # checking if point is geopandas GeoDataFrame
+                if(isinstance(aoi, (geopandas.geodataframe.GeoDataFrame))):
+
+                    # convert to 4326, and extract lat/lng from Pandas GeoDataFrame
+                    lng = float(aoi.to_crs(4326)['geometry'].x)
+                    lat = float(aoi.to_crs(4326)['geometry'].y)
+                
+                    # lng, lat coordinates
+                    coord_lst = [lng, lat]
+
+                    # round coordinates to 5 decimal places
+                    coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+                    # return list of coordinates
+                    return coord_lst
+                    
+        # check if aoi is a Pandas dataframe
+        if(isinstance(aoi, (pd.core.frame.DataFrame))):
+            
+            # extract first and second columns
+            lng = float(aoi.iloc[:, 0])
+            lat = float(aoi.iloc[:, 1])
+
+            # lng, lat coordinates
+            coord_lst = [lng, lat]
+            
+            # round coordinates to 5 decimal places
+            coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+            # return list of coordinates
+            return coord_lst
+
+        # check if aoi is a dictionary
+        if(isinstance(aoi, (dict))):
+            
+            # extract "X" and "Y" dict keys
+            lng = float(aoi["X"])
+            lat = float(aoi["Y"])
+
+            # lng, lat coordinates
+            coord_lst = [lng, lat]
+            
+            # round coordinates to 5 decimal places
+            coord_lst = [f'{num:.5f}' for num in coord_lst]
+
+            # return list of coordinates
+            return coord_lst
+
+def _check_radius(
+    aoi    = None,
+    radius = None
+    ):
+
+    """Internal function for radius argument value is within the valid value range for location search queries. 
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None.
+
+    Returns:
+        int: radius value between 1-150 miles
+    """
+    # convert str radius value to int
+    if(isinstance(radius, (str))):
+        radius = int(radius)
+
+    # if spatial data is provided, check type and try to extract XY coordinates
+    if aoi is not None:
+        # print("AOI arg is NOT None")
+
+        # if radius is not NULL, and is larger than 150, set to max of 150. if NULL radius is provided with spatial data, default to 150 miles
+        if radius is not None:
+            # print("radius arg is NOT None")
+            
+            # if radius value is over max, set to 150
+            if(radius > 150):
+
+                # print("radius arg > 150, so set to 150")
+                radius = 150
+
+            # if radius value is under min, set to 1
+            if(radius <= 0):
+                # print("radius arg <= 0, so set to 1")
+                radius = 1
+
+        # if no radius given, set to 20 miles
+        else:
+            # print("radius arg is None, default to 20 miles")
+            radius = 20
+    else:
+        # print("AOI arg is None")
+        radius = None
+    
+    # Return radius value
+    return radius
+
+
+def _check_aoi(
+    aoi    = None, 
+    radius = None
+    ):
+
+    """Internal function for checking AOI and radius arguments are valid for use in location search queries.
+    Function takes in a list/tuple of an XY coordinate pair, a Pandas Dataframe, or a Geopandas GeoDataFrame/GeoSeries of spatial objects,
+    along with a radius value between 1-150 miles.
+    The extracts the necessary coordinates from the given aoi parameter and also makes sure the radius value is within the valid value range. 
+    The function then returns a list of length 2, indicating the XY coordinate pair. 
+    If the object provided is a Polygon/LineString/LinearRing, the function will return the XY coordinates of the centroid of the spatial object.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None.
+
+    Returns:
+        list: list containing the latitude, longitude, and radius values to use for location search queries.
+    """
+
+    # convert str radius value to int
+    if(isinstance(radius, (str))):
+        radius = int(radius)
+
+    # extract lat/long coords for query
+    if(aoi is not None):
+        # extract coordinates from matrix/dataframe/sf object
+        coord_df = _extract_coords(aoi = aoi)
+        
+        # check radius is valid and fix if necessary
+        radius = _check_radius(
+            aoi    = aoi,
+            radius = radius
+            )
+
+        # lat/long coords
+        lng = coord_df[0]
+        lat = coord_df[1]
+    
+    else:
+        # if None aoi given, set coords and radius to None
+        lng    = None
+        lat    = None
+        radius = None
+    
+    # create list to return container longitude, latitude, and radius
+    aoi_lst = [lng, lat, radius]
+    
+    # return lng, lat, radius list
+    return aoi_lst  
+
+def _aoi_mask(
+    aoi = None,
+    pts = None
+    ):
+
+    """For location search queries using a polygon, the response data from the CDSS API will be masked to the polygon area, removing any extra points.
+    Internal helper function, if aoi is None, then the function will just return the original dataset. 
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        pts (pandas dataframe): pandas dataframe of points that should be masked to the given aoi. Dataframe must contain "utmY" and "utmX" columns
+
+    Returns:
+        pandas dataframe: pandas dataframe with all points within the given aoi polygon area
+    """
+
+    # if AOI and pts are None, return None
+    if all(i is None for i in [aoi, pts]):
+        return None
+
+    # if no 'aoi' is given (None), just return original pts data. Default behavior
+    if(aoi is None):
+        return pts
+    
+    # check if aoi is a shapely geometry polygon
+    if(isinstance(aoi, (shapely.geometry.polygon.Polygon))):
+
+        # if aoi geometry type is polygon/line/linearRing
+        if("Polygon" in aoi.geom_type):
+
+            rel_pts = geopandas.overlay(
+                geopandas.GeoDataFrame(pts, geometry = geopandas.points_from_xy(pts['utmX'], pts['utmY'])).set_crs(26913).to_crs(4326), 
+                geopandas.GeoDataFrame(index = [0], crs = 'epsg:4326', geometry = [aoi]), 
+                how = 'intersection'
+                )
+
+            # convert geopandas dataframe to pandas dataframe and drop geometry column
+            rel_pts = pd.DataFrame(rel_pts.drop(columns='geometry'))
+
+            return rel_pts
+        else:
+            return pts
+    
+        
+    # check if aoi is a geopandas geoseries or geodataframe 
+    if(isinstance(aoi, (geopandas.geoseries.GeoSeries, geopandas.geodataframe.GeoDataFrame))):
+
+        # if aoi geometry type is polygon/line/linearRing
+        if(["Polygon"] in aoi.geom_type.values):
+
+            # convert CRS to 4326
+            aoi = aoi.to_crs(4326)
+            
+            # get intersection of points and polygons 
+            rel_pts = geopandas.overlay(
+                geopandas.GeoDataFrame(pts, geometry = geopandas.points_from_xy(pts['utmX'], pts['utmY'])).set_crs(26913).to_crs(4326), 
+                geopandas.GeoDataFrame(aoi.geometry),
+                how = 'intersection'
+                )
+
+            # convert geopandas dataframe to pandas dataframe and drop geometry column
+            rel_pts = pd.DataFrame(rel_pts.drop(columns='geometry'))
+
+            return rel_pts
+        else:
+            return pts
+    else:
         return pts
```

### Comparing `cdsspy-1.2.70/cdsspy/water_rights.py` & `cdsspy-1.2.71/cdsspy/water_rights.py`

 * *Ordering differences only*

 * *Files 12% similar despite different names*

```diff
@@ -1,258 +1,258 @@
-import pandas as pd
-import requests
-import datetime
-import geopandas
-import shapely
-import pyproj
-
-# from cdsspy.utils import utils2
-# from cdsspy.cdsspy2 import utils
-from cdsspy import utils
-
-def get_water_rights_netamount(
-    aoi                 = None,
-    radius              = None, 
-    county              = None,
-    division            = None,
-    water_district      = None,
-    wdid                = None,
-    api_key             = None
-    ):
-    """Return water rights net amounts data
-
-    Make a request to the /waterrights/netamount endpoint to retrieve water rights net amounts data via a spatial search or by county, division, water district, or WDID, within a given date range (start and end dates).
-    Returns current status of a water right based on all of its court decreed actions.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        county (str, optional): County to query for water rights. Defaults to None.
-        division (int, str, optional):  Water division to query for water rights. Defaults to None.
-        water_district (str, optional): Water district to query for water rights. Defaults to None.
-        wdid (str, optional): WDID code of water right. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of water rights net amounts data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [aoi, county, division, water_district, wdid]):
-    #     raise TypeError("Invalid 'aoi', 'county', 'division', 'water_district', or 'wdid' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/waterrights/netamount/?"
-
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving water rights net amounts data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}'
-            f'&division={division or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&wdid={wdid or ""}'
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-
-    return data_df
-
-def get_water_rights_trans(
-    aoi                 = None,
-    radius              = None, 
-    county              = None,
-    division            = None,
-    water_district      = None,
-    wdid                = None,
-    api_key             = None
-    ):
-    """Return water rights transactions data
-
-    Make a request to the /waterrights/transaction endpoint to retrieve water rights transactions data via a spatial search or by county, division, water district, or WDID, within a given date range (start and end dates).
-    Returns List of court decreed actions that affect amount and use(s) that can be used by each water right.
-
-    Args:
-        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
-        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
-        county (str, optional): County to query for water rights. Defaults to None.
-        division (int, str, optional):  Water division to query for water rights transactions. Defaults to None.
-        water_district (str, optional): Water district to query for water rights transactions. Defaults to None.
-        wdid (str, optional): WDID code of water right transaction. Defaults to None.
-        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
-
-    Returns:
-        pandas dataframe object: dataframe of water rights transactions data
-    """
-
-    # # If all inputs are None, then return error message
-    # if all(i is None for i in [aoi, county, division, water_district, wdid]):
-    #     raise TypeError("Invalid 'aoi', 'county', 'division', 'water_district', or 'wdid' parameters")
-
-    # list of function inputs
-    input_args = locals()
-
-    # check function arguments for missing/invalid inputs
-    arg_lst = utils._check_args(
-        arg_dict = input_args,
-        ignore   = ["api_key"],
-        f        = all
-        )
-    
-    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
-    if arg_lst is not None:
-        raise Exception(arg_lst)
-
-    #  base API URL
-    base = "https://dwr.state.co.us/Rest/GET/api/v2/waterrights/transaction/?"
-
-    # check and extract spatial data from 'aoi' and 'radius' args for location search query
-    aoi_lst = utils._check_aoi(
-        aoi    = aoi,
-        radius = radius
-        )
-
-    # lat/long coords and radius
-    lng    = aoi_lst[0]
-    lat    = aoi_lst[1]
-    radius = aoi_lst[2]
-
-    # maximum records per page
-    page_size = 50000
-
-    # initialize empty dataframe to store data from multiple pages
-    data_df = pd.DataFrame()
-
-    # initialize first page index
-    page_index = 1
-
-    # Loop through pages until there are no more pages to get
-    more_pages = True
-
-    print("Retrieving water rights transactions data")
-
-    # Loop through pages until last page of data is found, binding each response dataframe together
-    while more_pages == True:
-
-        # create query URL string
-        url = (
-            f'{base}format=json&dateFormat=spaceSepToSeconds'
-            f'&county={county or ""}'
-            f'&division={division or ""}'
-            f'&waterDistrict={water_district or ""}'
-            f'&wdid={wdid or ""}'
-            f'&latitude={lat or ""}' 
-            f'&longitude={lng or ""}' 
-            f'&radius={radius or ""}' 
-            f'&units=miles' 
-            f'&pageSize={page_size}&pageIndex={page_index}'
-            )
-
-        # If an API key is provided, add it to query URL
-        if api_key is not None:
-            # Construct query URL w/ API key
-            url = url + "&apiKey=" + str(api_key)
-
-        # make API call w/ error handling
-        cdss_req = utils._parse_gets(
-            url      = url, 
-            arg_dict = input_args,
-            ignore   = None
-            )
-
-        # extract dataframe from list column
-        cdss_df = cdss_req.json()
-        cdss_df = pd.DataFrame(cdss_df)
-        cdss_df = cdss_df["ResultList"].apply(pd.Series)
-
-        # bind data from this page
-        data_df = pd.concat([data_df, cdss_df])
-
-        # Check if more pages to get to continue/stop while loop
-        if len(cdss_df.index) < page_size:
-            more_pages = False
-        else:
-            page_index += 1
-
-    # mask data if necessary
-    data_df = utils._aoi_mask(
-        aoi = aoi,
-        pts = data_df
-        )
-    
+import pandas as pd
+import requests
+import datetime
+import geopandas
+import shapely
+import pyproj
+
+# from cdsspy.utils import utils2
+# from cdsspy.cdsspy2 import utils
+from cdsspy import utils
+
+def get_water_rights_netamount(
+    aoi                 = None,
+    radius              = None, 
+    county              = None,
+    division            = None,
+    water_district      = None,
+    wdid                = None,
+    api_key             = None
+    ):
+    """Return water rights net amounts data
+
+    Make a request to the /waterrights/netamount endpoint to retrieve water rights net amounts data via a spatial search or by county, division, water district, or WDID, within a given date range (start and end dates).
+    Returns current status of a water right based on all of its court decreed actions.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        county (str, optional): County to query for water rights. Defaults to None.
+        division (int, str, optional):  Water division to query for water rights. Defaults to None.
+        water_district (str, optional): Water district to query for water rights. Defaults to None.
+        wdid (str, optional): WDID code of water right. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of water rights net amounts data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [aoi, county, division, water_district, wdid]):
+    #     raise TypeError("Invalid 'aoi', 'county', 'division', 'water_district', or 'wdid' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/waterrights/netamount/?"
+
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving water rights net amounts data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}'
+            f'&division={division or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&wdid={wdid or ""}'
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+
+    return data_df
+
+def get_water_rights_trans(
+    aoi                 = None,
+    radius              = None, 
+    county              = None,
+    division            = None,
+    water_district      = None,
+    wdid                = None,
+    api_key             = None
+    ):
+    """Return water rights transactions data
+
+    Make a request to the /waterrights/transaction endpoint to retrieve water rights transactions data via a spatial search or by county, division, water district, or WDID, within a given date range (start and end dates).
+    Returns List of court decreed actions that affect amount and use(s) that can be used by each water right.
+
+    Args:
+        aoi (list, tuple, dict, DataFrame, shapely geometry, GeoDataFrame, GeoSeries): a list/tuple of an XY coordinate pair, a dictionary with XY keys, a Pandas Dataframe, a shapely Point/Polygon/LineString, or a Geopandas GeoDataFrame/GeoSeries containing a Point/Polygon/LineString/LinearRing. Defaults to None.
+        radius (int, str, optional): radius value between 1-150 miles. Defaults to None, and if an aoi is given, the radius will default to a 20 mile radius.
+        county (str, optional): County to query for water rights. Defaults to None.
+        division (int, str, optional):  Water division to query for water rights transactions. Defaults to None.
+        water_district (str, optional): Water district to query for water rights transactions. Defaults to None.
+        wdid (str, optional): WDID code of water right transaction. Defaults to None.
+        api_key (str, optional): API authorization token, optional. If more than maximum number of requests per day is desired, an API key can be obtained from CDSS. Defaults to None.
+
+    Returns:
+        pandas dataframe object: dataframe of water rights transactions data
+    """
+
+    # # If all inputs are None, then return error message
+    # if all(i is None for i in [aoi, county, division, water_district, wdid]):
+    #     raise TypeError("Invalid 'aoi', 'county', 'division', 'water_district', or 'wdid' parameters")
+
+    # list of function inputs
+    input_args = locals()
+
+    # check function arguments for missing/invalid inputs
+    arg_lst = utils._check_args(
+        arg_dict = input_args,
+        ignore   = ["api_key"],
+        f        = all
+        )
+    
+    # if an error statement is returned (not None), then raise exception with dynamic error message and stop function
+    if arg_lst is not None:
+        raise Exception(arg_lst)
+
+    #  base API URL
+    base = "https://dwr.state.co.us/Rest/GET/api/v2/waterrights/transaction/?"
+
+    # check and extract spatial data from 'aoi' and 'radius' args for location search query
+    aoi_lst = utils._check_aoi(
+        aoi    = aoi,
+        radius = radius
+        )
+
+    # lat/long coords and radius
+    lng    = aoi_lst[0]
+    lat    = aoi_lst[1]
+    radius = aoi_lst[2]
+
+    # maximum records per page
+    page_size = 50000
+
+    # initialize empty dataframe to store data from multiple pages
+    data_df = pd.DataFrame()
+
+    # initialize first page index
+    page_index = 1
+
+    # Loop through pages until there are no more pages to get
+    more_pages = True
+
+    print("Retrieving water rights transactions data")
+
+    # Loop through pages until last page of data is found, binding each response dataframe together
+    while more_pages == True:
+
+        # create query URL string
+        url = (
+            f'{base}format=json&dateFormat=spaceSepToSeconds'
+            f'&county={county or ""}'
+            f'&division={division or ""}'
+            f'&waterDistrict={water_district or ""}'
+            f'&wdid={wdid or ""}'
+            f'&latitude={lat or ""}' 
+            f'&longitude={lng or ""}' 
+            f'&radius={radius or ""}' 
+            f'&units=miles' 
+            f'&pageSize={page_size}&pageIndex={page_index}'
+            )
+
+        # If an API key is provided, add it to query URL
+        if api_key is not None:
+            # Construct query URL w/ API key
+            url = url + "&apiKey=" + str(api_key)
+
+        # make API call w/ error handling
+        cdss_req = utils._parse_gets(
+            url      = url, 
+            arg_dict = input_args,
+            ignore   = None
+            )
+
+        # extract dataframe from list column
+        cdss_df = cdss_req.json()
+        cdss_df = pd.DataFrame(cdss_df)
+        cdss_df = cdss_df["ResultList"].apply(pd.Series)
+
+        # bind data from this page
+        data_df = pd.concat([data_df, cdss_df])
+
+        # Check if more pages to get to continue/stop while loop
+        if len(cdss_df.index) < page_size:
+            more_pages = False
+        else:
+            page_index += 1
+
+    # mask data if necessary
+    data_df = utils._aoi_mask(
+        aoi = aoi,
+        pts = data_df
+        )
+    
     return data_df
```

### Comparing `cdsspy-1.2.70/cdsspy.egg-info/PKG-INFO` & `cdsspy-1.2.71/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,290 +1,279 @@
-Metadata-Version: 2.1
-Name: cdsspy
-Version: 1.2.70
-Summary: Provides Python functions for discovering and requesting data from the CDSS REST API.
-Author: Angus Watters
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **cdsspy** <img src="https://cdsspy-images.s3.us-west-1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
-
-<!-- badges: start -->
-
-[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
-[![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
-<!-- badges: end -->
-
-<div align="left">
-
-<p align="left">
-<a href="https://dwr.state.co.us/Tools"><strong>Â« CDSS Â»</strong></a>
-<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
-Services</a>
-</p>
-
-</div>
-
-<hr>
-
-The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
-
-The Coloradoâ€™s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
-
-Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
-
-<br>
-
-> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
-
----
-
-- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
-
-- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
-
-- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
-
-- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
-
----
-
-<br> 
-
-## **Installation**
-Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
-
-``` 
-pip install cdsspy
-```
-<br>
-
-## **Available endpoints**
-
-Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
-|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
-|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
-|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
-|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
-|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
-|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
-|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-<br>
-
-## **Identify query inputs using reference tables**
-
-The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
-
-<br>
-
-```python
-# available parameters for telemetry stations
-telemetry_params = cdsspy.get_reference_tbl(
-    table_name = "telemetryparams"
-    )
-```
-
-|    | Parameter   |
-|---:|:------------|
-|  0 | AIRTEMP     |
-|  1 | BAR_P       |
-|  2 | BATTERY     |
-|  3 | COND        |
-|  4 | D1          |
-|  5 | D2          |
-|  6 | DISCHRG     |
-|  7 | DISCHRG1    |
-|  8 | DISCHRG2    |
-|  9 | DISCHRG3    |
-| 10 | DISCHRG4    |
-| 11 | ELEV        |
-
-<br>
-<br>
-<br>
-
-## **Locate structures**
-
-**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
-|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
-|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
-|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
-|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
-
-<br>
-
-### **Example: Locating telemetry stations by county:**
-
-```python
-# identify telemetry stations in Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    county = "Boulder"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/county_telem_stations2.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations around a point**
-
-```python
-# identify telemetry stations within a 15 mile radius of the center point of Boulder County
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = [-105.358164, 40.092608],
-    radius = 15
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/poi_telem_stations.png)
-
-<br>
-<br>
-
-### **Example: Locating telemetry stations within a spatial extent**
-A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
-
-```python
-# identify telemetry stations 15 miles around the centroid of a polygon
-stations  = cdsspy.get_telemetry_stations(
-    aoi    = geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_county.gpkg")
-    radius = 15
-    )
-```
-
-This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve time series data** 
-
-The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
-
-|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
-|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
-|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
-|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
-|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
-|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
-|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
-
-<br>
-<br>
-
-#### **Example: Daily discharge at a telemetry station**
-We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
-
-<br>
-
-The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
-
-```python
-# Daily discharge at "ANDDITCO" telemetry station
-discharge_ts   = cdsspy.get_telemetry_ts(
-    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
-    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
-    start_date     = "2015-01-01",   # Starting date
-    end_date       = "2022-01-01",   # Ending date
-    timescale      = "day"           # select daily timescale
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
-
-<br>
-<br>
-
-#### **Example: Retrieve Diversion records for multiple structures**
-Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
-
-
-1. Executing a spatial search using **`get_structures()`** 
-2. Selecting the WDIDs of interest from the search results
-3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
-
-
-```python 
-# 1. Executing a spatial search
-structures = cdsspy.get_structures(
-    aoi    = [-105.3578, 40.09244],
-    radius = 5
-    )
-
-# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
-ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
-ditch_wdids = list(ditch_wdids['wdid'])
-
-# 3. Providing the WDID's as a list to get_structures_divrec_ts()
-diversion_rec  = cdsspy.get_structures_divrec_ts(
-    wdid           = ditch_wdids,
-    wc_identifier  = "diversion",
-    timescale      = "month"
-    )
-```
-**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
-
-<br>
-<br>
-<br>
-<br>
-
-## **Retrieve groundwater data**
-The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
-
-| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
-|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
-| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
-| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
-| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
-| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
-
-<br>
-
-Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
-
-```python
-# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
-well_measure = cdsspy.get_gw_wl_wellmeasures(
-    wellid     = "1274",
-    start_date = "1990-01-01",
-    end_date   = "2022-01-01"
-    )
-```
-
-![](https://cdsspy-images.s3.us-west-1.amazonaws.com/gw_depth_to_water_plot2.png)
+# **cdsspy** <img src="img/co_dnr_div_cdss_cwcbdwr_transparent.png" align="right" width="25%" />
+
+<!-- badges: start -->
+
+[![Dependencies](https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#)
+[![License:
+MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://choosealicense.com/licenses/mit/)
+<!-- badges: end -->
+
+<div align="left">
+
+<p align="left">
+<a href="https://dwr.state.co.us/Tools"><strong>« CDSS »</strong></a>
+<br /> <a href="https://dwr.state.co.us/Rest/GET/Help">CDSS REST Web
+Services</a>
+</p>
+
+</div>
+
+<hr>
+
+The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide functions that help Python users to navigate, explore, and make requests to the CDSS REST API web service. 
+
+The Colorado’s Decision Support Systems (CDSS) is a water management system created and developed by the Colorado Water Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
+
+Thank you to those at CWCB and DWR for providing an accessible and well documented REST API!
+
+<br>
+
+> See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R** version of this package
+
+---
+
+- [**cdssr (R)**](https://github.com/anguswg-ucsb/cdssr)
+
+- [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/)
+
+- [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy)
+
+- [**cdsspy documentation**](https://pypi.org/project/cdsspy/)
+
+---
+
+<br> 
+
+## **Installation**
+Install the latest version of **`cdsspy`** from [PyPI](https://pypi.org/project/cdsspy/):
+
+``` 
+pip install cdsspy
+```
+<br>
+
+## **Available endpoints**
+
+Below is a table of all of the CDSS API endpoints **`cdsspy`** provides functions for.
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_admin_calls()**          | Returns list of active/historic administrative calls               | [administrativecalls/active](https://dwr.state.co.us/rest/get/help#Datasets&#AdministrativeCallsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600964&dbid=0&#gettingstarted&#jsonxml)            |
+|2     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |
+|3     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|4     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|5     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|6     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|7     | **get_climate_frostdates()**           | Returns Climate Station Frost Dates             | [climatedata/climatestationfrostdates](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|8     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|9     | **get_gw_gplogs_geologpicks()**          | Returns Groundwater Geophysical Log picks by well ID           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|10     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|11     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|12     | **get_reference_tbl()**        | Returns reference tables list                                      | [referencetables/](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml)                      |
+|13     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|14    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|15    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |
+|16    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+|17    | **get_water_rights_netamount()**   | Returns current status of a water right based on all of its court decreed actions | [waterrights/netamount](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)    |
+|18    | **get_water_rights_trans()**         | Returns court decreed actions that affect amount and use(s) that can be used by each water right | [waterrights/transaction](https://dwr.state.co.us/rest/get/help#Datasets&#WaterRightsController&#gettingstarted&#jsonxml)|
+|19    | **get_call_analysis_wdid()**   | 	Performs a call analysis that returns a time series showing the percentage of each day that the specified WDID and priority was out of priority and the downstream call in priority | [analysisservices/callanalysisbywdid](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)    |
+|20    | **get_source_route_framework()**         | Returns the DWR source route framework reference table for the criteria specified | [analysisservices/watersourcerouteframework](https://dwr.state.co.us/rest/get/help#Datasets&#AnalysisServicesController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+<br>
+
+## **Identify query inputs using reference tables**
+
+The **`get_reference_tbl()`** function will return tables that makes it easier to know what information should be supplied to the data retrieval functions in **`cdsspy`**. For more information on the source reference tables click [here](https://dwr.state.co.us/rest/get/help#Datasets&#ReferenceTablesController&#gettingstarted&#jsonxml).
+
+<br>
+
+```python
+# available parameters for telemetry stations
+telemetry_params = cdsspy.get_reference_tbl(
+    table_name = "telemetryparams"
+    )
+```
+
+|    | Parameter   |
+|---:|:------------|
+|  0 | AIRTEMP     |
+|  1 | BAR_P       |
+|  2 | BATTERY     |
+|  3 | COND        |
+|  4 | D1          |
+|  5 | D2          |
+|  6 | DISCHRG     |
+|  7 | DISCHRG1    |
+|  8 | DISCHRG2    |
+|  9 | DISCHRG3    |
+| 10 | DISCHRG4    |
+| 11 | ELEV        |
+
+<br>
+<br>
+<br>
+
+## **Locate structures**
+
+**`cdsspy`** provides functions for locating structures/stations/wells/sites by providing a spatial extent, water district, division, county, designated basin, or management district to the functions in the table below. Site data can also be retrieved by providing the site specific abbreviations, GNIS IDs, USGS IDs, WDIDs, or Well IDs.
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures()**           | Returns list of administrative structures                          | [structures](https://dwr.state.co.us/rest/get/help#Datasets&#StructuresController&#gettingstarted&#jsonxml)                            |          |
+|2     | **get_climate_stations()**     | Returns Climate Stations                                           | [climatedata/climatestations](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)           |
+|3     | **get_gw_gplogs_wells()**          | Returns Groundwater GeophysicalLogsWell from filters           | [groundwater/geophysicallogs/](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterGeophysicalLogsController&#gettingstarted&#jsonxml)                          |
+|4     | **get_gw_wl_wells()**          | Returns WaterLevelsWell from filters           | [groundwater/waterlevels/wells](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5     | **get_sw_stations()**          | Returns Surface Water Station info                                 | [surfacewater/surfacewaterstations](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)     |
+|6    | **get_telemetry_stations()**   | Returns telemetry stations and their most recent parameter reading | [telemetrystations/telemetrystation](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)    |                     
+
+<br>
+
+### **Example: Locating telemetry stations by county:**
+
+```python
+# identify telemetry stations in Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    county = "Boulder"
+    )
+```
+
+![](img/county_telem_stations2.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations around a point**
+
+```python
+# identify telemetry stations within a 15 mile radius of the center point of Boulder County
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = [-105.358164, 40.092608],
+    radius = 15
+    )
+```
+
+![](img/poi_telem_stations.png)
+
+<br>
+<br>
+
+### **Example: Locating telemetry stations within a spatial extent**
+A masking operation is performed when a location search is done using a **polygon**. This ensures that the function only returns points that are ***within*** the given polygon. 
+
+```python
+# identify telemetry stations 15 miles around the centroid of a polygon
+stations  = cdsspy.get_telemetry_stations(
+    aoi    = geopandas.read_file("example-data/boulder_county.gpkg")
+    radius = 15
+    )
+```
+
+This gif highlights the masking process that happens when the **`aoi`** argument is given a **polygon** 
+
+![](img/boulder_telem_stations_poly2.gif)
+
+<br>
+<br>
+<br>
+<br>
+
+
+## **Retrieve time series data** 
+
+The functions in the table below retrieve time series data from the various time series related CDSS API endpoints.  
+
+|**-** |**Function**                    | **Description**                                                    | **Endpoint**                                 |
+|------|--------------------------------| -------------------------------------------------------------------|----------------------------------------------|
+|1     | **get_structures_divrec_ts()**    | Returns list of diversion/release records based on WDID      | [structures/divrec/divrec](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|2     | **get_structures_stage_ts()**    | Returns list of stage/volume records based on WDID      | [structures/divrec/stagevolume](https://dwr.state.co.us/rest/get/help#Datasets&#DiversionRecordsController&https://dnrweblink.state.co.us/dwr/ElectronicFile.aspx?docid=3600965&dbid=0&#gettingstarted&#jsonxml)              |
+|3     | **get_climate_ts()**           | Returns Climate Station Time Series (day, month, year)             | [climatedata/climatestationts](https://dwr.state.co.us/rest/get/help#Datasets&#ClimateStationsController&https://www.ncdc.noaa.gov/cdo-web/webservices&https://www.northernwater.org/our-data/weather-data&#gettingstarted&#jsonxml)       |
+|4     | **get_gw_wl_wellmeasures()**          | Returns  Groundwater Measurements | [groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/rest/get/help#Datasets&#GroundwaterLevelsController&#gettingstarted&#jsonxml)                          |
+|5    | **get_sw_ts()**                | Returns Surface Water Time Series                                  | [surfacewater/surfacewaterts](https://dwr.state.co.us/rest/get/help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml)        |
+|6    | **get_telemetry_ts()**         | Returns telemetry time series data (raw, hour, day) | [telemetrystations/telemetrytimeseries](https://dwr.state.co.us/rest/get/help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml)|
+
+<br>
+<br>
+
+#### **Example: Daily discharge at a telemetry station**
+We can then take a station abbreviations from the **`get_telemetry_stations()`** call, a parameter from the **`get_reference_tbl()`** call, and use this information as inputs into the **`get_telemetry_ts()`** function. 
+
+<br>
+
+The function below returns a dataframe of daily discharge for the "ANDDITCO" site between 2015-2022.
+
+```python
+# Daily discharge at "ANDDITCO" telemetry station
+discharge_ts   = cdsspy.get_telemetry_ts(
+    abbrev         = "ANDDITCO",     # Site abbreviation from the outputs of get_telemetry_stations()
+    parameter      = "DISCHRG",      # Desired parameter, identified by the get_reference_tbl()
+    start_date     = "2015-01-01",   # Starting date
+    end_date       = "2022-01-01",   # Ending date
+    timescale      = "day"           # select daily timescale
+    )
+```
+
+![](img/discharge_timeseries_plot2.png)
+
+<br>
+<br>
+
+#### **Example: Retrieve Diversion records for multiple structures**
+Some of the CDSS API endpoints allow users to request data from multiple structures if you provide a list of IDs. If we want to get diversion data from multiple structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs within a given area by:  
+
+
+1. Executing a spatial search using **`get_structures()`** 
+2. Selecting the WDIDs of interest from the search results
+3. Providing the WDIDs as a vector to **`get_structures_divrec_ts()`** 
+
+
+```python 
+# 1. Executing a spatial search
+structures = cdsspy.get_structures(
+    aoi    = [-105.3578, 40.09244],
+    radius = 5
+    )
+
+# 2. Selecting the WDID's of interest from search results and putting WDIDs into a list
+ditch_wdids = structures[(structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
+ditch_wdids = list(ditch_wdids['wdid'])
+
+# 3. Providing the WDID's as a list to get_structures_divrec_ts()
+diversion_rec  = cdsspy.get_structures_divrec_ts(
+    wdid           = ditch_wdids,
+    wc_identifier  = "diversion",
+    timescale      = "month"
+    )
+```
+**Note:** Data availability can vary between structures (i.e. Missing data, not all structures have every data type/temporal resolution available, etc.) 
+
+![](img/divrec_facet_plot.png)
+
+<br>
+<br>
+<br>
+<br>
+
+## **Retrieve groundwater data**
+The **`get_gw_()`** set of functions lets users retrieve data from the various groundwater related API endpoints shown in the table below:
+
+| **-** | **Function**                    | **Endpoint**                                                                                                                                     |
+|-------|---------------------------------|--------------------------------------------------------------------------------------------------------------------------------------------------|
+| 1     | **get_gw_wl_wellmeasures()**    | [api/v2/groundwater/waterlevels/wellmeasurements](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wellmeasurements) |
+| 2     | **get_gw_wl_wells()**           | [api/v2/groundwater/waterlevels/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-waterlevels-wells)                       |
+| 3     | **get_gw_gplogs_wells()**       | [api/v2/groundwater/geophysicallogs/wells](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-wells)               |
+| 4     | **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-geophysicallogs-geoplogpicks) |
+
+<br>
+
+Here we will retrieve groundwater well measurement data for Well ID 1274 between 2021-2022.
+
+```python
+# Request wellmeasurements endpoint (api/v2/groundwater/waterlevels/wellmeasurements)
+well_measure = cdsspy.get_gw_wl_wellmeasures(
+    wellid     = "1274",
+    start_date = "1990-01-01",
+    end_date   = "2022-01-01"
+    )
+```
+
+![](img/gw_depth_to_water_plot2.png)
```

#### html2text {}

```diff
@@ -1,24 +1,18 @@
-Metadata-Version: 2.1 Name: cdsspy Version: 1.2.70 Summary: Provides Python
-functions for discovering and requesting data from the CDSS REST API. Author:
-Angus Watters Classifier: Programming Language :: Python :: 3 Classifier:
-License :: OSI Approved :: MIT License Classifier: Operating System :: OS
-Independent Requires-Python: >=3.6 Description-Content-Type: text/markdown
-License-File: LICENSE # **cdsspy** [https://cdsspy-images.s3.us-west-
-1.amazonaws.com/co_dnr_div_cdss_cwcbdwr_transparent.png][![Dependencies](https:
-//img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [![License:
-MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
+# **cdsspy** [img/co_dnr_div_cdss_cwcbdwr_transparent.png][![Dependencies]
+(https://img.shields.io/badge/dependencies-12/01-orange?style=flat)](#) [!
+[License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://
 choosealicense.com/licenses/mit/)
-_?Ã_?_?Â_?«_ _CC_DD_SS_SS_ _?Ã_?_?Â_?»
+_?Â_?«_ _CC_DD_SS_SS_ _?Â_?»
 _C_D_S_S_ _R_E_S_T_ _W_e_b_ _S_e_r_v_i_c_e_s
 ===============================================================================
 The goal of [**`cdsspy`**](https://pypi.org/project/cdsspy/) is to provide
 functions that help Python users to navigate, explore, and make requests to the
-CDSS REST API web service. The ColoradoÃ¢â¬â¢s Decision Support Systems
-(CDSS) is a water management system created and developed by the Colorado Water
+CDSS REST API web service. The Coloradoâs Decision Support Systems (CDSS) is
+a water management system created and developed by the Colorado Water
 Conservation Board (CWCB) and the Colorado Division of Water Resources (DWR).
 Thank you to those at CWCB and DWR for providing an accessible and well
 documented REST API!
 > See [**`cdssr`**](https://github.com/anguswg-ucsb/cdssr), for the **R**
 version of this package --- - [**cdssr (R)**](https://github.com/anguswg-ucsb/
 cdssr) - [**cdssr documentation**](https://anguswg-ucsb.github.io/cdssr/) -
 [**cdsspy (Python)**](https://github.com/anguswg-ucsb/cdsspy) - [**cdsspy
@@ -146,32 +140,29 @@
 help#Datasets&#SurfaceWaterController&#gettingstarted&#jsonxml) | |6 |
 **get_telemetry_stations()** | Returns telemetry stations and their most recent
 parameter reading | [telemetrystations/telemetrystation](https://
 dwr.state.co.us/rest/get/
 help#Datasets&#TelemetryStationsController&#gettingstarted&#jsonxml) |
 ### **Example: Locating telemetry stations by county:** ```python # identify
 telemetry stations in Boulder County stations = cdsspy.get_telemetry_stations
-( county = "Boulder" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/county_telem_stations2.png)
+( county = "Boulder" ) ``` ![](img/county_telem_stations2.png)
 
 ### **Example: Locating telemetry stations around a point** ```python #
 identify telemetry stations within a 15 mile radius of the center point of
 Boulder County stations = cdsspy.get_telemetry_stations( aoi = [-105.358164,
-40.092608], radius = 15 ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/poi_telem_stations.png)
+40.092608], radius = 15 ) ``` ![](img/poi_telem_stations.png)
 
 ### **Example: Locating telemetry stations within a spatial extent** A masking
 operation is performed when a location search is done using a **polygon**. This
 ensures that the function only returns points that are ***within*** the given
 polygon. ```python # identify telemetry stations 15 miles around the centroid
 of a polygon stations = cdsspy.get_telemetry_stations( aoi =
-geopandas.read_file("https://cdsspy-images.s3.us-west-1.amazonaws.com/
-boulder_county.gpkg") radius = 15 ) ``` This gif highlights the masking process
-that happens when the **`aoi`** argument is given a **polygon** ![](https://
-cdsspy-images.s3.us-west-1.amazonaws.com/boulder_telem_stations_poly2.gif)
+geopandas.read_file("example-data/boulder_county.gpkg") radius = 15 ) ``` This
+gif highlights the masking process that happens when the **`aoi`** argument is
+given a **polygon** ![](img/boulder_telem_stations_poly2.gif)
 
 
 
 ## **Retrieve time series data** The functions in the table below retrieve time
 series data from the various time series related CDSS API endpoints. |**-**
 |**Function** | **Description** | **Endpoint** | |------|----------------------
 ----------| -------------------------------------------------------------------
@@ -205,16 +196,16 @@
 into the **`get_telemetry_ts()`** function.
 The function below returns a dataframe of daily discharge for the "ANDDITCO"
 site between 2015-2022. ```python # Daily discharge at "ANDDITCO" telemetry
 station discharge_ts = cdsspy.get_telemetry_ts( abbrev = "ANDDITCO", # Site
 abbreviation from the outputs of get_telemetry_stations() parameter =
 "DISCHRG", # Desired parameter, identified by the get_reference_tbl()
 start_date = "2015-01-01", # Starting date end_date = "2022-01-01", # Ending
-date timescale = "day" # select daily timescale ) ``` ![](https://cdsspy-
-images.s3.us-west-1.amazonaws.com/discharge_timeseries_plot2.png)
+date timescale = "day" # select daily timescale ) ``` ![](img/
+discharge_timeseries_plot2.png)
 
 #### **Example: Retrieve Diversion records for multiple structures** Some of
 the CDSS API endpoints allow users to request data from multiple structures if
 you provide a list of IDs. If we want to get diversion data from multiple
 structure locations, we'll need to get a list of WDIDs. We can get a list WDIDs
 within a given area by: 1. Executing a spatial search using **`get_structures
 ()`** 2. Selecting the WDIDs of interest from the search results 3. Providing
@@ -224,15 +215,15 @@
 search results and putting WDIDs into a list ditch_wdids = structures[
 (structures["ciuCode"] == "A") & (structures["structureType"] == "DITCH")]
 ditch_wdids = list(ditch_wdids['wdid']) # 3. Providing the WDID's as a list to
 get_structures_divrec_ts() diversion_rec = cdsspy.get_structures_divrec_ts
 ( wdid = ditch_wdids, wc_identifier = "diversion", timescale = "month" ) ```
 **Note:** Data availability can vary between structures (i.e. Missing data, not
 all structures have every data type/temporal resolution available, etc.) ![]
-(https://cdsspy-images.s3.us-west-1.amazonaws.com/divrec_facet_plot.png)
+(img/divrec_facet_plot.png)
 
 
 
 ## **Retrieve groundwater data** The **`get_gw_()`** set of functions lets
 users retrieve data from the various groundwater related API endpoints shown in
 the table below: | **-** | **Function** | **Endpoint** | |-------|-------------
 --------------------|----------------------------------------------------------
@@ -247,9 +238,8 @@
 **get_gw_gplogs_geologpicks()** | [api/v2/groundwater/geophysicallogs/
 geoplogpicks](https://dwr.state.co.us/Rest/GET/Help/Api/GET-api-v2-groundwater-
 geophysicallogs-geoplogpicks) |
 Here we will retrieve groundwater well measurement data for Well ID 1274
 between 2021-2022. ```python # Request wellmeasurements endpoint (api/v2/
 groundwater/waterlevels/wellmeasurements) well_measure =
 cdsspy.get_gw_wl_wellmeasures( wellid = "1274", start_date = "1990-01-01",
-end_date = "2022-01-01" ) ``` ![](https://cdsspy-images.s3.us-west-
-1.amazonaws.com/gw_depth_to_water_plot2.png)
+end_date = "2022-01-01" ) ``` ![](img/gw_depth_to_water_plot2.png)
```

### Comparing `cdsspy-1.2.70/setup.py` & `cdsspy-1.2.71/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-import setuptools
-
-with open("README.md", "r") as fh:
-    long_description = fh.read()
-
-setuptools.setup(
-    name="cdsspy",                     # This is the name of the package
-    version="1.2.70",                        # The initial release version
-    author="Angus Watters",                     # Full name of the author
-    description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
-    long_description=long_description,      # Long description read from the the readme file
-    long_description_content_type="text/markdown",
-    packages=setuptools.find_packages(),
-    # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
-    classifiers=[
-        "Programming Language :: Python :: 3",
-        "License :: OSI Approved :: MIT License",
-        "Operating System :: OS Independent",
-    ],                                      # Information to filter the project on PyPi website
-    python_requires='>=3.6',                # Minimum version requirement of the package
-    # py_modules=["cdsspy"],             # Name of the python package
-    # package_dir={'':'cdsspy/cdsspy'},     # Directory of the source code of the package
-    install_requires=['pandas', 'datetime', 'requests', 'geopandas', 'shapely', 'pyproj']
+import setuptools
+
+with open("README.md", "r") as fh:
+    long_description = fh.read()
+
+setuptools.setup(
+    name="cdsspy",                     # This is the name of the package
+    version="1.2.71",                        # The initial release version
+    author="Angus Watters",                     # Full name of the author
+    description="Provides Python functions for discovering and requesting data from the CDSS REST API.",
+    long_description=long_description,      # Long description read from the the readme file
+    long_description_content_type="text/markdown",
+    packages=setuptools.find_packages(),
+    # packages=setuptools.find_packages(exclude=["cdsspy.egg_info"]),    # List of all python modules to be installed
+    classifiers=[
+        "Programming Language :: Python :: 3",
+        "License :: OSI Approved :: MIT License",
+        "Operating System :: OS Independent",
+    ],                                      # Information to filter the project on PyPi website
+    python_requires='>=3.6',                # Minimum version requirement of the package
+    # py_modules=["cdsspy"],             # Name of the python package
+    # package_dir={'':'cdsspy/cdsspy'},     # Directory of the source code of the package
+    install_requires=['pandas', 'datetime', 'requests', 'geopandas', 'shapely', 'pyproj']
 )
```

