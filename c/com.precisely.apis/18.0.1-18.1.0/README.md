# Comparing `tmp/com.precisely.apis-18.0.1.tar.gz` & `tmp/com_precisely_apis-18.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.precisely.apis-18.0.1.tar", last modified: Thu Apr 11 06:29:37 2024, max compression
+gzip compressed data, was "com_precisely_apis-18.1.0.tar", last modified: Tue May  7 07:02:36 2024, max compression
```

## Comparing `com.precisely.apis-18.0.1.tar` & `com_precisely_apis-18.1.0.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.278974 com.precisely.apis-18.0.1/
--rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com.precisely.apis-18.0.1/LICENSE
--rw-rw-rw-   0        0        0      540 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/PKG-INFO
--rw-rw-rw-   0        0        0    52015 2024-02-13 12:52:53.000000 com.precisely.apis-18.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.180625 com.precisely.apis-18.0.1/com/
--rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.211875 com.precisely.apis-18.0.1/com/precisely/
--rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.296609 com.precisely.apis-18.0.1/com/precisely/apis/
--rw-rw-rw-   0        0        0      828 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.597407 com.precisely.apis-18.0.1/com/precisely/apis/api/
--rw-rw-rw-   0        0        0      251 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/__init__.py
--rw-rw-rw-   0        0        0    16731 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
--rw-rw-rw-   0        0        0    11240 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_service_api.py
--rw-rw-rw-   0        0        0    30342 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_verification_service_api.py
--rw-rw-rw-   0        0        0    23486 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/addresses_service__api.py
--rw-rw-rw-   0        0        0    42885 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/demographics_service_api.py
--rw-rw-rw-   0        0        0     5850 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/email_verification_service_api.py
--rw-rw-rw-   0        0        0    47771 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/geocode_service_api.py
--rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/geolocation_service_api.py
--rw-rw-rw-   0        0        0    53765 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/local_tax_service_api.py
--rw-rw-rw-   0        0        0     6006 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/neighborhoods_service__api.py
--rw-rw-rw-   0        0        0     5902 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/phone_verification_service_api.py
--rw-rw-rw-   0        0        0    66165 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/places_service__api.py
--rw-rw-rw-   0        0        0    24854 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/property_information_service_api.py
--rw-rw-rw-   0        0        0    25323 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/psap_911_service_api.py
--rw-rw-rw-   0        0        0   154048 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/risks_service_api.py
--rw-rw-rw-   0        0        0    57476 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/routing_service_api.py
--rw-rw-rw-   0        0        0    10328 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/schools_service_api.py
--rw-rw-rw-   0        0        0    19000 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/streets_service_api.py
--rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/telecomm_info_service_api.py
--rw-rw-rw-   0        0        0    21347 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/time_zone_service_api.py
--rw-rw-rw-   0        0        0    53780 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/zones_service_api.py
--rw-rw-rw-   0        0        0    38586 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api_client.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.613034 com.precisely.apis-18.0.1/com/precisely/apis/apis/
--rw-rw-rw-   0        0        0     2215 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/apis/__init__.py
--rw-rw-rw-   0        0        0    16559 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/configuration.py
--rw-rw-rw-   0        0        0     5117 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.248573 com.precisely.apis-18.0.1/com/precisely/apis/model/
--rw-rw-rw-   0        0        0      348 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/__init__.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/absentee_owner.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/accuracy.py
--rw-rw-rw-   0        0        0    17255 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address.py
--rw-rw-rw-   0        0        0    17258 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address1.py
--rw-rw-rw-   0        0        0    17791 2024-04-11 06:20:39.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address2.py
--rw-rw-rw-   0        0        0    11460 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address_time.py
--rw-rw-rw-   0        0        0    11285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address_type.py
--rw-rw-rw-   0        0        0    13513 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_by_boundary_request.py
--rw-rw-rw-   0        0        0    11159 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_count.py
--rw-rw-rw-   0        0        0    14966 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_dto.py
--rw-rw-rw-   0        0        0    11321 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_preferences.py
--rw-rw-rw-   0        0        0    11720 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_response.py
--rw-rw-rw-   0        0        0    17285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ah_jmailing_address.py
--rw-rw-rw-   0        0        0    13338 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj.py
--rw-rw-rw-   0        0        0    11201 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_list.py
--rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_plus_psap_response.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/amenities.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area.py
--rw-rw-rw-   0        0        0    12644 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area_code_info.py
--rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area_v2.py
--rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/assets_and_wealth_theme.py
--rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/base_flood_elevation.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/basement_type.py
--rw-rw-rw-   0        0        0    12377 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/basic_boundary.py
--rw-rw-rw-   0        0        0    11770 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundaries.py
--rw-rw-rw-   0        0        0    12162 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary.py
--rw-rw-rw-   0        0        0    11763 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_buffer.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_point.py
--rw-rw-rw-   0        0        0    11294 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buffer_relation.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_class.py
--rw-rw-rw-   0        0        0    11262 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_condition.py
--rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_features_sqft.py
--rw-rw-rw-   0        0        0    11564 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_area.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_quality.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_style.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_view.py
--rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/building_sqft_source.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/business_id.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ca_exemptions.py
--rw-rw-rw-   0        0        0    13761 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate.py
--rw-rw-rw-   0        0        0    13101 2024-02-13 12:54:08.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range.py
--rw-rw-rw-   0        0        0    12226 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range_unit.py
--rw-rw-rw-   0        0        0    11233 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/carrier.py
--rw-rw-rw-   0        0        0    11930 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/category.py
--rw-rw-rw-   0        0        0    12296 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/category_metadata.py
--rw-rw-rw-   0        0        0    11224 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cbsa.py
--rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/census.py
--rw-rw-rw-   0        0        0    11277 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/center.py
--rw-rw-rw-   0        0        0    11259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/city.py
--rw-rw-rw-   0        0        0    11893 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/common_geometry.py
--rw-rw-rw-   0        0        0    11420 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/community.py
--rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/community_group.py
--rw-rw-rw-   0        0        0    11297 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/consistency_code.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/construction.py
--rw-rw-rw-   0        0        0    12229 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/contact_details.py
--rw-rw-rw-   0        0        0    12861 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/contact_person.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cooling_type.py
--rw-rw-rw-   0        0        0    11691 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cost.py
--rw-rw-rw-   0        0        0    11230 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/county.py
--rw-rw-rw-   0        0        0    11464 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/coverage.py
--rw-rw-rw-   0        0        0    11830 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_boundary.py
--rw-rw-rw-   0        0        0    11750 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_index_theme.py
--rw-rw-rw-   0        0        0    11834 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py
--rw-rw-rw-   0        0        0    11331 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_preferences.py
--rw-rw-rw-   0        0        0    12263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response.py
--rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response_list.py
--rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crs.py
--rw-rw-rw-   0        0        0    11342 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/damage_group.py
--rw-rw-rw-   0        0        0    12065 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics.py
--rw-rw-rw-   0        0        0    11567 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_preferences.py
--rw-rw-rw-   0        0        0    12118 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_request.py
--rw-rw-rw-   0        0        0    11960 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry.py
--rw-rw-rw-   0        0        0    11557 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry_crc.py
--rw-rw-rw-   0        0        0    15660 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_themes_v2.py
--rw-rw-rw-   0        0        0    11232 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/depth.py
--rw-rw-rw-   0        0        0    11328 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/direction_geometry.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance1.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_border.py
--rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
--rw-rw-rw-   0        0        0    11880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
--rw-rw-rw-   0        0        0    11406 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py
--rw-rw-rw-   0        0        0    11288 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/district_type.py
--rw-rw-rw-   0        0        0    11642 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/domestic_ultimate_business.py
--rw-rw-rw-   0        0        0    11266 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_date_time.py
--rw-rw-rw-   0        0        0    13648 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_event.py
--rw-rw-rw-   0        0        0    11621 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_events_response.py
--rw-rw-rw-   0        0        0    11981 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_history.py
--rw-rw-rw-   0        0        0    11313 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_location.py
--rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11815 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12371 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response.py
--rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response_list.py
--rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/education_theme.py
--rw-rw-rw-   0        0        0    11358 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/employee_count.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/employment_theme.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/energy_type.py
--rw-rw-rw-   0        0        0    11332 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_code.py
--rw-rw-rw-   0        0        0    11260 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_info.py
--rw-rw-rw-   0        0        0    11263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_info1.py
--rw-rw-rw-   0        0        0    13880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/events_count.py
--rw-rw-rw-   0        0        0    12070 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/expenditure_theme.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/exterior_walls.py
--rw-rw-rw-   0        0        0    11589 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/extra_feature_sqft.py
--rw-rw-rw-   0        0        0    11445 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/field.py
--rw-rw-rw-   0        0        0    14301 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fields_matching.py
--rw-rw-rw-   0        0        0    12318 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_department.py
--rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event.py
--rw-rw-rw-   0        0        0    12071 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event_v2.py
--rw-rw-rw-   0        0        0    11282 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_response.py
--rw-rw-rw-   0        0        0    11303 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_v2_response.py
--rw-rw-rw-   0        0        0    11733 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history.py
--rw-rw-rw-   0        0        0    11754 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history_v2.py
--rw-rw-rw-   0        0        0    11780 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12122 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response_list.py
--rw-rw-rw-   0        0        0    16206 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response.py
--rw-rw-rw-   0        0        0    11378 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response_list.py
--rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_shed.py
--rw-rw-rw-   0        0        0    13259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station_contact_details.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_stations.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fireplace_type.py
--rw-rw-rw-   0        0        0    11868 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_hazard_preferences.py
--rw-rw-rw-   0        0        0    11819 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11836 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_location_request.py
--rw-rw-rw-   0        0        0    11616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_preferences.py
--rw-rw-rw-   0        0        0    12803 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response.py
--rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response_list.py
--rw-rw-rw-   0        0        0    12555 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_zone.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/floor_type.py
--rw-rw-rw-   0        0        0    13506 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/formatted_tax_address.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/foundation.py
--rw-rw-rw-   0        0        0    11679 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py
--rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/frequency_group.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fuel_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/garage_type.py
--rw-rw-rw-   0        0        0    11682 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_access_point.py
--rw-rw-rw-   0        0        0    11479 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_country.py
--rw-rw-rw-   0        0        0    11957 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_ip_addr.py
--rw-rw-rw-   0        0        0    13204 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_place.py
--rw-rw-rw-   0        0        0    11295 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_state.py
--rw-rw-rw-   0        0        0    11638 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_pos.py
--rw-rw-rw-   0        0        0    14447 2024-02-13 12:54:42.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_address.py
--rw-rw-rw-   0        0        0    18616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_preferences.py
--rw-rw-rw-   0        0        0    11970 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_request.py
--rw-rw-rw-   0        0        0    12023 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response.py
--rw-rw-rw-   0        0        0    11418 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response_list.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geolocation_geometry.py
--rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry.py
--rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_crc.py
--rw-rw-rw-   0        0        0    11088 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_properties.py
--rw-rw-rw-   0        0        0    11461 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input.py
--rw-rw-rw-   0        0        0    11984 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py
--rw-rw-rw-   0        0        0    12600 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_options.py
--rw-rw-rw-   0        0        0    13593 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_output.py
--rw-rw-rw-   0        0        0    11912 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_request.py
--rw-rw-rw-   0        0        0    11470 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_response.py
--rw-rw-rw-   0        0        0    11400 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input.py
--rw-rw-rw-   0        0        0    12159 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py
--rw-rw-rw-   0        0        0    11710 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_options.py
--rw-rw-rw-   0        0        0    13110 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
--rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_request.py
--rw-rw-rw-   0        0        0    11409 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_response.py
--rw-rw-rw-   0        0        0    11636 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/global_ultimate_business.py
--rw-rw-rw-   0        0        0    13489 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/grade_levels_taught.py
--rw-rw-rw-   0        0        0    11435 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/greatschools.py
--rw-rw-rw-   0        0        0    11462 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/grid.py
--rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/health_theme.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/heating_type.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/households_theme.py
--rw-rw-rw-   0        0        0    12058 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/housing_theme.py
--rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/income_theme.py
--rw-rw-rw-   0        0        0    11874 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/index_variable.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/individual_value_variable.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/interior_wall.py
--rw-rw-rw-   0        0        0    11319 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intermediate_points.py
--rw-rw-rw-   0        0        0    12291 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intersection.py
--rw-rw-rw-   0        0        0    11686 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intersection_response.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ip_info.py
--rw-rw-rw-   0        0        0    13054 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd.py
--rw-rw-rw-   0        0        0    11890 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11871 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/key_lookup_request.py
--rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/keys.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/land_use.py
--rw-rw-rw-   0        0        0    12232 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/lat_long_fields.py
--rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/life_style_theme.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/loc_code.py
--rw-rw-rw-   0        0        0    11343 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_geometry.py
--rw-rw-rw-   0        0        0    14407 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_preferences.py
--rw-rw-rw-   0        0        0    11217 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/location.py
--rw-rw-rw-   0        0        0    12025 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/location_time.py
--rw-rw-rw-   0        0        0    12175 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/magnitude.py
--rw-rw-rw-   0        0        0    11972 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/match.py
--rw-rw-rw-   0        0        0    11975 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/match1.py
--rw-rw-rw-   0        0        0    17276 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/matched_address.py
--rw-rw-rw-   0        0        0    12342 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/matrix.py
--rw-rw-rw-   0        0        0    11221 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/mcd.py
--rw-rw-rw-   0        0        0    11652 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/metadata_response.py
--rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/mitigation_group.py
--rw-rw-rw-   0        0        0    11474 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/name.py
--rw-rw-rw-   0        0        0    11477 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/name1.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/neighborhoods_response.py
--rw-rw-rw-   0        0        0    13019 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/network.py
--rw-rw-rw-   0        0        0    11496 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/organization_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/other_rooms.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/owner_vest_type.py
--rw-rw-rw-   0        0        0    11899 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/owners.py
--rw-rw-rw-   0        0        0    13778 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_boundary_v2.py
--rw-rw-rw-   0        0        0    12581 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_v2.py
--rw-rw-rw-   0        0        0    11612 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parent_business.py
--rw-rw-rw-   0        0        0    11412 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_address_request.py
--rw-rw-rw-   0        0        0    11468 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response_list.py
--rw-rw-rw-   0        0        0    11646 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pbkey.py
--rw-rw-rw-   0        0        0    11383 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification.py
--rw-rw-rw-   0        0        0    12826 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification_output.py
--rw-rw-rw-   0        0        0    11592 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/place.py
--rw-rw-rw-   0        0        0    11602 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/place1.py
--rw-rw-rw-   0        0        0    12227 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/places_response.py
--rw-rw-rw-   0        0        0    20808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi.py
--rw-rw-rw-   0        0        0    12870 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary.py
--rw-rw-rw-   0        0        0    11840 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_address_request.py
--rw-rw-rw-   0        0        0    11900 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_location_request.py
--rw-rw-rw-   0        0        0    11825 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_locations.py
--rw-rw-rw-   0        0        0    11548 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_preferences.py
--rw-rw-rw-   0        0        0    11333 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_response.py
--rw-rw-rw-   0        0        0    11800 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_classification.py
--rw-rw-rw-   0        0        0    11116 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count.py
--rw-rw-rw-   0        0        0    12954 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count_request.py
--rw-rw-rw-   0        0        0    13374 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poiby_geometry_request.py
--rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/points.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pool_type.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/population_theme.py
--rw-rw-rw-   0        0        0    11114 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/preferenc_time_zone.py
--rw-rw-rw-   0        0        0    11280 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/primary_zone.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/prior_sale_code.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/prop_site_influene.py
--rw-rw-rw-   0        0        0    11106 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/properties.py
--rw-rw-rw-   0        0        0    46206 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_attributes.py
--rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_geometry.py
--rw-rw-rw-   0        0        0    11918 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_address_request.py
--rw-rw-rw-   0        0        0    11133 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_preferences.py
--rw-rw-rw-   0        0        0    12002 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_response.py
--rw-rw-rw-   0        0        0    11457 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_responses.py
--rw-rw-rw-   0        0        0    12031 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry.py
--rw-rw-rw-   0        0        0    11578 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry_crc.py
--rw-rw-rw-   0        0        0    11696 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/proxy.py
--rw-rw-rw-   0        0        0    13793 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/psap_response.py
--rw-rw-rw-   0        0        0    12085 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py
--rw-rw-rw-   0        0        0    12626 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/range_variable.py
--rw-rw-rw-   0        0        0    11664 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/rate.py
--rw-rw-rw-   0        0        0    13762 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/rate_center_response.py
--rw-rw-rw-   0        0        0    12337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/return_fields_descriptor.py
--rw-rw-rw-   0        0        0    11723 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/reverse_geocode_request.py
--rw-rw-rw-   0        0        0    14978 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk.py
--rw-rw-rw-   0        0        0    17267 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_address.py
--rw-rw-rw-   0        0        0    11337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_geometry.py
--rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_locations.py
--rw-rw-rw-   0        0        0    11601 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_preferences.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_boundaries.py
--rw-rw-rw-   0        0        0    11368 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_crime_theme.py
--rw-rw-rw-   0        0        0    11536 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_geometry_crc.py
--rw-rw-rw-   0        0        0    13324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/road.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_cover_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_frame_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_shape_type.py
--rw-rw-rw-   0        0        0    12381 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_direction.py
--rw-rw-rw-   0        0        0    11304 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_geometry.py
--rw-rw-rw-   0        0        0    13382 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_response.py
--rw-rw-rw-   0        0        0    13904 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sales_tax.py
--rw-rw-rw-   0        0        0    11569 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sales_volume.py
--rw-rw-rw-   0        0        0    19116 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school.py
--rw-rw-rw-   0        0        0    12879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_district.py
--rw-rw-rw-   0        0        0    13410 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_profile.py
--rw-rw-rw-   0        0        0    12471 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_ranking.py
--rw-rw-rw-   0        0        0    12003 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/schools_near_by_response.py
--rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation.py
--rw-rw-rw-   0        0        0    11365 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation_themes.py
--rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/severity_group.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/shore_line_distance.py
--rw-rw-rw-   0        0        0    12022 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sic.py
--rw-rw-rw-   0        0        0    12330 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sic_metadata.py
--rw-rw-rw-   0        0        0    12078 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/site_details.py
--rw-rw-rw-   0        0        0    13485 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/situs_address.py
--rw-rw-rw-   0        0        0    12476 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district.py
--rw-rw-rw-   0        0        0    11579 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district_tax.py
--rw-rw-rw-   0        0        0    13049 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/speed_limit.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/start_end_point.py
--rw-rw-rw-   0        0        0    11227 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/state.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/status.py
--rw-rw-rw-   0        0        0    11273 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/stories.py
--rw-rw-rw-   0        0        0    12424 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/student_ethnicity.py
--rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/supply_and_demand_theme.py
--rw-rw-rw-   0        0        0    18388 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address.py
--rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address_request.py
--rw-rw-rw-   0        0        0    11239 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_county.py
--rw-rw-rw-   0        0        0    13607 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response.py
--rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response_list.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_doc_type.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_exemption.py
--rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_geometry.py
--rw-rw-rw-   0        0        0    12257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_location_request.py
--rw-rw-rw-   0        0        0    11787 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_locations.py
--rw-rw-rw-   0        0        0    12845 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_place.py
--rw-rw-rw-   0        0        0    18168 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address.py
--rw-rw-rw-   0        0        0    11919 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address_request.py
--rw-rw-rw-   0        0        0    11810 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_location_request.py
--rw-rw-rw-   0        0        0    17504 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_matched_address.py
--rw-rw-rw-   0        0        0    14126 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_response.py
--rw-rw-rw-   0        0        0    11346 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_responses.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_sales_price_code.py
--rw-rw-rw-   0        0        0    11236 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_state.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/time.py
--rw-rw-rw-   0        0        0    11731 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_address_request.py
--rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_geometry.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_location_request.py
--rw-rw-rw-   0        0        0    15252 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response.py
--rw-rw-rw-   0        0        0    11352 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response_list.py
--rw-rw-rw-   0        0        0    11354 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundaries.py
--rw-rw-rw-   0        0        0    11234 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundary.py
--rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_cost_matrix_response.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/type.py
--rw-rw-rw-   0        0        0    13895 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_location.py
--rw-rw-rw-   0        0        0    11353 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_locations.py
--rw-rw-rw-   0        0        0    11505 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_range.py
--rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_unit.py
--rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/unit.py
--rw-rw-rw-   0        0        0    13898 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/use_tax.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/vacancy.py
--rw-rw-rw-   0        0        0    11817 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_request.py
--rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_response.py
--rw-rw-rw-   0        0        0    11429 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input.py
--rw-rw-rw-   0        0        0    16658 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input_row.py
--rw-rw-rw-   0        0        0    15324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_output.py
--rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input.py
--rw-rw-rw-   0        0        0    13503 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_options.py
--rw-rw-rw-   0        0        0    15940 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_output.py
--rw-rw-rw-   0        0        0    11520 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py
--rw-rw-rw-   0        0        0    14342 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
--rw-rw-rw-   0        0        0    15105 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py
--rw-rw-rw-   0        0        0    39660 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py
--rw-rw-rw-   0        0        0    12012 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py
--rw-rw-rw-   0        0        0    11529 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py
--rw-rw-rw-   0        0        0    11480 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py
--rw-rw-rw-   0        0        0    13512 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
--rw-rw-rw-   0        0        0    14100 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py
--rw-rw-rw-   0        0        0    18611 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py
--rw-rw-rw-   0        0        0    11944 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py
--rw-rw-rw-   0        0        0    11489 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py
--rw-rw-rw-   0        0        0    11891 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_request.py
--rw-rw-rw-   0        0        0    11458 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_response.py
--rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
--rw-rw-rw-   0        0        0    14701 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
--rw-rw-rw-   0        0        0    36257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
--rw-rw-rw-   0        0        0    49413 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
--rw-rw-rw-   0        0        0    12029 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
--rw-rw-rw-   0        0        0    11539 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
--rw-rw-rw-   0        0        0    11488 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request.py
--rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py
--rw-rw-rw-   0        0        0    11377 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
--rw-rw-rw-   0        0        0    11760 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/water_body.py
--rw-rw-rw-   0        0        0    11870 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/water_body_response.py
--rw-rw-rw-   0        0        0    17270 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_address.py
--rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_boundary_geometry.py
--rw-rw-rw-   0        0        0    11574 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_contact_details.py
--rw-rw-rw-   0        0        0    11340 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_geometry.py
--rw-rw-rw-   0        0        0    11091 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_parent_business.py
--rw-rw-rw-   0        0        0    14879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi.py
--rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_classification.py
--rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_geometry.py
--rw-rw-rw-   0        0        0    11791 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_sic.py
--rw-rw-rw-   0        0        0    81943 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/model_utils.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/com/precisely/apis/models/
--rw-rw-rw-   0        0        0    28241 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/models/__init__.py
--rw-rw-rw-   0        0        0    14245 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/rest.py
-drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/
--rw-rw-rw-   0        0        0      540 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19569 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2024-04-11 06:29:37.291172 com.precisely.apis-18.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1224 2024-04-11 06:23:16.000000 com.precisely.apis-18.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:36.140033 com_precisely_apis-18.1.0/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com_precisely_apis-18.1.0/LICENSE
+-rw-rw-rw-   0        0        0      540 2024-05-07 07:02:36.136032 com_precisely_apis-18.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0    52015 2024-02-13 12:52:53.000000 com_precisely_apis-18.1.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:31.081960 com_precisely_apis-18.1.0/com/
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:31.262220 com_precisely_apis-18.1.0/com/precisely/
+-rw-rw-rw-   0        0        0        0 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:31.315221 com_precisely_apis-18.1.0/com/precisely/apis/
+-rw-rw-rw-   0        0        0      828 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:31.586233 com_precisely_apis-18.1.0/com/precisely/apis/api/
+-rw-rw-rw-   0        0        0      251 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/__init__.py
+-rw-rw-rw-   0        0        0    16731 2024-04-25 06:40:40.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
+-rw-rw-rw-   0        0        0    11240 2024-04-25 06:40:40.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/address_autocomplete_service_api.py
+-rw-rw-rw-   0        0        0    30342 2024-04-25 06:40:40.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/address_verification_service_api.py
+-rw-rw-rw-   0        0        0    23486 2024-04-25 06:40:41.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/addresses_service__api.py
+-rw-rw-rw-   0        0        0    42885 2024-04-25 06:40:41.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/demographics_service_api.py
+-rw-rw-rw-   0        0        0     5850 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/email_verification_service_api.py
+-rw-rw-rw-   0        0        0    47380 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/geocode_service_api.py
+-rw-rw-rw-   0        0        0    11824 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/geolocation_service_api.py
+-rw-rw-rw-   0        0        0    53765 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/local_tax_service_api.py
+-rw-rw-rw-   0        0        0     6006 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/neighborhoods_service__api.py
+-rw-rw-rw-   0        0        0     5902 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/phone_verification_service_api.py
+-rw-rw-rw-   0        0        0    66165 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/places_service__api.py
+-rw-rw-rw-   0        0        0    24854 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/property_information_service_api.py
+-rw-rw-rw-   0        0        0    25323 2024-04-25 06:40:42.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/psap_911_service_api.py
+-rw-rw-rw-   0        0        0   154048 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/risks_service_api.py
+-rw-rw-rw-   0        0        0    57476 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/routing_service_api.py
+-rw-rw-rw-   0        0        0    10328 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/schools_service_api.py
+-rw-rw-rw-   0        0        0    19000 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/streets_service_api.py
+-rw-rw-rw-   0        0        0    11449 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/telecomm_info_service_api.py
+-rw-rw-rw-   0        0        0    21347 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/time_zone_service_api.py
+-rw-rw-rw-   0        0        0    53780 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api/zones_service_api.py
+-rw-rw-rw-   0        0        0    38586 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/api_client.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:31.659237 com_precisely_apis-18.1.0/com/precisely/apis/apis/
+-rw-rw-rw-   0        0        0     2215 2024-04-25 06:40:44.000000 com_precisely_apis-18.1.0/com/precisely/apis/apis/__init__.py
+-rw-rw-rw-   0        0        0    16559 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/configuration.py
+-rw-rw-rw-   0        0        0     5117 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:36.069306 com_precisely_apis-18.1.0/com/precisely/apis/model/
+-rw-rw-rw-   0        0        0      348 2024-04-25 06:40:44.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/__init__.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/absentee_owner.py
+-rw-rw-rw-   0        0        0    11241 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/accuracy.py
+-rw-rw-rw-   0        0        0    17255 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/address.py
+-rw-rw-rw-   0        0        0    17258 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/address1.py
+-rw-rw-rw-   0        0        0    17791 2024-05-07 06:57:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/address2.py
+-rw-rw-rw-   0        0        0    11460 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/address_time.py
+-rw-rw-rw-   0        0        0    11285 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/address_type.py
+-rw-rw-rw-   0        0        0    13513 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_by_boundary_request.py
+-rw-rw-rw-   0        0        0    11159 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_count.py
+-rw-rw-rw-   0        0        0    14966 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_dto.py
+-rw-rw-rw-   0        0        0    11321 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_preferences.py
+-rw-rw-rw-   0        0        0    11720 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_response.py
+-rw-rw-rw-   0        0        0    17285 2024-04-25 06:40:06.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ah_jmailing_address.py
+-rw-rw-rw-   0        0        0    13338 2024-04-25 06:40:05.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ahj.py
+-rw-rw-rw-   0        0        0    11201 2024-04-25 06:40:05.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ahj_list.py
+-rw-rw-rw-   0        0        0    11761 2024-04-25 06:40:05.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ahj_plus_psap_response.py
+-rw-rw-rw-   0        0        0    11244 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/amenities.py
+-rw-rw-rw-   0        0        0    11229 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/area.py
+-rw-rw-rw-   0        0        0    12644 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/area_code_info.py
+-rw-rw-rw-   0        0        0    11235 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/area_v2.py
+-rw-rw-rw-   0        0        0    12082 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/assets_and_wealth_theme.py
+-rw-rw-rw-   0        0        0    11271 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/base_flood_elevation.py
+-rw-rw-rw-   0        0        0    11253 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/basement_type.py
+-rw-rw-rw-   0        0        0    12377 2024-04-25 06:40:07.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/basic_boundary.py
+-rw-rw-rw-   0        0        0    11770 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/boundaries.py
+-rw-rw-rw-   0        0        0    12162 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/boundary.py
+-rw-rw-rw-   0        0        0    11763 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/boundary_buffer.py
+-rw-rw-rw-   0        0        0    11298 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/boundary_point.py
+-rw-rw-rw-   0        0        0    11294 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buffer_relation.py
+-rw-rw-rw-   0        0        0    11250 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_class.py
+-rw-rw-rw-   0        0        0    11262 2024-04-25 06:40:08.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_condition.py
+-rw-rw-rw-   0        0        0    11595 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_features_sqft.py
+-rw-rw-rw-   0        0        0    11564 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_improve_area.py
+-rw-rw-rw-   0        0        0    11268 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_improve_type.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_quality.py
+-rw-rw-rw-   0        0        0    11250 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_style.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_type.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_view.py
+-rw-rw-rw-   0        0        0    11271 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/building_sqft_source.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:09.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/business_id.py
+-rw-rw-rw-   0        0        0    11253 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ca_exemptions.py
+-rw-rw-rw-   0        0        0    13761 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/candidate.py
+-rw-rw-rw-   0        0        0    13101 2024-05-07 06:56:46.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/candidate_range.py
+-rw-rw-rw-   0        0        0    12226 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/candidate_range_unit.py
+-rw-rw-rw-   0        0        0    11233 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/carrier.py
+-rw-rw-rw-   0        0        0    11930 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/category.py
+-rw-rw-rw-   0        0        0    12296 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/category_metadata.py
+-rw-rw-rw-   0        0        0    11224 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/cbsa.py
+-rw-rw-rw-   0        0        0    12050 2024-04-25 06:40:10.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/census.py
+-rw-rw-rw-   0        0        0    11277 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/center.py
+-rw-rw-rw-   0        0        0    11259 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/city.py
+-rw-rw-rw-   0        0        0    11893 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/common_geometry.py
+-rw-rw-rw-   0        0        0    11420 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/community.py
+-rw-rw-rw-   0        0        0    11716 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/community_group.py
+-rw-rw-rw-   0        0        0    11297 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/consistency_code.py
+-rw-rw-rw-   0        0        0    11253 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/construction.py
+-rw-rw-rw-   0        0        0    12229 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/contact_details.py
+-rw-rw-rw-   0        0        0    12861 2024-04-25 06:40:11.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/contact_person.py
+-rw-rw-rw-   0        0        0    11250 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/cooling_type.py
+-rw-rw-rw-   0        0        0    11691 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/cost.py
+-rw-rw-rw-   0        0        0    11230 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/county.py
+-rw-rw-rw-   0        0        0    11464 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/coverage.py
+-rw-rw-rw-   0        0        0    11830 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_boundary.py
+-rw-rw-rw-   0        0        0    11750 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_index_theme.py
+-rw-rw-rw-   0        0        0    11834 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11851 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py
+-rw-rw-rw-   0        0        0    11331 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_preferences.py
+-rw-rw-rw-   0        0        0    12263 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_response_list.py
+-rw-rw-rw-   0        0        0    11530 2024-04-25 06:40:12.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/crs.py
+-rw-rw-rw-   0        0        0    11342 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/damage_group.py
+-rw-rw-rw-   0        0        0    12065 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics.py
+-rw-rw-rw-   0        0        0    11567 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_advanced_preferences.py
+-rw-rw-rw-   0        0        0    12118 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_advanced_request.py
+-rw-rw-rw-   0        0        0    11960 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_geometry.py
+-rw-rw-rw-   0        0        0    11557 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_geometry_crc.py
+-rw-rw-rw-   0        0        0    15660 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_themes_v2.py
+-rw-rw-rw-   0        0        0    11232 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/depth.py
+-rw-rw-rw-   0        0        0    11328 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/direction_geometry.py
+-rw-rw-rw-   0        0        0    11241 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance.py
+-rw-rw-rw-   0        0        0    11244 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance1.py
+-rw-rw-rw-   0        0        0    11265 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_border.py
+-rw-rw-rw-   0        0        0    11863 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
+-rw-rw-rw-   0        0        0    11880 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
+-rw-rw-rw-   0        0        0    11406 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_response.py
+-rw-rw-rw-   0        0        0    11288 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/district_type.py
+-rw-rw-rw-   0        0        0    11642 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/domestic_ultimate_business.py
+-rw-rw-rw-   0        0        0    11266 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_date_time.py
+-rw-rw-rw-   0        0        0    13648 2024-04-25 06:40:13.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_event.py
+-rw-rw-rw-   0        0        0    11621 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_events_response.py
+-rw-rw-rw-   0        0        0    11981 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_history.py
+-rw-rw-rw-   0        0        0    11313 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_location.py
+-rw-rw-rw-   0        0        0    11798 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11815 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12371 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_response.py
+-rw-rw-rw-   0        0        0    11447 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_response_list.py
+-rw-rw-rw-   0        0        0    12064 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/education_theme.py
+-rw-rw-rw-   0        0        0    11358 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/employee_count.py
+-rw-rw-rw-   0        0        0    12067 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/employment_theme.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/energy_type.py
+-rw-rw-rw-   0        0        0    11332 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/error_code.py
+-rw-rw-rw-   0        0        0    11260 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/error_info.py
+-rw-rw-rw-   0        0        0    11263 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/error_info1.py
+-rw-rw-rw-   0        0        0    13880 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/events_count.py
+-rw-rw-rw-   0        0        0    12070 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/expenditure_theme.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:14.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/exterior_walls.py
+-rw-rw-rw-   0        0        0    11589 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/extra_feature_sqft.py
+-rw-rw-rw-   0        0        0    11445 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/field.py
+-rw-rw-rw-   0        0        0    14301 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fields_matching.py
+-rw-rw-rw-   0        0        0    12318 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_department.py
+-rw-rw-rw-   0        0        0    12050 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_event.py
+-rw-rw-rw-   0        0        0    12071 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_event_v2.py
+-rw-rw-rw-   0        0        0    11282 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_events_response.py
+-rw-rw-rw-   0        0        0    11303 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_events_v2_response.py
+-rw-rw-rw-   0        0        0    11733 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_history.py
+-rw-rw-rw-   0        0        0    11754 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_history_v2.py
+-rw-rw-rw-   0        0        0    11780 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11797 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12122 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_response.py
+-rw-rw-rw-   0        0        0    11357 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_response_list.py
+-rw-rw-rw-   0        0        0    16206 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_v2_response.py
+-rw-rw-rw-   0        0        0    11378 2024-04-25 06:40:15.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_v2_response_list.py
+-rw-rw-rw-   0        0        0    11725 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_shed.py
+-rw-rw-rw-   0        0        0    13259 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_station.py
+-rw-rw-rw-   0        0        0    11677 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_station_contact_details.py
+-rw-rw-rw-   0        0        0    11677 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fire_stations.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fireplace_type.py
+-rw-rw-rw-   0        0        0    11868 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_hazard_preferences.py
+-rw-rw-rw-   0        0        0    11819 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11836 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    11616 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_preferences.py
+-rw-rw-rw-   0        0        0    12803 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_response_list.py
+-rw-rw-rw-   0        0        0    12555 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/flood_zone.py
+-rw-rw-rw-   0        0        0    11244 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/floor_type.py
+-rw-rw-rw-   0        0        0    13506 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/formatted_tax_address.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/foundation.py
+-rw-rw-rw-   0        0        0    11679 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/free_or_reduced_price_lunches.py
+-rw-rw-rw-   0        0        0    11716 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/frequency_group.py
+-rw-rw-rw-   0        0        0    11241 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/fuel_type.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/garage_type.py
+-rw-rw-rw-   0        0        0    11682 2024-04-25 06:40:16.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_access_point.py
+-rw-rw-rw-   0        0        0    11479 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_country.py
+-rw-rw-rw-   0        0        0    11957 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_ip_addr.py
+-rw-rw-rw-   0        0        0    13204 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_place.py
+-rw-rw-rw-   0        0        0    11295 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_state.py
+-rw-rw-rw-   0        0        0    11638 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geo_pos.py
+-rw-rw-rw-   0        0        0    14447 2024-05-07 06:56:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_address.py
+-rw-rw-rw-   0        0        0    18616 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_preferences.py
+-rw-rw-rw-   0        0        0    11970 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_request.py
+-rw-rw-rw-   0        0        0    12023 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_service_response.py
+-rw-rw-rw-   0        0        0    11418 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_service_response_list.py
+-rw-rw-rw-   0        0        0    11316 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geolocation_geometry.py
+-rw-rw-rw-   0        0        0    11283 2024-04-25 06:40:17.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geometry.py
+-rw-rw-rw-   0        0        0    11521 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geometry_crc.py
+-rw-rw-rw-   0        0        0    11088 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/geometry_properties.py
+-rw-rw-rw-   0        0        0    11461 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_input.py
+-rw-rw-rw-   0        0        0    11984 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_input_row.py
+-rw-rw-rw-   0        0        0    12600 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_options.py
+-rw-rw-rw-   0        0        0    13593 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_output.py
+-rw-rw-rw-   0        0        0    11912 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_request.py
+-rw-rw-rw-   0        0        0    11470 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_response.py
+-rw-rw-rw-   0        0        0    11400 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_input.py
+-rw-rw-rw-   0        0        0    12159 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_input_row.py
+-rw-rw-rw-   0        0        0    11710 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_options.py
+-rw-rw-rw-   0        0        0    13110 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_output.py
+-rw-rw-rw-   0        0        0    11316 2024-04-25 06:40:18.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
+-rw-rw-rw-   0        0        0    11808 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_request.py
+-rw-rw-rw-   0        0        0    11409 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_response.py
+-rw-rw-rw-   0        0        0    11636 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/global_ultimate_business.py
+-rw-rw-rw-   0        0        0    13489 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/grade_levels_taught.py
+-rw-rw-rw-   0        0        0    11435 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/greatschools.py
+-rw-rw-rw-   0        0        0    11462 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/grid.py
+-rw-rw-rw-   0        0        0    12055 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/health_theme.py
+-rw-rw-rw-   0        0        0    11250 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/heating_type.py
+-rw-rw-rw-   0        0        0    12067 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/households_theme.py
+-rw-rw-rw-   0        0        0    12058 2024-04-25 06:40:19.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/housing_theme.py
+-rw-rw-rw-   0        0        0    12055 2024-04-25 06:40:20.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/income_theme.py
+-rw-rw-rw-   0        0        0    11874 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/index_variable.py
+-rw-rw-rw-   0        0        0    11677 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/individual_value_variable.py
+-rw-rw-rw-   0        0        0    11253 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/interior_wall.py
+-rw-rw-rw-   0        0        0    11319 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/intermediate_points.py
+-rw-rw-rw-   0        0        0    12291 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/intersection.py
+-rw-rw-rw-   0        0        0    11686 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/intersection_response.py
+-rw-rw-rw-   0        0        0    12067 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ip_info.py
+-rw-rw-rw-   0        0        0    13054 2024-04-25 06:40:21.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ipd.py
+-rw-rw-rw-   0        0        0    11890 2024-04-25 06:40:20.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11871 2024-04-25 06:40:20.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/ipd_tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11808 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/key_lookup_request.py
+-rw-rw-rw-   0        0        0    11446 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/keys.py
+-rw-rw-rw-   0        0        0    11238 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/land_use.py
+-rw-rw-rw-   0        0        0    12232 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/lat_long_fields.py
+-rw-rw-rw-   0        0        0    12064 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/life_style_theme.py
+-rw-rw-rw-   0        0        0    11238 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/loc_code.py
+-rw-rw-rw-   0        0        0    11343 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/local_tax_geometry.py
+-rw-rw-rw-   0        0        0    14407 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/local_tax_preferences.py
+-rw-rw-rw-   0        0        0    11217 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/location.py
+-rw-rw-rw-   0        0        0    12025 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/location_time.py
+-rw-rw-rw-   0        0        0    12175 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/magnitude.py
+-rw-rw-rw-   0        0        0    11972 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/match.py
+-rw-rw-rw-   0        0        0    11975 2024-04-25 06:40:22.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/match1.py
+-rw-rw-rw-   0        0        0    17276 2024-04-25 06:40:23.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/matched_address.py
+-rw-rw-rw-   0        0        0    12342 2024-04-25 06:40:23.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/matrix.py
+-rw-rw-rw-   0        0        0    11221 2024-04-25 06:40:23.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/mcd.py
+-rw-rw-rw-   0        0        0    11652 2024-04-25 06:40:23.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/metadata_response.py
+-rw-rw-rw-   0        0        0    11709 2024-04-25 06:40:24.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/mitigation_group.py
+-rw-rw-rw-   0        0        0    11474 2024-04-25 06:40:24.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/name.py
+-rw-rw-rw-   0        0        0    11477 2024-04-25 06:40:24.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/name1.py
+-rw-rw-rw-   0        0        0    11298 2024-04-25 06:40:24.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/neighborhoods_response.py
+-rw-rw-rw-   0        0        0    13019 2024-04-25 06:40:25.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/network.py
+-rw-rw-rw-   0        0        0    11496 2024-04-25 06:40:25.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/organization_type.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:25.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/other_rooms.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:25.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/owner_vest_type.py
+-rw-rw-rw-   0        0        0    11899 2024-04-25 06:40:25.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/owners.py
+-rw-rw-rw-   0        0        0    13778 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/parcel_boundary_v2.py
+-rw-rw-rw-   0        0        0    12581 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/parcel_v2.py
+-rw-rw-rw-   0        0        0    11612 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/parent_business.py
+-rw-rw-rw-   0        0        0    11412 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_address_request.py
+-rw-rw-rw-   0        0        0    11468 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_response.py
+-rw-rw-rw-   0        0        0    11250 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_response_list.py
+-rw-rw-rw-   0        0        0    11646 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/pbkey.py
+-rw-rw-rw-   0        0        0    11383 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/phone_verification.py
+-rw-rw-rw-   0        0        0    12826 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/phone_verification_output.py
+-rw-rw-rw-   0        0        0    11592 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/place.py
+-rw-rw-rw-   0        0        0    11602 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/place1.py
+-rw-rw-rw-   0        0        0    12227 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/places_response.py
+-rw-rw-rw-   0        0        0    20808 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi.py
+-rw-rw-rw-   0        0        0    12870 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary.py
+-rw-rw-rw-   0        0        0    11840 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_address_request.py
+-rw-rw-rw-   0        0        0    11900 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_location_request.py
+-rw-rw-rw-   0        0        0    11825 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_locations.py
+-rw-rw-rw-   0        0        0    11548 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_preferences.py
+-rw-rw-rw-   0        0        0    11333 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_response.py
+-rw-rw-rw-   0        0        0    11800 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_classification.py
+-rw-rw-rw-   0        0        0    11116 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_count.py
+-rw-rw-rw-   0        0        0    12954 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poi_count_request.py
+-rw-rw-rw-   0        0        0    13374 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/poiby_geometry_request.py
+-rw-rw-rw-   0        0        0    11725 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/points.py
+-rw-rw-rw-   0        0        0    11241 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/pool_type.py
+-rw-rw-rw-   0        0        0    12067 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/population_theme.py
+-rw-rw-rw-   0        0        0    11114 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/preferenc_time_zone.py
+-rw-rw-rw-   0        0        0    11280 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/primary_zone.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:27.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/prior_sale_code.py
+-rw-rw-rw-   0        0        0    11265 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/prop_site_influene.py
+-rw-rw-rw-   0        0        0    11106 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/properties.py
+-rw-rw-rw-   0        0        0    46206 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_attributes.py
+-rw-rw-rw-   0        0        0    11349 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_geometry.py
+-rw-rw-rw-   0        0        0    11918 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_address_request.py
+-rw-rw-rw-   0        0        0    11133 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_preferences.py
+-rw-rw-rw-   0        0        0    12002 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_response.py
+-rw-rw-rw-   0        0        0    11457 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_responses.py
+-rw-rw-rw-   0        0        0    12031 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_information_geometry.py
+-rw-rw-rw-   0        0        0    11578 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/property_information_geometry_crc.py
+-rw-rw-rw-   0        0        0    11696 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/proxy.py
+-rw-rw-rw-   0        0        0    13793 2024-04-25 06:40:26.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/psap_response.py
+-rw-rw-rw-   0        0        0    12085 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/race_and_ethnicity_theme.py
+-rw-rw-rw-   0        0        0    12626 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/range_variable.py
+-rw-rw-rw-   0        0        0    11664 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/rate.py
+-rw-rw-rw-   0        0        0    13762 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/rate_center_response.py
+-rw-rw-rw-   0        0        0    12337 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/return_fields_descriptor.py
+-rw-rw-rw-   0        0        0    11723 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/reverse_geocode_request.py
+-rw-rw-rw-   0        0        0    14978 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risk.py
+-rw-rw-rw-   0        0        0    17267 2024-04-25 06:40:28.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risk_address.py
+-rw-rw-rw-   0        0        0    11337 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risk_geometry.py
+-rw-rw-rw-   0        0        0    11797 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risk_locations.py
+-rw-rw-rw-   0        0        0    11601 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risk_preferences.py
+-rw-rw-rw-   0        0        0    11316 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risks_boundaries.py
+-rw-rw-rw-   0        0        0    11368 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risks_crime_theme.py
+-rw-rw-rw-   0        0        0    11536 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/risks_geometry_crc.py
+-rw-rw-rw-   0        0        0    13324 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/road.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/roof_cover_type.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/roof_frame_type.py
+-rw-rw-rw-   0        0        0    11256 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/roof_shape_type.py
+-rw-rw-rw-   0        0        0    12381 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/route_direction.py
+-rw-rw-rw-   0        0        0    11304 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/route_geometry.py
+-rw-rw-rw-   0        0        0    13382 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/route_response.py
+-rw-rw-rw-   0        0        0    13904 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/sales_tax.py
+-rw-rw-rw-   0        0        0    11569 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/sales_volume.py
+-rw-rw-rw-   0        0        0    19116 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/school.py
+-rw-rw-rw-   0        0        0    12879 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/school_district.py
+-rw-rw-rw-   0        0        0    13410 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/school_profile.py
+-rw-rw-rw-   0        0        0    12471 2024-04-25 06:40:29.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/school_ranking.py
+-rw-rw-rw-   0        0        0    12003 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/schools_near_by_response.py
+-rw-rw-rw-   0        0        0    11761 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/segmentation.py
+-rw-rw-rw-   0        0        0    11365 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/segmentation_themes.py
+-rw-rw-rw-   0        0        0    11709 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/severity_group.py
+-rw-rw-rw-   0        0        0    11268 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/shore_line_distance.py
+-rw-rw-rw-   0        0        0    12022 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/sic.py
+-rw-rw-rw-   0        0        0    12330 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/sic_metadata.py
+-rw-rw-rw-   0        0        0    12078 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/site_details.py
+-rw-rw-rw-   0        0        0    13485 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/situs_address.py
+-rw-rw-rw-   0        0        0    12476 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/special_purpose_district.py
+-rw-rw-rw-   0        0        0    11579 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/special_purpose_district_tax.py
+-rw-rw-rw-   0        0        0    13049 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/speed_limit.py
+-rw-rw-rw-   0        0        0    11298 2024-04-25 06:40:30.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/start_end_point.py
+-rw-rw-rw-   0        0        0    11227 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/state.py
+-rw-rw-rw-   0        0        0    11265 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/status.py
+-rw-rw-rw-   0        0        0    11273 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/stories.py
+-rw-rw-rw-   0        0        0    12424 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/student_ethnicity.py
+-rw-rw-rw-   0        0        0    12082 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/supply_and_demand_theme.py
+-rw-rw-rw-   0        0        0    18388 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_address.py
+-rw-rw-rw-   0        0        0    11824 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_address_request.py
+-rw-rw-rw-   0        0        0    11239 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_county.py
+-rw-rw-rw-   0        0        0    13607 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_district_response.py
+-rw-rw-rw-   0        0        0    11446 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_district_response_list.py
+-rw-rw-rw-   0        0        0    11247 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_doc_type.py
+-rw-rw-rw-   0        0        0    11253 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_exemption.py
+-rw-rw-rw-   0        0        0    11334 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_geometry.py
+-rw-rw-rw-   0        0        0    12257 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11798 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_location_request.py
+-rw-rw-rw-   0        0        0    11787 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_locations.py
+-rw-rw-rw-   0        0        0    12845 2024-04-25 06:40:31.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_place.py
+-rw-rw-rw-   0        0        0    18168 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_address.py
+-rw-rw-rw-   0        0        0    11919 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_address_request.py
+-rw-rw-rw-   0        0        0    11810 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_location_request.py
+-rw-rw-rw-   0        0        0    17504 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_matched_address.py
+-rw-rw-rw-   0        0        0    14126 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_response.py
+-rw-rw-rw-   0        0        0    11346 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_responses.py
+-rw-rw-rw-   0        0        0    11268 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_sales_price_code.py
+-rw-rw-rw-   0        0        0    11236 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/tax_state.py
+-rw-rw-rw-   0        0        0    11229 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/time.py
+-rw-rw-rw-   0        0        0    11731 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_address_request.py
+-rw-rw-rw-   0        0        0    11349 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_geometry.py
+-rw-rw-rw-   0        0        0    11357 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_location_request.py
+-rw-rw-rw-   0        0        0    15252 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_response.py
+-rw-rw-rw-   0        0        0    11352 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_response_list.py
+-rw-rw-rw-   0        0        0    11354 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/travel_boundaries.py
+-rw-rw-rw-   0        0        0    11234 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/travel_boundary.py
+-rw-rw-rw-   0        0        0    11283 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/travel_cost_matrix_response.py
+-rw-rw-rw-   0        0        0    11229 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/type.py
+-rw-rw-rw-   0        0        0    13895 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_location.py
+-rw-rw-rw-   0        0        0    11353 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_locations.py
+-rw-rw-rw-   0        0        0    11505 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_range.py
+-rw-rw-rw-   0        0        0    11595 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_unit.py
+-rw-rw-rw-   0        0        0    11235 2024-04-25 06:40:32.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/unit.py
+-rw-rw-rw-   0        0        0    13898 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/use_tax.py
+-rw-rw-rw-   0        0        0    11238 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/vacancy.py
+-rw-rw-rw-   0        0        0    11817 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_api_request.py
+-rw-rw-rw-   0        0        0    11447 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_api_response.py
+-rw-rw-rw-   0        0        0    11429 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_input.py
+-rw-rw-rw-   0        0        0    16658 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_input_row.py
+-rw-rw-rw-   0        0        0    15324 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_output.py
+-rw-rw-rw-   0        0        0    11449 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_input.py
+-rw-rw-rw-   0        0        0    13503 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_input_row.py
+-rw-rw-rw-   0        0        0    11357 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_options.py
+-rw-rw-rw-   0        0        0    15940 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_output.py
+-rw-rw-rw-   0        0        0    11520 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_input.py
+-rw-rw-rw-   0        0        0    14342 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
+-rw-rw-rw-   0        0        0    15105 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_options.py
+-rw-rw-rw-   0        0        0    39660 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_output.py
+-rw-rw-rw-   0        0        0    12012 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_request.py
+-rw-rw-rw-   0        0        0    11529 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_response.py
+-rw-rw-rw-   0        0        0    11480 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_input.py
+-rw-rw-rw-   0        0        0    13512 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
+-rw-rw-rw-   0        0        0    14100 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_options.py
+-rw-rw-rw-   0        0        0    18611 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_output.py
+-rw-rw-rw-   0        0        0    11944 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_request.py
+-rw-rw-rw-   0        0        0    11489 2024-04-25 06:40:33.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_response.py
+-rw-rw-rw-   0        0        0    11891 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_request.py
+-rw-rw-rw-   0        0        0    11458 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_response.py
+-rw-rw-rw-   0        0        0    11530 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
+-rw-rw-rw-   0        0        0    14701 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
+-rw-rw-rw-   0        0        0    36257 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
+-rw-rw-rw-   0        0        0    49413 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
+-rw-rw-rw-   0        0        0    12029 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
+-rw-rw-rw-   0        0        0    11539 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
+-rw-rw-rw-   0        0        0    11488 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request.py
+-rw-rw-rw-   0        0        0    11521 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request_input.py
+-rw-rw-rw-   0        0        0    11377 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
+-rw-rw-rw-   0        0        0    11760 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/water_body.py
+-rw-rw-rw-   0        0        0    11870 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/water_body_response.py
+-rw-rw-rw-   0        0        0    17270 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_address.py
+-rw-rw-rw-   0        0        0    11334 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_boundary_geometry.py
+-rw-rw-rw-   0        0        0    11574 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_contact_details.py
+-rw-rw-rw-   0        0        0    11340 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_geometry.py
+-rw-rw-rw-   0        0        0    11091 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_parent_business.py
+-rw-rw-rw-   0        0        0    14879 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi.py
+-rw-rw-rw-   0        0        0    11851 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi_classification.py
+-rw-rw-rw-   0        0        0    11863 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi_geometry.py
+-rw-rw-rw-   0        0        0    11791 2024-04-25 06:40:34.000000 com_precisely_apis-18.1.0/com/precisely/apis/model/zones_sic.py
+-rw-rw-rw-   0        0        0    81943 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/model_utils.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:36.108311 com_precisely_apis-18.1.0/com/precisely/apis/models/
+-rw-rw-rw-   0        0        0    28241 2024-04-25 06:40:44.000000 com_precisely_apis-18.1.0/com/precisely/apis/models/__init__.py
+-rw-rw-rw-   0        0        0    14245 2024-04-25 06:40:43.000000 com_precisely_apis-18.1.0/com/precisely/apis/rest.py
+drwxrwxrwx   0        0        0        0 2024-05-07 07:02:36.117299 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/
+-rw-rw-rw-   0        0        0      540 2024-05-07 07:02:30.000000 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19569 2024-05-07 07:02:30.000000 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-07 07:02:30.000000 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-05-07 07:02:30.000000 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-05-07 07:02:30.000000 com_precisely_apis-18.1.0/com.precisely.apis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2024-05-07 07:02:36.154988 com_precisely_apis-18.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2024-05-07 06:55:11.000000 com_precisely_apis-18.1.0/setup.py
```

### Comparing `com.precisely.apis-18.0.1/LICENSE` & `com_precisely_apis-18.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.1/PKG-INFO` & `com_precisely_apis-18.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.precisely.apis
-Version: 18.0.1
+Version: 18.1.0
 Summary: Precisely APIs
 Home-page: https://developer.precisely.com/
 Author: Precisely APIs Support
 Author-email: PreciselyAPIs-Support@precisely.com
 License: Apache 2.0
 Keywords: Precisely APIs
 Requires-Python: >=3.6
```

### Comparing `com.precisely.apis-18.0.1/README.md` & `com_precisely_apis-18.1.0/README.md`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/__init__.py` & `com_precisely_apis-18.1.0/com/precisely/apis/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # flake8: noqa
 
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
-__version__ = "18.0.0"
+__version__ = "18.1.0"
 
 # import ApiClient
 from com.precisely.apis.api_client import ApiClient
 
 # import Configuration
 from com.precisely.apis.configuration import Configuration
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/address_autocomplete_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/address_verification_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/address_verification_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/addresses_service__api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/addresses_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/demographics_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/demographics_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/email_verification_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/email_verification_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/geocode_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/geocode_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -64,15 +64,14 @@
                     'fallback_postal',
                     'max_cands',
                     'street_offset',
                     'street_offset_units',
                     'corner_offset',
                     'corner_offset_units',
                     'remove_accent_marks',
-                    'find_dpv',
                 ],
                 'required': [
                     'datapack_bundle',
                 ],
                 'nullable': [
                 ],
                 'enum': [
@@ -135,46 +134,42 @@
                         (str,),
                     'corner_offset':
                         (str,),
                     'corner_offset_units':
                         (str,),
                     'remove_accent_marks':
                         (str,),
-                    'find_dpv':
-                        (str,),
                 },
                 'attribute_map': {
                     'datapack_bundle': 'datapackBundle',
                     'country': 'country',
                     'main_address': 'mainAddress',
                     'match_mode': 'matchMode',
                     'fallback_geo': 'fallbackGeo',
                     'fallback_postal': 'fallbackPostal',
                     'max_cands': 'maxCands',
                     'street_offset': 'streetOffset',
                     'street_offset_units': 'streetOffsetUnits',
                     'corner_offset': 'cornerOffset',
                     'corner_offset_units': 'cornerOffsetUnits',
                     'remove_accent_marks': 'removeAccentMarks',
-                    'find_dpv': 'findDPV',
                 },
                 'location_map': {
                     'datapack_bundle': 'path',
                     'country': 'query',
                     'main_address': 'query',
                     'match_mode': 'query',
                     'fallback_geo': 'query',
                     'fallback_postal': 'query',
                     'max_cands': 'query',
                     'street_offset': 'query',
                     'street_offset_units': 'query',
                     'corner_offset': 'query',
                     'corner_offset_units': 'query',
                     'remove_accent_marks': 'query',
-                    'find_dpv': 'query',
                 },
                 'collection_format_map': {
                 }
             },
             headers_map={
                 'accept': [
                     'application/json',
@@ -652,15 +647,14 @@
             fallback_postal (str): Specifies whether to attempt to determine a post code centroid when an address-level geocode cannot be determined.. [optional] if omitted the server will use the default value of "true"
             max_cands (str): The maximum number of candidates to return.. [optional] if omitted the server will use the default value of "1"
             street_offset (str): Indicates the offset distance from the street segments to use in street-level geocoding.. [optional] if omitted the server will use the default value of "7"
             street_offset_units (str): Specifies the unit of measurement for the street offset.. [optional] if omitted the server will use the default value of "METERS"
             corner_offset (str): Specifies the distance to offset the street end points in street-level matching.. [optional] if omitted the server will use the default value of "7"
             corner_offset_units (str): Specifies the unit of measurement for the corner offset.. [optional] if omitted the server will use the default value of "METERS"
             remove_accent_marks (str): Specifies whether to Suppress accents and other diacritical marks.. [optional] if omitted the server will use the default value of "false"
-            find_dpv (str): Specifies if Delivery Point Validation is required. Note: This parameter is only applicable for USA addresses.. [optional] if omitted the server will use the default value of "false"
             _return_http_data_only (bool): response data without head status
                 code and headers. Default is True.
             _preload_content (bool): if False, the urllib3.HTTPResponse object
                 will be returned without reading/decoding response data.
                 Default is True.
             _request_timeout (int/float/tuple): timeout setting for this request. If
                 one number provided, it will be total request timeout. It can also
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/geolocation_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/geolocation_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/local_tax_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/local_tax_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/neighborhoods_service__api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/neighborhoods_service__api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/phone_verification_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/phone_verification_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/places_service__api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/places_service__api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/property_information_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/property_information_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/psap_911_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/psap_911_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/risks_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/risks_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/routing_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/routing_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/schools_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/schools_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/streets_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/streets_service_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/telecomm_info_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/telecomm_info_service_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/time_zone_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/time_zone_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api/zones_service_api.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api/zones_service_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/api_client.py` & `com_precisely_apis-18.1.0/com/precisely/apis/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import json
 import atexit
 import mimetypes
@@ -80,15 +80,15 @@
 
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'OpenAPI-Generator/18.0.0/python'
+        self.user_agent = 'OpenAPI-Generator/18.1.0/python'
 
     def __enter__(self):
         return self
 
     def __exit__(self, exc_type, exc_value, traceback):
         self.close()
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/apis/__init__.py` & `com_precisely_apis-18.1.0/com/precisely/apis/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/configuration.py` & `com_precisely_apis-18.1.0/com/precisely/apis/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import copy
 import logging
 import multiprocessing
@@ -383,16 +383,16 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 18.0.0\n"\
-               "SDK Package Version: 18.0.0".\
+               "Version of the API: 18.1.0\n"\
+               "SDK Package Version: 18.1.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
         """
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/exceptions.py` & `com_precisely_apis-18.1.0/com/precisely/apis/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 
 class OpenApiException(Exception):
     """The base exception class for all OpenAPIExceptions"""
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/absentee_owner.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/absentee_owner.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/accuracy.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/accuracy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/address1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/address1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/address2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/address2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/address_time.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/address_time.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/address_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/address_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_by_boundary_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_by_boundary_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_count.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_dto.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_dto.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/addresses_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ah_jmailing_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ah_jmailing_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ahj.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ahj_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_plus_psap_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ahj_plus_psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/amenities.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/amenities.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/area.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/area.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/area_code_info.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/area_code_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/area_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/area_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/assets_and_wealth_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/assets_and_wealth_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/base_flood_elevation.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/base_flood_elevation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/basement_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/basement_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/basic_boundary.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/basic_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/boundaries.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/boundaries.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/boundary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_buffer.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/boundary_buffer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_point.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/boundary_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buffer_relation.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buffer_relation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_class.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_class.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_condition.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_condition.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_features_sqft.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_features_sqft.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_area.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_improve_area.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_improve_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_quality.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_quality.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_style.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_style.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fuel_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class BuildgType(ModelNormal):
+class FuelType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """BuildgType - a model defined in OpenAPI
+        """FuelType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """BuildgType - a model defined in OpenAPI
+        """FuelType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_view.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_view.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/building_sqft_source.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/building_sqft_source.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/business_id.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/business_id.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ca_exemptions.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ca_exemptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/candidate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/candidate_range.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range_unit.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/candidate_range_unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/carrier.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/carrier.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/category.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/category.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/category_metadata.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/category_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/cbsa.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/cbsa.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/census.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/census.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/center.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/center.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/city.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/city.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/common_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/common_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/community.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/community.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/community_group.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/community_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/consistency_code.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/consistency_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/construction.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/construction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/contact_details.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/contact_person.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/contact_person.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/cooling_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/vacancy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class CoolingType(ModelNormal):
+class Vacancy(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """CoolingType - a model defined in OpenAPI
+        """Vacancy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """CoolingType - a model defined in OpenAPI
+        """Vacancy - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/cost.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/cost.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/county.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/county.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/coverage.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/coverage.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_boundary.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_index_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_index_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crime_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/crs.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/crs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/damage_group.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/damage_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_advanced_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_advanced_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry_crc.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_themes_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/demographics_themes_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/depth.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/depth.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/direction_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/direction_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_border.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_border.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/distance_to_flood_hazard_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/district_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/district_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/domestic_ultimate_business.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/domestic_ultimate_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_date_time.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_date_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_event.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_event.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_events_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_events_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_history.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_location.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/earthquake_risk_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/education_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/education_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/employee_count.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/employee_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/employment_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/employment_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/energy_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/energy_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/error_code.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/error_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/error_info.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/error_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/error_info1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/error_info1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/events_count.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/events_count.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/expenditure_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/expenditure_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/exterior_walls.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/exterior_walls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/extra_feature_sqft.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/extra_feature_sqft.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/field.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/field.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fields_matching.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fields_matching.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_department.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_department.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_event.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_event_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_events_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_v2_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_events_v2_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_history_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_by_location_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_v2_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_risk_v2_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_shed.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_shed.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_station.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station_contact_details.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_station_contact_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_stations.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fire_stations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fireplace_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/fireplace_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_hazard_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_hazard_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_by_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_by_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_risk_response_list.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_zone.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/flood_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/floor_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/floor_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/formatted_tax_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/formatted_tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/foundation.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/foundation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/free_or_reduced_price_lunches.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/frequency_group.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/frequency_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/fuel_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/garage_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class FuelType(ModelNormal):
+class GarageType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """FuelType - a model defined in OpenAPI
+        """GarageType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """FuelType - a model defined in OpenAPI
+        """GarageType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/garage_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/buildg_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class GarageType(ModelNormal):
+class BuildgType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """GarageType - a model defined in OpenAPI
+        """BuildgType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """GarageType - a model defined in OpenAPI
+        """BuildgType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_access_point.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_access_point.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_country.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_ip_addr.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_ip_addr.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_place.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_state.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_location_state.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_pos.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geo_pos.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_request.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_service_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geocode_service_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geolocation_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geolocation_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_crc.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_properties.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/geometry_properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_city_state_province_api_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_options.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/get_postal_codes_api_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/global_ultimate_business.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/global_ultimate_business.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/grade_levels_taught.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/grade_levels_taught.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/greatschools.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/greatschools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/grid.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/grid.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/health_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/health_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/heating_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/heating_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/households_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/households_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/housing_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/housing_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/income_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/income_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/index_variable.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/index_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/individual_value_variable.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/individual_value_variable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/interior_wall.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/interior_wall.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/intermediate_points.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/intermediate_points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/intersection.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/intersection.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/intersection_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/intersection_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ip_info.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ip_info.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ipd.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/ipd_tax_jurisdiction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/key_lookup_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/key_lookup_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/keys.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/keys.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/land_use.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/land_use.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/lat_long_fields.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/lat_long_fields.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/life_style_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/life_style_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/loc_code.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/loc_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/local_tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/local_tax_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/location.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/location_time.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/location_time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/magnitude.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/magnitude.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/match.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/match.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/match1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/match1.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/matched_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/matrix.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/matrix.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/mcd.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/mcd.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/metadata_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/metadata_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/mitigation_group.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/mitigation_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/name.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/name.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/name1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/name1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/neighborhoods_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/neighborhoods_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/network.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/organization_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/organization_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/other_rooms.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/other_rooms.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/owner_vest_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/owner_vest_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/owners.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/owners.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_boundary_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/parcel_boundary_v2.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_v2.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/parcel_v2.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/parent_business.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/parent_business.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_address_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/pb_key_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/pbkey.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/pbkey.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/phone_verification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/phone_verification_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/place.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/place.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/place1.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/place1.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/places_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/places_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_locations.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_boundary_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_classification.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_count.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poi_count_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/poiby_geometry_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/poiby_geometry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/points.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/points.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/pool_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/pool_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/population_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/population_theme.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/preferenc_time_zone.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/preferenc_time_zone.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/primary_zone.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/primary_zone.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/prior_sale_code.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/prior_sale_code.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/prop_site_influene.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/prop_site_influene.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/properties.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/properties.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_attributes.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_attributes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_preferences.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_responses.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_info_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_information_geometry.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry_crc.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/property_information_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/proxy.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/proxy.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/psap_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/psap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/race_and_ethnicity_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/range_variable.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/range_variable.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/rate.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/rate.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/rate_center_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/rate_center_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/return_fields_descriptor.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/return_fields_descriptor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/reverse_geocode_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/reverse_geocode_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risk.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risk.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risk_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risk_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_locations.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risk_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_preferences.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risk_preferences.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_boundaries.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risks_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_crime_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risks_crime_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_geometry_crc.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/risks_geometry_crc.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/road.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/road.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_cover_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/roof_cover_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_frame_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/roof_frame_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_shape_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/roof_shape_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/route_direction.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/route_direction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/route_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/route_geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/route_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/route_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/sales_tax.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/sales_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/sales_volume.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/sales_volume.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/school.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/school.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/school_district.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/school_district.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/school_profile.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/school_profile.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/school_ranking.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/school_ranking.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/schools_near_by_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/schools_near_by_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/segmentation.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation_themes.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/segmentation_themes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/severity_group.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/severity_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/shore_line_distance.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/shore_line_distance.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/sic.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/sic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/sic_metadata.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/sic_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/site_details.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/site_details.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/situs_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/situs_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/special_purpose_district.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district_tax.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/special_purpose_district_tax.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/speed_limit.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/speed_limit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/start_end_point.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/start_end_point.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/state.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/status.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/stories.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/stories.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/student_ethnicity.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/student_ethnicity.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/supply_and_demand_theme.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/supply_and_demand_theme.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_county.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_county.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_district_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_district_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_doc_type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_doc_type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_exemption.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_exemption.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_jurisdiction.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_jurisdiction.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_locations.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_place.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_place.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_matched_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_matched_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_rate_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_responses.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_responses.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_sales_price_code.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_sales_price_code.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_state.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/tax_state.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/time.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/time.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_location_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_location_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response_list.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/timezone_response_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundaries.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/travel_boundaries.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundary.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/travel_boundary.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_cost_matrix_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/travel_cost_matrix_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/type.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/type.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_location.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_location.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_locations.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_locations.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_range.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_range.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_unit.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/typeahead_unit.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/unit.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/unit.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/use_tax.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/use_tax.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/vacancy.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/cooling_type.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
 
@@ -26,15 +26,15 @@
     validate_get_composed_info,
     OpenApiModel
 )
 from com.precisely.apis.exceptions import ApiAttributeError
 
 
 
-class Vacancy(ModelNormal):
+class CoolingType(ModelNormal):
     """NOTE: This class is auto generated by OpenAPI Generator.
     Ref: https://openapi-generator.tech
 
     Do not edit the class manually.
 
     Attributes:
       allowed_values (dict): The key is the tuple path to the attribute
@@ -99,15 +99,15 @@
     }
 
     _composed_schemas = {}
 
     @classmethod
     @convert_js_args_to_python_args
     def _from_openapi_data(cls, *args, **kwargs):  # noqa: E501
-        """Vacancy - a model defined in OpenAPI
+        """CoolingType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
@@ -182,15 +182,15 @@
         '_path_to_item',
         '_configuration',
         '_visited_composed_classes',
     ])
 
     @convert_js_args_to_python_args
     def __init__(self, *args, **kwargs):  # noqa: E501
-        """Vacancy - a model defined in OpenAPI
+        """CoolingType - a model defined in OpenAPI
 
         Keyword Args:
             _check_type (bool): if True, values for parameters in openapi_types
                                 will be type checked and a TypeError will be
                                 raised if the wrong type is input.
                                 Defaults to True
             _path_to_item (tuple/list): This is a list of keys or values to
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_api_request.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_api_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_input.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_email_address_output.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_premium_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_pro_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/water_body.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/water_body.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/water_body_response.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/water_body_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_address.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_boundary_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_boundary_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_contact_details.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_contact_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_parent_business.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_parent_business.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_classification.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi_classification.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_geometry.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_poi_geometry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_sic.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model/zones_sic.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import re  # noqa: F401
 import sys  # noqa: F401
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/model_utils.py` & `com_precisely_apis-18.1.0/com/precisely/apis/model_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 from datetime import date, datetime  # noqa: F401
 from copy import deepcopy
 import inspect
```

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/models/__init__.py` & `com_precisely_apis-18.1.0/com/precisely/apis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.1/com/precisely/apis/rest.py` & `com_precisely_apis-18.1.0/com/precisely/apis/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """
     Precisely APIs
 
     Enhance & enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.  # noqa: E501
 
-    The version of the OpenAPI document: 18.0.0
+    The version of the OpenAPI document: 18.1.0
     Generated by: https://openapi-generator.tech
 """
 
 
 import io
 import json
 import logging
```

### Comparing `com.precisely.apis-18.0.1/com.precisely.apis.egg-info/PKG-INFO` & `com_precisely_apis-18.1.0/com.precisely.apis.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: com.precisely.apis
-Version: 18.0.1
+Version: 18.1.0
 Summary: Precisely APIs
 Home-page: https://developer.precisely.com/
 Author: Precisely APIs Support
 Author-email: PreciselyAPIs-Support@precisely.com
 License: Apache 2.0
 Keywords: Precisely APIs
 Requires-Python: >=3.6
```

### Comparing `com.precisely.apis-18.0.1/com.precisely.apis.egg-info/SOURCES.txt` & `com_precisely_apis-18.1.0/com.precisely.apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.1/setup.py` & `com_precisely_apis-18.1.0/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "com.precisely.apis"
-VERSION = "18.0.1"
+VERSION = "18.1.0"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

