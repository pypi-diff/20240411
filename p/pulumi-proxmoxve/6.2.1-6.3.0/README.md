# Comparing `tmp/pulumi_proxmoxve-6.2.1.tar.gz` & `tmp/pulumi_proxmoxve-6.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_proxmoxve-6.2.1.tar", last modified: Fri Apr  5 06:20:18 2024, max compression
+gzip compressed data, was "pulumi_proxmoxve-6.3.0.tar", last modified: Thu Apr 11 12:05:16 2024, max compression
```

## Comparing `pulumi_proxmoxve-6.2.1.tar` & `pulumi_proxmoxve-6.3.0.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.576816 pulumi_proxmoxve-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-05 06:20:18.576816 pulumi_proxmoxve-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.564816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/
--rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/certifi.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.568816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/get_nodes.py
--rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.568816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/vars.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.568816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/
--rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    55933 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/container.py
--rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/dns.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.568816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/download/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/download/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/get_node.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.568816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/ha_group.py
--rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/ha_resource.py
--rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/hosts.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.572816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_alias.py
--rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_ip_set.py
--rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_options.py
--rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_rules.py
--rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_security_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_hosts.py
--rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_time.py
--rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_version.py
--rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/network_bridge.py
--rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/network_vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/outputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.572816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/
--rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_role.py
--rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/role.py
--rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.572816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/
--rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    30843 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/get_datastores.py
--rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/time.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.576816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/
--rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    84161 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/get_virtual_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/get_virtual_machines.py
--rw-r--r--   0 runner    (1001) docker     (127)    73253 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/outputs.py
--rw-r--r--   0 runner    (1001) docker     (127)   119846 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/virtual_machine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 06:20:18.564816 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 06:20:18.576816 pulumi_proxmoxve-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-05 06:20:18.000000 pulumi_proxmoxve-6.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.507322 pulumi_proxmoxve-6.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-11 12:05:16.507322 pulumi_proxmoxve-6.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6356 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.495322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/
+-rw-r--r--   0 runner    (1001) docker     (127)     5715 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10248 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22894 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/certifi.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.495322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6962 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/get_nodes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    50170 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.495322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7007 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/vars.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.495322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/
+-rw-r--r--   0 runner    (1001) docker     (127)      339 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    37038 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55933 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/container.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32232 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9231 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/dns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.499322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/download/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38162 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/download/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6328 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/get_node.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.499322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5530 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2960 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6349 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4285 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16803 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/ha_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18333 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/ha_resource.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12761 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/hosts.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.503322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25888 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15509 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16129 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_alias.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17761 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_ip_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33135 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16835 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_rules.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18078 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_security_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3784 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4934 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_hosts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4382 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4096 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24956 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/network_bridge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25357 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/network_vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22405 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/outputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.503322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/
+-rw-r--r--   0 runner    (1001) docker     (127)      593 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6185 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4355 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3270 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3857 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3403 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_role.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3726 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7017 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6567 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11621 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9837 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9200 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8481 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/role.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25681 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14153 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.503322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/
+-rw-r--r--   0 runner    (1001) docker     (127)      364 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5583 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30815 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7630 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/get_datastores.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5302 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10139 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/time.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.507322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    87552 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4579 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/get_virtual_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4575 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/get_virtual_machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75694 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   122141 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/virtual_machine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:05:16.495322 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6778 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2861 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:05:16.507322 pulumi_proxmoxve-6.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1366 2024-04-11 12:05:16.000000 pulumi_proxmoxve-6.3.0/setup.py
```

### Comparing `pulumi_proxmoxve-6.2.1/PKG-INFO` & `pulumi_proxmoxve-6.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_proxmoxve
-Version: 6.2.1
+Version: 6.3.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.2.1/README.md` & `pulumi_proxmoxve-6.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/__init__.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/_utilities.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/certifi.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/certifi.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/get_nodes.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/get_nodes.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/cluster/options.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/cluster/options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/config/vars.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/container.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ct/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ct/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/dns.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/download/file.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/download/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/get_node.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/get_node.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_group.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_groups.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_resource.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/get_ha_resources.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/get_ha_resources.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/ha_group.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/ha_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/ha/ha_resource.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/ha/ha_resource.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/hosts.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/__init__.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_alias.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_alias.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_ip_set.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_ip_set.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_options.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_options.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_rules.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_rules.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/firewall_security_group.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/firewall_security_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_dns.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_dns.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_hosts.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_hosts.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_time.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/get_version.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/get_version.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/network_bridge.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/network_bridge.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/network_vlan.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/network_vlan.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/network/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/network/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/__init__.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_group.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_groups.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_groups.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_pool.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_pools.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_pools.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_role.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_roles.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_roles.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_user.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/get_users.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/get_users.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/group.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/group.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/pool.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/role.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/role.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/permission/user.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/permission/user.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/provider.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/file.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/file.py`

 * *Files 0% similar despite different names*

```diff
@@ -351,15 +351,15 @@
         """
         Manages a file.
 
         ## Example Usage
 
         ### Backups (`dump`)
 
-        > **Note:** The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
+        > The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         backup = proxmoxve.storage.File("backup",
@@ -370,15 +370,15 @@
                 path="vzdump-lxc-100-2023_11_08-23_10_05.tar",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Images
 
-        **Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.**
+        > Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
@@ -389,15 +389,15 @@
                 path="https://cloud-images.ubuntu.com/jammy/20230929/jammy-server-cloudimg-amd64-disk-kvm.img",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Container Template (`vztmpl`)
 
-        **Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.**
+        > Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
@@ -467,15 +467,15 @@
         """
         Manages a file.
 
         ## Example Usage
 
         ### Backups (`dump`)
 
-        > **Note:** The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
+        > The resource with this content type uses SSH access to the node. You might need to configure the `ssh` option in the `provider` section.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         backup = proxmoxve.storage.File("backup",
@@ -486,15 +486,15 @@
                 path="vzdump-lxc-100-2023_11_08-23_10_05.tar",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Images
 
-        **Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.**
+        > Consider using `Download.File` resource instead. Using this resource for images is less efficient (requires to transfer uploaded image to node) though still supported.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
@@ -505,15 +505,15 @@
                 path="https://cloud-images.ubuntu.com/jammy/20230929/jammy-server-cloudimg-amd64-disk-kvm.img",
             ))
         ```
         <!--End PulumiCodeChooser -->
 
         ### Container Template (`vztmpl`)
 
-        **Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.**
+        > Consider using `Download.File` resource instead. Using this resource for container images is less efficient (requires to transfer uploaded image to node) though still supported.
 
         <!--Start PulumiCodeChooser -->
         ```python
         import pulumi
         import pulumi_proxmoxve as proxmoxve
 
         ubuntu_container_template = proxmoxve.storage.File("ubuntuContainerTemplate",
```

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/get_datastores.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/get_datastores.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/storage/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/storage/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/time.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/time.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/_inputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,14 +23,15 @@
     'VirtualMachineInitializationDnsArgs',
     'VirtualMachineInitializationIpConfigArgs',
     'VirtualMachineInitializationIpConfigIpv4Args',
     'VirtualMachineInitializationIpConfigIpv6Args',
     'VirtualMachineInitializationUserAccountArgs',
     'VirtualMachineMemoryArgs',
     'VirtualMachineNetworkDeviceArgs',
+    'VirtualMachineNumaArgs',
     'VirtualMachineOperatingSystemArgs',
     'VirtualMachineSerialDeviceArgs',
     'VirtualMachineSmbiosArgs',
     'VirtualMachineStartupArgs',
     'VirtualMachineTpmStateArgs',
     'VirtualMachineUsbArgs',
     'VirtualMachineVgaArgs',
@@ -375,15 +376,15 @@
                - `+ssbd`/`-ssbd` - Protection for "Speculative Store Bypass" for Intel
                models.
                - `+virt-ssbd`/`-virt-ssbd` - Basis for "Speculative Store Bypass"
                protection for AMD models.
         :param pulumi.Input[int] hotplugged: The number of hotplugged vCPUs (defaults
                to `0`).
         :param pulumi.Input[int] limit: Limit of CPU usage, `0...128`. (defaults to `0` -- no limit).
-        :param pulumi.Input[bool] numa: Enable/disable NUMA. (default to `false`)
+        :param pulumi.Input[bool] numa: The NUMA configuration.
         :param pulumi.Input[int] sockets: The number of CPU sockets (defaults to `1`).
         :param pulumi.Input[str] type: The VGA type (defaults to `std`).
         :param pulumi.Input[int] units: The CPU units (defaults to `1024`).
         """
         if affinity is not None:
             pulumi.set(__self__, "affinity", affinity)
         if architecture is not None:
@@ -503,15 +504,15 @@
     def limit(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "limit", value)
 
     @property
     @pulumi.getter
     def numa(self) -> Optional[pulumi.Input[bool]]:
         """
-        Enable/disable NUMA. (default to `false`)
+        The NUMA configuration.
         """
         return pulumi.get(self, "numa")
 
     @numa.setter
     def numa(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "numa", value)
 
@@ -1186,14 +1187,15 @@
                  datastore_id: Optional[pulumi.Input[str]] = None,
                  dns: Optional[pulumi.Input['VirtualMachineInitializationDnsArgs']] = None,
                  interface: Optional[pulumi.Input[str]] = None,
                  ip_configs: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineInitializationIpConfigArgs']]]] = None,
                  meta_data_file_id: Optional[pulumi.Input[str]] = None,
                  network_data_file_id: Optional[pulumi.Input[str]] = None,
                  type: Optional[pulumi.Input[str]] = None,
+                 upgrade: Optional[pulumi.Input[bool]] = None,
                  user_account: Optional[pulumi.Input['VirtualMachineInitializationUserAccountArgs']] = None,
                  user_data_file_id: Optional[pulumi.Input[str]] = None,
                  vendor_data_file_id: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
         :param pulumi.Input['VirtualMachineInitializationDnsArgs'] dns: The DNS configuration.
@@ -1205,14 +1207,15 @@
                device).
         :param pulumi.Input[str] meta_data_file_id: The identifier for a file containing
                all meta data passed to the VM via cloud-init.
         :param pulumi.Input[str] network_data_file_id: The identifier for a file containing
                network configuration data passed to the VM via cloud-init (conflicts
                with `ip_config`).
         :param pulumi.Input[str] type: The VGA type (defaults to `std`).
+        :param pulumi.Input[bool] upgrade: Whether to do an automatic package upgrade after the first boot (defaults to `true`).
         :param pulumi.Input['VirtualMachineInitializationUserAccountArgs'] user_account: The user account configuration (conflicts
                with `user_data_file_id`).
         :param pulumi.Input[str] user_data_file_id: The identifier for a file containing
                custom user data (conflicts with `user_account`).
         :param pulumi.Input[str] vendor_data_file_id: The identifier for a file containing
                all vendor data passed to the VM via cloud-init.
         """
@@ -1226,14 +1229,16 @@
             pulumi.set(__self__, "ip_configs", ip_configs)
         if meta_data_file_id is not None:
             pulumi.set(__self__, "meta_data_file_id", meta_data_file_id)
         if network_data_file_id is not None:
             pulumi.set(__self__, "network_data_file_id", network_data_file_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
+        if upgrade is not None:
+            pulumi.set(__self__, "upgrade", upgrade)
         if user_account is not None:
             pulumi.set(__self__, "user_account", user_account)
         if user_data_file_id is not None:
             pulumi.set(__self__, "user_data_file_id", user_data_file_id)
         if vendor_data_file_id is not None:
             pulumi.set(__self__, "vendor_data_file_id", vendor_data_file_id)
 
@@ -1326,14 +1331,26 @@
         return pulumi.get(self, "type")
 
     @type.setter
     def type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "type", value)
 
     @property
+    @pulumi.getter
+    def upgrade(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether to do an automatic package upgrade after the first boot (defaults to `true`).
+        """
+        return pulumi.get(self, "upgrade")
+
+    @upgrade.setter
+    def upgrade(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "upgrade", value)
+
+    @property
     @pulumi.getter(name="userAccount")
     def user_account(self) -> Optional[pulumi.Input['VirtualMachineInitializationUserAccountArgs']]:
         """
         The user account configuration (conflicts
         with `user_data_file_id`).
         """
         return pulumi.get(self, "user_account")
@@ -1903,14 +1920,100 @@
 
     @vlan_id.setter
     def vlan_id(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "vlan_id", value)
 
 
 @pulumi.input_type
+class VirtualMachineNumaArgs:
+    def __init__(__self__, *,
+                 cpus: pulumi.Input[str],
+                 device: pulumi.Input[str],
+                 memory: pulumi.Input[int],
+                 hostnodes: Optional[pulumi.Input[str]] = None,
+                 policy: Optional[pulumi.Input[str]] = None):
+        """
+        :param pulumi.Input[str] cpus: The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
+        :param pulumi.Input[str] device: The device (defaults to `socket`).
+               - `/dev/*` - A host serial device.
+        :param pulumi.Input[int] memory: The VGA memory in megabytes (defaults to `16`).
+        :param pulumi.Input[str] hostnodes: The NUMA host nodes.
+        :param pulumi.Input[str] policy: The NUMA policy (defaults to `preferred`).
+        """
+        pulumi.set(__self__, "cpus", cpus)
+        pulumi.set(__self__, "device", device)
+        pulumi.set(__self__, "memory", memory)
+        if hostnodes is not None:
+            pulumi.set(__self__, "hostnodes", hostnodes)
+        if policy is not None:
+            pulumi.set(__self__, "policy", policy)
+
+    @property
+    @pulumi.getter
+    def cpus(self) -> pulumi.Input[str]:
+        """
+        The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
+        """
+        return pulumi.get(self, "cpus")
+
+    @cpus.setter
+    def cpus(self, value: pulumi.Input[str]):
+        pulumi.set(self, "cpus", value)
+
+    @property
+    @pulumi.getter
+    def device(self) -> pulumi.Input[str]:
+        """
+        The device (defaults to `socket`).
+        - `/dev/*` - A host serial device.
+        """
+        return pulumi.get(self, "device")
+
+    @device.setter
+    def device(self, value: pulumi.Input[str]):
+        pulumi.set(self, "device", value)
+
+    @property
+    @pulumi.getter
+    def memory(self) -> pulumi.Input[int]:
+        """
+        The VGA memory in megabytes (defaults to `16`).
+        """
+        return pulumi.get(self, "memory")
+
+    @memory.setter
+    def memory(self, value: pulumi.Input[int]):
+        pulumi.set(self, "memory", value)
+
+    @property
+    @pulumi.getter
+    def hostnodes(self) -> Optional[pulumi.Input[str]]:
+        """
+        The NUMA host nodes.
+        """
+        return pulumi.get(self, "hostnodes")
+
+    @hostnodes.setter
+    def hostnodes(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "hostnodes", value)
+
+    @property
+    @pulumi.getter
+    def policy(self) -> Optional[pulumi.Input[str]]:
+        """
+        The NUMA policy (defaults to `preferred`).
+        """
+        return pulumi.get(self, "policy")
+
+    @policy.setter
+    def policy(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "policy", value)
+
+
+@pulumi.input_type
 class VirtualMachineOperatingSystemArgs:
     def __init__(__self__, *,
                  type: Optional[pulumi.Input[str]] = None):
         """
         :param pulumi.Input[str] type: The VGA type (defaults to `std`).
         """
         if type is not None:
```

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/get_virtual_machine.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/get_virtual_machine.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/get_virtual_machines.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/get_virtual_machines.py`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/outputs.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/outputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     'VirtualMachineInitializationDns',
     'VirtualMachineInitializationIpConfig',
     'VirtualMachineInitializationIpConfigIpv4',
     'VirtualMachineInitializationIpConfigIpv6',
     'VirtualMachineInitializationUserAccount',
     'VirtualMachineMemory',
     'VirtualMachineNetworkDevice',
+    'VirtualMachineNuma',
     'VirtualMachineOperatingSystem',
     'VirtualMachineSerialDevice',
     'VirtualMachineSmbios',
     'VirtualMachineStartup',
     'VirtualMachineTpmState',
     'VirtualMachineUsb',
     'VirtualMachineVga',
@@ -355,15 +356,15 @@
                - `+ssbd`/`-ssbd` - Protection for "Speculative Store Bypass" for Intel
                models.
                - `+virt-ssbd`/`-virt-ssbd` - Basis for "Speculative Store Bypass"
                protection for AMD models.
         :param int hotplugged: The number of hotplugged vCPUs (defaults
                to `0`).
         :param int limit: Limit of CPU usage, `0...128`. (defaults to `0` -- no limit).
-        :param bool numa: Enable/disable NUMA. (default to `false`)
+        :param bool numa: The NUMA configuration.
         :param int sockets: The number of CPU sockets (defaults to `1`).
         :param str type: The VGA type (defaults to `std`).
         :param int units: The CPU units (defaults to `1024`).
         """
         if affinity is not None:
             pulumi.set(__self__, "affinity", affinity)
         if architecture is not None:
@@ -459,15 +460,15 @@
         """
         return pulumi.get(self, "limit")
 
     @property
     @pulumi.getter
     def numa(self) -> Optional[bool]:
         """
-        Enable/disable NUMA. (default to `false`)
+        The NUMA configuration.
         """
         return pulumi.get(self, "numa")
 
     @property
     @pulumi.getter
     def sockets(self) -> Optional[int]:
         """
@@ -1107,14 +1108,15 @@
                  datastore_id: Optional[str] = None,
                  dns: Optional['outputs.VirtualMachineInitializationDns'] = None,
                  interface: Optional[str] = None,
                  ip_configs: Optional[Sequence['outputs.VirtualMachineInitializationIpConfig']] = None,
                  meta_data_file_id: Optional[str] = None,
                  network_data_file_id: Optional[str] = None,
                  type: Optional[str] = None,
+                 upgrade: Optional[bool] = None,
                  user_account: Optional['outputs.VirtualMachineInitializationUserAccount'] = None,
                  user_data_file_id: Optional[str] = None,
                  vendor_data_file_id: Optional[str] = None):
         """
         :param str datastore_id: The identifier for the datastore to create the
                cloud-init disk in (defaults to `local-lvm`).
         :param 'VirtualMachineInitializationDnsArgs' dns: The DNS configuration.
@@ -1126,14 +1128,15 @@
                device).
         :param str meta_data_file_id: The identifier for a file containing
                all meta data passed to the VM via cloud-init.
         :param str network_data_file_id: The identifier for a file containing
                network configuration data passed to the VM via cloud-init (conflicts
                with `ip_config`).
         :param str type: The VGA type (defaults to `std`).
+        :param bool upgrade: Whether to do an automatic package upgrade after the first boot (defaults to `true`).
         :param 'VirtualMachineInitializationUserAccountArgs' user_account: The user account configuration (conflicts
                with `user_data_file_id`).
         :param str user_data_file_id: The identifier for a file containing
                custom user data (conflicts with `user_account`).
         :param str vendor_data_file_id: The identifier for a file containing
                all vendor data passed to the VM via cloud-init.
         """
@@ -1147,14 +1150,16 @@
             pulumi.set(__self__, "ip_configs", ip_configs)
         if meta_data_file_id is not None:
             pulumi.set(__self__, "meta_data_file_id", meta_data_file_id)
         if network_data_file_id is not None:
             pulumi.set(__self__, "network_data_file_id", network_data_file_id)
         if type is not None:
             pulumi.set(__self__, "type", type)
+        if upgrade is not None:
+            pulumi.set(__self__, "upgrade", upgrade)
         if user_account is not None:
             pulumi.set(__self__, "user_account", user_account)
         if user_data_file_id is not None:
             pulumi.set(__self__, "user_data_file_id", user_data_file_id)
         if vendor_data_file_id is not None:
             pulumi.set(__self__, "vendor_data_file_id", vendor_data_file_id)
 
@@ -1219,14 +1224,22 @@
     def type(self) -> Optional[str]:
         """
         The VGA type (defaults to `std`).
         """
         return pulumi.get(self, "type")
 
     @property
+    @pulumi.getter
+    def upgrade(self) -> Optional[bool]:
+        """
+        Whether to do an automatic package upgrade after the first boot (defaults to `true`).
+        """
+        return pulumi.get(self, "upgrade")
+
+    @property
     @pulumi.getter(name="userAccount")
     def user_account(self) -> Optional['outputs.VirtualMachineInitializationUserAccount']:
         """
         The user account configuration (conflicts
         with `user_data_file_id`).
         """
         return pulumi.get(self, "user_account")
@@ -1707,14 +1720,80 @@
         """
         The VLAN identifier.
         """
         return pulumi.get(self, "vlan_id")
 
 
 @pulumi.output_type
+class VirtualMachineNuma(dict):
+    def __init__(__self__, *,
+                 cpus: str,
+                 device: str,
+                 memory: int,
+                 hostnodes: Optional[str] = None,
+                 policy: Optional[str] = None):
+        """
+        :param str cpus: The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
+        :param str device: The device (defaults to `socket`).
+               - `/dev/*` - A host serial device.
+        :param int memory: The VGA memory in megabytes (defaults to `16`).
+        :param str hostnodes: The NUMA host nodes.
+        :param str policy: The NUMA policy (defaults to `preferred`).
+        """
+        pulumi.set(__self__, "cpus", cpus)
+        pulumi.set(__self__, "device", device)
+        pulumi.set(__self__, "memory", memory)
+        if hostnodes is not None:
+            pulumi.set(__self__, "hostnodes", hostnodes)
+        if policy is not None:
+            pulumi.set(__self__, "policy", policy)
+
+    @property
+    @pulumi.getter
+    def cpus(self) -> str:
+        """
+        The CPU cores to assign to the NUMA node (format is `0-7;16-31`).
+        """
+        return pulumi.get(self, "cpus")
+
+    @property
+    @pulumi.getter
+    def device(self) -> str:
+        """
+        The device (defaults to `socket`).
+        - `/dev/*` - A host serial device.
+        """
+        return pulumi.get(self, "device")
+
+    @property
+    @pulumi.getter
+    def memory(self) -> int:
+        """
+        The VGA memory in megabytes (defaults to `16`).
+        """
+        return pulumi.get(self, "memory")
+
+    @property
+    @pulumi.getter
+    def hostnodes(self) -> Optional[str]:
+        """
+        The NUMA host nodes.
+        """
+        return pulumi.get(self, "hostnodes")
+
+    @property
+    @pulumi.getter
+    def policy(self) -> Optional[str]:
+        """
+        The NUMA policy (defaults to `preferred`).
+        """
+        return pulumi.get(self, "policy")
+
+
+@pulumi.output_type
 class VirtualMachineOperatingSystem(dict):
     def __init__(__self__, *,
                  type: Optional[str] = None):
         """
         :param str type: The VGA type (defaults to `std`).
         """
         if type is not None:
```

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve/vm/virtual_machine.py` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve/vm/virtual_machine.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,14 +35,15 @@
                  kvm_arguments: Optional[pulumi.Input[str]] = None,
                  mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input['VirtualMachineMemoryArgs']] = None,
                  migrate: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_devices: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]]] = None,
+                 numas: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]] = None,
                  on_boot: Optional[pulumi.Input[bool]] = None,
                  operating_system: Optional[pulumi.Input['VirtualMachineOperatingSystemArgs']] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protection: Optional[pulumi.Input[bool]] = None,
                  reboot: Optional[pulumi.Input[bool]] = None,
                  scsi_hardware: Optional[pulumi.Input[str]] = None,
                  serial_devices: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineSerialDeviceArgs']]]] = None,
@@ -91,14 +92,15 @@
                to the network device configuration, if the agent is disabled
         :param pulumi.Input[str] machine: The VM machine type (defaults to `pc`).
         :param pulumi.Input['VirtualMachineMemoryArgs'] memory: The VGA memory in megabytes (defaults to `16`).
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]] network_devices: A network device (multiple blocks supported).
+        :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]] numas: The NUMA configuration.
         :param pulumi.Input[bool] on_boot: Specifies whether a VM will be started during system
                boot. (defaults to `true`)
         :param pulumi.Input['VirtualMachineOperatingSystemArgs'] operating_system: The Operating System configuration.
         :param pulumi.Input[str] pool_id: The identifier for a pool to assign the virtual machine to.
         :param pulumi.Input[bool] protection: Sets the protection flag of the VM. This will disable the remove VM and remove disk operations (defaults to `false`).
         :param pulumi.Input[bool] reboot: Reboot the VM after initial creation. (defaults to `false`)
         :param pulumi.Input[str] scsi_hardware: The SCSI hardware type (defaults to
@@ -179,14 +181,16 @@
             pulumi.set(__self__, "memory", memory)
         if migrate is not None:
             pulumi.set(__self__, "migrate", migrate)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if network_devices is not None:
             pulumi.set(__self__, "network_devices", network_devices)
+        if numas is not None:
+            pulumi.set(__self__, "numas", numas)
         if on_boot is not None:
             pulumi.set(__self__, "on_boot", on_boot)
         if operating_system is not None:
             pulumi.set(__self__, "operating_system", operating_system)
         if pool_id is not None:
             pulumi.set(__self__, "pool_id", pool_id)
         if protection is not None:
@@ -514,14 +518,26 @@
         return pulumi.get(self, "network_devices")
 
     @network_devices.setter
     def network_devices(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]]]):
         pulumi.set(self, "network_devices", value)
 
     @property
+    @pulumi.getter
+    def numas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]]:
+        """
+        The NUMA configuration.
+        """
+        return pulumi.get(self, "numas")
+
+    @numas.setter
+    def numas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]]):
+        pulumi.set(self, "numas", value)
+
+    @property
     @pulumi.getter(name="onBoot")
     def on_boot(self) -> Optional[pulumi.Input[bool]]:
         """
         Specifies whether a VM will be started during system
         boot. (defaults to `true`)
         """
         return pulumi.get(self, "on_boot")
@@ -871,14 +887,15 @@
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input['VirtualMachineMemoryArgs']] = None,
                  migrate: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_devices: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]]] = None,
                  network_interface_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 numas: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]] = None,
                  on_boot: Optional[pulumi.Input[bool]] = None,
                  operating_system: Optional[pulumi.Input['VirtualMachineOperatingSystemArgs']] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protection: Optional[pulumi.Input[bool]] = None,
                  reboot: Optional[pulumi.Input[bool]] = None,
                  scsi_hardware: Optional[pulumi.Input[str]] = None,
                  serial_devices: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineSerialDeviceArgs']]]] = None,
@@ -933,14 +950,15 @@
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNetworkDeviceArgs']]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_interface_names: The network interface names published by the QEMU
                agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
                to.
+        :param pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]] numas: The NUMA configuration.
         :param pulumi.Input[bool] on_boot: Specifies whether a VM will be started during system
                boot. (defaults to `true`)
         :param pulumi.Input['VirtualMachineOperatingSystemArgs'] operating_system: The Operating System configuration.
         :param pulumi.Input[str] pool_id: The identifier for a pool to assign the virtual machine to.
         :param pulumi.Input[bool] protection: Sets the protection flag of the VM. This will disable the remove VM and remove disk operations (defaults to `false`).
         :param pulumi.Input[bool] reboot: Reboot the VM after initial creation. (defaults to `false`)
         :param pulumi.Input[str] scsi_hardware: The SCSI hardware type (defaults to
@@ -1028,14 +1046,16 @@
             pulumi.set(__self__, "name", name)
         if network_devices is not None:
             pulumi.set(__self__, "network_devices", network_devices)
         if network_interface_names is not None:
             pulumi.set(__self__, "network_interface_names", network_interface_names)
         if node_name is not None:
             pulumi.set(__self__, "node_name", node_name)
+        if numas is not None:
+            pulumi.set(__self__, "numas", numas)
         if on_boot is not None:
             pulumi.set(__self__, "on_boot", on_boot)
         if operating_system is not None:
             pulumi.set(__self__, "operating_system", operating_system)
         if pool_id is not None:
             pulumi.set(__self__, "pool_id", pool_id)
         if protection is not None:
@@ -1402,14 +1422,26 @@
         return pulumi.get(self, "node_name")
 
     @node_name.setter
     def node_name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "node_name", value)
 
     @property
+    @pulumi.getter
+    def numas(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]]:
+        """
+        The NUMA configuration.
+        """
+        return pulumi.get(self, "numas")
+
+    @numas.setter
+    def numas(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['VirtualMachineNumaArgs']]]]):
+        pulumi.set(self, "numas", value)
+
+    @property
     @pulumi.getter(name="onBoot")
     def on_boot(self) -> Optional[pulumi.Input[bool]]:
         """
         Specifies whether a VM will be started during system
         boot. (defaults to `true`)
         """
         return pulumi.get(self, "on_boot")
@@ -1758,14 +1790,15 @@
                  mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']]] = None,
                  migrate: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 numas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]]] = None,
                  on_boot: Optional[pulumi.Input[bool]] = None,
                  operating_system: Optional[pulumi.Input[pulumi.InputType['VirtualMachineOperatingSystemArgs']]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protection: Optional[pulumi.Input[bool]] = None,
                  reboot: Optional[pulumi.Input[bool]] = None,
                  scsi_hardware: Optional[pulumi.Input[str]] = None,
                  serial_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineSerialDeviceArgs']]]]] = None,
@@ -1830,14 +1863,15 @@
         :param pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']] memory: The VGA memory in megabytes (defaults to `16`).
         :param pulumi.Input[bool] migrate: Migrate the VM on node change instead of re-creating
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
                to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]] numas: The NUMA configuration.
         :param pulumi.Input[bool] on_boot: Specifies whether a VM will be started during system
                boot. (defaults to `true`)
         :param pulumi.Input[pulumi.InputType['VirtualMachineOperatingSystemArgs']] operating_system: The Operating System configuration.
         :param pulumi.Input[str] pool_id: The identifier for a pool to assign the virtual machine to.
         :param pulumi.Input[bool] protection: Sets the protection flag of the VM. This will disable the remove VM and remove disk operations (defaults to `false`).
         :param pulumi.Input[bool] reboot: Reboot the VM after initial creation. (defaults to `false`)
         :param pulumi.Input[str] scsi_hardware: The SCSI hardware type (defaults to
@@ -1932,14 +1966,15 @@
                  mac_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  machine: Optional[pulumi.Input[str]] = None,
                  memory: Optional[pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']]] = None,
                  migrate: Optional[pulumi.Input[bool]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  network_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]]] = None,
                  node_name: Optional[pulumi.Input[str]] = None,
+                 numas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]]] = None,
                  on_boot: Optional[pulumi.Input[bool]] = None,
                  operating_system: Optional[pulumi.Input[pulumi.InputType['VirtualMachineOperatingSystemArgs']]] = None,
                  pool_id: Optional[pulumi.Input[str]] = None,
                  protection: Optional[pulumi.Input[bool]] = None,
                  reboot: Optional[pulumi.Input[bool]] = None,
                  scsi_hardware: Optional[pulumi.Input[str]] = None,
                  serial_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineSerialDeviceArgs']]]]] = None,
@@ -1992,14 +2027,15 @@
             __props__.__dict__["memory"] = memory
             __props__.__dict__["migrate"] = migrate
             __props__.__dict__["name"] = name
             __props__.__dict__["network_devices"] = network_devices
             if node_name is None and not opts.urn:
                 raise TypeError("Missing required property 'node_name'")
             __props__.__dict__["node_name"] = node_name
+            __props__.__dict__["numas"] = numas
             __props__.__dict__["on_boot"] = on_boot
             __props__.__dict__["operating_system"] = operating_system
             __props__.__dict__["pool_id"] = pool_id
             __props__.__dict__["protection"] = protection
             __props__.__dict__["reboot"] = reboot
             __props__.__dict__["scsi_hardware"] = scsi_hardware
             __props__.__dict__["serial_devices"] = serial_devices
@@ -2057,14 +2093,15 @@
             machine: Optional[pulumi.Input[str]] = None,
             memory: Optional[pulumi.Input[pulumi.InputType['VirtualMachineMemoryArgs']]] = None,
             migrate: Optional[pulumi.Input[bool]] = None,
             name: Optional[pulumi.Input[str]] = None,
             network_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]]] = None,
             network_interface_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
             node_name: Optional[pulumi.Input[str]] = None,
+            numas: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]]] = None,
             on_boot: Optional[pulumi.Input[bool]] = None,
             operating_system: Optional[pulumi.Input[pulumi.InputType['VirtualMachineOperatingSystemArgs']]] = None,
             pool_id: Optional[pulumi.Input[str]] = None,
             protection: Optional[pulumi.Input[bool]] = None,
             reboot: Optional[pulumi.Input[bool]] = None,
             scsi_hardware: Optional[pulumi.Input[str]] = None,
             serial_devices: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineSerialDeviceArgs']]]]] = None,
@@ -2124,14 +2161,15 @@
                it (defaults to `false`).
         :param pulumi.Input[str] name: The virtual machine name.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNetworkDeviceArgs']]]] network_devices: A network device (multiple blocks supported).
         :param pulumi.Input[Sequence[pulumi.Input[str]]] network_interface_names: The network interface names published by the QEMU
                agent (empty list when `agent.enabled` is `false`)
         :param pulumi.Input[str] node_name: The name of the node to assign the virtual machine
                to.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['VirtualMachineNumaArgs']]]] numas: The NUMA configuration.
         :param pulumi.Input[bool] on_boot: Specifies whether a VM will be started during system
                boot. (defaults to `true`)
         :param pulumi.Input[pulumi.InputType['VirtualMachineOperatingSystemArgs']] operating_system: The Operating System configuration.
         :param pulumi.Input[str] pool_id: The identifier for a pool to assign the virtual machine to.
         :param pulumi.Input[bool] protection: Sets the protection flag of the VM. This will disable the remove VM and remove disk operations (defaults to `false`).
         :param pulumi.Input[bool] reboot: Reboot the VM after initial creation. (defaults to `false`)
         :param pulumi.Input[str] scsi_hardware: The SCSI hardware type (defaults to
@@ -2197,14 +2235,15 @@
         __props__.__dict__["machine"] = machine
         __props__.__dict__["memory"] = memory
         __props__.__dict__["migrate"] = migrate
         __props__.__dict__["name"] = name
         __props__.__dict__["network_devices"] = network_devices
         __props__.__dict__["network_interface_names"] = network_interface_names
         __props__.__dict__["node_name"] = node_name
+        __props__.__dict__["numas"] = numas
         __props__.__dict__["on_boot"] = on_boot
         __props__.__dict__["operating_system"] = operating_system
         __props__.__dict__["pool_id"] = pool_id
         __props__.__dict__["protection"] = protection
         __props__.__dict__["reboot"] = reboot
         __props__.__dict__["scsi_hardware"] = scsi_hardware
         __props__.__dict__["serial_devices"] = serial_devices
@@ -2442,14 +2481,22 @@
         """
         The name of the node to assign the virtual machine
         to.
         """
         return pulumi.get(self, "node_name")
 
     @property
+    @pulumi.getter
+    def numas(self) -> pulumi.Output[Optional[Sequence['outputs.VirtualMachineNuma']]]:
+        """
+        The NUMA configuration.
+        """
+        return pulumi.get(self, "numas")
+
+    @property
     @pulumi.getter(name="onBoot")
     def on_boot(self) -> pulumi.Output[Optional[bool]]:
         """
         Specifies whether a VM will be started during system
         boot. (defaults to `true`)
         """
         return pulumi.get(self, "on_boot")
```

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/PKG-INFO` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-proxmoxve
-Version: 6.2.1
+Version: 6.3.0
 Summary: A Pulumi package for creating and managing Proxmox Virtual Environment cloud resources.
 Home-page: https://github.com/muhlba91/pulumi-proxmoxve
 License: Apache-2.0
 Project-URL: Repository, https://github.com/muhlba91/pulumi-proxmoxve
 Keywords: pulumi proxmox proxmoxve
 Platform: UNKNOWN
 Requires-Python: >=3.8
```

### Comparing `pulumi_proxmoxve-6.2.1/pulumi_proxmoxve.egg-info/SOURCES.txt` & `pulumi_proxmoxve-6.3.0/pulumi_proxmoxve.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_proxmoxve-6.2.1/setup.py` & `pulumi_proxmoxve-6.3.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "6.2.1"
+VERSION = "6.3.0"
 def readme():
     try:
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "proxmoxve Pulumi Package - Development Version"
```

