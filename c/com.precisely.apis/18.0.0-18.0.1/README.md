# Comparing `tmp/com.precisely.apis-18.0.0.tar.gz` & `tmp/com.precisely.apis-18.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "com.precisely.apis-18.0.0.tar", last modified: Tue Feb 13 12:56:36 2024, max compression
+gzip compressed data, was "com.precisely.apis-18.0.1.tar", last modified: Thu Apr 11 06:29:37 2024, max compression
```

## Comparing `com.precisely.apis-18.0.0.tar` & `com.precisely.apis-18.0.1.tar`

### file list

```diff
@@ -1,432 +1,432 @@
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.901008 com.precisely.apis-18.0.0/
--rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com.precisely.apis-18.0.0/LICENSE
--rw-rw-rw-   0        0        0      515 2024-02-13 12:56:36.901008 com.precisely.apis-18.0.0/PKG-INFO
--rw-rw-rw-   0        0        0    52015 2024-02-13 12:52:53.000000 com.precisely.apis-18.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:35.995391 com.precisely.apis-18.0.0/com/
--rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.039421 com.precisely.apis-18.0.0/com/precisely/
--rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.055459 com.precisely.apis-18.0.0/com/precisely/apis/
--rw-rw-rw-   0        0        0      828 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/__init__.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.122007 com.precisely.apis-18.0.0/com/precisely/apis/api/
--rw-rw-rw-   0        0        0      251 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/__init__.py
--rw-rw-rw-   0        0        0    16731 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
--rw-rw-rw-   0        0        0    11240 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/address_autocomplete_service_api.py
--rw-rw-rw-   0        0        0    30342 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/address_verification_service_api.py
--rw-rw-rw-   0        0        0    23486 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/addresses_service__api.py
--rw-rw-rw-   0        0        0    42885 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/demographics_service_api.py
--rw-rw-rw-   0        0        0     5850 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/email_verification_service_api.py
--rw-rw-rw-   0        0        0    47771 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/geocode_service_api.py
--rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/geolocation_service_api.py
--rw-rw-rw-   0        0        0    53765 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/local_tax_service_api.py
--rw-rw-rw-   0        0        0     6006 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/neighborhoods_service__api.py
--rw-rw-rw-   0        0        0     5902 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/phone_verification_service_api.py
--rw-rw-rw-   0        0        0    66165 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/places_service__api.py
--rw-rw-rw-   0        0        0    24854 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/property_information_service_api.py
--rw-rw-rw-   0        0        0    25323 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/psap_911_service_api.py
--rw-rw-rw-   0        0        0   154048 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/risks_service_api.py
--rw-rw-rw-   0        0        0    57476 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/routing_service_api.py
--rw-rw-rw-   0        0        0    10328 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/schools_service_api.py
--rw-rw-rw-   0        0        0    19000 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/streets_service_api.py
--rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/telecomm_info_service_api.py
--rw-rw-rw-   0        0        0    21347 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/time_zone_service_api.py
--rw-rw-rw-   0        0        0    53780 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api/zones_service_api.py
--rw-rw-rw-   0        0        0    38586 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/api_client.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.137005 com.precisely.apis-18.0.0/com/precisely/apis/apis/
--rw-rw-rw-   0        0        0     2215 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/apis/__init__.py
--rw-rw-rw-   0        0        0    16559 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/configuration.py
--rw-rw-rw-   0        0        0     5117 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/exceptions.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.896005 com.precisely.apis-18.0.0/com/precisely/apis/model/
--rw-rw-rw-   0        0        0      348 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/__init__.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/absentee_owner.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/accuracy.py
--rw-rw-rw-   0        0        0    17255 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/address.py
--rw-rw-rw-   0        0        0    17258 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/address1.py
--rw-rw-rw-   0        0        0    17940 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/address2.py
--rw-rw-rw-   0        0        0    11460 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/address_time.py
--rw-rw-rw-   0        0        0    11285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/address_type.py
--rw-rw-rw-   0        0        0    13513 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_by_boundary_request.py
--rw-rw-rw-   0        0        0    11159 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_count.py
--rw-rw-rw-   0        0        0    14966 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_dto.py
--rw-rw-rw-   0        0        0    11321 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_preferences.py
--rw-rw-rw-   0        0        0    11720 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_response.py
--rw-rw-rw-   0        0        0    17285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ah_jmailing_address.py
--rw-rw-rw-   0        0        0    13338 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ahj.py
--rw-rw-rw-   0        0        0    11201 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ahj_list.py
--rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ahj_plus_psap_response.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/amenities.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/area.py
--rw-rw-rw-   0        0        0    12644 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/area_code_info.py
--rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/area_v2.py
--rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/assets_and_wealth_theme.py
--rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/base_flood_elevation.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/basement_type.py
--rw-rw-rw-   0        0        0    12377 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/basic_boundary.py
--rw-rw-rw-   0        0        0    11770 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/boundaries.py
--rw-rw-rw-   0        0        0    12162 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/boundary.py
--rw-rw-rw-   0        0        0    11763 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/boundary_buffer.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/boundary_point.py
--rw-rw-rw-   0        0        0    11294 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buffer_relation.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_class.py
--rw-rw-rw-   0        0        0    11262 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_condition.py
--rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_features_sqft.py
--rw-rw-rw-   0        0        0    11564 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_improve_area.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_improve_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_quality.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_style.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_view.py
--rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/building_sqft_source.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/business_id.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ca_exemptions.py
--rw-rw-rw-   0        0        0    13761 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/candidate.py
--rw-rw-rw-   0        0        0    13101 2024-02-13 12:54:08.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/candidate_range.py
--rw-rw-rw-   0        0        0    12226 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/candidate_range_unit.py
--rw-rw-rw-   0        0        0    11233 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/carrier.py
--rw-rw-rw-   0        0        0    11930 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/category.py
--rw-rw-rw-   0        0        0    12296 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/category_metadata.py
--rw-rw-rw-   0        0        0    11224 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/cbsa.py
--rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/census.py
--rw-rw-rw-   0        0        0    11277 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/center.py
--rw-rw-rw-   0        0        0    11259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/city.py
--rw-rw-rw-   0        0        0    11893 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/common_geometry.py
--rw-rw-rw-   0        0        0    11420 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/community.py
--rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/community_group.py
--rw-rw-rw-   0        0        0    11297 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/consistency_code.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/construction.py
--rw-rw-rw-   0        0        0    12229 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/contact_details.py
--rw-rw-rw-   0        0        0    12861 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/contact_person.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/cooling_type.py
--rw-rw-rw-   0        0        0    11691 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/cost.py
--rw-rw-rw-   0        0        0    11230 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/county.py
--rw-rw-rw-   0        0        0    11464 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/coverage.py
--rw-rw-rw-   0        0        0    11830 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_boundary.py
--rw-rw-rw-   0        0        0    11750 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_index_theme.py
--rw-rw-rw-   0        0        0    11834 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py
--rw-rw-rw-   0        0        0    11331 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_preferences.py
--rw-rw-rw-   0        0        0    12263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_response.py
--rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_response_list.py
--rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/crs.py
--rw-rw-rw-   0        0        0    11342 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/damage_group.py
--rw-rw-rw-   0        0        0    12065 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics.py
--rw-rw-rw-   0        0        0    11567 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_advanced_preferences.py
--rw-rw-rw-   0        0        0    12118 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_advanced_request.py
--rw-rw-rw-   0        0        0    11960 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_geometry.py
--rw-rw-rw-   0        0        0    11557 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_geometry_crc.py
--rw-rw-rw-   0        0        0    15660 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_themes_v2.py
--rw-rw-rw-   0        0        0    11232 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/depth.py
--rw-rw-rw-   0        0        0    11328 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/direction_geometry.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance1.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_border.py
--rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
--rw-rw-rw-   0        0        0    11880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
--rw-rw-rw-   0        0        0    11406 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py
--rw-rw-rw-   0        0        0    11288 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/district_type.py
--rw-rw-rw-   0        0        0    11642 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/domestic_ultimate_business.py
--rw-rw-rw-   0        0        0    11266 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_date_time.py
--rw-rw-rw-   0        0        0    13648 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_event.py
--rw-rw-rw-   0        0        0    11621 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_events_response.py
--rw-rw-rw-   0        0        0    11981 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_history.py
--rw-rw-rw-   0        0        0    11313 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_location.py
--rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11815 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12371 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_response.py
--rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_response_list.py
--rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/education_theme.py
--rw-rw-rw-   0        0        0    11358 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/employee_count.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/employment_theme.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/energy_type.py
--rw-rw-rw-   0        0        0    11332 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/error_code.py
--rw-rw-rw-   0        0        0    11260 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/error_info.py
--rw-rw-rw-   0        0        0    11263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/error_info1.py
--rw-rw-rw-   0        0        0    13880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/events_count.py
--rw-rw-rw-   0        0        0    12070 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/expenditure_theme.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/exterior_walls.py
--rw-rw-rw-   0        0        0    11589 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/extra_feature_sqft.py
--rw-rw-rw-   0        0        0    11445 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/field.py
--rw-rw-rw-   0        0        0    14301 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fields_matching.py
--rw-rw-rw-   0        0        0    12318 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_department.py
--rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_event.py
--rw-rw-rw-   0        0        0    12071 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_event_v2.py
--rw-rw-rw-   0        0        0    11282 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_events_response.py
--rw-rw-rw-   0        0        0    11303 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_events_v2_response.py
--rw-rw-rw-   0        0        0    11733 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_history.py
--rw-rw-rw-   0        0        0    11754 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_history_v2.py
--rw-rw-rw-   0        0        0    11780 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_by_location_request.py
--rw-rw-rw-   0        0        0    12122 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_response.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_response_list.py
--rw-rw-rw-   0        0        0    16206 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_v2_response.py
--rw-rw-rw-   0        0        0    11378 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_v2_response_list.py
--rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_shed.py
--rw-rw-rw-   0        0        0    13259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_station.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_station_contact_details.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fire_stations.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fireplace_type.py
--rw-rw-rw-   0        0        0    11868 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_hazard_preferences.py
--rw-rw-rw-   0        0        0    11819 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_by_address_request.py
--rw-rw-rw-   0        0        0    11836 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_by_location_request.py
--rw-rw-rw-   0        0        0    11616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_preferences.py
--rw-rw-rw-   0        0        0    12803 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_response.py
--rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_response_list.py
--rw-rw-rw-   0        0        0    12555 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/flood_zone.py
--rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/floor_type.py
--rw-rw-rw-   0        0        0    13506 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/formatted_tax_address.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/foundation.py
--rw-rw-rw-   0        0        0    11679 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py
--rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/frequency_group.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/fuel_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/garage_type.py
--rw-rw-rw-   0        0        0    11682 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_access_point.py
--rw-rw-rw-   0        0        0    11479 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_country.py
--rw-rw-rw-   0        0        0    11957 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_ip_addr.py
--rw-rw-rw-   0        0        0    13204 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_place.py
--rw-rw-rw-   0        0        0    11295 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_state.py
--rw-rw-rw-   0        0        0    11638 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geo_pos.py
--rw-rw-rw-   0        0        0    14447 2024-02-13 12:54:42.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_address.py
--rw-rw-rw-   0        0        0    18616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_preferences.py
--rw-rw-rw-   0        0        0    11970 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_request.py
--rw-rw-rw-   0        0        0    12023 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_service_response.py
--rw-rw-rw-   0        0        0    11418 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_service_response_list.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geolocation_geometry.py
--rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geometry.py
--rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geometry_crc.py
--rw-rw-rw-   0        0        0    11088 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/geometry_properties.py
--rw-rw-rw-   0        0        0    11461 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_input.py
--rw-rw-rw-   0        0        0    11984 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py
--rw-rw-rw-   0        0        0    12600 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_options.py
--rw-rw-rw-   0        0        0    13593 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_output.py
--rw-rw-rw-   0        0        0    11912 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_request.py
--rw-rw-rw-   0        0        0    11470 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_response.py
--rw-rw-rw-   0        0        0    11400 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_input.py
--rw-rw-rw-   0        0        0    12159 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py
--rw-rw-rw-   0        0        0    11710 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_options.py
--rw-rw-rw-   0        0        0    13110 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_output.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
--rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_request.py
--rw-rw-rw-   0        0        0    11409 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_response.py
--rw-rw-rw-   0        0        0    11636 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/global_ultimate_business.py
--rw-rw-rw-   0        0        0    13489 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/grade_levels_taught.py
--rw-rw-rw-   0        0        0    11435 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/greatschools.py
--rw-rw-rw-   0        0        0    11462 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/grid.py
--rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/health_theme.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/heating_type.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/households_theme.py
--rw-rw-rw-   0        0        0    12058 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/housing_theme.py
--rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/income_theme.py
--rw-rw-rw-   0        0        0    11874 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/index_variable.py
--rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/individual_value_variable.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/interior_wall.py
--rw-rw-rw-   0        0        0    11319 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/intermediate_points.py
--rw-rw-rw-   0        0        0    12291 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/intersection.py
--rw-rw-rw-   0        0        0    11686 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/intersection_response.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ip_info.py
--rw-rw-rw-   0        0        0    13054 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ipd.py
--rw-rw-rw-   0        0        0    11890 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
--rw-rw-rw-   0        0        0    11871 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/key_lookup_request.py
--rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/keys.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/land_use.py
--rw-rw-rw-   0        0        0    12232 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/lat_long_fields.py
--rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/life_style_theme.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/loc_code.py
--rw-rw-rw-   0        0        0    11343 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/local_tax_geometry.py
--rw-rw-rw-   0        0        0    14407 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/local_tax_preferences.py
--rw-rw-rw-   0        0        0    11217 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/location.py
--rw-rw-rw-   0        0        0    12025 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/location_time.py
--rw-rw-rw-   0        0        0    12175 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/magnitude.py
--rw-rw-rw-   0        0        0    11972 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/match.py
--rw-rw-rw-   0        0        0    11975 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/match1.py
--rw-rw-rw-   0        0        0    17276 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/matched_address.py
--rw-rw-rw-   0        0        0    12342 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/matrix.py
--rw-rw-rw-   0        0        0    11221 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/mcd.py
--rw-rw-rw-   0        0        0    11652 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/metadata_response.py
--rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/mitigation_group.py
--rw-rw-rw-   0        0        0    11474 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/name.py
--rw-rw-rw-   0        0        0    11477 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/name1.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/neighborhoods_response.py
--rw-rw-rw-   0        0        0    13019 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/network.py
--rw-rw-rw-   0        0        0    11496 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/organization_type.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/other_rooms.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/owner_vest_type.py
--rw-rw-rw-   0        0        0    11899 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/owners.py
--rw-rw-rw-   0        0        0    13778 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/parcel_boundary_v2.py
--rw-rw-rw-   0        0        0    12581 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/parcel_v2.py
--rw-rw-rw-   0        0        0    11612 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/parent_business.py
--rw-rw-rw-   0        0        0    11412 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_address_request.py
--rw-rw-rw-   0        0        0    11468 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_response.py
--rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_response_list.py
--rw-rw-rw-   0        0        0    11646 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/pbkey.py
--rw-rw-rw-   0        0        0    11383 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/phone_verification.py
--rw-rw-rw-   0        0        0    12826 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/phone_verification_output.py
--rw-rw-rw-   0        0        0    11592 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/place.py
--rw-rw-rw-   0        0        0    11602 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/place1.py
--rw-rw-rw-   0        0        0    12227 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/places_response.py
--rw-rw-rw-   0        0        0    20808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi.py
--rw-rw-rw-   0        0        0    12870 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary.py
--rw-rw-rw-   0        0        0    11840 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_address_request.py
--rw-rw-rw-   0        0        0    11900 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_location_request.py
--rw-rw-rw-   0        0        0    11825 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_locations.py
--rw-rw-rw-   0        0        0    11548 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_preferences.py
--rw-rw-rw-   0        0        0    11333 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_response.py
--rw-rw-rw-   0        0        0    11800 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_classification.py
--rw-rw-rw-   0        0        0    11116 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_count.py
--rw-rw-rw-   0        0        0    12954 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poi_count_request.py
--rw-rw-rw-   0        0        0    13374 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/poiby_geometry_request.py
--rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/points.py
--rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/pool_type.py
--rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/population_theme.py
--rw-rw-rw-   0        0        0    11114 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/preferenc_time_zone.py
--rw-rw-rw-   0        0        0    11280 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/primary_zone.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/prior_sale_code.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/prop_site_influene.py
--rw-rw-rw-   0        0        0    11106 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/properties.py
--rw-rw-rw-   0        0        0    46206 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_attributes.py
--rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_geometry.py
--rw-rw-rw-   0        0        0    11918 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_address_request.py
--rw-rw-rw-   0        0        0    11133 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_preferences.py
--rw-rw-rw-   0        0        0    12002 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_response.py
--rw-rw-rw-   0        0        0    11457 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_responses.py
--rw-rw-rw-   0        0        0    12031 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_information_geometry.py
--rw-rw-rw-   0        0        0    11578 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/property_information_geometry_crc.py
--rw-rw-rw-   0        0        0    11696 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/proxy.py
--rw-rw-rw-   0        0        0    13793 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/psap_response.py
--rw-rw-rw-   0        0        0    12085 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py
--rw-rw-rw-   0        0        0    12626 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/range_variable.py
--rw-rw-rw-   0        0        0    11664 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/rate.py
--rw-rw-rw-   0        0        0    13762 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/rate_center_response.py
--rw-rw-rw-   0        0        0    12337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/return_fields_descriptor.py
--rw-rw-rw-   0        0        0    11723 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/reverse_geocode_request.py
--rw-rw-rw-   0        0        0    14978 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risk.py
--rw-rw-rw-   0        0        0    17267 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risk_address.py
--rw-rw-rw-   0        0        0    11337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risk_geometry.py
--rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risk_locations.py
--rw-rw-rw-   0        0        0    11601 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risk_preferences.py
--rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risks_boundaries.py
--rw-rw-rw-   0        0        0    11368 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risks_crime_theme.py
--rw-rw-rw-   0        0        0    11536 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/risks_geometry_crc.py
--rw-rw-rw-   0        0        0    13324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/road.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/roof_cover_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/roof_frame_type.py
--rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/roof_shape_type.py
--rw-rw-rw-   0        0        0    12381 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/route_direction.py
--rw-rw-rw-   0        0        0    11304 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/route_geometry.py
--rw-rw-rw-   0        0        0    13382 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/route_response.py
--rw-rw-rw-   0        0        0    13904 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/sales_tax.py
--rw-rw-rw-   0        0        0    11569 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/sales_volume.py
--rw-rw-rw-   0        0        0    19116 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/school.py
--rw-rw-rw-   0        0        0    12879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/school_district.py
--rw-rw-rw-   0        0        0    13410 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/school_profile.py
--rw-rw-rw-   0        0        0    12471 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/school_ranking.py
--rw-rw-rw-   0        0        0    12003 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/schools_near_by_response.py
--rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/segmentation.py
--rw-rw-rw-   0        0        0    11365 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/segmentation_themes.py
--rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/severity_group.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/shore_line_distance.py
--rw-rw-rw-   0        0        0    12022 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/sic.py
--rw-rw-rw-   0        0        0    12330 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/sic_metadata.py
--rw-rw-rw-   0        0        0    12078 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/site_details.py
--rw-rw-rw-   0        0        0    13485 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/situs_address.py
--rw-rw-rw-   0        0        0    12476 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/special_purpose_district.py
--rw-rw-rw-   0        0        0    11579 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/special_purpose_district_tax.py
--rw-rw-rw-   0        0        0    13049 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/speed_limit.py
--rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/start_end_point.py
--rw-rw-rw-   0        0        0    11227 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/state.py
--rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/status.py
--rw-rw-rw-   0        0        0    11273 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/stories.py
--rw-rw-rw-   0        0        0    12424 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/student_ethnicity.py
--rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/supply_and_demand_theme.py
--rw-rw-rw-   0        0        0    18388 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_address.py
--rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_address_request.py
--rw-rw-rw-   0        0        0    11239 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_county.py
--rw-rw-rw-   0        0        0    13607 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_district_response.py
--rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_district_response_list.py
--rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_doc_type.py
--rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_exemption.py
--rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_geometry.py
--rw-rw-rw-   0        0        0    12257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_jurisdiction.py
--rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_location_request.py
--rw-rw-rw-   0        0        0    11787 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_locations.py
--rw-rw-rw-   0        0        0    12845 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_place.py
--rw-rw-rw-   0        0        0    18168 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_address.py
--rw-rw-rw-   0        0        0    11919 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_address_request.py
--rw-rw-rw-   0        0        0    11810 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_location_request.py
--rw-rw-rw-   0        0        0    17504 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_matched_address.py
--rw-rw-rw-   0        0        0    14126 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_response.py
--rw-rw-rw-   0        0        0    11346 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_responses.py
--rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_sales_price_code.py
--rw-rw-rw-   0        0        0    11236 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/tax_state.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/time.py
--rw-rw-rw-   0        0        0    11731 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_address_request.py
--rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_geometry.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_location_request.py
--rw-rw-rw-   0        0        0    15252 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_response.py
--rw-rw-rw-   0        0        0    11352 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_response_list.py
--rw-rw-rw-   0        0        0    11354 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/travel_boundaries.py
--rw-rw-rw-   0        0        0    11234 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/travel_boundary.py
--rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/travel_cost_matrix_response.py
--rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/type.py
--rw-rw-rw-   0        0        0    13895 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_location.py
--rw-rw-rw-   0        0        0    11353 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_locations.py
--rw-rw-rw-   0        0        0    11505 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_range.py
--rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_unit.py
--rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/unit.py
--rw-rw-rw-   0        0        0    13898 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/use_tax.py
--rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/vacancy.py
--rw-rw-rw-   0        0        0    11817 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_api_request.py
--rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_api_response.py
--rw-rw-rw-   0        0        0    11429 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_input.py
--rw-rw-rw-   0        0        0    16658 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_input_row.py
--rw-rw-rw-   0        0        0    15324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_output.py
--rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_input.py
--rw-rw-rw-   0        0        0    13503 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py
--rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_options.py
--rw-rw-rw-   0        0        0    15940 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_output.py
--rw-rw-rw-   0        0        0    11520 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py
--rw-rw-rw-   0        0        0    14342 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
--rw-rw-rw-   0        0        0    15105 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py
--rw-rw-rw-   0        0        0    39660 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py
--rw-rw-rw-   0        0        0    12012 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py
--rw-rw-rw-   0        0        0    11529 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py
--rw-rw-rw-   0        0        0    11480 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py
--rw-rw-rw-   0        0        0    13512 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
--rw-rw-rw-   0        0        0    14100 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py
--rw-rw-rw-   0        0        0    18611 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py
--rw-rw-rw-   0        0        0    11944 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py
--rw-rw-rw-   0        0        0    11489 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py
--rw-rw-rw-   0        0        0    11891 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_request.py
--rw-rw-rw-   0        0        0    11458 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_response.py
--rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
--rw-rw-rw-   0        0        0    14701 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
--rw-rw-rw-   0        0        0    36257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
--rw-rw-rw-   0        0        0    49413 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
--rw-rw-rw-   0        0        0    12029 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
--rw-rw-rw-   0        0        0    11539 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
--rw-rw-rw-   0        0        0    11488 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request.py
--rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py
--rw-rw-rw-   0        0        0    11377 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
--rw-rw-rw-   0        0        0    11760 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/water_body.py
--rw-rw-rw-   0        0        0    11870 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/water_body_response.py
--rw-rw-rw-   0        0        0    17270 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_address.py
--rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_boundary_geometry.py
--rw-rw-rw-   0        0        0    11574 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_contact_details.py
--rw-rw-rw-   0        0        0    11340 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_geometry.py
--rw-rw-rw-   0        0        0    11091 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_parent_business.py
--rw-rw-rw-   0        0        0    14879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi.py
--rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi_classification.py
--rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi_geometry.py
--rw-rw-rw-   0        0        0    11791 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.0/com/precisely/apis/model/zones_sic.py
--rw-rw-rw-   0        0        0    81943 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/model_utils.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.898009 com.precisely.apis-18.0.0/com/precisely/apis/models/
--rw-rw-rw-   0        0        0    28241 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/models/__init__.py
--rw-rw-rw-   0        0        0    14245 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.0/com/precisely/apis/rest.py
-drwxrwxrwx   0        0        0        0 2024-02-13 12:56:36.899008 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/
--rw-rw-rw-   0        0        0      515 2024-02-13 12:56:35.000000 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0    19569 2024-02-13 12:56:35.000000 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-13 12:56:35.000000 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2024-02-13 12:56:35.000000 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2024-02-13 12:56:35.000000 com.precisely.apis-18.0.0/com.precisely.apis.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       76 2024-02-13 12:56:36.903007 com.precisely.apis-18.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1210 2024-02-13 12:51:24.000000 com.precisely.apis-18.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.278974 com.precisely.apis-18.0.1/
+-rw-rw-rw-   0        0        0    11558 2023-05-02 10:12:45.000000 com.precisely.apis-18.0.1/LICENSE
+-rw-rw-rw-   0        0        0      540 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0    52015 2024-02-13 12:52:53.000000 com.precisely.apis-18.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.180625 com.precisely.apis-18.0.1/com/
+-rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.211875 com.precisely.apis-18.0.1/com/precisely/
+-rw-rw-rw-   0        0        0        0 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.296609 com.precisely.apis-18.0.1/com/precisely/apis/
+-rw-rw-rw-   0        0        0      828 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.597407 com.precisely.apis-18.0.1/com/precisely/apis/api/
+-rw-rw-rw-   0        0        0      251 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/__init__.py
+-rw-rw-rw-   0        0        0    16731 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py
+-rw-rw-rw-   0        0        0    11240 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_service_api.py
+-rw-rw-rw-   0        0        0    30342 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/address_verification_service_api.py
+-rw-rw-rw-   0        0        0    23486 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/addresses_service__api.py
+-rw-rw-rw-   0        0        0    42885 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/demographics_service_api.py
+-rw-rw-rw-   0        0        0     5850 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/email_verification_service_api.py
+-rw-rw-rw-   0        0        0    47771 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/geocode_service_api.py
+-rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/geolocation_service_api.py
+-rw-rw-rw-   0        0        0    53765 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/local_tax_service_api.py
+-rw-rw-rw-   0        0        0     6006 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/neighborhoods_service__api.py
+-rw-rw-rw-   0        0        0     5902 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/phone_verification_service_api.py
+-rw-rw-rw-   0        0        0    66165 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/places_service__api.py
+-rw-rw-rw-   0        0        0    24854 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/property_information_service_api.py
+-rw-rw-rw-   0        0        0    25323 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/psap_911_service_api.py
+-rw-rw-rw-   0        0        0   154048 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/risks_service_api.py
+-rw-rw-rw-   0        0        0    57476 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/routing_service_api.py
+-rw-rw-rw-   0        0        0    10328 2024-02-13 11:11:53.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/schools_service_api.py
+-rw-rw-rw-   0        0        0    19000 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/streets_service_api.py
+-rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/telecomm_info_service_api.py
+-rw-rw-rw-   0        0        0    21347 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/time_zone_service_api.py
+-rw-rw-rw-   0        0        0    53780 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api/zones_service_api.py
+-rw-rw-rw-   0        0        0    38586 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/api_client.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:27.613034 com.precisely.apis-18.0.1/com/precisely/apis/apis/
+-rw-rw-rw-   0        0        0     2215 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/apis/__init__.py
+-rw-rw-rw-   0        0        0    16559 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/configuration.py
+-rw-rw-rw-   0        0        0     5117 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/exceptions.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.248573 com.precisely.apis-18.0.1/com/precisely/apis/model/
+-rw-rw-rw-   0        0        0      348 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/__init__.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/absentee_owner.py
+-rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/accuracy.py
+-rw-rw-rw-   0        0        0    17255 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address.py
+-rw-rw-rw-   0        0        0    17258 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address1.py
+-rw-rw-rw-   0        0        0    17791 2024-04-11 06:20:39.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address2.py
+-rw-rw-rw-   0        0        0    11460 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address_time.py
+-rw-rw-rw-   0        0        0    11285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/address_type.py
+-rw-rw-rw-   0        0        0    13513 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_by_boundary_request.py
+-rw-rw-rw-   0        0        0    11159 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_count.py
+-rw-rw-rw-   0        0        0    14966 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_dto.py
+-rw-rw-rw-   0        0        0    11321 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_preferences.py
+-rw-rw-rw-   0        0        0    11720 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_response.py
+-rw-rw-rw-   0        0        0    17285 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ah_jmailing_address.py
+-rw-rw-rw-   0        0        0    13338 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj.py
+-rw-rw-rw-   0        0        0    11201 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_list.py
+-rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_plus_psap_response.py
+-rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/amenities.py
+-rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area.py
+-rw-rw-rw-   0        0        0    12644 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area_code_info.py
+-rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/area_v2.py
+-rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/assets_and_wealth_theme.py
+-rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/base_flood_elevation.py
+-rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/basement_type.py
+-rw-rw-rw-   0        0        0    12377 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/basic_boundary.py
+-rw-rw-rw-   0        0        0    11770 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundaries.py
+-rw-rw-rw-   0        0        0    12162 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary.py
+-rw-rw-rw-   0        0        0    11763 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_buffer.py
+-rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_point.py
+-rw-rw-rw-   0        0        0    11294 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buffer_relation.py
+-rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:49.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_class.py
+-rw-rw-rw-   0        0        0    11262 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_condition.py
+-rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_features_sqft.py
+-rw-rw-rw-   0        0        0    11564 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_area.py
+-rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_type.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_quality.py
+-rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_style.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_type.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_view.py
+-rw-rw-rw-   0        0        0    11271 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/building_sqft_source.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/business_id.py
+-rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ca_exemptions.py
+-rw-rw-rw-   0        0        0    13761 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate.py
+-rw-rw-rw-   0        0        0    13101 2024-02-13 12:54:08.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range.py
+-rw-rw-rw-   0        0        0    12226 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range_unit.py
+-rw-rw-rw-   0        0        0    11233 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/carrier.py
+-rw-rw-rw-   0        0        0    11930 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/category.py
+-rw-rw-rw-   0        0        0    12296 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/category_metadata.py
+-rw-rw-rw-   0        0        0    11224 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cbsa.py
+-rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/census.py
+-rw-rw-rw-   0        0        0    11277 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/center.py
+-rw-rw-rw-   0        0        0    11259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/city.py
+-rw-rw-rw-   0        0        0    11893 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/common_geometry.py
+-rw-rw-rw-   0        0        0    11420 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/community.py
+-rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/community_group.py
+-rw-rw-rw-   0        0        0    11297 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/consistency_code.py
+-rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/construction.py
+-rw-rw-rw-   0        0        0    12229 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/contact_details.py
+-rw-rw-rw-   0        0        0    12861 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/contact_person.py
+-rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cooling_type.py
+-rw-rw-rw-   0        0        0    11691 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/cost.py
+-rw-rw-rw-   0        0        0    11230 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/county.py
+-rw-rw-rw-   0        0        0    11464 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/coverage.py
+-rw-rw-rw-   0        0        0    11830 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_boundary.py
+-rw-rw-rw-   0        0        0    11750 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_index_theme.py
+-rw-rw-rw-   0        0        0    11834 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py
+-rw-rw-rw-   0        0        0    11331 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_preferences.py
+-rw-rw-rw-   0        0        0    12263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response_list.py
+-rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/crs.py
+-rw-rw-rw-   0        0        0    11342 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/damage_group.py
+-rw-rw-rw-   0        0        0    12065 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics.py
+-rw-rw-rw-   0        0        0    11567 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_preferences.py
+-rw-rw-rw-   0        0        0    12118 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_request.py
+-rw-rw-rw-   0        0        0    11960 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry.py
+-rw-rw-rw-   0        0        0    11557 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry_crc.py
+-rw-rw-rw-   0        0        0    15660 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_themes_v2.py
+-rw-rw-rw-   0        0        0    11232 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/depth.py
+-rw-rw-rw-   0        0        0    11328 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/direction_geometry.py
+-rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance.py
+-rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance1.py
+-rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_border.py
+-rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py
+-rw-rw-rw-   0        0        0    11880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py
+-rw-rw-rw-   0        0        0    11406 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py
+-rw-rw-rw-   0        0        0    11288 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/district_type.py
+-rw-rw-rw-   0        0        0    11642 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/domestic_ultimate_business.py
+-rw-rw-rw-   0        0        0    11266 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_date_time.py
+-rw-rw-rw-   0        0        0    13648 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_event.py
+-rw-rw-rw-   0        0        0    11621 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_events_response.py
+-rw-rw-rw-   0        0        0    11981 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_history.py
+-rw-rw-rw-   0        0        0    11313 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_location.py
+-rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11815 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12371 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response.py
+-rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response_list.py
+-rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/education_theme.py
+-rw-rw-rw-   0        0        0    11358 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/employee_count.py
+-rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/employment_theme.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/energy_type.py
+-rw-rw-rw-   0        0        0    11332 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_code.py
+-rw-rw-rw-   0        0        0    11260 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_info.py
+-rw-rw-rw-   0        0        0    11263 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/error_info1.py
+-rw-rw-rw-   0        0        0    13880 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/events_count.py
+-rw-rw-rw-   0        0        0    12070 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/expenditure_theme.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/exterior_walls.py
+-rw-rw-rw-   0        0        0    11589 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/extra_feature_sqft.py
+-rw-rw-rw-   0        0        0    11445 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/field.py
+-rw-rw-rw-   0        0        0    14301 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fields_matching.py
+-rw-rw-rw-   0        0        0    12318 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_department.py
+-rw-rw-rw-   0        0        0    12050 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event.py
+-rw-rw-rw-   0        0        0    12071 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event_v2.py
+-rw-rw-rw-   0        0        0    11282 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_response.py
+-rw-rw-rw-   0        0        0    11303 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_v2_response.py
+-rw-rw-rw-   0        0        0    11733 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history.py
+-rw-rw-rw-   0        0        0    11754 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history_v2.py
+-rw-rw-rw-   0        0        0    11780 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    12122 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response.py
+-rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response_list.py
+-rw-rw-rw-   0        0        0    16206 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response.py
+-rw-rw-rw-   0        0        0    11378 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response_list.py
+-rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_shed.py
+-rw-rw-rw-   0        0        0    13259 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station.py
+-rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station_contact_details.py
+-rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:50.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fire_stations.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fireplace_type.py
+-rw-rw-rw-   0        0        0    11868 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_hazard_preferences.py
+-rw-rw-rw-   0        0        0    11819 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_address_request.py
+-rw-rw-rw-   0        0        0    11836 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_location_request.py
+-rw-rw-rw-   0        0        0    11616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_preferences.py
+-rw-rw-rw-   0        0        0    12803 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response.py
+-rw-rw-rw-   0        0        0    11372 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response_list.py
+-rw-rw-rw-   0        0        0    12555 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/flood_zone.py
+-rw-rw-rw-   0        0        0    11244 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/floor_type.py
+-rw-rw-rw-   0        0        0    13506 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/formatted_tax_address.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/foundation.py
+-rw-rw-rw-   0        0        0    11679 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py
+-rw-rw-rw-   0        0        0    11716 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/frequency_group.py
+-rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/fuel_type.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/garage_type.py
+-rw-rw-rw-   0        0        0    11682 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_access_point.py
+-rw-rw-rw-   0        0        0    11479 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_country.py
+-rw-rw-rw-   0        0        0    11957 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_ip_addr.py
+-rw-rw-rw-   0        0        0    13204 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_place.py
+-rw-rw-rw-   0        0        0    11295 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_state.py
+-rw-rw-rw-   0        0        0    11638 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geo_pos.py
+-rw-rw-rw-   0        0        0    14447 2024-02-13 12:54:42.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_address.py
+-rw-rw-rw-   0        0        0    18616 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_preferences.py
+-rw-rw-rw-   0        0        0    11970 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_request.py
+-rw-rw-rw-   0        0        0    12023 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response.py
+-rw-rw-rw-   0        0        0    11418 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response_list.py
+-rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geolocation_geometry.py
+-rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry.py
+-rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_crc.py
+-rw-rw-rw-   0        0        0    11088 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_properties.py
+-rw-rw-rw-   0        0        0    11461 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input.py
+-rw-rw-rw-   0        0        0    11984 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py
+-rw-rw-rw-   0        0        0    12600 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_options.py
+-rw-rw-rw-   0        0        0    13593 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_output.py
+-rw-rw-rw-   0        0        0    11912 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_request.py
+-rw-rw-rw-   0        0        0    11470 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_response.py
+-rw-rw-rw-   0        0        0    11400 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input.py
+-rw-rw-rw-   0        0        0    12159 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py
+-rw-rw-rw-   0        0        0    11710 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_options.py
+-rw-rw-rw-   0        0        0    13110 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output.py
+-rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py
+-rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_request.py
+-rw-rw-rw-   0        0        0    11409 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_response.py
+-rw-rw-rw-   0        0        0    11636 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/global_ultimate_business.py
+-rw-rw-rw-   0        0        0    13489 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/grade_levels_taught.py
+-rw-rw-rw-   0        0        0    11435 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/greatschools.py
+-rw-rw-rw-   0        0        0    11462 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/grid.py
+-rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/health_theme.py
+-rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/heating_type.py
+-rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/households_theme.py
+-rw-rw-rw-   0        0        0    12058 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/housing_theme.py
+-rw-rw-rw-   0        0        0    12055 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/income_theme.py
+-rw-rw-rw-   0        0        0    11874 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/index_variable.py
+-rw-rw-rw-   0        0        0    11677 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/individual_value_variable.py
+-rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/interior_wall.py
+-rw-rw-rw-   0        0        0    11319 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intermediate_points.py
+-rw-rw-rw-   0        0        0    12291 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intersection.py
+-rw-rw-rw-   0        0        0    11686 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/intersection_response.py
+-rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ip_info.py
+-rw-rw-rw-   0        0        0    13054 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd.py
+-rw-rw-rw-   0        0        0    11890 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py
+-rw-rw-rw-   0        0        0    11871 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/key_lookup_request.py
+-rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/keys.py
+-rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/land_use.py
+-rw-rw-rw-   0        0        0    12232 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/lat_long_fields.py
+-rw-rw-rw-   0        0        0    12064 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/life_style_theme.py
+-rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/loc_code.py
+-rw-rw-rw-   0        0        0    11343 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_geometry.py
+-rw-rw-rw-   0        0        0    14407 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_preferences.py
+-rw-rw-rw-   0        0        0    11217 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/location.py
+-rw-rw-rw-   0        0        0    12025 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/location_time.py
+-rw-rw-rw-   0        0        0    12175 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/magnitude.py
+-rw-rw-rw-   0        0        0    11972 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/match.py
+-rw-rw-rw-   0        0        0    11975 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/match1.py
+-rw-rw-rw-   0        0        0    17276 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/matched_address.py
+-rw-rw-rw-   0        0        0    12342 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/matrix.py
+-rw-rw-rw-   0        0        0    11221 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/mcd.py
+-rw-rw-rw-   0        0        0    11652 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/metadata_response.py
+-rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/mitigation_group.py
+-rw-rw-rw-   0        0        0    11474 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/name.py
+-rw-rw-rw-   0        0        0    11477 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/name1.py
+-rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/neighborhoods_response.py
+-rw-rw-rw-   0        0        0    13019 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/network.py
+-rw-rw-rw-   0        0        0    11496 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/organization_type.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/other_rooms.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/owner_vest_type.py
+-rw-rw-rw-   0        0        0    11899 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/owners.py
+-rw-rw-rw-   0        0        0    13778 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_boundary_v2.py
+-rw-rw-rw-   0        0        0    12581 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_v2.py
+-rw-rw-rw-   0        0        0    11612 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/parent_business.py
+-rw-rw-rw-   0        0        0    11412 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_address_request.py
+-rw-rw-rw-   0        0        0    11468 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response.py
+-rw-rw-rw-   0        0        0    11250 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response_list.py
+-rw-rw-rw-   0        0        0    11646 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pbkey.py
+-rw-rw-rw-   0        0        0    11383 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification.py
+-rw-rw-rw-   0        0        0    12826 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification_output.py
+-rw-rw-rw-   0        0        0    11592 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/place.py
+-rw-rw-rw-   0        0        0    11602 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/place1.py
+-rw-rw-rw-   0        0        0    12227 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/places_response.py
+-rw-rw-rw-   0        0        0    20808 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi.py
+-rw-rw-rw-   0        0        0    12870 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary.py
+-rw-rw-rw-   0        0        0    11840 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_address_request.py
+-rw-rw-rw-   0        0        0    11900 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_location_request.py
+-rw-rw-rw-   0        0        0    11825 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_locations.py
+-rw-rw-rw-   0        0        0    11548 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_preferences.py
+-rw-rw-rw-   0        0        0    11333 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_response.py
+-rw-rw-rw-   0        0        0    11800 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_classification.py
+-rw-rw-rw-   0        0        0    11116 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count.py
+-rw-rw-rw-   0        0        0    12954 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count_request.py
+-rw-rw-rw-   0        0        0    13374 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/poiby_geometry_request.py
+-rw-rw-rw-   0        0        0    11725 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/points.py
+-rw-rw-rw-   0        0        0    11241 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/pool_type.py
+-rw-rw-rw-   0        0        0    12067 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/population_theme.py
+-rw-rw-rw-   0        0        0    11114 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/preferenc_time_zone.py
+-rw-rw-rw-   0        0        0    11280 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/primary_zone.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/prior_sale_code.py
+-rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/prop_site_influene.py
+-rw-rw-rw-   0        0        0    11106 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/properties.py
+-rw-rw-rw-   0        0        0    46206 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_attributes.py
+-rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_geometry.py
+-rw-rw-rw-   0        0        0    11918 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_address_request.py
+-rw-rw-rw-   0        0        0    11133 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_preferences.py
+-rw-rw-rw-   0        0        0    12002 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_response.py
+-rw-rw-rw-   0        0        0    11457 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_responses.py
+-rw-rw-rw-   0        0        0    12031 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry.py
+-rw-rw-rw-   0        0        0    11578 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry_crc.py
+-rw-rw-rw-   0        0        0    11696 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/proxy.py
+-rw-rw-rw-   0        0        0    13793 2024-02-13 11:11:51.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/psap_response.py
+-rw-rw-rw-   0        0        0    12085 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py
+-rw-rw-rw-   0        0        0    12626 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/range_variable.py
+-rw-rw-rw-   0        0        0    11664 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/rate.py
+-rw-rw-rw-   0        0        0    13762 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/rate_center_response.py
+-rw-rw-rw-   0        0        0    12337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/return_fields_descriptor.py
+-rw-rw-rw-   0        0        0    11723 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/reverse_geocode_request.py
+-rw-rw-rw-   0        0        0    14978 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk.py
+-rw-rw-rw-   0        0        0    17267 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_address.py
+-rw-rw-rw-   0        0        0    11337 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_geometry.py
+-rw-rw-rw-   0        0        0    11797 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_locations.py
+-rw-rw-rw-   0        0        0    11601 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risk_preferences.py
+-rw-rw-rw-   0        0        0    11316 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_boundaries.py
+-rw-rw-rw-   0        0        0    11368 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_crime_theme.py
+-rw-rw-rw-   0        0        0    11536 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/risks_geometry_crc.py
+-rw-rw-rw-   0        0        0    13324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/road.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_cover_type.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_frame_type.py
+-rw-rw-rw-   0        0        0    11256 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/roof_shape_type.py
+-rw-rw-rw-   0        0        0    12381 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_direction.py
+-rw-rw-rw-   0        0        0    11304 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_geometry.py
+-rw-rw-rw-   0        0        0    13382 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/route_response.py
+-rw-rw-rw-   0        0        0    13904 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sales_tax.py
+-rw-rw-rw-   0        0        0    11569 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sales_volume.py
+-rw-rw-rw-   0        0        0    19116 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school.py
+-rw-rw-rw-   0        0        0    12879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_district.py
+-rw-rw-rw-   0        0        0    13410 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_profile.py
+-rw-rw-rw-   0        0        0    12471 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/school_ranking.py
+-rw-rw-rw-   0        0        0    12003 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/schools_near_by_response.py
+-rw-rw-rw-   0        0        0    11761 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation.py
+-rw-rw-rw-   0        0        0    11365 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation_themes.py
+-rw-rw-rw-   0        0        0    11709 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/severity_group.py
+-rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/shore_line_distance.py
+-rw-rw-rw-   0        0        0    12022 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sic.py
+-rw-rw-rw-   0        0        0    12330 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/sic_metadata.py
+-rw-rw-rw-   0        0        0    12078 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/site_details.py
+-rw-rw-rw-   0        0        0    13485 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/situs_address.py
+-rw-rw-rw-   0        0        0    12476 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district.py
+-rw-rw-rw-   0        0        0    11579 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district_tax.py
+-rw-rw-rw-   0        0        0    13049 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/speed_limit.py
+-rw-rw-rw-   0        0        0    11298 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/start_end_point.py
+-rw-rw-rw-   0        0        0    11227 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/state.py
+-rw-rw-rw-   0        0        0    11265 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/status.py
+-rw-rw-rw-   0        0        0    11273 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/stories.py
+-rw-rw-rw-   0        0        0    12424 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/student_ethnicity.py
+-rw-rw-rw-   0        0        0    12082 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/supply_and_demand_theme.py
+-rw-rw-rw-   0        0        0    18388 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address.py
+-rw-rw-rw-   0        0        0    11824 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address_request.py
+-rw-rw-rw-   0        0        0    11239 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_county.py
+-rw-rw-rw-   0        0        0    13607 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response.py
+-rw-rw-rw-   0        0        0    11446 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response_list.py
+-rw-rw-rw-   0        0        0    11247 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_doc_type.py
+-rw-rw-rw-   0        0        0    11253 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_exemption.py
+-rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_geometry.py
+-rw-rw-rw-   0        0        0    12257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_jurisdiction.py
+-rw-rw-rw-   0        0        0    11798 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_location_request.py
+-rw-rw-rw-   0        0        0    11787 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_locations.py
+-rw-rw-rw-   0        0        0    12845 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_place.py
+-rw-rw-rw-   0        0        0    18168 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address.py
+-rw-rw-rw-   0        0        0    11919 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address_request.py
+-rw-rw-rw-   0        0        0    11810 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_location_request.py
+-rw-rw-rw-   0        0        0    17504 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_matched_address.py
+-rw-rw-rw-   0        0        0    14126 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_response.py
+-rw-rw-rw-   0        0        0    11346 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_responses.py
+-rw-rw-rw-   0        0        0    11268 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_sales_price_code.py
+-rw-rw-rw-   0        0        0    11236 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/tax_state.py
+-rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/time.py
+-rw-rw-rw-   0        0        0    11731 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_address_request.py
+-rw-rw-rw-   0        0        0    11349 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_geometry.py
+-rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_location_request.py
+-rw-rw-rw-   0        0        0    15252 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response.py
+-rw-rw-rw-   0        0        0    11352 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response_list.py
+-rw-rw-rw-   0        0        0    11354 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundaries.py
+-rw-rw-rw-   0        0        0    11234 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundary.py
+-rw-rw-rw-   0        0        0    11283 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/travel_cost_matrix_response.py
+-rw-rw-rw-   0        0        0    11229 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/type.py
+-rw-rw-rw-   0        0        0    13895 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_location.py
+-rw-rw-rw-   0        0        0    11353 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_locations.py
+-rw-rw-rw-   0        0        0    11505 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_range.py
+-rw-rw-rw-   0        0        0    11595 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_unit.py
+-rw-rw-rw-   0        0        0    11235 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/unit.py
+-rw-rw-rw-   0        0        0    13898 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/use_tax.py
+-rw-rw-rw-   0        0        0    11238 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/vacancy.py
+-rw-rw-rw-   0        0        0    11817 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_request.py
+-rw-rw-rw-   0        0        0    11447 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_response.py
+-rw-rw-rw-   0        0        0    11429 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input.py
+-rw-rw-rw-   0        0        0    16658 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input_row.py
+-rw-rw-rw-   0        0        0    15324 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_output.py
+-rw-rw-rw-   0        0        0    11449 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input.py
+-rw-rw-rw-   0        0        0    13503 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py
+-rw-rw-rw-   0        0        0    11357 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_options.py
+-rw-rw-rw-   0        0        0    15940 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_output.py
+-rw-rw-rw-   0        0        0    11520 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py
+-rw-rw-rw-   0        0        0    14342 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py
+-rw-rw-rw-   0        0        0    15105 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py
+-rw-rw-rw-   0        0        0    39660 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py
+-rw-rw-rw-   0        0        0    12012 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py
+-rw-rw-rw-   0        0        0    11529 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py
+-rw-rw-rw-   0        0        0    11480 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py
+-rw-rw-rw-   0        0        0    13512 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py
+-rw-rw-rw-   0        0        0    14100 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py
+-rw-rw-rw-   0        0        0    18611 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py
+-rw-rw-rw-   0        0        0    11944 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py
+-rw-rw-rw-   0        0        0    11489 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py
+-rw-rw-rw-   0        0        0    11891 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_request.py
+-rw-rw-rw-   0        0        0    11458 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_response.py
+-rw-rw-rw-   0        0        0    11530 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py
+-rw-rw-rw-   0        0        0    14701 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py
+-rw-rw-rw-   0        0        0    36257 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py
+-rw-rw-rw-   0        0        0    49413 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py
+-rw-rw-rw-   0        0        0    12029 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py
+-rw-rw-rw-   0        0        0    11539 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py
+-rw-rw-rw-   0        0        0    11488 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request.py
+-rw-rw-rw-   0        0        0    11521 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py
+-rw-rw-rw-   0        0        0    11377 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py
+-rw-rw-rw-   0        0        0    11760 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/water_body.py
+-rw-rw-rw-   0        0        0    11870 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/water_body_response.py
+-rw-rw-rw-   0        0        0    17270 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_address.py
+-rw-rw-rw-   0        0        0    11334 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_boundary_geometry.py
+-rw-rw-rw-   0        0        0    11574 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_contact_details.py
+-rw-rw-rw-   0        0        0    11340 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_geometry.py
+-rw-rw-rw-   0        0        0    11091 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_parent_business.py
+-rw-rw-rw-   0        0        0    14879 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi.py
+-rw-rw-rw-   0        0        0    11851 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_classification.py
+-rw-rw-rw-   0        0        0    11863 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_geometry.py
+-rw-rw-rw-   0        0        0    11791 2024-02-13 11:11:52.000000 com.precisely.apis-18.0.1/com/precisely/apis/model/zones_sic.py
+-rw-rw-rw-   0        0        0    81943 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/model_utils.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/com/precisely/apis/models/
+-rw-rw-rw-   0        0        0    28241 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/models/__init__.py
+-rw-rw-rw-   0        0        0    14245 2024-02-13 11:11:54.000000 com.precisely.apis-18.0.1/com/precisely/apis/rest.py
+drwxrwxrwx   0        0        0        0 2024-04-11 06:29:37.270942 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/
+-rw-rw-rw-   0        0        0      540 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0    19569 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2024-04-11 06:29:27.000000 com.precisely.apis-18.0.1/com.precisely.apis.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       76 2024-04-11 06:29:37.291172 com.precisely.apis-18.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1224 2024-04-11 06:23:16.000000 com.precisely.apis-18.0.1/setup.py
```

### Comparing `com.precisely.apis-18.0.0/LICENSE` & `com.precisely.apis-18.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/PKG-INFO` & `com.precisely.apis-18.0.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: com.precisely.apis
-Version: 18.0.0
+Version: 18.0.1
 Summary: Precisely APIs
 Home-page: https://developer.precisely.com/
 Author: Precisely APIs Support
 Author-email: PreciselyAPIs-Support@precisely.com
 License: Apache 2.0
 Keywords: Precisely APIs
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: urllib3>=1.25.3
 Requires-Dist: python-dateutil
+Requires-Dist: requests
 
     Enhance and enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.
```

### Comparing `com.precisely.apis-18.0.0/README.md` & `com.precisely.apis-18.0.1/README.md`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/__init__.py` & `com.precisely.apis-18.0.1/com/precisely/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_enterprise_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/address_autocomplete_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/address_autocomplete_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/address_verification_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/address_verification_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/addresses_service__api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/addresses_service__api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/demographics_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/demographics_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/email_verification_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/email_verification_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/geocode_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/geocode_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/geolocation_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/geolocation_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/local_tax_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/local_tax_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/neighborhoods_service__api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/neighborhoods_service__api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/phone_verification_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/phone_verification_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/places_service__api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/places_service__api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/property_information_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/property_information_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/psap_911_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/psap_911_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/risks_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/risks_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/routing_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/routing_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/schools_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/schools_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/streets_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/streets_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/telecomm_info_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/telecomm_info_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/time_zone_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/time_zone_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api/zones_service_api.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api/zones_service_api.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/api_client.py` & `com.precisely.apis-18.0.1/com/precisely/apis/api_client.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/apis/__init__.py` & `com.precisely.apis-18.0.1/com/precisely/apis/apis/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/configuration.py` & `com.precisely.apis-18.0.1/com/precisely/apis/configuration.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/exceptions.py` & `com.precisely.apis-18.0.1/com/precisely/apis/exceptions.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/absentee_owner.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/absentee_owner.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/accuracy.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/accuracy.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/address1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/address1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/address2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/address2.py`

 * *Files 1% similar despite different names*

```diff
@@ -108,15 +108,15 @@
             'post_code_ext': (str,),  # noqa: E501
             'country': (str,),  # noqa: E501
             'address_number': (str,),  # noqa: E501
             'street_name': (str,),  # noqa: E501
             'unit_type': (str,),  # noqa: E501
             'unit_value': (str,),  # noqa: E501
             'postal_verified': (str,),  # noqa: E501
-            'custom_fields': ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)},),  # noqa: E501
+            'custom_fields': (dict,)   # noqa: E501
         }
 
     @cached_property
     def discriminator():
         return None
 
 
@@ -223,15 +223,15 @@
             post_code_ext (str): [optional]  # noqa: E501
             country (str): [optional]  # noqa: E501
             address_number (str): [optional]  # noqa: E501
             street_name (str): [optional]  # noqa: E501
             unit_type (str): [optional]  # noqa: E501
             unit_value (str): [optional]  # noqa: E501
             postal_verified (str): [optional]  # noqa: E501
-            custom_fields ({str: ({str: (bool, date, datetime, dict, float, int, list, str, none_type)},)}): [optional]  # noqa: E501
+            custom_fields (dict,): [optional]  # noqa: E501
         """
 
         _check_type = kwargs.pop('_check_type', True)
         _spec_property_naming = kwargs.pop('_spec_property_naming', False)
         _path_to_item = kwargs.pop('_path_to_item', ())
         _configuration = kwargs.pop('_configuration', None)
         _visited_composed_classes = kwargs.pop('_visited_composed_classes', ())
```

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/address_time.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/address_time.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/address_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/address_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_by_boundary_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_by_boundary_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_count.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_count.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_dto.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_dto.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/addresses_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/addresses_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ah_jmailing_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ah_jmailing_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ahj.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ahj_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ahj_plus_psap_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ahj_plus_psap_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/amenities.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/amenities.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/area.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/area.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/area_code_info.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/area_code_info.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/area_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/area_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/assets_and_wealth_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/assets_and_wealth_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/base_flood_elevation.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/base_flood_elevation.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/basement_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/basement_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/basic_boundary.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/basic_boundary.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/boundaries.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/boundaries.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/boundary.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/boundary_buffer.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_buffer.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/boundary_point.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/boundary_point.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buffer_relation.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buffer_relation.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_class.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_class.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_condition.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_condition.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_features_sqft.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_features_sqft.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_improve_area.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_area.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_improve_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_improve_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_quality.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_quality.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_style.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_style.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/buildg_view.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/buildg_view.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/building_sqft_source.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/building_sqft_source.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/business_id.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/business_id.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ca_exemptions.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ca_exemptions.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/candidate.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/candidate_range.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/candidate_range_unit.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/candidate_range_unit.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/carrier.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/carrier.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/category.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/category.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/category_metadata.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/category_metadata.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/cbsa.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/cbsa.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/census.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/census.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/center.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/center.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/city.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/city.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/common_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/common_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/community.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/community.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/community_group.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/community_group.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/consistency_code.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/consistency_code.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/construction.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/construction.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/contact_details.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/contact_details.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/contact_person.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/contact_person.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/cooling_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/cooling_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/cost.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/cost.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/county.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/county.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/coverage.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/coverage.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_boundary.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_boundary.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_index_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_index_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_by_address_batch_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_address_batch_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_by_location_batch_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_by_location_batch_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crime_risk_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crime_risk_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/crs.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/crs.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/damage_group.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/damage_group.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_advanced_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_advanced_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_advanced_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_geometry_crc.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_geometry_crc.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/demographics_themes_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/demographics_themes_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/depth.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/depth.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/direction_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/direction_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_border.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_border.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/distance_to_flood_hazard_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/distance_to_flood_hazard_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/district_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/district_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/domestic_ultimate_business.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/domestic_ultimate_business.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_date_time.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_date_time.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_event.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_event.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_events_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_events_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_history.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_history.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_location.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_location.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_by_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_by_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_by_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/earthquake_risk_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/earthquake_risk_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/education_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/education_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/employee_count.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/employee_count.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/employment_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/employment_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/energy_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/energy_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/error_code.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/error_code.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/error_info.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/error_info.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/error_info1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/error_info1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/events_count.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/events_count.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/expenditure_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/expenditure_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/exterior_walls.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/exterior_walls.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/extra_feature_sqft.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/extra_feature_sqft.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/field.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/field.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fields_matching.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fields_matching.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_department.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_department.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_event.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_event_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_event_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_events_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_events_v2_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_events_v2_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_history.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_history_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_history_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_by_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_by_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_by_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_v2_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_risk_v2_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_risk_v2_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_shed.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_shed.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_station.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_station_contact_details.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_station_contact_details.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fire_stations.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fire_stations.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fireplace_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fireplace_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_hazard_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_hazard_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_by_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_by_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_by_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_risk_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_risk_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/flood_zone.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/flood_zone.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/floor_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/floor_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/formatted_tax_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/formatted_tax_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/foundation.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/foundation.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/free_or_reduced_price_lunches.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/free_or_reduced_price_lunches.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/frequency_group.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/frequency_group.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/fuel_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/fuel_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/garage_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/garage_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_access_point.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_access_point.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_country.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_country.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_ip_addr.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_ip_addr.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_place.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_place.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_location_state.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_location_state.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geo_pos.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geo_pos.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_service_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geocode_service_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geocode_service_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geolocation_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geolocation_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geometry_crc.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_crc.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/geometry_properties.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/geometry_properties.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_city_state_province_api_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_city_state_province_api_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_output_user_fields.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/get_postal_codes_api_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/get_postal_codes_api_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/global_ultimate_business.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/global_ultimate_business.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/grade_levels_taught.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/grade_levels_taught.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/greatschools.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/greatschools.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/grid.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/grid.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/health_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/health_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/heating_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/heating_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/households_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/households_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/housing_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/housing_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/income_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/income_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/index_variable.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/index_variable.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/individual_value_variable.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/individual_value_variable.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/interior_wall.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/interior_wall.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/intermediate_points.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/intermediate_points.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/intersection.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/intersection.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/intersection_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/intersection_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ip_info.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ip_info.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ipd.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ipd_tax_by_address_batch_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_by_address_batch_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/ipd_tax_jurisdiction.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/ipd_tax_jurisdiction.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/key_lookup_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/key_lookup_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/keys.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/keys.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/land_use.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/land_use.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/lat_long_fields.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/lat_long_fields.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/life_style_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/life_style_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/loc_code.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/loc_code.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/local_tax_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/local_tax_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/local_tax_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/location.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/location.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/location_time.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/location_time.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/magnitude.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/magnitude.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/match.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/match.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/match1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/match1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/matched_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/matched_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/matrix.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/matrix.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/mcd.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/mcd.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/metadata_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/metadata_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/mitigation_group.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/mitigation_group.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/name.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/name.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/name1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/name1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/neighborhoods_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/neighborhoods_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/network.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/network.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/organization_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/organization_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/other_rooms.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/other_rooms.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/owner_vest_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/owner_vest_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/owners.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/owners.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/parcel_boundary_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_boundary_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/parcel_v2.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/parcel_v2.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/parent_business.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/parent_business.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/pb_key_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/pb_key_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/pbkey.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/pbkey.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/phone_verification.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/phone_verification_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/phone_verification_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/place.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/place.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/place1.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/place1.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/places_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/places_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_locations.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_locations.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_boundary_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_boundary_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_classification.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_classification.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_count.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poi_count_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poi_count_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/poiby_geometry_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/poiby_geometry_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/points.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/points.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/pool_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/pool_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/population_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/population_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/preferenc_time_zone.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/preferenc_time_zone.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/primary_zone.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/primary_zone.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/prior_sale_code.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/prior_sale_code.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/prop_site_influene.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/prop_site_influene.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/properties.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/properties.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_attributes.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_attributes.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_info_responses.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_info_responses.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_information_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/property_information_geometry_crc.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/property_information_geometry_crc.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/proxy.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/proxy.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/psap_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/psap_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/race_and_ethnicity_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/race_and_ethnicity_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/range_variable.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/range_variable.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/rate.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/rate.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/rate_center_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/rate_center_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/return_fields_descriptor.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/return_fields_descriptor.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/reverse_geocode_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/reverse_geocode_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risk.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risk.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risk_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risk_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risk_locations.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_locations.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risk_preferences.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risk_preferences.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risks_boundaries.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_boundaries.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risks_crime_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_crime_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/risks_geometry_crc.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/risks_geometry_crc.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/road.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/road.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/roof_cover_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_cover_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/roof_frame_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_frame_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/roof_shape_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/roof_shape_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/route_direction.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/route_direction.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/route_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/route_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/route_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/route_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/sales_tax.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/sales_tax.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/sales_volume.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/sales_volume.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/school.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/school.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/school_district.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/school_district.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/school_profile.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/school_profile.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/school_ranking.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/school_ranking.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/schools_near_by_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/schools_near_by_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/segmentation.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/segmentation_themes.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/segmentation_themes.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/severity_group.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/severity_group.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/shore_line_distance.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/shore_line_distance.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/sic.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/sic.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/sic_metadata.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/sic_metadata.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/site_details.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/site_details.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/situs_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/situs_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/special_purpose_district.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/special_purpose_district_tax.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/special_purpose_district_tax.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/speed_limit.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/speed_limit.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/start_end_point.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/start_end_point.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/state.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/state.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/status.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/status.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/stories.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/stories.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/student_ethnicity.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/student_ethnicity.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/supply_and_demand_theme.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/supply_and_demand_theme.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_county.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_county.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_district_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_district_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_district_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_doc_type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_doc_type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_exemption.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_exemption.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_jurisdiction.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_jurisdiction.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_locations.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_locations.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_place.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_place.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_matched_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_matched_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_rate_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_rate_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_responses.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_responses.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_sales_price_code.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_sales_price_code.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/tax_state.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/tax_state.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/time.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/time.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_location_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_location_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/timezone_response_list.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/timezone_response_list.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/travel_boundaries.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundaries.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/travel_boundary.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_boundary.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/travel_cost_matrix_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/travel_cost_matrix_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/type.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/type.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_location.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_location.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_locations.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_locations.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_range.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_range.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/typeahead_unit.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/typeahead_unit.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/unit.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/unit.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/use_tax.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/use_tax.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/vacancy.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/vacancy.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_api_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_api_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_api_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_email_address_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_email_address_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_premium_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_premium_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_pro_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_pro_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_options.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_output.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_mailing_address_uscanapi_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request_input.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/validate_phone_number_api_request_input_row.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/validate_phone_number_api_request_input_row.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/water_body.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/water_body.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/water_body_response.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/water_body_response.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_address.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_address.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_boundary_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_boundary_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_contact_details.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_contact_details.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_parent_business.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_parent_business.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi_classification.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_classification.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_poi_geometry.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_poi_geometry.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model/zones_sic.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model/zones_sic.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/model_utils.py` & `com.precisely.apis-18.0.1/com/precisely/apis/model_utils.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/models/__init__.py` & `com.precisely.apis-18.0.1/com/precisely/apis/models/__init__.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com/precisely/apis/rest.py` & `com.precisely.apis-18.0.1/com/precisely/apis/rest.py`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/com.precisely.apis.egg-info/PKG-INFO` & `com.precisely.apis-18.0.1/com.precisely.apis.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: com.precisely.apis
-Version: 18.0.0
+Version: 18.0.1
 Summary: Precisely APIs
 Home-page: https://developer.precisely.com/
 Author: Precisely APIs Support
 Author-email: PreciselyAPIs-Support@precisely.com
 License: Apache 2.0
 Keywords: Precisely APIs
 Requires-Python: >=3.6
 License-File: LICENSE
 Requires-Dist: urllib3>=1.25.3
 Requires-Dist: python-dateutil
+Requires-Dist: requests
 
     Enhance and enrich your data, applications, business processes, and workflows with rich location, information, and identify APIs.
```

### Comparing `com.precisely.apis-18.0.0/com.precisely.apis.egg-info/SOURCES.txt` & `com.precisely.apis-18.0.1/com.precisely.apis.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `com.precisely.apis-18.0.0/setup.py` & `com.precisely.apis-18.0.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,25 +7,26 @@
     Generated by: https://openapi-generator.tech
 """
 
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "com.precisely.apis"
-VERSION = "18.0.0"
+VERSION = "18.0.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
 
 REQUIRES = [
   "urllib3 >= 1.25.3",
   "python-dateutil",
+  "requests"
 ]
 
 setup(
     name=NAME,
     version=VERSION,
     description="Precisely APIs",
     author="Precisely APIs Support",
```

