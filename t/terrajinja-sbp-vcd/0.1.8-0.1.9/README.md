# Comparing `tmp/terrajinja-sbp-vcd-0.1.8.tar.gz` & `tmp/terrajinja-sbp-vcd-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "terrajinja-sbp-vcd-0.1.8.tar", last modified: Tue Mar 26 20:22:01 2024, max compression
+gzip compressed data, was "terrajinja-sbp-vcd-0.1.9.tar", last modified: Wed Apr 10 19:53:22 2024, max compression
```

## Comparing `terrajinja-sbp-vcd-0.1.8.tar` & `terrajinja-sbp-vcd-0.1.9.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.901740 terrajinja-sbp-vcd-0.1.8/
--rw-rw-rw-   0 root         (0) root         (0)       80 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/HISTORY.md
--rw-r--r--   0 root         (0) root         (0)     1061 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      336 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)    14080 2024-03-26 20:22:01.901740 terrajinja-sbp-vcd-0.1.8/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      417 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/Pipfile
--rw-rw-rw-   0 root         (0) root         (0)    13274 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/VERSION
--rw-rw-rw-   0 root         (0) root         (0)      166 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/requirements.txt
--rw-r--r--   0 root         (0) root         (0)       38 2024-03-26 20:22:01.901740 terrajinja-sbp-vcd-0.1.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1353 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.890740 terrajinja-sbp-vcd-0.1.8/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.890740 terrajinja-sbp-vcd-0.1.8/src/terrajinja/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.890740 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.896740 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/
--rw-rw-rw-   0 root         (0) root         (0)        0 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1616 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      702 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
--rw-rw-rw-   0 root         (0) root         (0)     1529 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     1388 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     2293 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2163 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     2835 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     2860 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2447 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2058 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     2787 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     2997 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)     8977 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)     2996 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/rde.py
--rw-rw-rw-   0 root         (0) root         (0)    12351 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/vm.py
--rw-rw-rw-   0 root         (0) root         (0)     1774 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/vm_internal_disk.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.900740 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/
--rw-r--r--   0 root         (0) root         (0)    14080 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1687 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      130 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2024-03-26 20:22:01.000000 terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-03-26 20:22:01.900740 terrajinja-sbp-vcd-0.1.8/tests/
--rw-rw-rw-   0 root         (0) root         (0)     1426 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_data_vcd_catalog_vapp_template.py
--rw-rw-rw-   0 root         (0) root         (0)      890 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_data_vcd_vm_placement_policy.py
--rw-rw-rw-   0 root         (0) root         (0)     2043 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_network_routed_v2.py
--rw-rw-rw-   0 root         (0) root         (0)     1172 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_alb_pool.py
--rw-rw-rw-   0 root         (0) root         (0)     2750 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_app_port_profile.py
--rw-rw-rw-   0 root         (0) root         (0)     4347 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_distributed_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     4001 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_edge_firewall.py
--rw-rw-rw-   0 root         (0) root         (0)     2520 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
--rw-rw-rw-   0 root         (0) root         (0)     4921 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_ip_set.py
--rw-rw-rw-   0 root         (0) root         (0)    28148 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_nat_rule.py
--rw-rw-rw-   0 root         (0) root         (0)      985 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_virtual_service.py
--rw-rw-rw-   0 root         (0) root         (0)     1486 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_rde.py
--rw-rw-rw-   0 root         (0) root         (0)      912 2024-03-26 20:22:00.000000 terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_vm.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.517024 terrajinja-sbp-vcd-0.1.9/
+-rw-rw-rw-   0 root         (0) root         (0)       80 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/HISTORY.md
+-rw-r--r--   0 root         (0) root         (0)     1061 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      336 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      417 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/Pipfile
+-rw-rw-rw-   0 root         (0) root         (0)    13274 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/VERSION
+-rw-rw-rw-   0 root         (0) root         (0)      166 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/requirements.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-10 19:53:22.517024 terrajinja-sbp-vcd-0.1.9/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1353 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.507023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.513023 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1616 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      702 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py
+-rw-rw-rw-   0 root         (0) root         (0)     1529 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     1388 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2655 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2163 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     2835 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     2860 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2447 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2152 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     2787 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     2997 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)     8977 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/rde.py
+-rw-rw-rw-   0 root         (0) root         (0)    12351 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm.py
+-rw-rw-rw-   0 root         (0) root         (0)     1774 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm_internal_disk.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    14080 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1687 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      130 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2024-04-10 19:53:22.000000 terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-10 19:53:22.516023 terrajinja-sbp-vcd-0.1.9/tests/
+-rw-rw-rw-   0 root         (0) root         (0)     1426 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_catalog_vapp_template.py
+-rw-rw-rw-   0 root         (0) root         (0)      890 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_vm_placement_policy.py
+-rw-rw-rw-   0 root         (0) root         (0)     2043 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_network_routed_v2.py
+-rw-rw-rw-   0 root         (0) root         (0)     2002 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_alb_pool.py
+-rw-rw-rw-   0 root         (0) root         (0)     2750 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_app_port_profile.py
+-rw-rw-rw-   0 root         (0) root         (0)     4347 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_distributed_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     4001 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_firewall.py
+-rw-rw-rw-   0 root         (0) root         (0)     2520 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py
+-rw-rw-rw-   0 root         (0) root         (0)     4921 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_ip_set.py
+-rw-rw-rw-   0 root         (0) root         (0)    28148 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_nat_rule.py
+-rw-rw-rw-   0 root         (0) root         (0)      985 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_virtual_service.py
+-rw-rw-rw-   0 root         (0) root         (0)     1486 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_rde.py
+-rw-rw-rw-   0 root         (0) root         (0)      912 2024-04-10 19:53:21.000000 terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_vm.py
```

### Comparing `terrajinja-sbp-vcd-0.1.8/LICENSE` & `terrajinja-sbp-vcd-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/PKG-INFO` & `terrajinja-sbp-vcd-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.1.8
+Version: 0.1.9
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.1.8/README.md` & `terrajinja-sbp-vcd-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/setup.py` & `terrajinja-sbp-vcd-0.1.9/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 requirements = [line.strip()
           for line in open('requirements.txt').readlines()
           if line.strip() and not line.startswith('#')]
 
 readme = open('README.md').read()
 history = open('HISTORY.md').read()
-version = '0.1.8'
+version = '0.1.9'
 name= 'terrajinja-sbp-vcd'
 package_path= name.replace('-', '.')
 
 # only the cli has an entry point
 entry_points=None
 if name=='terrajinja-cli':
     entry_points={
```

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_nsxt_alb_edgegateway_service_engine_group.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/decorators.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/decorators.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/network_routed_v2.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/network_routed_v2.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_pool.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from dataclasses import dataclass
 from constructs import Construct
 from terrajinja.imports.vcd.nsxt_alb_pool import NsxtAlbPool
 from .decorators import run_once
 from .nsxt_ip_set import SbpVcdNsxtIpSet
+from ipaddress import IPv4Network, AddressValueError
 
 
 @dataclass
 class SbpLoadbalancerPool:
     scope: Construct
     destination_address_name: str
     destination_port: int
@@ -40,32 +41,41 @@
 
 
 @run_once(parameter_match=["destination_address_name", "destination_port"])
 class SbpVcdNsxtAlbPool(NsxtAlbPool):
     """Extends the original class to ensure that it only gets called once"""
 
     def __init__(self, scope: Construct, destination_address_name: str, destination_port: int,
-                 algorithm: str, persistence: str, vip_port: int, destination_address: list,
+                 algorithm: str, persistence: str, vip_port: int, destination_address: (list | str),
                  edge_gateway_id: str, id_=None, **kwargs):
 
         pool = SbpLoadbalancerPool(
             scope=scope,
             destination_address_name=destination_address_name,
             destination_port=destination_port,
             algorithm=algorithm,
             persistence=persistence,
             default_port=vip_port,
             destination_address=destination_address,
             edge_gateway_id=edge_gateway_id
         )
 
+        if isinstance(destination_address, str):
+            destination_address = [destination_address]
+
+        try:
+            IPv4Network(destination_address[0])
+            member_group_id = pool.member_group_id
+        except AddressValueError:
+            member_group_id = destination_address[0]
+
         super().__init__(
             scope=scope,
             id_=pool.name,
             name=pool.name,
             algorithm=pool.algorithm,
             persistence_profile=pool.persistence_profile,
             default_port=pool.default_port,
-            member_group_id=pool.member_group_id,
+            member_group_id=member_group_id,
             edge_gateway_id=edge_gateway_id,
             **kwargs
         )
```

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_alb_virtual_service.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_edge_loadbalancer.py`

 * *Files 19% similar despite different names*

```diff
@@ -44,9 +44,10 @@
                 scope=scope,
                 service_engine_group_id=vcd_nsxt_alb_edgegateway_service_engine_group_id,
                 edge_gateway_id=edge_gateway_id,
                 vip_name=rule.get('vip_name'),
                 pool_id=pool.id,
                 virtual_ip_address=rule.get('vip_ip'),
                 service_type=loadbalancer.get('service_type'),
-                vip_port=rule.get('vip_port')
+                vip_port=rule.get('vip_port'),
+                is_transparent_mode_enabled=loadbalancer.get('is_transparent_mode_enabled'),
             )
```

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/rde.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/rde.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/vm.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja/sbp/vcd/vm_internal_disk.py` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja/sbp/vcd/vm_internal_disk.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/PKG-INFO` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: terrajinja-sbp-vcd
-Version: 0.1.8
+Version: 0.1.9
 Summary: Terrajinja extension for automation using cdktf
 Home-page: https://gitlab/terrajinja
 Author: Terrajinja Team
 Author-email: int-terrajinja@schubergphilis.com
 License: MIT
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `terrajinja-sbp-vcd-0.1.8/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt` & `terrajinja-sbp-vcd-0.1.9/src/terrajinja_sbp_vcd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_data_vcd_catalog_vapp_template.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_catalog_vapp_template.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_data_vcd_vm_placement_policy.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_data_vcd_vm_placement_policy.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_network_routed_v2.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_network_routed_v2.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_alb_pool.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_alb_pool.py`

 * *Files 18% similar despite different names*

```diff
@@ -27,10 +27,32 @@
         has_resource(synthesized, "vcd_nsxt_alb_pool")
         has_resource(synthesized, "vcd_nsxt_ip_set")
         # we should have 1 ip sets
         has_resource_count(synthesized, "vcd_nsxt_ip_set", 1)
         # containing 3 addresses
         assert len(j['resource']['vcd_nsxt_ip_set']['NAME']['ip_addresses']) == 3
 
+    def test_resource(self, stack):
+        pool = SbpVcdNsxtAlbPool(
+            scope=stack,
+            destination_address_name="name",
+            destination_port=8080,
+            algorithm="Least connections",
+            persistence="Client IP",
+            destination_address="id_to_resource",
+            edge_gateway_id="edge_gateway_id",
+            vip_port=8080
+        )
+        # We should have gotten a formatted pool name
+        assert pool.name_input == 'NAME-8080-POOL'
+
+        synthesized = Testing.synth(stack)
+        j = json.loads(synthesized)
+        print(synthesized)
+
+        has_resource(synthesized, "vcd_nsxt_alb_pool")
+        # resource has a link to an other resource instead of ips
+        assert j['resource']['vcd_nsxt_alb_pool']['NAME-8080-POOL']['member_group_id'] == "id_to_resource"
+
 
 if __name__ == "__main__":
     pytest.main()
```

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_app_port_profile.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_app_port_profile.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_distributed_firewall.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_distributed_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_edge_firewall.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_firewall.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_edge_loadbalancer.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_firewall_rule_parser.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_ip_set.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_ip_set.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_nat_rule.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_nat_rule.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_nsxt_virtual_service.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_nsxt_virtual_service.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_rde.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_rde.py`

 * *Files identical despite different names*

### Comparing `terrajinja-sbp-vcd-0.1.8/tests/test_sbp_vcd_vm.py` & `terrajinja-sbp-vcd-0.1.9/tests/test_sbp_vcd_vm.py`

 * *Files identical despite different names*

