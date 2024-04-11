# Comparing `tmp/ms_salesforce_api-2.2.0.tar.gz` & `tmp/ms_salesforce_api-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ms_salesforce_api-2.2.0.tar", max compression
+gzip compressed data, was "ms_salesforce_api-2.2.1.tar", max compression
```

## Comparing `ms_salesforce_api-2.2.0.tar` & `ms_salesforce_api-2.2.1.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    35149 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/LICENSE
--rw-r--r--   0        0        0     8326 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/README.md
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/__init__.py
--rw-r--r--   0        0        0     1491 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/Auth.py
--rw-r--r--   0        0        0     1244 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/JWTGenerator.py
--rw-r--r--   0        0        0     2926 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/__init__.py
--rw-r--r--   0        0        0     2749 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py
--rw-r--r--   0        0        0     2205 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
--rw-r--r--   0        0        0     5168 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/__init__.py
--rw-r--r--   0        0        0     1620 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py
--rw-r--r--   0        0        0     4905 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/constants.py
--rw-r--r--   0        0        0    13944 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
--rw-r--r--   0        0        0     5205 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
--rw-r--r--   0        0        0     6011 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    10789 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0      303 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/helpers.py
--rw-r--r--   0        0        0     3788 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
--rw-r--r--   0        0        0    24171 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
--rw-r--r--   0        0        0    10375 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/constants.py
--rw-r--r--   0        0        0     3967 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
--rw-r--r--   0        0        0    28492 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
--rw-r--r--   0        0        0     2313 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/__init__.py
--rw-r--r--   0        0        0     8840 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
--rw-r--r--   0        0        0    12640 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
--rw-r--r--   0        0        0    13717 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
--rw-r--r--   0        0        0        0 2024-03-22 10:31:17.078657 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/helpers/__init__.py
--rw-r--r--   0        0        0      303 2024-03-22 10:31:17.082656 ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/helpers/string.py
--rw-r--r--   0        0        0     1055 2024-03-22 10:31:17.082656 ms_salesforce_api-2.2.0/pyproject.toml
--rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.2.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/LICENSE
+-rw-r--r--   0        0        0     8326 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/README.md
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/__init__.py
+-rw-r--r--   0        0        0     1491 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/Auth.py
+-rw-r--r--   0        0        0     1244 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/JWTGenerator.py
+-rw-r--r--   0        0        0     2926 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/__init__.py
+-rw-r--r--   0        0        0     2749 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py
+-rw-r--r--   0        0        0     2205 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py
+-rw-r--r--   0        0        0     5168 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/__init__.py
+-rw-r--r--   0        0        0     1620 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/__init__.py
+-rw-r--r--   0        0        0     4925 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/constants.py
+-rw-r--r--   0        0        0    14424 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/dto/__init__.py
+-rw-r--r--   0        0        0     5242 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py
+-rw-r--r--   0        0        0     6011 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    10789 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0      303 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/helpers.py
+-rw-r--r--   0        0        0     3788 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/__tests__/__init__.py
+-rw-r--r--   0        0        0    24290 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py
+-rw-r--r--   0        0        0    10430 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/constants.py
+-rw-r--r--   0        0        0     3967 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py
+-rw-r--r--   0        0        0    28488 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py
+-rw-r--r--   0        0        0     2485 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/__init__.py
+-rw-r--r--   0        0        0     8873 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py
+-rw-r--r--   0        0        0    12640 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/__init__.py
+-rw-r--r--   0        0        0    13717 2024-04-10 09:20:56.040676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py
+-rw-r--r--   0        0        0        0 2024-04-10 09:20:56.044676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/helpers/__init__.py
+-rw-r--r--   0        0        0      303 2024-04-10 09:20:56.044676 ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/helpers/string.py
+-rw-r--r--   0        0        0     1055 2024-04-10 09:20:56.044676 ms_salesforce_api-2.2.1/pyproject.toml
+-rw-r--r--   0        0        0     9153 1970-01-01 00:00:00.000000 ms_salesforce_api-2.2.1/PKG-INFO
```

### Comparing `ms_salesforce_api-2.2.0/LICENSE` & `ms_salesforce_api-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/README.md` & `ms_salesforce_api-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/Auth.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/JWTGenerator.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/SalesforceQueryExecutor.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_Auth.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_Auth.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_JWTGenerator.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/__tests__/test_SalesforceRequester.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/__init__.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/constants.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/constants.py`

 * *Files 4% similar despite different names*

```diff
@@ -48,14 +48,15 @@
     ROI_Analysis_Completed__c,
     Servicios_Asociados__c,
     StageName,
     Start_Date__c,
     Tier_Short__c,
     TotalOpportunityQuantity,
     Year_Created__c,
+    LKP_Project__c,
     (
         SELECT
             Id,
             Product2.Id,
             Product2.LKP_ProfitCenter__r.Name,
             toLabel(Product2.LKP_ProfitCenter__r.PCK_Country__c),
             FRM_ProductName__c,
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/dto/OpportunityDTO.py`

 * *Files 2% similar despite different names*

```diff
@@ -108,14 +108,15 @@
         associated_services,
         stage_name,
         start_date,
         tier_short,
         total_opportunity_quantity,
         year_created,
         opportunity_line_items,
+        lkp_project,
     ):
         self.opportunity_id = opportunity_id
         self.account_billing_country = account_billing_country
         self.account_owner = account_owner
         self.account_id = account_id
         self.amount = amount
         self.amount_eur = amount_eur
@@ -162,17 +163,28 @@
         self.associated_services = associated_services
         self.stage_name = stage_name
         self.start_date = start_date
         self.tier_short = tier_short
         self.total_opportunity_quantity = total_opportunity_quantity
         self.year_created = year_created
         self.opportunity_line_items = opportunity_line_items
+        self.lkp_project = lkp_project
 
     @staticmethod
     def from_salesforce_record(record):
+        def _get_year_created(key: str):
+            try:
+                year = int(record[key])
+                # We set allways the January first date because they want
+                # a Date field for this value.
+                return f"{year}-01-01"
+
+            except (TypeError, KeyError):
+                return ""
+
         opportunity_line_items = record.get("OpportunityLineItems", {})
         if opportunity_line_items and isinstance(opportunity_line_items, dict):
             line_items_records = record.get("OpportunityLineItems", {}).get(
                 "records", []
             )
             opportunity_line_items = [
                 OpportunityLineItemDTO.from_salesforce_record(
@@ -204,15 +216,15 @@
             ),
             end_date=normalize_value(record.get("EndDate__c", "")),
             expected_revenue=normalize_value(
                 record.get("ExpectedRevenue", "")
             ),
             fiscal=normalize_value(record.get("Fiscal", "")),
             fiscal_quarter=normalize_value(record.get("FiscalQuarter", "")),
-            fiscal_year=normalize_value(record.get("FiscalYear", "")),
+            fiscal_year=_get_year_created("FiscalYear"),
             jira_default_name=normalize_value(
                 record.get("FRM_JiraDefaultName__c", "")
             ),
             ga_client_id=normalize_value(record.get("GACLIENTID__c", "")),
             ga_track_id=normalize_value(record.get("GATRACKID__c", "")),
             ga_user_id=normalize_value(record.get("GAUSERID__c", "")),
             is_global=normalize_value(record.get("Global__c", "")),
@@ -270,16 +282,17 @@
             ),
             stage_name=normalize_value(record.get("StageName", "")),
             start_date=normalize_value(record.get("Start_Date__c", "")),
             tier_short=normalize_value(record.get("Tier_Short__c", "")),
             total_opportunity_quantity=normalize_value(
                 record.get("TotalOpportunityQuantity", "")
             ),
-            year_created=normalize_value(record.get("Year_Created__c", "")),
+            year_created=_get_year_created("Year_Created__c"),
             opportunity_line_items=opportunity_line_items,
+            lkp_project=normalize_value(record.get("LKP_Project__c", "")),
         )
 
     def to_dict(self):
         return {
             "opportunity_id": self.opportunity_id,
             "account_billing_country": self.account_billing_country,
             "account_owner": self.account_owner,
@@ -329,8 +342,9 @@
             "associated_services": self.associated_services,
             "stage_name": self.stage_name,
             "start_date": self.start_date,
             "tier_short": self.tier_short,
             "total_opportunity_quantity": self.total_opportunity_quantity,
             "year_created": self.year_created,
             "opportunity_line_items": self.opportunity_line_items,
+            "lkp_project": self.lkp_project,
         }
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/Bigquery.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
                 "close_date": "DATE",
                 "contact_id": "STRING",
                 "curreny_iso_code": "STRING",
                 "end_date": "DATE",
                 "expected_revenue": "FLOAT",
                 "fiscal": "STRING",
                 "fiscal_quarter": "INTEGER",
-                "fiscal_year": "INTEGER",
+                "fiscal_year": "DATE",
                 "jira_default_name": "STRING",
                 "ga_client_id": "STRING",
                 "ga_track_id": "STRING",
                 "ga_user_id": "FLOAT",
                 "is_global": "BOOLEAN",
                 "has_opportunity_lineitem": "BOOLEAN",
                 "has_overdue_task": "BOOLEAN",
@@ -72,15 +72,16 @@
                 "record_type_id": "STRING",
                 "roi_analysis_completed": "BOOLEAN",
                 "associated_services": "STRING",
                 "stage_name": "STRING",
                 "tier_short": "STRING",
                 "total_opportunity_quantity": "FLOAT",
                 "start_date": "DATE",
-                "year_created": "FLOAT",
+                "year_created": "DATE",
+                "lkp_project": "STRING",
             },
             "opportunity_line_item": {
                 "opportunity_id": "STRING",
                 "product_id": "STRING",
                 "profit_center_name": "STRING",
                 "country": "STRING",
                 "product_name": "STRING",
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/opportunity/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/__init__.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/__init__.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/__tests__/test_Project.py`

 * *Files 0% similar despite different names*

```diff
@@ -383,15 +383,16 @@
 
         opportunity = opportunities[0]
         self.assertIsInstance(opportunity, dict)
         self.assertDictEqual(
             opportunity,
             {
                 "account_assigment_group": "03",
-                "account_billing_address": "211 Main Street, Webster, Maine, 01570, United States",
+                "account_billing_address": "211 Main Street, Webster, Maine, 01570, United "
+                "States",
                 "account_billing_city": "Webster",
                 "account_billing_country": "US",
                 "account_billing_postal_code": "01570",
                 "account_billing_state_code": "ME",
                 "account_billing_street": "211 Main Street",
                 "account_business_function": "BP03",
                 "account_business_name": "THE COMMERCE INSURANCE COMPANY",
@@ -411,15 +412,15 @@
                 "account_phone": None,
                 "account_sap_id": "10000319",
                 "account_tax_category": None,
                 "account_tax_classification": "0",
                 "account_tax_id_type": "US01",
                 "account_tier": "T1",
                 "account_website": None,
-                "amount": 0,
+                "amount": 0.0,
                 "billing_lines": [
                     {
                         "billing_amount": 6708.0,
                         "billing_date": "2022-08-31",
                         "billing_period_ending_date": "2022-08-31",
                         "billing_period_starting_date": "2022-08-01",
                         "billing_plan_amount": "6708",
@@ -469,14 +470,15 @@
                         "country": None,
                         "created_date": "2022-08-02T15:44:34.000+0000",
                         "effort": "516",
                         "ending_date": "2022-12-31",
                         "id": "a0VAX000000EE0b2AG",
                         "last_modified_date": "2023-06-20T22:33:36.000+0000",
                         "ms_pli_name": "USA_UX/UI Design_USMSEX05508",
+                        "ms_project_code": None,
                         "product_name": "UXUI Project",
                         "project_id": "a00AX000002DVi1YAG",
                         "quantity": 516.0,
                         "starting_date": "2022-08-01",
                         "total_price": 33540.0,
                         "unit_price": 65.0,
                     },
@@ -484,14 +486,15 @@
                         "country": None,
                         "created_date": "2022-08-09T14:54:59.000+0000",
                         "effort": "331",
                         "ending_date": "2022-12-31",
                         "id": "a0VAX000000ELU52AO",
                         "last_modified_date": "2023-06-20T22:33:36.000+0000",
                         "ms_pli_name": "ES_UX/UI Design_USMSEX05508",
+                        "ms_project_code": None,
                         "product_name": "UXUI Project",
                         "project_id": "a00AX000002DVi1YAG",
                         "quantity": 331.0,
                         "starting_date": "2022-08-01",
                         "total_price": 21515.0,
                         "unit_price": 65.0,
                     },
```

#### html2text {}

```diff
@@ -153,30 +153,30 @@
 mock_authenticate): mock_authenticate.return_value = "access_token" client_id =
 "client_id" username = "username" domain = "https://auth.example.com"
 private_key = "private_key" project = Project( client_id, username, domain,
 private_key, audience="https://login.salesforce.com", ) opportunities =
 project.get_all() self.assertEqual(len(opportunities), 1) opportunity =
 opportunities[0] self.assertIsInstance(opportunity, dict) self.assertDictEqual
 ( opportunity, { "account_assigment_group": "03", "account_billing_address":
-"211 Main Street, Webster, Maine, 01570, United States",
+"211 Main Street, Webster, Maine, 01570, United " "States",
 "account_billing_city": "Webster", "account_billing_country": "US",
 "account_billing_postal_code": "01570", "account_billing_state_code": "ME",
 "account_billing_street": "211 Main Street", "account_business_function":
 "BP03", "account_business_name": "THE COMMERCE INSURANCE COMPANY",
 "account_cif": "042495247", "account_company_invoicing": "",
 "account_created_date": "2020-03-18T15:32:15.000+0000",
 "account_currency_code": "EUR", "account_customer_groupId": "1",
 "account_customer_subgroupId": "5", "account_fax": None,
 "account_invoicing_email": "client1@test.com", "account_mail_invoicing":
 "client1@test.com", "account_name": "MAPFRE USA", "account_office": "Making
 Science LLC", "account_payment_terms": "T060", "account_pec_email": None,
 "account_phone": None, "account_sap_id": "10000319", "account_tax_category":
 None, "account_tax_classification": "0", "account_tax_id_type": "US01",
-"account_tier": "T1", "account_website": None, "amount": 0, "billing_lines": [
-{ "billing_amount": 6708.0, "billing_date": "2022-08-31",
+"account_tier": "T1", "account_website": None, "amount": 0.0, "billing_lines":
+[ { "billing_amount": 6708.0, "billing_date": "2022-08-31",
 "billing_period_ending_date": "2022-08-31", "billing_period_starting_date":
 "2022-08-01", "billing_plan_amount": "6708", "billing_plan_billing_date":
 "2022-08-31", "billing_plan_item": "1", "billing_plan_service_end_date": "2022-
 08-31", "billing_plan_service_start_date": "2022-08-01", "created_date": "2022-
 08-09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
 "a0sAX000000I8lgYAC", "last_modified_date": "2022-10-16T18:56:34.000+0000",
 "name": "BL-000175313", "project_code": "USMSEX05508", "project_id":
@@ -194,35 +194,35 @@
 "Crosselling/upselling", "operation_coordinator_email": "employee5@test.com",
 "operation_coordinator_sub_email": "employee5@test.com", "opportunity_name":
 "New Site Mapfre AAA", "opportunity_percentage": 100.0, "profit_center":
 "200018", "project_code": "USMSEX05508", "project_id": "a00AX000002DVi1YAG",
 "project_line_items": [ { "country": None, "created_date": "2022-08-02T15:44:
 34.000+0000", "effort": "516", "ending_date": "2022-12-31", "id":
 "a0VAX000000EE0b2AG", "last_modified_date": "2023-06-20T22:33:36.000+0000",
-"ms_pli_name": "USA_UX/UI Design_USMSEX05508", "product_name": "UXUI Project",
-"project_id": "a00AX000002DVi1YAG", "quantity": 516.0, "starting_date": "2022-
-08-01", "total_price": 33540.0, "unit_price": 65.0, }, { "country": None,
-"created_date": "2022-08-09T14:54:59.000+0000", "effort": "331", "ending_date":
-"2022-12-31", "id": "a0VAX000000ELU52AO", "last_modified_date": "2023-06-20T22:
-33:36.000+0000", "ms_pli_name": "ES_UX/UI Design_USMSEX05508", "product_name":
-"UXUI Project", "project_id": "a00AX000002DVi1YAG", "quantity": 331.0,
-"starting_date": "2022-08-01", "total_price": 21515.0, "unit_price": 65.0, },
-], "project_name": "MapfreAAA", "project_start_date": "2022-08-01",
-"project_tier": "Unkown", "stage": "Closed Won", "subgroup_bqid": "5",
-"subgroup_end_date": "2100-12-12", "subgroup_groupid": "a0cAX000000TSWUYA4",
-"subgroup_name": "MAPFRE USA", "subgroup_owner_email": "employee1@test.com",
-"subgroup_start_date": "2023-06-01", "subgroup_subgroupid":
-"a19AX0000004simYAA", }, ) billing_line = opportunity["billing_lines"][0]
-self.assertDictEqual( billing_line, { "billing_amount": 6708.0, "billing_date":
-"2022-08-31", "billing_period_ending_date": "2022-08-31",
-"billing_period_starting_date": "2022-08-01", "billing_plan_amount": "6708",
-"billing_plan_billing_date": "2022-08-31", "billing_plan_item": "1",
-"billing_plan_service_end_date": "2022-08-31",
-"billing_plan_service_start_date": "2022-08-01", "created_date": "2022-08-
-09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
+"ms_pli_name": "USA_UX/UI Design_USMSEX05508", "ms_project_code": None,
+"product_name": "UXUI Project", "project_id": "a00AX000002DVi1YAG", "quantity":
+516.0, "starting_date": "2022-08-01", "total_price": 33540.0, "unit_price":
+65.0, }, { "country": None, "created_date": "2022-08-09T14:54:59.000+0000",
+"effort": "331", "ending_date": "2022-12-31", "id": "a0VAX000000ELU52AO",
+"last_modified_date": "2023-06-20T22:33:36.000+0000", "ms_pli_name": "ES_UX/UI
+Design_USMSEX05508", "ms_project_code": None, "product_name": "UXUI Project",
+"project_id": "a00AX000002DVi1YAG", "quantity": 331.0, "starting_date": "2022-
+08-01", "total_price": 21515.0, "unit_price": 65.0, }, ], "project_name":
+"MapfreAAA", "project_start_date": "2022-08-01", "project_tier": "Unkown",
+"stage": "Closed Won", "subgroup_bqid": "5", "subgroup_end_date": "2100-12-12",
+"subgroup_groupid": "a0cAX000000TSWUYA4", "subgroup_name": "MAPFRE USA",
+"subgroup_owner_email": "employee1@test.com", "subgroup_start_date": "2023-06-
+01", "subgroup_subgroupid": "a19AX0000004simYAA", }, ) billing_line =
+opportunity["billing_lines"][0] self.assertDictEqual( billing_line,
+{ "billing_amount": 6708.0, "billing_date": "2022-08-31",
+"billing_period_ending_date": "2022-08-31", "billing_period_starting_date":
+"2022-08-01", "billing_plan_amount": "6708", "billing_plan_billing_date":
+"2022-08-31", "billing_plan_item": "1", "billing_plan_service_end_date": "2022-
+08-31", "billing_plan_service_start_date": "2022-08-01", "created_date": "2022-
+08-09T14:56:23.000+0000", "currency": "USD", "hourly_price": 65.0, "id":
 "a0sAX000000I8lgYAC", "last_modified_date": "2022-10-16T18:56:34.000+0000",
 "name": "BL-000175313", "project_code": "USMSEX05508", "project_id":
 "a00AX000002DVi1YAG", "revenue_dedication": 103.2, }, )
 mock_make_request.assert_called() @patch
 (
 "ms_salesforce_api.salesforce.api.project.SalesforceQueryExecutor.authenticate"
 # noqa: E501 ) @patch
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/constants.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 DEFAULT_PROJECT_OPPORTUNITY_QUERY = """
 SELECT
+    RU_TotalAmount__c,
     CurrencyIsoCode,
     LKP_MSCompanyInvoicing__r.PCK_Country__c,
     Operation_Coordinator__r.Name,
     Operation_Coordinator_Sub__r.Name,
     CreatedDate,
     LastModifiedDate,
     Opportunity__r.Opportunity_Name_Short__c,
@@ -85,15 +86,16 @@
             Sales_Order_Item__c,
             End_Date__c,
             Revenue_Type__c,
             Effort__c,
             Total_Billing_Amount_Billing_Lines__c,
             MS_PLI_Name__c,
             SapNetAmount__c,
-            Country__c
+            Country__c,
+            MS_Project_Code__c
         FROM
             Project_Line_Items__r
     )
 FROM
     Project__c
 """
 # Project__c   WHERE Id = 'a00AX000002DVi1YAG'
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/BillingLineDTO.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/OpportunityDTO.py`

 * *Files 0% similar despite different names*

```diff
@@ -608,15 +608,15 @@
         )
 
         return OpportunityDTO(
             account_business_name=_get_account_business_name(),
             account_name=_get_account_name(),
             account_id=_get_account_id(),
             currency=record["CurrencyIsoCode"],
-            amount=record.get("Total_Project_Amount__c", 0),
+            amount=record.get("RU_TotalAmount__c", 0.0),
             invoicing_country_code=_get_country_code(),
             operation_coordinator_email=_get_operation_coordinator_email(),
             operation_coordinator_sub_email=_get_operation_coordinator_sub_email(),  # noqa: E501
             created_at=record["CreatedDate"],
             last_updated_at=record["LastModifiedDate"],
             opportunity_name=_get_opportunity_name(),
             stage=_get_stage(),
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/dto/ProjectLineItemDTO.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,28 +9,30 @@
         quantity,
         unit_price,
         total_price,
         ending_date,
         effort,
         ms_pli_name,
         country,
+        project_code,
         project_id,
     ):
         self.id = id
         self.created_date = created_date
         self.last_modified_date = last_modified_date
         self.product_name = product_name
         self.starting_date = starting_date
         self.quantity = quantity
         self.unit_price = unit_price
         self.total_price = total_price
         self.ending_date = ending_date
         self.effort = effort
         self.ms_pli_name = ms_pli_name
         self.country = country
+        self.project_code = project_code
         self.project_id = project_id
 
     @classmethod
     def from_salesforce_record(cls, record, project_id):
         product_name = (
             record.get("ProductNew__r", {}).get("Name")
             if record.get("ProductNew__r")
@@ -45,14 +47,15 @@
             quantity=record.get("Quantity__c"),
             unit_price=record.get("UnitPrice__c"),
             total_price=record.get("Total_Price__c"),
             ending_date=record.get("Ending_Date__c"),
             effort=record.get("Effort__c"),
             ms_pli_name=record.get("MS_PLI_Name__c"),
             country=record.get("Country__c"),
+            project_code=record.get("MS_Project_Code__c"),
             project_id=project_id,
         )
 
     def to_dict(self):
         return {
             "country": self.country,
             "created_date": self.created_date,
@@ -63,8 +66,9 @@
             "ms_pli_name": self.ms_pli_name,
             "product_name": self.product_name,
             "quantity": self.quantity,
             "starting_date": self.starting_date,
             "total_price": self.total_price,
             "unit_price": self.unit_price,
             "project_id": self.project_id,
+            "ms_project_code": self.project_code,
         }
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/Bigquery.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,16 +20,16 @@
         self.project_id = project_id
         self.dataset_id = dataset_id
         self.client = BigQueryManager(
             project_id=project_id, dataset_id=dataset_id
         )
         self.batch_size = 200
         self.schemas = {
-            "opportunities": {
-                "amount": "INTEGER",
+            "projects": {
+                "amount": "FLOAT",
                 "controller_email": "STRING",
                 "controller_sub_email": "STRING",
                 "cost_center": "INTEGER",
                 "created_at": "TIMESTAMP",
                 "currency": "STRING",
                 "invoicing_country_code": "STRING",
                 "jira_task_url": "STRING",
@@ -74,14 +74,15 @@
                 "ending_date": "DATE",
                 "id": "STRING",
                 "last_modified_date": "TIMESTAMP",
                 "ms_pli_name": "STRING",
                 "product_name": "STRING",
                 "project_id": "STRING",
                 "project_code": "STRING",
+                "ms_project_code": "STRING",
                 "quantity": "FLOAT",
                 "starting_date": "DATE",
                 "total_price": "FLOAT",
                 "unit_price": "FLOAT",
             },
             "accounts": {
                 "assigment_group": "INTEGER",
@@ -202,15 +203,15 @@
 
             account_data.append(opportunity_account_data)
             group_data.append(opportunity_group_data)
             subgroup_data.append(opportunity_subgroup_data)
 
         self.client.load_massive_data(
             rows_to_insert=opportunities,
-            table_name="opportunities",
+            table_name="projects",
         )
         self.client.load_massive_data(
             rows_to_insert=group_data,
             table_name="groups",
         )
         self.client.load_massive_data(
             rows_to_insert=subgroup_data,
```

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py` & `ms_salesforce_api-2.2.1/ms_salesforce_api/salesforce/api/project/export_data/__tests__/test_CloudSQL.py`

 * *Files identical despite different names*

### Comparing `ms_salesforce_api-2.2.0/pyproject.toml` & `ms_salesforce_api-2.2.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ms-salesforce-api"
-version = "2.2.0"
+version = "2.2.1"
 description = "Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres."
 authors = ["Making Science"]
 readme = "README.md"
 packages = [{include = "ms_salesforce_api"}]
 include = ["pre-commit-config.yaml"]
 
 [tool.poetry.dependencies]
```

### Comparing `ms_salesforce_api-2.2.0/PKG-INFO` & `ms_salesforce_api-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ms-salesforce-api
-Version: 2.2.0
+Version: 2.2.1
 Summary: Python library used to extract data from Salesforce API and migrate it to Bigquery and Postgres.
 Author: Making Science
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

