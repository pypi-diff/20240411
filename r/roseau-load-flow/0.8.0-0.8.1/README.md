# Comparing `tmp/roseau_load_flow-0.8.0.tar.gz` & `tmp/roseau_load_flow-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "roseau_load_flow-0.8.0.tar", max compression
+gzip compressed data, was "roseau_load_flow-0.8.1.tar", max compression
```

## Comparing `roseau_load_flow-0.8.0.tar` & `roseau_load_flow-0.8.1.tar`

### file list

```diff
@@ -1,124 +1,124 @@
--rw-r--r--   0        0        0     1506 2024-01-24 09:03:05.866361 roseau_load_flow-0.8.0/LICENSE.md
--rw-r--r--   0        0        0     2600 2024-03-19 14:17:40.264738 roseau_load_flow-0.8.0/README.md
--rw-r--r--   0        0        0     3895 2024-03-19 14:26:07.012538 roseau_load_flow-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      605 2024-01-24 09:03:07.250351 roseau_load_flow-0.8.0/roseau/load_flow/__about__.py
--rw-r--r--   0        0        0     2191 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/__init__.py
--rw-r--r--   0        0        0     1541 2024-01-24 09:03:07.250351 roseau_load_flow-0.8.0/roseau/load_flow/_compat.py
--rw-r--r--   0        0        0     8308 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/_solvers.py
--rw-r--r--   0        0        0     5525 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/_wrapper.py
--rw-r--r--   0        0        0     6865 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/converters.py
--rw-r--r--   0        0        0    22124 2024-01-24 09:03:07.254351 roseau_load_flow-0.8.0/roseau/load_flow/data/lines/Catalogue.csv
--rw-r--r--   0        0        0     7873 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/Catalogue.json
--rw-r--r--   0        0        0    12124 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder00939_Summer.json
--rw-r--r--   0        0        0    12121 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder00939_Winter.json
--rw-r--r--   0        0        0     9884 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder02639_Summer.json
--rw-r--r--   0        0        0     9880 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder02639_Winter.json
--rw-r--r--   0        0        0     7216 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder04790_Summer.json
--rw-r--r--   0        0        0     7215 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder04790_Winter.json
--rw-r--r--   0        0        0     4421 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06713_Summer.json
--rw-r--r--   0        0        0     4419 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06713_Winter.json
--rw-r--r--   0        0        0     4465 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06926_Summer.json
--rw-r--r--   0        0        0     4463 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06926_Winter.json
--rw-r--r--   0        0        0     8610 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06975_Summer.json
--rw-r--r--   0        0        0     8606 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06975_Winter.json
--rw-r--r--   0        0        0    27812 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18498_Summer.json
--rw-r--r--   0        0        0    27802 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18498_Winter.json
--rw-r--r--   0        0        0    10602 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18769_Summer.json
--rw-r--r--   0        0        0    10599 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18769_Winter.json
--rw-r--r--   0        0        0     4678 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder19558_Summer.json
--rw-r--r--   0        0        0     4675 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder19558_Winter.json
--rw-r--r--   0        0        0    11264 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder20256_Summer.json
--rw-r--r--   0        0        0    11268 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder20256_Winter.json
--rw-r--r--   0        0        0     4657 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder23832_Summer.json
--rw-r--r--   0        0        0     4655 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder23832_Winter.json
--rw-r--r--   0        0        0     5613 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder24400_Summer.json
--rw-r--r--   0        0        0     5612 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder24400_Winter.json
--rw-r--r--   0        0        0    16899 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27429_Summer.json
--rw-r--r--   0        0        0    16890 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27429_Winter.json
--rw-r--r--   0        0        0     4475 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27681_Summer.json
--rw-r--r--   0        0        0     4476 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27681_Winter.json
--rw-r--r--   0        0        0    12891 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder30216_Summer.json
--rw-r--r--   0        0        0    12883 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder30216_Winter.json
--rw-r--r--   0        0        0     6254 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder31441_Summer.json
--rw-r--r--   0        0        0     6252 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder31441_Winter.json
--rw-r--r--   0        0        0     6922 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36284_Summer.json
--rw-r--r--   0        0        0     6924 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36284_Winter.json
--rw-r--r--   0        0        0    13353 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36360_Summer.json
--rw-r--r--   0        0        0    13345 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36360_Winter.json
--rw-r--r--   0        0        0     4775 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder37263_Summer.json
--rw-r--r--   0        0        0     4773 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder37263_Winter.json
--rw-r--r--   0        0        0     7998 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder38211_Summer.json
--rw-r--r--   0        0        0     7989 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder38211_Winter.json
--rw-r--r--   0        0        0    19166 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder004_Summer.json
--rw-r--r--   0        0        0    19142 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder004_Winter.json
--rw-r--r--   0        0        0    78312 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder011_Summer.json
--rw-r--r--   0        0        0    78090 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder011_Winter.json
--rw-r--r--   0        0        0    35712 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder015_Summer.json
--rw-r--r--   0        0        0    35661 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder015_Winter.json
--rw-r--r--   0        0        0    61840 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder032_Summer.json
--rw-r--r--   0        0        0    61912 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder032_Winter.json
--rw-r--r--   0        0        0    95006 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder041_Summer.json
--rw-r--r--   0        0        0    95105 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder041_Winter.json
--rw-r--r--   0        0        0    47638 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder063_Summer.json
--rw-r--r--   0        0        0    47572 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder063_Winter.json
--rw-r--r--   0        0        0    89894 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder078_Summer.json
--rw-r--r--   0        0        0    89717 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder078_Winter.json
--rw-r--r--   0        0        0    12151 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder115_Summer.json
--rw-r--r--   0        0        0    12130 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder115_Winter.json
--rw-r--r--   0        0        0    81931 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder128_Summer.json
--rw-r--r--   0        0        0    81943 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder128_Winter.json
--rw-r--r--   0        0        0    63043 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder151_Summer.json
--rw-r--r--   0        0        0    63061 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder151_Winter.json
--rw-r--r--   0        0        0     8776 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder159_Summer.json
--rw-r--r--   0        0        0     8776 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder159_Winter.json
--rw-r--r--   0        0        0    34801 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder176_Summer.json
--rw-r--r--   0        0        0    34723 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder176_Winter.json
--rw-r--r--   0        0        0   146325 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder210_Summer.json
--rw-r--r--   0        0        0   146163 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder210_Winter.json
--rw-r--r--   0        0        0    91949 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder217_Summer.json
--rw-r--r--   0        0        0    91835 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder217_Winter.json
--rw-r--r--   0        0        0    68046 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder232_Summer.json
--rw-r--r--   0        0        0    68004 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder232_Winter.json
--rw-r--r--   0        0        0   153496 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder251_Summer.json
--rw-r--r--   0        0        0   153340 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder251_Winter.json
--rw-r--r--   0        0        0    17398 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder290_Summer.json
--rw-r--r--   0        0        0    17326 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder290_Winter.json
--rw-r--r--   0        0        0    20701 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder312_Summer.json
--rw-r--r--   0        0        0    20677 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder312_Winter.json
--rw-r--r--   0        0        0    23624 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder320_Summer.json
--rw-r--r--   0        0        0    23606 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder320_Winter.json
--rw-r--r--   0        0        0    42014 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder339_Summer.json
--rw-r--r--   0        0        0    41888 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder339_Winter.json
--rw-r--r--   0        0        0    18419 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/data/transformers/Catalogue.csv
--rw-r--r--   0        0        0     3743 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/exceptions.py
--rw-r--r--   0        0        0      465 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/io/__init__.py
--rw-r--r--   0        0        0    15183 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/io/dgs.py
--rw-r--r--   0        0        0    18718 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/io/dict.py
--rw-r--r--   0        0        0     3505 2024-02-08 15:27:07.859968 roseau_load_flow-0.8.0/roseau/load_flow/license.py
--rw-r--r--   0        0        0     1330 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/__init__.py
--rw-r--r--   0        0        0     7282 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/branches.py
--rw-r--r--   0        0        0    18665 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/buses.py
--rw-r--r--   0        0        0     7412 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/core.py
--rw-r--r--   0        0        0     4762 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/grounds.py
--rw-r--r--   0        0        0      177 2023-02-21 17:58:50.482091 roseau_load_flow-0.8.0/roseau/load_flow/models/lines/__init__.py
--rw-r--r--   0        0        0    18432 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/lines/lines.py
--rw-r--r--   0        0        0    42770 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/lines/parameters.py
--rw-r--r--   0        0        0      351 2023-02-21 17:58:50.482091 roseau_load_flow-0.8.0/roseau/load_flow/models/loads/__init__.py
--rw-r--r--   0        0        0    56917 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/loads/flexible_parameters.py
--rw-r--r--   0        0        0    21837 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/loads/loads.py
--rw-r--r--   0        0        0     5239 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/potential_refs.py
--rw-r--r--   0        0        0     8495 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.0/roseau/load_flow/models/sources.py
--rw-r--r--   0        0        0      219 2023-02-21 17:58:50.486091 roseau_load_flow-0.8.0/roseau/load_flow/models/transformers/__init__.py
--rw-r--r--   0        0        0    21429 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/models/transformers/parameters.py
--rw-r--r--   0        0        0    14347 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/models/transformers/transformers.py
--rw-r--r--   0        0        0    71608 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/network.py
--rw-r--r--   0        0        0     2737 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/typing.py
--rw-r--r--   0        0        0     1917 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/units.py
--rw-r--r--   0        0        0      855 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/utils/__init__.py
--rw-r--r--   0        0        0     1357 2023-11-29 10:46:50.086602 roseau_load_flow-0.8.0/roseau/load_flow/utils/_optional_deps.py
--rw-r--r--   0        0        0     1185 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.0/roseau/load_flow/utils/_versions.py
--rw-r--r--   0        0        0     2768 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.0/roseau/load_flow/utils/constants.py
--rw-r--r--   0        0        0      600 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.0/roseau/load_flow/utils/log.py
--rw-r--r--   0        0        0    12581 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/utils/mixins.py
--rw-r--r--   0        0        0     6016 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.0/roseau/load_flow/utils/types.py
--rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 roseau_load_flow-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1506 2024-01-24 09:03:05.866361 roseau_load_flow-0.8.1/LICENSE.md
+-rw-r--r--   0        0        0     2600 2024-04-11 16:24:32.969372 roseau_load_flow-0.8.1/README.md
+-rw-r--r--   0        0        0     3987 2024-04-11 16:24:32.993372 roseau_load_flow-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      669 2024-04-11 16:24:32.993372 roseau_load_flow-0.8.1/roseau/load_flow/__about__.py
+-rw-r--r--   0        0        0     2191 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/__init__.py
+-rw-r--r--   0        0        0     1541 2024-01-24 09:03:07.250351 roseau_load_flow-0.8.1/roseau/load_flow/_compat.py
+-rw-r--r--   0        0        0     8308 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/_solvers.py
+-rw-r--r--   0        0        0     5525 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/_wrapper.py
+-rw-r--r--   0        0        0     6865 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/converters.py
+-rw-r--r--   0        0        0    22124 2024-01-24 09:03:07.254351 roseau_load_flow-0.8.1/roseau/load_flow/data/lines/Catalogue.csv
+-rw-r--r--   0        0        0     7873 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/Catalogue.json
+-rw-r--r--   0        0        0    12124 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder00939_Summer.json
+-rw-r--r--   0        0        0    12121 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder00939_Winter.json
+-rw-r--r--   0        0        0     9884 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder02639_Summer.json
+-rw-r--r--   0        0        0     9880 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder02639_Winter.json
+-rw-r--r--   0        0        0     7216 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder04790_Summer.json
+-rw-r--r--   0        0        0     7215 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder04790_Winter.json
+-rw-r--r--   0        0        0     4421 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06713_Summer.json
+-rw-r--r--   0        0        0     4419 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06713_Winter.json
+-rw-r--r--   0        0        0     4465 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06926_Summer.json
+-rw-r--r--   0        0        0     4463 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06926_Winter.json
+-rw-r--r--   0        0        0     8610 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06975_Summer.json
+-rw-r--r--   0        0        0     8606 2024-03-19 13:35:49.235841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06975_Winter.json
+-rw-r--r--   0        0        0    27812 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18498_Summer.json
+-rw-r--r--   0        0        0    27802 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18498_Winter.json
+-rw-r--r--   0        0        0    10602 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18769_Summer.json
+-rw-r--r--   0        0        0    10599 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18769_Winter.json
+-rw-r--r--   0        0        0     4678 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder19558_Summer.json
+-rw-r--r--   0        0        0     4675 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder19558_Winter.json
+-rw-r--r--   0        0        0    11264 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder20256_Summer.json
+-rw-r--r--   0        0        0    11268 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder20256_Winter.json
+-rw-r--r--   0        0        0     4657 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder23832_Summer.json
+-rw-r--r--   0        0        0     4655 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder23832_Winter.json
+-rw-r--r--   0        0        0     5613 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder24400_Summer.json
+-rw-r--r--   0        0        0     5612 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder24400_Winter.json
+-rw-r--r--   0        0        0    16899 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27429_Summer.json
+-rw-r--r--   0        0        0    16890 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27429_Winter.json
+-rw-r--r--   0        0        0     4475 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27681_Summer.json
+-rw-r--r--   0        0        0     4476 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27681_Winter.json
+-rw-r--r--   0        0        0    12891 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder30216_Summer.json
+-rw-r--r--   0        0        0    12883 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder30216_Winter.json
+-rw-r--r--   0        0        0     6254 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder31441_Summer.json
+-rw-r--r--   0        0        0     6252 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder31441_Winter.json
+-rw-r--r--   0        0        0     6922 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36284_Summer.json
+-rw-r--r--   0        0        0     6924 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36284_Winter.json
+-rw-r--r--   0        0        0    13353 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36360_Summer.json
+-rw-r--r--   0        0        0    13345 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36360_Winter.json
+-rw-r--r--   0        0        0     4775 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder37263_Summer.json
+-rw-r--r--   0        0        0     4773 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder37263_Winter.json
+-rw-r--r--   0        0        0     7998 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder38211_Summer.json
+-rw-r--r--   0        0        0     7989 2024-03-19 13:35:49.239841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder38211_Winter.json
+-rw-r--r--   0        0        0    19166 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder004_Summer.json
+-rw-r--r--   0        0        0    19142 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder004_Winter.json
+-rw-r--r--   0        0        0    78312 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder011_Summer.json
+-rw-r--r--   0        0        0    78090 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder011_Winter.json
+-rw-r--r--   0        0        0    35712 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder015_Summer.json
+-rw-r--r--   0        0        0    35661 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder015_Winter.json
+-rw-r--r--   0        0        0    61840 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder032_Summer.json
+-rw-r--r--   0        0        0    61912 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder032_Winter.json
+-rw-r--r--   0        0        0    95006 2024-03-19 13:35:49.243841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder041_Summer.json
+-rw-r--r--   0        0        0    95105 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder041_Winter.json
+-rw-r--r--   0        0        0    47638 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder063_Summer.json
+-rw-r--r--   0        0        0    47572 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder063_Winter.json
+-rw-r--r--   0        0        0    89894 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder078_Summer.json
+-rw-r--r--   0        0        0    89717 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder078_Winter.json
+-rw-r--r--   0        0        0    12151 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder115_Summer.json
+-rw-r--r--   0        0        0    12130 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder115_Winter.json
+-rw-r--r--   0        0        0    81931 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder128_Summer.json
+-rw-r--r--   0        0        0    81943 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder128_Winter.json
+-rw-r--r--   0        0        0    63043 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder151_Summer.json
+-rw-r--r--   0        0        0    63061 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder151_Winter.json
+-rw-r--r--   0        0        0     8776 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder159_Summer.json
+-rw-r--r--   0        0        0     8776 2024-03-19 13:35:49.247841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder159_Winter.json
+-rw-r--r--   0        0        0    34801 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder176_Summer.json
+-rw-r--r--   0        0        0    34723 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder176_Winter.json
+-rw-r--r--   0        0        0   146325 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder210_Summer.json
+-rw-r--r--   0        0        0   146163 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder210_Winter.json
+-rw-r--r--   0        0        0    91949 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder217_Summer.json
+-rw-r--r--   0        0        0    91835 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder217_Winter.json
+-rw-r--r--   0        0        0    68046 2024-03-19 13:35:49.251841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder232_Summer.json
+-rw-r--r--   0        0        0    68004 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder232_Winter.json
+-rw-r--r--   0        0        0   153496 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder251_Summer.json
+-rw-r--r--   0        0        0   153340 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder251_Winter.json
+-rw-r--r--   0        0        0    17398 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder290_Summer.json
+-rw-r--r--   0        0        0    17326 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder290_Winter.json
+-rw-r--r--   0        0        0    20701 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder312_Summer.json
+-rw-r--r--   0        0        0    20677 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder312_Winter.json
+-rw-r--r--   0        0        0    23624 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder320_Summer.json
+-rw-r--r--   0        0        0    23606 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder320_Winter.json
+-rw-r--r--   0        0        0    42014 2024-03-19 13:35:49.255841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder339_Summer.json
+-rw-r--r--   0        0        0    41888 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder339_Winter.json
+-rw-r--r--   0        0        0    18419 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/data/transformers/Catalogue.csv
+-rw-r--r--   0        0        0     3781 2024-04-11 16:24:32.993372 roseau_load_flow-0.8.1/roseau/load_flow/exceptions.py
+-rw-r--r--   0        0        0      465 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/io/__init__.py
+-rw-r--r--   0        0        0    15183 2024-04-11 14:05:17.054894 roseau_load_flow-0.8.1/roseau/load_flow/io/dgs.py
+-rw-r--r--   0        0        0    18718 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/io/dict.py
+-rw-r--r--   0        0        0     3505 2024-02-08 15:27:07.859968 roseau_load_flow-0.8.1/roseau/load_flow/license.py
+-rw-r--r--   0        0        0     1330 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/__init__.py
+-rw-r--r--   0        0        0     7282 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/branches.py
+-rw-r--r--   0        0        0    18665 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/buses.py
+-rw-r--r--   0        0        0     7412 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/core.py
+-rw-r--r--   0        0        0     4762 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/grounds.py
+-rw-r--r--   0        0        0      177 2023-02-21 17:58:50.482091 roseau_load_flow-0.8.1/roseau/load_flow/models/lines/__init__.py
+-rw-r--r--   0        0        0    18432 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/lines/lines.py
+-rw-r--r--   0        0        0    42768 2024-04-11 16:24:32.993372 roseau_load_flow-0.8.1/roseau/load_flow/models/lines/parameters.py
+-rw-r--r--   0        0        0      351 2023-02-21 17:58:50.482091 roseau_load_flow-0.8.1/roseau/load_flow/models/loads/__init__.py
+-rw-r--r--   0        0        0    56917 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/loads/flexible_parameters.py
+-rw-r--r--   0        0        0    21837 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/loads/loads.py
+-rw-r--r--   0        0        0     5239 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/potential_refs.py
+-rw-r--r--   0        0        0     8495 2024-03-19 13:35:49.259841 roseau_load_flow-0.8.1/roseau/load_flow/models/sources.py
+-rw-r--r--   0        0        0      219 2023-02-21 17:58:50.486091 roseau_load_flow-0.8.1/roseau/load_flow/models/transformers/__init__.py
+-rw-r--r--   0        0        0    21429 2024-04-11 14:05:17.058894 roseau_load_flow-0.8.1/roseau/load_flow/models/transformers/parameters.py
+-rw-r--r--   0        0        0    14347 2024-04-11 14:05:17.058894 roseau_load_flow-0.8.1/roseau/load_flow/models/transformers/transformers.py
+-rw-r--r--   0        0        0    72084 2024-04-11 16:24:32.993372 roseau_load_flow-0.8.1/roseau/load_flow/network.py
+-rw-r--r--   0        0        0     2737 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.1/roseau/load_flow/typing.py
+-rw-r--r--   0        0        0     1917 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.1/roseau/load_flow/units.py
+-rw-r--r--   0        0        0      855 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.1/roseau/load_flow/utils/__init__.py
+-rw-r--r--   0        0        0     1357 2023-11-29 10:46:50.086602 roseau_load_flow-0.8.1/roseau/load_flow/utils/_optional_deps.py
+-rw-r--r--   0        0        0     1185 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.1/roseau/load_flow/utils/_versions.py
+-rw-r--r--   0        0        0     2768 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.1/roseau/load_flow/utils/constants.py
+-rw-r--r--   0        0        0      600 2024-01-24 09:03:07.274351 roseau_load_flow-0.8.1/roseau/load_flow/utils/log.py
+-rw-r--r--   0        0        0    12581 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.1/roseau/load_flow/utils/mixins.py
+-rw-r--r--   0        0        0     6016 2024-03-19 13:35:49.263841 roseau_load_flow-0.8.1/roseau/load_flow/utils/types.py
+-rw-r--r--   0        0        0     3995 1970-01-01 00:00:00.000000 roseau_load_flow-0.8.1/PKG-INFO
```

### Comparing `roseau_load_flow-0.8.0/LICENSE.md` & `roseau_load_flow-0.8.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/README.md` & `roseau_load_flow-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/pyproject.toml` & `roseau_load_flow-0.8.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 [tool.poetry]
 name = "roseau-load-flow"
-version = "0.8.0"
+version = "0.8.1"
 description = "Highly capable three-phase load flow solver"
 authors = [
     "Ali Hamdan <ali.hamdan@roseautechnologies.com>",
     "Sébastien Vallet <sebastien.vallet@roseautechnologies.com>",
     "Benoît Vinot <benoit.vinot@roseautechnologies.com>",
     "Florent Cadoux <florent.cadoux@roseautechnologies.com>",
+    "Louise Muller <louise.muller@roseautechnologies.com>",
     "Victor Gouin",
 ]
 maintainers = ["Ali Hamdan <ali.hamdan@roseautechnologies.com>"]
 license = "BSD-3-Clause"
 repository = "https://github.com/RoseauTechnologies/Roseau_Load_Flow/"
 readme = "README.md"
 include = [
@@ -45,28 +46,28 @@
 shapely = ">=2.0.0"
 regex = ">=2022.1.18"
 pint = ">=0.21.0"
 typing-extensions = ">=4.6.2"
 pyproj = ">=3.3.0"
 certifi = ">=2023.5.7"
 platformdirs = ">=4.0.0"
-roseau-load-flow-engine = "==0.13.0"
+roseau-load-flow-engine = "==0.13.1"
 
 # Optional dependencies
 matplotlib = { version = ">=3.7.2", optional = true }
 networkx = { version = ">=3.0.0", optional = true }
 
 [tool.poetry.extras]
 # DO NOT forget to update the installation page in the documentation when extras change
 plot = ["matplotlib"]
 graph = ["networkx"]
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
-pytest-cov = "^4.0.0"
+pytest-cov = "^5.0.0"
 pytest-xdist = "^3.1.0"
 coverage = { version = "^7.0.5", extras = ["toml"] }
 matplotlib = ">=3.7.2"
 networkx = ">=3.0.0"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.0.0"
@@ -79,14 +80,15 @@
 sphinx-autoapi = "^3.0.0"
 sphinx-copybutton = ">=0.5.1"
 sphinx-inline-tabs = ">=2022.1.2b11"
 furo = ">=2022.9.29"
 sphinxcontrib-googleanalytics = ">=0.3"
 sphinxcontrib-bibtex = "^2.5.0"
 sphinx-sitemap = "^2.5.1"
+sphinxext-opengraph = ">=0.9.1"
 
 [tool.ruff]
 line-length = 120
 target-version = "py310"
 show-fixes = true
 extend-include = ["*.ipynb"]
 namespace-packages = ["roseau"]
```

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/__about__.py` & `roseau_load_flow-0.8.1/roseau/load_flow/__about__.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 __authors__ = ", ".join(
     (
         "Ali Hamdan <ali.hamdan@roseautechnologies.com>",
         "Sébastien Vallet <sebastien.vallet@roseautechnologies.com>",
         "Benoît Vinot <benoit.vinot@roseautechnologies.com>",
         "Florent Cadoux <florent.cadoux@roseautechnologies.com>",
+        "Louise Muller <louise.muller@roseautechnologies.com>",
         "Victor Gouin",
     )
 )
 __copyright__ = "Roseau Technologies 2018"
 __credits__ = "Roseau Technologies"
 __license__ = "BSD-3-Clause"
 __maintainer__ = "Ali Hamdan"
```

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/__init__.py` & `roseau_load_flow-0.8.1/roseau/load_flow/__init__.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/_compat.py` & `roseau_load_flow-0.8.1/roseau/load_flow/_compat.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/_solvers.py` & `roseau_load_flow-0.8.1/roseau/load_flow/_solvers.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/_wrapper.py` & `roseau_load_flow-0.8.1/roseau/load_flow/_wrapper.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/converters.py` & `roseau_load_flow-0.8.1/roseau/load_flow/converters.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/lines/Catalogue.csv` & `roseau_load_flow-0.8.1/roseau/load_flow/data/lines/Catalogue.csv`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/Catalogue.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/Catalogue.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder00939_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder00939_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder00939_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder00939_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder02639_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder02639_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder02639_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder02639_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder04790_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder04790_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder04790_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder04790_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06713_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06713_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06713_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06713_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06926_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06926_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06926_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06926_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06975_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06975_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder06975_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder06975_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18498_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18498_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18498_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18498_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18769_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18769_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder18769_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder18769_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder19558_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder19558_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder19558_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder19558_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder20256_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder20256_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder20256_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder20256_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder23832_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder23832_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder23832_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder23832_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder24400_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder24400_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder24400_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder24400_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27429_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27429_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27429_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27429_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27681_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27681_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder27681_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder27681_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder30216_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder30216_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder30216_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder30216_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder31441_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder31441_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder31441_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder31441_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36284_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36284_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36284_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36284_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36360_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36360_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder36360_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder36360_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder37263_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder37263_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder37263_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder37263_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder38211_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder38211_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/LVFeeder38211_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/LVFeeder38211_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder004_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder004_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder004_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder004_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder011_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder011_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder011_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder011_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder015_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder015_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder015_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder015_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder032_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder032_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder032_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder032_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder041_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder041_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder041_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder041_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder063_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder063_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder063_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder063_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder078_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder078_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder078_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder078_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder115_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder115_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder115_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder115_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder128_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder128_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder128_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder128_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder151_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder151_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder151_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder151_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder159_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder159_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder159_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder159_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder176_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder176_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder176_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder176_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder210_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder210_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder210_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder210_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder217_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder217_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder217_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder217_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder232_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder232_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder232_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder232_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder251_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder251_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder251_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder251_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder290_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder290_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder290_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder290_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder312_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder312_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder312_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder312_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder320_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder320_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder320_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder320_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder339_Summer.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder339_Summer.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/networks/MVFeeder339_Winter.json` & `roseau_load_flow-0.8.1/roseau/load_flow/data/networks/MVFeeder339_Winter.json`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/data/transformers/Catalogue.csv` & `roseau_load_flow-0.8.1/roseau/load_flow/data/transformers/Catalogue.csv`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/exceptions.py` & `roseau_load_flow-0.8.1/roseau/load_flow/exceptions.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     NO_POTENTIAL_REFERENCE = auto()
     SEVERAL_POTENTIAL_REFERENCE = auto()
     EMPTY_NETWORK = auto()
     UNKNOWN_ELEMENT = auto()
     NO_VOLTAGE_SOURCE = auto()
     BAD_ELEMENT_OBJECT = auto()
     DISCONNECTED_ELEMENT = auto()
+    POORLY_CONNECTED_ELEMENT = auto()
     NO_LOAD_FLOW_CONVERGENCE = auto()
     BAD_LOAD_FLOW_RESULT = auto()
     LOAD_FLOW_NOT_RUN = auto()
     SEVERAL_NETWORKS = auto()
     BAD_JACOBIAN = auto()
 
     # Solver
```

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/io/dgs.py` & `roseau_load_flow-0.8.1/roseau/load_flow/io/dgs.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/io/dict.py` & `roseau_load_flow-0.8.1/roseau/load_flow/io/dict.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/license.py` & `roseau_load_flow-0.8.1/roseau/load_flow/license.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/__init__.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/__init__.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/branches.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/branches.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/buses.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/buses.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/core.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/core.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/grounds.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/grounds.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/lines/lines.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/lines/lines.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/lines/parameters.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/lines/parameters.py`

 * *Files 0% similar despite different names*

```diff
@@ -949,15 +949,15 @@
             raise_if_not_found=False,
         )
         return catalogue_data.rename(
             columns={
                 "name": "Name",
                 "r": "Resistance (ohm/km)",
                 "x": "Reactance (ohm/km)",
-                "b": "Susceptance (µS/km)",
+                "b": "Susceptance (S/km)",
                 "maximal_current": "Maximal current (A)",
                 "type": "Line type",
                 "material": "Conductor material",
                 "insulator": "Insulator type",
                 "section": "Cross-section (mm²)",
             }
         ).set_index("Name")
```

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/loads/flexible_parameters.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/loads/flexible_parameters.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/loads/loads.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/loads/loads.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/potential_refs.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/potential_refs.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/sources.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/sources.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/transformers/parameters.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/transformers/parameters.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/models/transformers/transformers.py` & `roseau_load_flow-0.8.1/roseau/load_flow/models/transformers/transformers.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/network.py` & `roseau_load_flow-0.8.1/roseau/load_flow/network.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """
 This module defines the electrical network class.
 """
 
 import json
 import logging
 import re
+import textwrap
 import time
 import warnings
 from collections.abc import Iterable, Mapping, Sized
 from importlib import resources
 from itertools import chain
 from pathlib import Path
 from typing import TYPE_CHECKING, NoReturn, TypeVar
@@ -1276,46 +1277,54 @@
     def _reset_inputs(self) -> None:
         """Reset the input vector used for the first step of the newton algorithm to its initial value."""
         if self._solver is not None:
             self._solver.reset_inputs()
 
     def _propagate_potentials(self) -> None:
         """Set the bus potentials that have not been initialized yet."""
-        uninitialized = False
         all_phases = set()
         for bus in self.buses.values():
             if not bus._initialized:
-                uninitialized = True
                 all_phases |= set(bus.phases)
 
-        if uninitialized:
-            potentials, starting_source = self._get_potentials(all_phases)
-            elements = [(starting_source, potentials)]
-            visited = set()
-            while elements:
-                element, potentials = elements.pop(-1)
-                visited.add(element)
-                if isinstance(element, Bus) and not element._initialized:
-                    element.potentials = np.array([potentials[p] for p in element.phases], dtype=np.complex128)
-                    element._initialized_by_the_user = False  # only used for serialization
-                for e in element._connected_elements:
-                    if e not in visited and isinstance(e, (AbstractBranch, Bus)):
-                        if isinstance(element, Transformer):
-                            k = element.parameters._ulv / element.parameters._uhv
-                            phase_displacement = element.parameters.phase_displacement
-                            if phase_displacement is None:
-                                phase_displacement = 0
-                            new_potentials = potentials.copy()
-                            for key, p in new_potentials.items():
-                                new_potentials[key] = p * k * np.exp(phase_displacement * -1j * np.pi / 6.0)
-                            elements.append((e, new_potentials))
-                        else:
-                            elements.append((e, potentials))
+        starting_potentials, starting_bus = self._get_potentials(all_phases)
+        elements = [(starting_bus, starting_potentials)]
+        visited = set()
+        while elements:
+            element, potentials = elements.pop(-1)
+            visited.add(element)
+            if isinstance(element, Bus) and not element._initialized:
+                element.potentials = np.array([potentials[p] for p in element.phases], dtype=np.complex128)
+                element._initialized_by_the_user = False  # only used for serialization
+            for e in element._connected_elements:
+                if e not in visited and isinstance(e, (AbstractBranch, Bus)):
+                    if isinstance(element, Transformer):
+                        k = element.parameters._ulv / element.parameters._uhv
+                        phase_displacement = element.parameters.phase_displacement
+                        if phase_displacement is None:
+                            phase_displacement = 0
+                        new_potentials = potentials.copy()
+                        for key, p in new_potentials.items():
+                            new_potentials[key] = p * k * np.exp(phase_displacement * -1j * np.pi / 6.0)
+                        elements.append((e, new_potentials))
+                    else:
+                        elements.append((e, potentials))
+
+        if len(visited) < len(self.buses) + len(self.branches):
+            unconnected_elements = [
+                element for element in chain(self.buses.values(), self.branches.values()) if element not in visited
+            ]
+            printable_elements = textwrap.wrap(
+                ", ".join(f"{type(e).__name__}({e.id!r})" for e in unconnected_elements), 500
+            )
+            msg = f"The elements {printable_elements} are not electrically connected to a voltage source."
+            logger.error(msg)
+            raise RoseauLoadFlowException(msg=msg, code=RoseauLoadFlowExceptionCode.POORLY_CONNECTED_ELEMENT)
 
-    def _get_potentials(self, all_phases: set[str]) -> tuple[dict[str, complex], VoltageSource]:
+    def _get_potentials(self, all_phases: set[str]) -> tuple[dict[str, complex], Bus]:
         """Compute initial potentials from the voltages sources of the network, get also the starting source"""
         starting_source = None
         potentials = {"n": 0.0}
         # if there are multiple voltage sources, start from the higher one (the last one in the sorted below)
         for source in sorted(self.sources.values(), key=lambda x: np.average(np.abs(x._voltages))):
             source_voltages = source._voltages
             starting_source = source
@@ -1344,15 +1353,15 @@
             # We failed to determine all the potentials (the sources are strange), fallback to something simple
             v = np.average(np.abs(starting_source._voltages))
             potentials["a"] = v
             potentials["b"] = v * np.exp(-2j * np.pi / 3)
             potentials["c"] = v * np.exp(2j * np.pi / 3)
             potentials["n"] = 0.0
 
-        return potentials, starting_source
+        return potentials, starting_source.bus
 
     @staticmethod
     def _check_ref(elements: Iterable[Element]) -> None:
         """Check the number of potential references to avoid having a singular jacobian matrix."""
         visited_elements: set[Element] = set()
         for initial_element in elements:
             if initial_element in visited_elements or isinstance(initial_element, Transformer):
```

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/typing.py` & `roseau_load_flow-0.8.1/roseau/load_flow/typing.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/units.py` & `roseau_load_flow-0.8.1/roseau/load_flow/units.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/__init__.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/_optional_deps.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/_optional_deps.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/_versions.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/_versions.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/constants.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/constants.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/log.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/log.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/mixins.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/mixins.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/roseau/load_flow/utils/types.py` & `roseau_load_flow-0.8.1/roseau/load_flow/utils/types.py`

 * *Files identical despite different names*

### Comparing `roseau_load_flow-0.8.0/PKG-INFO` & `roseau_load_flow-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: roseau-load-flow
-Version: 0.8.0
+Version: 0.8.1
 Summary: Highly capable three-phase load flow solver
 Home-page: https://github.com/RoseauTechnologies/Roseau_Load_Flow/
 License: BSD-3-Clause
 Author: Ali Hamdan
 Author-email: ali.hamdan@roseautechnologies.com
 Maintainer: Ali Hamdan
 Maintainer-email: ali.hamdan@roseautechnologies.com
@@ -24,15 +24,15 @@
 Requires-Dist: networkx (>=3.0.0) ; extra == "graph"
 Requires-Dist: numpy (>=1.21.5)
 Requires-Dist: pandas (>=1.4.0)
 Requires-Dist: pint (>=0.21.0)
 Requires-Dist: platformdirs (>=4.0.0)
 Requires-Dist: pyproj (>=3.3.0)
 Requires-Dist: regex (>=2022.1.18)
-Requires-Dist: roseau-load-flow-engine (==0.13.0)
+Requires-Dist: roseau-load-flow-engine (==0.13.1)
 Requires-Dist: shapely (>=2.0.0)
 Requires-Dist: typing-extensions (>=4.6.2)
 Project-URL: Repository, https://github.com/RoseauTechnologies/Roseau_Load_Flow/
 Description-Content-Type: text/markdown
 
 # Roseau Load Flow
```

