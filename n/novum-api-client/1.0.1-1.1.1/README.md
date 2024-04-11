# Comparing `tmp/novum_api_client-1.0.1.tar.gz` & `tmp/novum_api_client-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "novum_api_client-1.0.1.tar", max compression
+gzip compressed data, was "novum_api_client-1.1.1.tar", max compression
```

## Comparing `novum_api_client-1.0.1.tar` & `novum_api_client-1.1.1.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0      385 2023-12-13 13:05:03.511057 novum_api_client-1.0.1/CHANGELOG.md
--rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-1.0.1/LICENSE
--rw-r--r--   0        0        0      313 2023-12-12 13:02:11.132292 novum_api_client-1.0.1/README.md
--rw-r--r--   0        0        0        0 2023-12-12 13:02:11.132292 novum_api_client-1.0.1/novum_api_client/__init__.py
--rw-r--r--   0        0        0    11711 2023-12-13 13:03:22.015545 novum_api_client-1.0.1/novum_api_client/api_type.py
--rw-r--r--   0        0        0    10916 2023-12-13 09:53:14.865816 novum_api_client-1.0.1/novum_api_client/base_client.py
--rw-r--r--   0        0        0    23352 2023-12-13 10:51:18.357867 novum_api_client-1.0.1/novum_api_client/client.py
--rw-r--r--   0        0        0        0 2023-12-12 13:02:11.132292 novum_api_client-1.0.1/novum_api_client/tests/__init__.py
--rw-r--r--   0        0        0    10238 2023-12-12 13:02:11.132292 novum_api_client-1.0.1/novum_api_client/tests/test_api_base.py
--rw-r--r--   0        0        0    22575 2023-12-12 13:02:11.132292 novum_api_client-1.0.1/novum_api_client/tests/test_api_public.py
--rw-r--r--   0        0        0      627 2023-12-13 13:05:41.034877 novum_api_client-1.0.1/pyproject.toml
--rw-r--r--   0        0        0      472 1970-01-01 00:00:00.000000 novum_api_client-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2023-07-05 06:53:04.093748 novum_api_client-1.1.1/LICENSE
+-rw-r--r--   0        0        0      737 2024-04-11 08:34:58.578504 novum_api_client-1.1.1/README.md
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.098131 novum_api_client-1.1.1/novum_api_client/__init__.py
+-rw-r--r--   0        0        0    12736 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/api_type.py
+-rw-r--r--   0        0        0    10916 2024-04-11 08:16:44.323742 novum_api_client-1.1.1/novum_api_client/base_client.py
+-rw-r--r--   0        0        0    25382 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/client.py
+-rw-r--r--   0        0        0        0 2024-01-02 08:51:00.102131 novum_api_client-1.1.1/novum_api_client/tests/__init__.py
+-rw-r--r--   0        0        0    10245 2024-04-11 08:16:44.323742 novum_api_client-1.1.1/novum_api_client/tests/test_api_base.py
+-rw-r--r--   0        0        0    25868 2024-04-11 08:16:47.635780 novum_api_client-1.1.1/novum_api_client/tests/test_api_public.py
+-rw-r--r--   0        0        0      537 2024-04-11 08:45:51.268680 novum_api_client-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1251 1970-01-01 00:00:00.000000 novum_api_client-1.1.1/PKG-INFO
```

### Comparing `novum_api_client-1.0.1/LICENSE` & `novum_api_client-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `novum_api_client-1.0.1/novum_api_client/api_type.py` & `novum_api_client-1.1.1/novum_api_client/api_type.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # pylint: disable=C0115
 
 import datetime
 from dataclasses import dataclass
-from typing import Dict, List, Optional, Union
+from typing import Dict, List, Literal, Optional, Union
 
 
 @dataclass
 class TNovumClient:
     pass
 
 
@@ -27,27 +27,27 @@
     email: Optional[str]
     email_verified: Optional[bool]
     picture: Optional[str]
 
 
 @dataclass
 class TServiceCenterSettings:
-    show_advanced_options: Optional[bool]
-    invert_axis: Optional[bool]
-    only_show_top_level_batteries: Optional[bool]
-    favorite_batteries_ids: Optional[List[str]]
-    battery_table_columns: Optional[List[str]]
-    dashboard_table_columns: Optional[List[str]]
-    eis_dataset_table_columns: Optional[List[str]]
-    capacity_measurement_table_columns: Optional[List[str]]
+    showAdvancedOptions: Optional[bool]
+    invertAxis: Optional[bool]
+    onlyShowTopLevelBatteries: Optional[bool]
+    favoriteBatteriesIds: Optional[List[str]]
+    batteryTableColumns: Optional[List[str]]
+    dashboardTableColumns: Optional[List[str]]
+    eisDatasetTableColumns: Optional[List[str]]
+    capacityMeasurementTableColumns: Optional[List[str]]
 
 
 @dataclass
 class TUserSettings:
-    service_center: Optional[TServiceCenterSettings]
+    ServiceCenterSettings: Optional[TServiceCenterSettings]
 
 
 @dataclass
 class TIDAndTimes:
     id: Optional[str]
     created_at: Optional[Union[datetime.datetime, str]] = None
     updated_at: Optional[Union[datetime.datetime, str]] = None
@@ -61,14 +61,15 @@
     roles: Optional[List[str]] = None
     profile: Optional[TProfile] = None
     settings: Optional[TUserSettings] = None
     permissions: Optional[List[str]] = None
     stats: Optional[TStats] = None
     meta_data: Optional[dict] = None
     scope: Optional[str] = None
+    expires_at: Optional[str] = None
 
 
 @dataclass
 class TUser(TUserEssentials, TIDAndTimes):
     "TUser"
 
 
@@ -98,37 +99,35 @@
 @dataclass
 class TChargeSetup:
     discharge_rate: Optional[float] = None
     charge_rate: Optional[float] = None
 
 
 @dataclass
-class TUserDocument:
-    original_file_name: Optional[str] = None
-    file_name: Optional[str] = None
-    file_url: Optional[str] = None
-    file_md5: Optional[str] = None
-    file_type: Optional[Dict[str, Union[str, int, float]]] = None
-    file_size: Optional[int] = None
-    aws_file_url: Optional[str] = None
-    aws_file_name: Optional[str] = None
-
-
-@dataclass
 class TBaseDocModel(TIDAndTimes):
     id: Optional[str] = None
     creator_id: Optional[str] = None
     updater_id: Optional[str] = None
 
 
 @dataclass
+class TUserDocument(TBaseDocModel):
+    originalFileName: Optional[str] = None
+    fileName: Optional[str] = None
+    fileURL: Optional[str] = None
+    fileMD5: Optional[str] = None
+    fileType: Optional[Dict[str, Union[str, int, float]]] = None
+    fileSize: Optional[int] = None
+    AWSFileURL: Optional[str] = None
+    AWSFileName: Optional[str] = None
+
+
+@dataclass
 class TDetails:
-    code: Optional[int]
-    error: Optional[str]
-    details: Optional[str]
+    statusCode: Optional[int]
     headers: Optional[Dict[str, str]]
 
 
 @dataclass
 class TAPIError:
     error: Optional[str]
     details: Optional[TDetails]
@@ -171,15 +170,15 @@
     scale: float
     top: float
     left: float
 
 
 @dataclass
 class TIndicatorProperties:
-    properties: Dict[str, TIndicatorProperty]
+    indicator_properties: Dict[str, TIndicatorProperty]
 
 
 @dataclass
 class TInsights:
     enabled: Optional[bool] = None
     image: Optional[str] = None
     image_styles: Optional[str] = None
@@ -223,28 +222,65 @@
 
 
 @dataclass
 class TEstimators:
     soc_estimator: Optional[TEstimatorOverview]
 
 
+TBatteryGrades = Literal[
+    "A",
+    "B",
+    "C",
+    "D",
+    "E",
+    "F",
+    "G",
+    "H",
+    "I",
+    "J",
+    "K",
+    "L",
+    "M",
+    "N",
+    "O",
+    "P",
+    "Q",
+    "R",
+    "S",
+    "T",
+    "U",
+    "V",
+    "W",
+    "X",
+    "Y",
+    "Z",
+]
+
+
+@dataclass
+class TLowerSoHLimit:
+    soh: float
+    grade: TBatteryGrades
+
+
 @dataclass
 class TBatteryTypeEssentials:
     """For writing"""
 
     name: str
     manufacturer: str
     nominal_voltage: float
     nominal_capacity: float
     description: Optional[str] = None
     cell_chemistry: Optional[str] = None
     battery_design: Optional[str] = None
     allowed_voltage_range_single_cell: Optional[TMinMax] = None
     allowed_voltage_range_battery_pack: Optional[TMinMax] = None
     allowed_peak_charge_current_range: Optional[TMinMax] = None
+    allowed_peak_discharge_current_range: Optional[TMinMax] = None
     allowed_continuous_charge_current_range: Optional[TMinMax] = None
     allowed_temperature_range_for_charging: Optional[TMinMax] = None
     allowed_temperature_range_for_storage: Optional[TMinMax] = None
     allowed_temperature_range_for_use: Optional[TMinMax] = None
     internal_resistance: Optional[float] = None
     self_discharge_rate_per_month: Optional[float] = None
     allowed_cycles_for_100_depth_of_discharge: Optional[int] = None
@@ -254,14 +290,15 @@
     default_eis_setup: Optional[TEISSetup] = None
     default_charge_setup: Optional[TChargeSetup] = None
     image: Optional[str] = None
     user_docs: Optional[List[TUserDocument]] = None
     user_doc_ids: Optional[List[str]] = None
     public: Optional[bool] = None
     tags: Optional[List[str]] = None
+    grade_lookup_table: Optional[List[TLowerSoHLimit]] = None
 
 
 @dataclass
 class TBatteryType(TBaseDocModel, TBatteryTypeEssentials):
     """For reading"""
 
 
@@ -468,7 +505,36 @@
     pass
 
 
 @dataclass
 class TDeviceMeasurement:
     device_id: str
     measurements: UITMeasurements
+
+
+@dataclass
+class TDeviceMeasurementsResult:
+    results: List[UITMeasurement]
+    rejectedDeviceIds: List[str]
+
+
+@dataclass
+class ReportStates:
+    Unread = "unread"
+    Viewed = "viewed"
+    Acknowledged = "acknowledged"
+
+
+@dataclass
+class TReportEssentials:
+    state: ReportStates
+    origin_id: Optional[str]
+    title: Optional[str]
+    description: Optional[str]
+    context_id: Optional[str]
+    meta: Optional[dict] = None
+    user_doc_ids: Optional[List[str]] = None
+
+
+@dataclass
+class TReport(TBaseDocModel, TReportEssentials):
+    "TReport"
```

### Comparing `novum_api_client-1.0.1/novum_api_client/base_client.py` & `novum_api_client-1.1.1/novum_api_client/base_client.py`

 * *Files identical despite different names*

### Comparing `novum_api_client-1.0.1/novum_api_client/client.py` & `novum_api_client-1.1.1/novum_api_client/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,26 +4,30 @@
 
 import json
 from typing import Optional, List
 import requests
 from dataclasses import dataclass
 from .base_client import BaseAPIClient, NovumAPIError
 from .api_type import (
-    TAPIInfoEssentials,
+    TUser,
+    TReport,
+    TDataset,
     TBattery,
     TBatteryType,
-    TCapacityMeasurement,
-    TDataset,
-    TDeviceMeasurement,
-    TUser,
+    TUserDocument,
+    TReportEssentials,
     TDatasetEssentials,
     TBatteryEssentials,
+    TAPIInfoEssentials,
+    TVersionEssentials,
+    TDeviceMeasurement,
+    TCapacityMeasurement,
     TBatteryTypeEssentials,
+    TDeviceMeasurementsResult,
     TCapacityMeasurementEssentials,
-    TVersionEssentials,
 )
 
 PRODUCTION_API_HOST: str = "https://novum-batteries.com"
 
 
 @dataclass
 class NovumAPIClient(BaseAPIClient):
@@ -110,22 +114,22 @@
 
     def get_battery_types_count(
         self,
         filter_types: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         return self._get_json(
             "/api/batman/v1/batteryTypes/count",
             filter_json=filter_types,
             option=option,
             fields=fields,
             timeout=timeout,
-        )
+        )  # type: ignore
 
     def get_battery_types_by_id(
         self, battery_type_id: str, timeout: float = 4.0
     ) -> TBatteryType:
         battery_type = self._get_json(
             f"/api/batman/v1/batteryTypes/{battery_type_id}", timeout=timeout
         )
@@ -210,42 +214,42 @@
 
     def get_datasets_count(
         self,
         filter_datasets: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         return self._get_json(
             "/api/batman/v1/datasets/count",
             filter_json=filter_datasets,
             option=option,
             fields=fields,
             timeout=timeout,
-        )
+        )  # type: ignore
 
     def get_datasets_count_by_battery(
         self,
         battery: TBattery,
         filter_datasets: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         filter_with_id = {"meta.battery._id": battery.id}
         if filter_datasets is not None:
             filter_with_id.update(filter_datasets)
         response = self._get_json(
             "/api/batman/v1/datasets/count",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        return response
+        return response  # type: ignore
 
     def update_dataset_by_id(
         self, dataset_id: str, dataset: TDatasetEssentials, timeout: float = 4.0
     ) -> TDataset:
         updated_dataset = self._put_json(
             f"/api/batman/v1/datasets/{dataset_id}",
             input_data=dataset,
@@ -319,22 +323,22 @@
 
     def get_batteries_count(
         self,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         return self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_batteries,
             option=option,
             fields=fields,
             timeout=timeout,
-        )
+        )  # type: ignore
 
     def get_children_of_battery_by_id(
         self,
         parent_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
@@ -357,26 +361,26 @@
     def get_children_of_battery_by_id_count(
         self,
         parent_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         filter_with_id = {"tree.parent": parent_battery_id}
         if filter_batteries is not None:
             filter_with_id.update(filter_batteries)
         response = self._get_json(
             "/api/batman/v1/batteries/count",
             filter_json=filter_with_id,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        return response
+        return response  # type: ignore
 
     def get_leaves_of_battery_by_id(
         self,
         ancestor_battery_id: str,
         filter_batteries: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
@@ -519,198 +523,240 @@
 
     def get_capacity_measurement_count(
         self,
         filter_measurements: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
+    ) -> int:
         response = self._get_json(
             "/api/batman/v1/capacityMeasurements/count",
             filter_json=filter_measurements,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        return response
+        return response  # type: ignore
 
     def get_capacity_measurement_by_id(
         self, capacity_measurement_id: str, timeout: float = 4.0
     ) -> TCapacityMeasurement:
         capacity_measurement = self._get_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             timeout=timeout,
         )
         return TCapacityMeasurement(**capacity_measurement)
 
     def get_capacity_measurements_count_by_battery(
         self, battery_id: str, timeout: float = 4.0
-    ) -> dict:
+    ) -> int:
         filter_by_id = {"battery._id": battery_id}
         response = self._get_json(
             "/api/batman/v1/capacityMeasurements/count",
             filter_json=filter_by_id,
             timeout=timeout,
         )
-        return response
+        return response  # type: ignore
 
     def capacity_measurement_exists_on_remote(
-        self, capacity_measurement_id: dict, timeout: float = 4.0
+        self, capacity_measurement_id: str, timeout: float = 4.0
     ) -> bool:
         response = self._get_json(
             f"/api/batman/v1/capacityMeasurements/{capacity_measurement_id}",
             timeout=timeout,
         )
         return response["id"] == capacity_measurement_id
 
     # ********************************************************
     # Section for the Measurements
     # ********************************************************
 
     def get_latests_measurements(
         self, device_id: str, count: int = 1, timeout: float = 4.0
-    ) -> dict:
-        return self._get_json(
+    ) -> TDeviceMeasurementsResult:
+        measurements_list = self._get_json(
             f"/api/time-series/v1/devices/{device_id}/measurements/last/{count}",
             timeout=timeout,
         )
 
+        return measurements_list  # type: ignore
+
     def write_device_measurements(
         self, device_measurements: List[TDeviceMeasurement], timeout: float = 4.0
-    ) -> dict:
-        return self._post_json(
+    ) -> TDeviceMeasurementsResult:
+        write_measurement = self._post_json(
             "/api/time-series/v1/measurements",
             input_data=device_measurements,
             timeout=timeout,
         )
+        return write_measurement  # type: ignore
 
     def read_device_measurements(
         self,
         device_filter: Optional[dict],
         option=None,
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
-        return self._get_json(
+    ) -> TDeviceMeasurementsResult:
+        read_measurements = self._get_json(
             "/api/time-series/v1/measurements",
             filter_json=device_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
+        return read_measurements  # type: ignore
 
     def read_device_measurements_by_id(
         self,
         battery_id,
         device_filter: Optional[dict],
         fields: Optional[dict] = None,
         timeout: float = 4.0,
-    ) -> dict:
-        return self._get_json(
+    ) -> TDeviceMeasurementsResult:
+        read_measurements_by_battery_id = self._get_json(
             f"/api/time-series/v1/measurements/{battery_id}",
             filter_json=device_filter,
             fields=fields,
             timeout=timeout,
         )
+        return read_measurements_by_battery_id  # type: ignore
 
     # ********************************************************
     # Section for the Reports
     # ********************************************************
 
-    def create_report(self, report, headers=None, timeout: float = 4.0):
-        return self._post_json(
-            "/api/batman/v1/reports", report, headers, timeout=timeout
-        )
+    def create_report(self, report: TReportEssentials, timeout: float = 4.0) -> TReport:
+        report_post = self._post_json("/api/batman/v1/reports", report, timeout=timeout)
+        return TReport(**report_post)
 
     def update_report_by_id(
-        self, report_id: str, report, headers=None, timeout: float = 4
-    ):
-        return self._put_json(
-            f"/api/batman/v1/reports/{report_id}", report, headers, timeout=timeout
+        self, report_id: str, report: TReportEssentials, timeout: float = 4
+    ) -> TReport:
+        update_report = self._put_json(
+            f"/api/batman/v1/reports/{report_id}", report, timeout=timeout
         )
+        return TReport(**update_report)
 
     def get_reports(
         self,
-        report_filter=None,
-        option=None,
+        report_filter: Optional[dict] = None,
+        option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
-    ):
-        response = self._get_json(
+    ) -> List[TReport]:
+        report_list = self._get_json(
             "/api/batman/v1/reports",
             filter_json=report_filter,
             fields=fields,
             option=option,
             timeout=timeout,
         )
-        return response
+        reports = [TReport(**report) for report in report_list]
+        return reports
 
     def get_reports_count(
         self,
-        report_filter=None,
-        option=None,
+        report_filter: Optional[dict] = None,
+        option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
-    ):
+    ) -> int:
         response = self._get_json(
             "/api/batman/v1/reports/count",
             report_filter,
             option=option,
             fields=fields,
             timeout=timeout,
         )
-        return response
+        return response  # type: ignore
 
-    def get_reports_count_by_battery(self, battery: TBattery, timeout: float = 4):
+    def get_reports_count_by_battery(
+        self, battery: TBattery, timeout: float = 4
+    ) -> int:
         response = self._get_json(
             "/api/batman/v1/reports/count",
             filter_json={"origin_id": battery.id},
             timeout=timeout,
         )
 
-        return response
+        return response  # type: ignore
 
-    def get_report_by_id(self, report_id: str, timeout: float = 4) -> dict:
-        return self._get_json(f"/api/batman/v1/reports/{report_id}", timeout=timeout)
+    def get_report_by_id(self, report_id: str, timeout: float = 4) -> TReport:
+        report = self._get_json(f"/api/batman/v1/reports/{report_id}", timeout=timeout)
+        return TReport(**report)
 
     def get_reports_by_origin_id(
         self,
         origin_id: str,
         report_filter: Optional[dict] = None,
-        option=None,
+        option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
-    ) -> dict:
-        return self._get_json(
+    ) -> List[TReport]:
+        report_list = self._get_json(
             f"/api/batman/v1/reports/byOriginId/{origin_id}",
             report_filter,
-            option,
+            option=option,
             fields=fields,
             timeout=timeout,
         )
 
+        reports = [TReport(**report) for report in report_list]
+
+        return reports
+
     def get_reports_by_origin_id_count(
         self,
         origin_id: str,
         report_filter: Optional[dict] = None,
         option: Optional[dict] = None,
         fields: Optional[dict] = None,
         timeout: float = 4,
-    ) -> dict:
-        return self._get_json(
+    ) -> int:
+        reports_count = self._get_json(
             f"/api/batman/v1/reports/byOriginId/{origin_id}/count",
             report_filter,
             option,
             fields=fields,
             timeout=timeout,
         )
+        return reports_count  # type: ignore
 
     def remove_report_by_id(
         self, report_id: str, report_filter=None, option=None, timeout: float = 4
     ):
         response = self._delete_json(
             f"/api/batman/v1/reports/{report_id}",
             filter_json=report_filter,
             option=option,
             timeout=timeout,
         )
-        return response
+        return "The report was removed."
+
+    # ********************************************************
+    # Section for the userDocs
+    # ********************************************************
+
+    def get_user_documents(
+        self,
+        document_filter: Optional[dict] = None,
+        option: Optional[dict] = None,
+        fields: Optional[dict] = None,
+        timeout: float = 4.0,
+    ) -> List[TUserDocument]:
+        user_documents_list = self._get_json(
+            "/api/batman/v1/userDocuments",
+            filter_json=document_filter,
+            option=option,
+            fields=fields,
+            timeout=timeout,
+        )
+
+        user_documents = [TUserDocument(**document) for document in user_documents_list]
+
+        return user_documents
+
+    def get_user_document_by_id(self, user_document_id: str) -> TUserDocument:
+        document = self._get_json(f"/api/batman/v1/userDocuments/{user_document_id}")
+
+        return TUserDocument(**document)
```

### Comparing `novum_api_client-1.0.1/novum_api_client/tests/test_api_base.py` & `novum_api_client-1.1.1/novum_api_client/tests/test_api_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
             last_name="Grey",
             given_name="The Enchanter",
             email="wizard@fantasyrealm.com",
             family_name="Grey",
             email_verified=True,
             picture="magical_staff.jpg",
         ),
-        settings=TUserSettings(service_center=None),
+        settings=TUserSettings(ServiceCenterSettings=None),
     )
 
 
 def test_get_sha_256():
     assert get_sha_256("hello world") == hashlib.sha256(b"hello world").hexdigest()
     assert get_sha_256("test") == hashlib.sha256(b"test").hexdigest()
```

### Comparing `novum_api_client-1.0.1/pyproject.toml` & `novum_api_client-1.1.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 [tool.poetry]
 name = "novum_api_client"
-version = "1.0.1"
+version = "1.1.1"
 description = "This library contains the basic api functions for Novum Service Center."
 authors = ["Leonardo <l.biz@novum-engineering.com>"]
-long_description_content_type = "text/markdown"
-include = ["README.md", "CHANGELOG.md"]
-
+readme = "README.md"
 
 [tool.poetry.metadata]
 description = "This library contains the basic api functions for Novum Service Center."
-long_description = "file: README.md"
+description-file = "README.md"
+license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 requests = "^2.28.2"
 
-[tool.poetry.dev-dependencies]
-
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

