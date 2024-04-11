# Comparing `tmp/module_qc_tools-2.2.2rc3.tar.gz` & `tmp/module_qc_tools-2.2.3.tar.gz`

## Comparing `module_qc_tools-2.2.2rc3.tar` & `module_qc_tools-2.2.3.tar`

### file list

```diff
@@ -1,68 +1,69 @@
--rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/.gitlab-ci.yml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/.gitmodules
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/.pre-commit-config.yaml
--rw-r--r--   0        0        0      899 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/tbump.toml
--rw-r--r--   0        0        0    42055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/ADC_CALIBRATION/2024-03-06_173431/20UPGXM1234567.json
--rw-r--r--   0        0        0   321535 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/ANALOG_READBACK/2024-03-06_173433/20UPGXM1234567.json
--rw-r--r--   0        0        0    25399 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/DATA_TRANSMISSION/2024-03-06_173456/20UPGXM1234567.json
--rw-r--r--   0        0        0    23049 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/INJECTION_CAPACITANCE/2024-03-06_173431/20UPGXM1234567.json
--rw-r--r--   0        0        0     9968 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/IV_MEASURE/2024-03-06_173519/20UPGXM1234567.json
--rw-r--r--   0        0        0    27706 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/LP_MODE/2024-03-06_173457/20UPGXM1234567.json
--rw-r--r--   0        0        0    24122 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/OVERVOLTAGE_PROTECTION/2024-03-06_173433/20UPGXM1234567.json
--rw-r--r--   0        0        0    82012 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/SLDO/2024-03-06_173447/20UPGXM1234567.json
--rw-r--r--   0        0        0    35406 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/UNDERSHUNT_PROTECTION/2024-03-06_173456/20UPGXM1234567.json
--rw-r--r--   0        0        0   148838 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/Measurements/VCAL_CALIBRATION/2024-03-06_173452/20UPGXM1234567.json
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/docs/.gitkeep
--rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/emulator/README.md
--rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/__init__.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/_version.py
--rw-r--r--   0        0        0     9630 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/ADC_CALIBRATION.py
--rw-r--r--   0        0        0    23739 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/ANALOG_READBACK.py
--rw-r--r--   0        0        0    10470 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/DATA_TRANSMISSION.py
--rw-r--r--   0        0        0     9972 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
--rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/IV_MEASURE.py
--rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/LP_MODE.py
--rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
--rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/SLDO.py
--rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py
--rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/VCAL_CALIBRATION.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/__init__.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/__main__.py
--rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/globals.py
--rw-r--r--   0        0        0    22966 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/hardware_emulator.py
--rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/main.py
--rw-r--r--   0        0        0     5016 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/upload_localdb.py
--rw-r--r--   0        0        0     5078 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/emulator_merged_vmux.json
--rw-r--r--   0        0        0     6041 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/example_merged_vmux.json
--rw-r--r--   0        0        0     6330 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/example_separate_vmux.json
--rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/module_state_template.json
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
--rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
--rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
--rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
--rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
--rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
--rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/ANALOG_READBACK.json
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json
--rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
--rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/IV_MEASURE.json
--rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/LP_MODE.json
--rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
--rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/SLDO.json
--rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json
--rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
--rw-r--r--   0        0        0    30007 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/common.json
--rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/config.json
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/__init__.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/hardware_control_base.py
--rw-r--r--   0        0        0     6293 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/misc.py
--rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/multimeter.py
--rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/ntc.py
--rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/power_supply.py
--rw-r--r--   0        0        0    17490 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/yarr.py
--rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/tests/test_package.py
--rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/.gitignore
--rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/LICENSE
--rw-r--r--   0        0        0    39358 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/README.md
--rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/pyproject.toml
--rw-r--r--   0        0        0    41602 2020-02-02 00:00:00.000000 module_qc_tools-2.2.2rc3/PKG-INFO
+-rw-r--r--   0        0        0    10245 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitlab-ci.yml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitmodules
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/tbump.toml
+-rw-r--r--   0        0        0    30217 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/ADC_CALIBRATION/2024-04-11_144359/20UPGXM1234567.json
+-rw-r--r--   0        0        0   321578 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/ANALOG_READBACK/2024-04-11_144351/20UPGXM1234567.json
+-rw-r--r--   0        0        0    25387 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/DATA_TRANSMISSION/2024-04-11_144358/20UPGXM1234567.json
+-rw-r--r--   0        0        0    23033 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/INJECTION_CAPACITANCE/2024-04-11_144353/20UPGXM1234567.json
+-rw-r--r--   0        0        0     9971 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/IV_MEASURE/2024-04-11_144408/20UPGXM1234567.json
+-rw-r--r--   0        0        0    27694 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/LP_MODE/2024-04-11_144406/20UPGXM1234567.json
+-rw-r--r--   0        0        0    24110 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/OVERVOLTAGE_PROTECTION/2024-04-11_144333/20UPGXM1234567.json
+-rw-r--r--   0        0        0    82000 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/SLDO/2024-04-11_144328/20UPGXM1234567.json
+-rw-r--r--   0        0        0    35394 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/UNDERSHUNT_PROTECTION/2024-04-11_144338/20UPGXM1234567.json
+-rw-r--r--   0        0        0   109866 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/Measurements/VCAL_CALIBRATION/2024-04-11_144330/20UPGXM1234567.json
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/docs/.gitkeep
+-rw-r--r--   0        0        0     3076 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/emulator/README.md
+-rw-r--r--   0        0        0      313 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/__init__.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/_version.py
+-rw-r--r--   0        0        0    10524 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/ADC_CALIBRATION.py
+-rw-r--r--   0        0        0    25909 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/ANALOG_READBACK.py
+-rw-r--r--   0        0        0    11023 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/DATA_TRANSMISSION.py
+-rw-r--r--   0        0        0    10986 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py
+-rw-r--r--   0        0        0    10290 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/IV_MEASURE.py
+-rw-r--r--   0        0        0    11468 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/LP_MODE.py
+-rw-r--r--   0        0        0    10807 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py
+-rw-r--r--   0        0        0     9644 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/SLDO.py
+-rw-r--r--   0        0        0    11922 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py
+-rw-r--r--   0        0        0    13093 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/VCAL_CALIBRATION.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/__init__.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/__main__.py
+-rw-r--r--   0        0        0     3812 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/globals.py
+-rw-r--r--   0        0        0    23129 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/hardware_emulator.py
+-rw-r--r--   0        0        0     2541 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/main.py
+-rw-r--r--   0        0        0     5055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/cli/upload_localdb.py
+-rw-r--r--   0        0        0     5230 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/emulator_merged_vmux.json
+-rw-r--r--   0        0        0     6158 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_merged_vmux.json
+-rw-r--r--   0        0        0     6447 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_separate_vmux.json
+-rw-r--r--   0        0        0     1437 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/module_state_template.json
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json
+-rw-r--r--   0        0        0  1905867 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json
+-rw-r--r--   0        0        0  1905871 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json
+-rw-r--r--   0        0        0  1905885 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json
+-rw-r--r--   0        0        0  1905869 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json
+-rw-r--r--   0        0        0      621 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json
+-rw-r--r--   0        0        0     1235 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json
+-rw-r--r--   0        0        0     5847 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ANALOG_READBACK.json
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json
+-rw-r--r--   0        0        0     1205 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json
+-rw-r--r--   0        0        0      919 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/IV_MEASURE.json
+-rw-r--r--   0        0        0     1421 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/LP_MODE.json
+-rw-r--r--   0        0        0     1351 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json
+-rw-r--r--   0        0        0     1457 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/SLDO.json
+-rw-r--r--   0        0        0     1259 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json
+-rw-r--r--   0        0        0     1284 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json
+-rw-r--r--   0        0        0    30007 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/common.json
+-rw-r--r--   0        0        0     8389 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/data/schema/config.json
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/__init__.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/hardware_control_base.py
+-rw-r--r--   0        0        0     6322 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/misc.py
+-rw-r--r--   0        0        0      851 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/multimeter.py
+-rw-r--r--   0        0        0      753 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/ntc.py
+-rw-r--r--   0        0        0     5951 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/power_supply.py
+-rw-r--r--   0        0        0    18004 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/src/module_qc_tools/utils/yarr.py
+-rw-r--r--   0        0        0      111 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/tests/test_package.py
+-rw-r--r--   0        0        0     2187 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/.gitignore
+-rw-r--r--   0        0        0     1067 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/LICENSE
+-rw-r--r--   0        0        0    39352 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/README.md
+-rw-r--r--   0        0        0     6055 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/pyproject.toml
+-rw-r--r--   0        0        0    41593 2020-02-02 00:00:00.000000 module_qc_tools-2.2.3/PKG-INFO
```

### Comparing `module_qc_tools-2.2.2rc3/.gitlab-ci.yml` & `module_qc_tools-2.2.3/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/.pre-commit-config.yaml` & `module_qc_tools-2.2.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/tbump.toml` & `module_qc_tools-2.2.3/tbump.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,57 +1,56 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2232 2e32 2e32 7263 3322 0a0a  t = "2.2.2rc3"..
-00000020: 2320 4578 616d 706c 6520 6f66 2061 2073  # Example of a s
-00000030: 656d 7665 7220 7265 6765 7870 2e0a 2320  emver regexp..# 
-00000040: 4d61 6b65 2073 7572 6520 7468 6973 206d  Make sure this m
-00000050: 6174 6368 6573 2063 7572 7265 6e74 5f76  atches current_v
-00000060: 6572 7369 6f6e 2062 6566 6f72 650a 2320  ersion before.# 
-00000070: 7573 696e 6720 7462 756d 700a 7265 6765  using tbump.rege
-00000080: 7820 3d20 2727 270a 2020 283f 503c 6d61  x = '''.  (?P<ma
-00000090: 6a6f 723e 5c64 2b29 0a20 205c 2e0a 2020  jor>\d+).  \..  
-000000a0: 283f 503c 6d69 6e6f 723e 5c64 2b29 0a20  (?P<minor>\d+). 
-000000b0: 205c 2e0a 2020 283f 503c 7061 7463 683e   \..  (?P<patch>
-000000c0: 5c64 2b29 0a20 2028 7263 0a20 2020 2028  \d+).  (rc.    (
-000000d0: 3f50 3c63 616e 6469 6461 7465 3e5c 642b  ?P<candidate>\d+
-000000e0: 290a 2020 293f 0a20 2027 2727 0a0a 5b67  ).  )?.  '''..[g
-000000f0: 6974 5d0a 2320 5468 6520 6375 7272 656e  it].# The curren
-00000100: 7420 7665 7273 696f 6e20 7769 6c6c 2067  t version will g
-00000110: 6574 2075 7064 6174 6564 2077 6865 6e20  et updated when 
-00000120: 7462 756d 7020 6973 2072 756e 0a6d 6573  tbump is run.mes
-00000130: 7361 6765 5f74 656d 706c 6174 6520 3d20  sage_template = 
-00000140: 2242 756d 7020 7665 7273 696f 6e3a 2032  "Bump version: 2
-00000150: 2e32 2e32 7263 3320 e286 9220 7b6e 6577  .2.2rc3 ... {new
-00000160: 5f76 6572 7369 6f6e 7d22 0a74 6167 5f74  _version}".tag_t
-00000170: 656d 706c 6174 6520 3d20 2276 7b6e 6577  emplate = "v{new
-00000180: 5f76 6572 7369 6f6e 7d22 0a0a 2320 466f  _version}"..# Fo
-00000190: 7220 6561 6368 2066 696c 6520 746f 2070  r each file to p
-000001a0: 6174 6368 2c20 6164 6420 6120 5b5b 6669  atch, add a [[fi
-000001b0: 6c65 5d5d 2063 6f6e 6669 670a 2320 7365  le]] config.# se
-000001c0: 6374 696f 6e20 636f 6e74 6169 6e69 6e67  ction containing
-000001d0: 2074 6865 2070 6174 6820 6f66 2074 6865   the path of the
-000001e0: 2066 696c 652c 2072 656c 6174 6976 6520   file, relative 
-000001f0: 746f 2074 6865 0a23 2074 6275 6d70 2e74  to the.# tbump.t
-00000200: 6f6d 6c20 6c6f 6361 7469 6f6e 2e0a 5b5b  oml location..[[
-00000210: 6669 6c65 5d5d 0a73 7263 203d 2022 7462  file]].src = "tb
-00000220: 756d 702e 746f 6d6c 220a 2320 5265 7374  ump.toml".# Rest
-00000230: 7269 6374 2073 6561 7263 6820 746f 206d  rict search to m
-00000240: 616b 6520 6974 2065 7870 6c69 6369 7420  ake it explicit 
-00000250: 7768 7920 7462 756d 702e 746f 6d6c 0a23  why tbump.toml.#
-00000260: 2069 7320 6576 656e 2069 6e63 6c75 6465   is even include
-00000270: 6420 6173 2061 2066 696c 6520 746f 2062  d as a file to b
-00000280: 756d 702c 2061 7320 6974 2077 696c 6c20  ump, as it will 
-00000290: 6765 740a 2320 6974 7320 7665 7273 696f  get.# its versio
-000002a0: 6e2e 6375 7272 656e 7420 6174 7472 6962  n.current attrib
-000002b0: 7574 6520 6275 6d70 6564 2061 6e79 7761  ute bumped anywa
-000002c0: 792e 0a73 6561 7263 6820 3d20 2242 756d  y..search = "Bum
-000002d0: 7020 7665 7273 696f 6e3a 207b 6375 7272  p version: {curr
-000002e0: 656e 745f 7665 7273 696f 6e7d 20e2 8692  ent_version} ...
-000002f0: 2022 0a0a 5b5b 6669 6c65 5d5d 0a73 7263   "..[[file]].src
-00000300: 203d 2022 5245 4144 4d45 2e6d 6422 0a0a   = "README.md"..
-00000310: 5b5b 6669 656c 645d 5d0a 2320 7468 6520  [[field]].# the 
-00000320: 6e61 6d65 206f 6620 7468 6520 6669 656c  name of the fiel
-00000330: 640a 6e61 6d65 203d 2022 6361 6e64 6964  d.name = "candid
-00000340: 6174 6522 0a23 2074 6865 2064 6566 6175  ate".# the defau
-00000350: 6c74 2076 616c 7565 2074 6f20 7573 652c  lt value to use,
-00000360: 2069 6620 7468 6572 6520 6973 206e 6f20   if there is no 
-00000370: 6d61 7463 680a 6465 6661 756c 7420 3d20  match.default = 
-00000380: 2222 0a                                  "".
+00000010: 7420 3d20 2232 2e32 2e33 220a 0a23 2045  t = "2.2.3"..# E
+00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
+00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
+00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
+00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
+00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
+00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
+00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
+00000090: 3e5c 642b 290a 2020 5c2e 0a20 2028 3f50  >\d+).  \..  (?P
+000000a0: 3c6d 696e 6f72 3e5c 642b 290a 2020 5c2e  <minor>\d+).  \.
+000000b0: 0a20 2028 3f50 3c70 6174 6368 3e5c 642b  .  (?P<patch>\d+
+000000c0: 290a 2020 2872 630a 2020 2020 283f 503c  ).  (rc.    (?P<
+000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
+000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
+000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
+00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
+00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
+00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
+00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
+00000140: 6d70 2076 6572 7369 6f6e 3a20 322e 322e  mp version: 2.2.
+00000150: 3320 e286 9220 7b6e 6577 5f76 6572 7369  3 ... {new_versi
+00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
+00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
+00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
+00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
+000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
+000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
+000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
+000001d0: 6174 6820 6f66 2074 6865 2066 696c 652c  ath of the file,
+000001e0: 2072 656c 6174 6976 6520 746f 2074 6865   relative to the
+000001f0: 0a23 2074 6275 6d70 2e74 6f6d 6c20 6c6f  .# tbump.toml lo
+00000200: 6361 7469 6f6e 2e0a 5b5b 6669 6c65 5d5d  cation..[[file]]
+00000210: 0a73 7263 203d 2022 7462 756d 702e 746f  .src = "tbump.to
+00000220: 6d6c 220a 2320 5265 7374 7269 6374 2073  ml".# Restrict s
+00000230: 6561 7263 6820 746f 206d 616b 6520 6974  earch to make it
+00000240: 2065 7870 6c69 6369 7420 7768 7920 7462   explicit why tb
+00000250: 756d 702e 746f 6d6c 0a23 2069 7320 6576  ump.toml.# is ev
+00000260: 656e 2069 6e63 6c75 6465 6420 6173 2061  en included as a
+00000270: 2066 696c 6520 746f 2062 756d 702c 2061   file to bump, a
+00000280: 7320 6974 2077 696c 6c20 6765 740a 2320  s it will get.# 
+00000290: 6974 7320 7665 7273 696f 6e2e 6375 7272  its version.curr
+000002a0: 656e 7420 6174 7472 6962 7574 6520 6275  ent attribute bu
+000002b0: 6d70 6564 2061 6e79 7761 792e 0a73 6561  mped anyway..sea
+000002c0: 7263 6820 3d20 2242 756d 7020 7665 7273  rch = "Bump vers
+000002d0: 696f 6e3a 207b 6375 7272 656e 745f 7665  ion: {current_ve
+000002e0: 7273 696f 6e7d 20e2 8692 2022 0a0a 5b5b  rsion} ... "..[[
+000002f0: 6669 6c65 5d5d 0a73 7263 203d 2022 5245  file]].src = "RE
+00000300: 4144 4d45 2e6d 6422 0a0a 5b5b 6669 656c  ADME.md"..[[fiel
+00000310: 645d 5d0a 2320 7468 6520 6e61 6d65 206f  d]].# the name o
+00000320: 6620 7468 6520 6669 656c 640a 6e61 6d65  f the field.name
+00000330: 203d 2022 6361 6e64 6964 6174 6522 0a23   = "candidate".#
+00000340: 2074 6865 2064 6566 6175 6c74 2076 616c   the default val
+00000350: 7565 2074 6f20 7573 652c 2069 6620 7468  ue to use, if th
+00000360: 6572 6520 6973 206e 6f20 6d61 7463 680a  ere is no match.
+00000370: 6465 6661 756c 7420 3d20 2222 0a         default = "".
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/ADC_CALIBRATION/2024-03-06_173431/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/UNDERSHUNT_PROTECTION/2024-04-11_144338/20UPGXM1234567.json`

 * *Files 24% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8411217591002746%*

 * *Differences: {'0': "{0: {'testType': 'UNDERSHUNT_PROTECTION', 'results': {'property': {replace: "*

 * *      "OrderedDict([('UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION', '2.2.3')])}, 'Measurements': "*

 * *      "{'Vmux30': {'Values': {delete: [26, 25, 24, 23, 22, 21, 20, 19, 18, 17, 16, 15, 14, 13, 12, "*

 * *      "11, 10, 9, 8, 7, 6, 5, 4, 3, 2, 1, 0]}}, 'Temperature': OrderedDict([('X', False), ('Unit', "*

 * *      "'C'), ('Values', [29.2, 29.2, 29.2])]), 'SetCurrent': OrderedDict([('X', False), ('Unit', "*

 * *      "'A'), ('Values', [2.1, […]*

```diff
@@ -1,194 +1,159 @@
 [
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
-                        ],
-                        "X": false
-                    },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
-                        "Values": [
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567,
-                            7567
-                        ],
-                        "X": false
-                    },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            600.0,
-                            700.0,
-                            800.0,
-                            900.0,
-                            1000.0,
-                            1100.0,
-                            1200.0,
-                            1300.0,
-                            1400.0,
-                            1500.0,
-                            1600.0,
-                            1700.0,
-                            1800.0,
-                            1900.0,
-                            2000.0,
-                            2100.0,
-                            2200.0,
-                            2300.0,
-                            2400.0,
-                            2500.0,
-                            2600.0,
-                            2700.0,
-                            2800.0,
-                            2900.0,
-                            3000.0,
-                            3100.0,
-                            3200.0,
-                            3300.0,
-                            3400.0
+                            2.1,
+                            2.1,
+                            2.1
                         ],
                         "X": true
                     },
-                    "Vmux30": {
+                    "Imux0": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1,
+                            2.1,
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2,
+                            29.2,
+                            29.2
+                        ],
+                        "X": false
+                    },
+                    "Vmux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux35": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux8": {
+                    "Vmux39": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -204,15 +169,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 4,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 3,
                                 "SldoTrimD": 4
                             },
@@ -246,213 +210,179 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746823,
-                    "TimeStart": 1709746472
+                    "TimeEnd": 1712846840,
+                    "TimeStart": 1712846618,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
-                        ],
-                        "X": false
-                    },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
-                        "Values": [
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705,
-                            7705
-                        ],
-                        "X": false
-                    },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            600.0,
-                            700.0,
-                            800.0,
-                            900.0,
-                            1000.0,
-                            1100.0,
-                            1200.0,
-                            1300.0,
-                            1400.0,
-                            1500.0,
-                            1600.0,
-                            1700.0,
-                            1800.0,
-                            1900.0,
-                            2000.0,
-                            2100.0,
-                            2200.0,
-                            2300.0,
-                            2400.0,
-                            2500.0,
-                            2600.0,
-                            2700.0,
-                            2800.0,
-                            2900.0,
-                            3000.0,
-                            3100.0,
-                            3200.0,
-                            3300.0,
-                            3400.0
+                            2.1,
+                            2.1,
+                            2.1
                         ],
                         "X": true
                     },
-                    "Vmux30": {
+                    "Imux0": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux28": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1,
+                            2.1,
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2,
+                            29.2,
+                            29.2
+                        ],
+                        "X": false
+                    },
+                    "Vmux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux35": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux8": {
+                    "Vmux39": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -468,15 +398,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 1,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 4,
                                 "SldoTrimD": 3
                             },
@@ -510,213 +439,179 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746823,
-                    "TimeStart": 1709746472
+                    "TimeEnd": 1712846840,
+                    "TimeStart": 1712846618,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
-                        ],
-                        "X": false
-                    },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
-                        "Values": [
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933,
-                            7933
-                        ],
-                        "X": false
-                    },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            600.0,
-                            700.0,
-                            800.0,
-                            900.0,
-                            1000.0,
-                            1100.0,
-                            1200.0,
-                            1300.0,
-                            1400.0,
-                            1500.0,
-                            1600.0,
-                            1700.0,
-                            1800.0,
-                            1900.0,
-                            2000.0,
-                            2100.0,
-                            2200.0,
-                            2300.0,
-                            2400.0,
-                            2500.0,
-                            2600.0,
-                            2700.0,
-                            2800.0,
-                            2900.0,
-                            3000.0,
-                            3100.0,
-                            3200.0,
-                            3300.0,
-                            3400.0
+                            2.1,
+                            2.1,
+                            2.1
                         ],
                         "X": true
                     },
-                    "Vmux30": {
+                    "Imux0": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux8": {
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1,
+                            2.1,
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2,
+                            29.2,
+                            29.2
+                        ],
+                        "X": false
+                    },
+                    "Vmux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux35": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -732,15 +627,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 65535,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 8,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 12,
                                 "SldoTrimD": 8
                             },
@@ -774,213 +668,179 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746823,
-                    "TimeStart": 1709746472
+                    "TimeEnd": 1712846840,
+                    "TimeStart": 1712846618,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ],
     [
         {
             "results": {
                 "Measurements": {
-                    "ADC_Vmux30": {
-                        "Unit": "Count",
+                    "Current": {
+                        "Unit": "A",
                         "Values": [
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0,
-                            0.0
-                        ],
-                        "X": false
-                    },
-                    "ADC_Vmux8": {
-                        "Unit": "Count",
-                        "Values": [
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765,
-                            7765
-                        ],
-                        "X": false
-                    },
-                    "DACs_input": {
-                        "Unit": "Count",
-                        "Values": [
-                            500.0,
-                            600.0,
-                            700.0,
-                            800.0,
-                            900.0,
-                            1000.0,
-                            1100.0,
-                            1200.0,
-                            1300.0,
-                            1400.0,
-                            1500.0,
-                            1600.0,
-                            1700.0,
-                            1800.0,
-                            1900.0,
-                            2000.0,
-                            2100.0,
-                            2200.0,
-                            2300.0,
-                            2400.0,
-                            2500.0,
-                            2600.0,
-                            2700.0,
-                            2800.0,
-                            2900.0,
-                            3000.0,
-                            3100.0,
-                            3200.0,
-                            3300.0,
-                            3400.0
+                            2.1,
+                            2.1,
+                            2.1
                         ],
                         "X": true
                     },
-                    "Vmux30": {
+                    "Imux0": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     },
-                    "Vmux8": {
+                    "Imux28": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux29": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux31": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Imux63": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "SetCurrent": {
+                        "Unit": "A",
+                        "Values": [
+                            2.1,
+                            2.1,
+                            2.1
+                        ],
+                        "X": false
+                    },
+                    "Temperature": {
+                        "Unit": "C",
+                        "Values": [
+                            29.2,
+                            29.2,
+                            29.2
+                        ],
+                        "X": false
+                    },
+                    "Vmux30": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux33": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux34": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux35": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux37": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux38": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
+                            6.191648388447707
+                        ],
+                        "X": false
+                    },
+                    "Vmux39": {
+                        "Unit": "V",
+                        "Values": [
                             6.191648388447707,
                             6.191648388447707,
                             6.191648388447707
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
+                    "AverageTemperature": 29.2,
                     "ChannelConfig": "",
                     "ChipConfigs": {
                         "RD53B": {
                             "GlobalConfig": {
                                 "AuroraActiveLanes": 1,
                                 "CmlBias0": 500,
                                 "CmlBias1": 100,
@@ -996,15 +856,14 @@
                                 "DiffPreampT": 500,
                                 "DiffPreampTL": 500,
                                 "DiffPreampTR": 500,
                                 "EnCoreCol0": 65535,
                                 "EnCoreCol1": 65535,
                                 "EnCoreCol2": 65535,
                                 "EnCoreCol3": 63,
-                                "InjVcalRange": 1,
                                 "MonitorI": 63,
                                 "MonitorV": 1,
                                 "SerEnLane": 1,
                                 "ServiceBlockEn": 1,
                                 "SldoTrimA": 8,
                                 "SldoTrimD": 5
                             },
@@ -1038,21 +897,22 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746823,
-                    "TimeStart": 1709746472
+                    "TimeEnd": 1712846840,
+                    "TimeStart": 1712846618,
+                    "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ADC_CALIBRATION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "UNDERSHUNT_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
-            "testType": "ADC_CALIBRATION"
+            "testType": "UNDERSHUNT_PROTECTION"
         }
     ]
 ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/ANALOG_READBACK/2024-03-06_173433/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/ANALOG_READBACK/2024-04-11_144351/20UPGXM1234567.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9909502036696582%*

 * *Differences: {'0': "{0: {'results': {'property': {'ANALOG_READBACK_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846635, 'TimeEnd': 1712848680}}}, 1: {'results': {'property': "*

 * *      "{'ANALOG_READBACK_MEASUREMENT_VERSION': '2.2.3'}, 'Measurements': {'Vmux2': {'Values': "*

 * *      '{insert: [(1, 5.690776913550724), (2, 5.690776913550724), (3, 5.690776913550724), (4, '*

 * *      '5.690776913550724), (5, 5.690776913550724), (6, 5.690776913550724), (7, 5.690776913550724), '*

 * *      '(8, 5.690776913550724),  […]*

```diff
@@ -450,21 +450,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746475,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712846635,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -926,83 +926,83 @@
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
                             5.690776913550724,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -1064,21 +1064,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709747101,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847632,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -2051,30 +2051,30 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724,
+                            5.690776913550724
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
                             5.690776913550724,
@@ -2180,21 +2180,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746856,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847244,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -2649,21 +2649,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746475,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712846635,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -3125,83 +3125,83 @@
                         ],
                         "X": false
                     },
                     "Vmux2": {
                         "Unit": "V",
                         "Values": [
                             6.3609321311585445,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     }
                 },
                 "Metadata": {
                     "ChannelConfig": "",
                     "ChipConfigs": {
@@ -3263,21 +3263,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709747101,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847632,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -4250,30 +4250,30 @@
                             15
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707,
-                            6.191648388447707
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445,
+                            6.3609321311585445
                         ],
                         "X": false
                     },
                     "Vmux34": {
                         "Unit": "V",
                         "Values": [
                             6.3609321311585445,
@@ -4379,21 +4379,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746856,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847244,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -4848,21 +4848,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746475,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712846635,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -5462,21 +5462,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709747101,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847632,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -6578,21 +6578,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746856,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847244,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ],
@@ -7047,21 +7047,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746475,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712846635,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VMEAS",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -7661,21 +7661,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709747101,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847632,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_TEMP",
             "testType": "ANALOG_READBACK"
         },
         {
@@ -8777,21 +8777,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709748628,
-                    "TimeStart": 1709746856,
+                    "TimeEnd": 1712848680,
+                    "TimeStart": 1712847244,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "ANALOG_READBACK_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "AR_VDD",
             "testType": "ANALOG_READBACK"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/DATA_TRANSMISSION/2024-03-06_173456/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/DATA_TRANSMISSION/2024-04-11_144358/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9912109375%*

 * *Differences: {'0': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846640, 'TimeEnd': 1712846649}}}}",*

 * * '1': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846640, 'TimeEnd': 1712846649}}}}",*

 * * '2': "{0: {'results': {'property': {'DATA_TRANSMISSION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846640, 'TimeEnd': 1712846649}}}}",*

 * * '3': "{0: {'results':  […]*

```diff
@@ -151,20 +151,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "Rx": [
                         2
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746505,
-                    "TimeStart": 1709746497
+                    "TimeEnd": 1712846649,
+                    "TimeStart": 1712846640
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -320,20 +320,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "Rx": [
                         1
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746505,
-                    "TimeStart": 1709746497
+                    "TimeEnd": 1712846649,
+                    "TimeStart": 1712846640
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -489,20 +489,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "Rx": [
                         0
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746505,
-                    "TimeStart": 1709746497
+                    "TimeEnd": 1712846649,
+                    "TimeStart": 1712846640
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ],
@@ -658,20 +658,20 @@
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "Rx": [
                         3
                     ],
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746505,
-                    "TimeStart": 1709746497
+                    "TimeEnd": 1712846649,
+                    "TimeStart": 1712846640
                 },
                 "comment": "",
                 "property": {
-                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "DATA_TRANSMISSION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "DATA_TRANSMISSION"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/INJECTION_CAPACITANCE/2024-03-06_173431/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/INJECTION_CAPACITANCE/2024-04-11_144353/20UPGXM1234567.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9908119658119658%*

 * *Differences: {'0': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Measurements': {'Vmux4': {'Values': {insert: [(0, 5.690776913550724)], delete: [0]}}, "*

 * *      "'Imux63': {'Values': [6.191648388447707, 6.191648388447707, 6.191648388447707, "*

 * *      "6.191648388447707, 6.191648388447707]}}, 'Metadata': {'TimeStart': 1712846636, 'TimeEnd': "*

 * *      '1712846859}}}}',*

 * * '1': "{0: {'results': {'property': {'INJECTION_CAPACITANCE_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Measureme […]*

```diff
@@ -24,19 +24,19 @@
                             5.690776913550724
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724,
-                            5.690776913550724
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
@@ -46,15 +46,15 @@
                             6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
+                            5.690776913550724,
                             5.690776913550724,
                             5.690776913550724,
                             5.690776913550724,
                             5.690776913550724
                         ],
                         "X": false
                     }
@@ -120,21 +120,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746659,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846859,
+                    "TimeStart": 1712846636,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -163,19 +163,19 @@
                             6.3609321311585445
                         ],
                         "X": false
                     },
                     "Imux63": {
                         "Unit": "V",
                         "Values": [
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445,
-                            6.3609321311585445
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707,
+                            6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux30": {
                         "Unit": "V",
                         "Values": [
                             6.191648388447707,
@@ -185,15 +185,15 @@
                             6.191648388447707
                         ],
                         "X": false
                     },
                     "Vmux4": {
                         "Unit": "V",
                         "Values": [
-                            6.191648388447707,
+                            6.3609321311585445,
                             6.3609321311585445,
                             6.3609321311585445,
                             6.3609321311585445,
                             6.3609321311585445
                         ],
                         "X": false
                     }
@@ -259,21 +259,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746659,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846859,
+                    "TimeStart": 1712846636,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -398,21 +398,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746659,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846859,
+                    "TimeStart": 1712846636,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ],
@@ -537,21 +537,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746659,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846859,
+                    "TimeStart": 1712846636,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "INJECTION_CAPACITANCE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "INJECTION_CAPACITANCE"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/IV_MEASURE/2024-03-06_173519/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/IV_MEASURE/2024-04-11_144408/20UPGXM1234567.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9884079371203214%*

 * *Differences: {'0': "{0: {'results': {'property': {'IV_MEASURE_MEASUREMENT_VERSION': '2.2.3'}, 'Measurements': "*

 * *      "{'time': {'Values': [3.4990110397338867, 10.654615640640259, 17.786351203918457, "*

 * *      '25.07872724533081, 32.36049175262451, 39.556445837020874, 46.76604914665222, '*

 * *      '54.03743767738342, 61.472991704940796, 68.75101113319397, 76.06875991821289, '*

 * *      '83.38463735580444, 90.61199283599854, 97.8469467163086, 105.29408407211304, '*

 * *      '113.04050135612488, 120.27624917030334, 127.51144671440125, […]*

```diff
@@ -101,102 +101,102 @@
                             0.0
                         ],
                         "X": false
                     },
                     "temperature": {
                         "Unit": "C",
                         "Values": [
-                            23.034,
-                            23.331,
-                            23.283,
-                            23.826,
-                            22.076,
-                            22.093,
-                            23.3,
-                            23.392,
-                            22.412,
-                            22.963,
-                            23.512,
-                            23.227,
-                            23.098,
-                            22.418,
-                            23.392,
-                            22.766,
-                            23.995,
-                            22.696,
-                            22.863,
-                            23.33,
-                            22.753,
-                            22.947,
-                            23.556,
-                            23.903,
-                            22.315,
-                            22.239,
-                            22.568,
-                            23.965,
-                            22.874,
-                            23.302,
-                            23.008,
-                            22.309,
+                            22.653,
+                            23.668,
+                            23.408,
+                            22.379,
+                            23.82,
+                            23.043,
+                            23.347,
                             22.894,
-                            23.89,
-                            22.5,
-                            22.568,
-                            23.032,
-                            23.574,
-                            23.617,
-                            23.36,
-                            22.106
+                            23.659,
+                            22.302,
+                            22.38,
+                            23.582,
+                            23.688,
+                            22.482,
+                            22.279,
+                            23.286,
+                            23.675,
+                            22.473,
+                            23.451,
+                            23.507,
+                            22.899,
+                            22.854,
+                            22.109,
+                            22.799,
+                            22.898,
+                            23.047,
+                            22.995,
+                            22.514,
+                            23.906,
+                            22.16,
+                            23.758,
+                            22.973,
+                            23.775,
+                            23.21,
+                            23.863,
+                            22.509,
+                            23.291,
+                            22.086,
+                            22.961,
+                            22.191,
+                            23.451
                         ],
                         "X": false
                     },
                     "time": {
                         "Unit": "s",
                         "Values": [
-                            3.852198362350464,
-                            11.97915267944336,
-                            20.28857111930847,
-                            28.26432776451111,
-                            36.66495680809021,
-                            45.253934383392334,
-                            53.639909982681274,
-                            62.261433601379395,
-                            70.71408796310425,
-                            79.2034637928009,
-                            87.30809903144836,
-                            95.49696040153503,
-                            103.7163360118866,
-                            111.60208010673523,
-                            119.79604744911194,
-                            127.79962372779846,
-                            135.94360280036926,
-                            144.07899975776672,
-                            152.22119402885437,
-                            160.42476224899292,
-                            168.6285457611084,
-                            176.79740929603577,
-                            184.7182652950287,
-                            192.97047090530396,
-                            201.05359816551208,
-                            209.33171367645264,
-                            217.71533298492432,
-                            225.662015914917,
-                            233.6281774044037,
-                            241.59542059898376,
-                            249.44944739341736,
-                            257.5624632835388,
-                            265.96672916412354,
-                            274.28706336021423,
-                            282.65309476852417,
-                            290.86373829841614,
-                            299.05615520477295,
-                            307.31417322158813,
-                            315.46597814559937,
-                            323.70287227630615,
-                            331.9319450855255
+                            3.4990110397338867,
+                            10.654615640640259,
+                            17.786351203918457,
+                            25.07872724533081,
+                            32.36049175262451,
+                            39.556445837020874,
+                            46.76604914665222,
+                            54.03743767738342,
+                            61.472991704940796,
+                            68.75101113319397,
+                            76.06875991821289,
+                            83.38463735580444,
+                            90.61199283599854,
+                            97.8469467163086,
+                            105.29408407211304,
+                            113.04050135612488,
+                            120.27624917030334,
+                            127.51144671440125,
+                            134.82101464271545,
+                            142.05521869659424,
+                            149.34129238128662,
+                            156.61187052726746,
+                            163.7993233203888,
+                            171.07467675209045,
+                            178.46036911010742,
+                            185.7854447364807,
+                            193.07947754859924,
+                            200.4380919933319,
+                            207.71494221687317,
+                            215.1624174118042,
+                            222.56464743614197,
+                            229.97363090515137,
+                            237.36760926246643,
+                            244.63192176818848,
+                            251.95480060577393,
+                            259.28730869293213,
+                            266.64627504348755,
+                            273.89922976493835,
+                            281.20752596855164,
+                            288.4393994808197,
+                            295.69199085235596
                         ],
                         "X": false
                     },
                     "voltage": {
                         "Unit": "V",
                         "Values": [
                             0.0,
@@ -241,25 +241,25 @@
                             -195.0,
                             -200.0
                         ],
                         "X": true
                     }
                 },
                 "Metadata": {
-                    "AverageTemperature": 23.03139024390244,
+                    "AverageTemperature": 23.02987804878049,
                     "DepletionVoltage": null,
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "SettlingTime": 2,
-                    "TimeEnd": 1709746946,
-                    "TimeStart": 1709746520
+                    "TimeEnd": 1712847025,
+                    "TimeStart": 1712846649
                 },
                 "comment": "",
                 "property": {
-                    "IV_MEASURE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "IV_MEASURE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "20UPGXM1234567",
             "subtestType": "",
             "testType": "IV_MEASURE"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/LP_MODE/2024-03-06_173457/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/LP_MODE/2024-04-11_144406/20UPGXM1234567.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {'0': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846647, 'TimeEnd': 1712846767}}}}",*

 * * '1': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846647, 'TimeEnd': 1712846767}}}}",*

 * * '2': "{0: {'results': {'property': {'LP_MODE_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846647, 'TimeEnd': 1712846767}}}}",*

 * * '3': "{0: {'results': {'property': {'LP_MODE_MEASURE […]*

```diff
@@ -164,21 +164,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746631,
-                    "TimeStart": 1709746497,
+                    "TimeEnd": 1712846767,
+                    "TimeStart": 1712846647,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -347,21 +347,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746631,
-                    "TimeStart": 1709746497,
+                    "TimeEnd": 1712846767,
+                    "TimeStart": 1712846647,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -530,21 +530,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746631,
-                    "TimeStart": 1709746498,
+                    "TimeEnd": 1712846767,
+                    "TimeStart": 1712846647,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ],
@@ -713,21 +713,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746631,
-                    "TimeStart": 1709746498,
+                    "TimeEnd": 1712846767,
+                    "TimeStart": 1712846647,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "LP_MODE_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "LP_MODE_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "LP_MODE"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/OVERVOLTAGE_PROTECTION/2024-03-06_173433/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/OVERVOLTAGE_PROTECTION/2024-04-11_144333/20UPGXM1234567.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {'0': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846614, 'TimeEnd': 1712846665}}}}",*

 * * '1': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846614, 'TimeEnd': 1712846665}}}}",*

 * * '2': "{0: {'results': {'property': {'OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION': '2.2.3'}, "*

 * *      "'Metadata': {'TimeStart': 1712846614, 'TimeEnd': 1712846665}}}}",*

 * * '3': "{ […]*

```diff
@@ -136,21 +136,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746525,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846665,
+                    "TimeStart": 1712846614,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -291,21 +291,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746525,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846665,
+                    "TimeStart": 1712846614,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -446,21 +446,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746525,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846665,
+                    "TimeStart": 1712846614,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ],
@@ -601,21 +601,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709746525,
-                    "TimeStart": 1709746473,
+                    "TimeEnd": 1712846665,
+                    "TimeStart": 1712846614,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "OVERVOLTAGE_PROTECTION_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "OVERVOLTAGE_PROTECTION"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/Measurements/SLDO/2024-03-06_173447/20UPGXM1234567.json` & `module_qc_tools-2.2.3/Measurements/SLDO/2024-04-11_144328/20UPGXM1234567.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9910714285714286%*

 * *Differences: {'0': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846609, 'TimeEnd': 1712848244}}}}",*

 * * '1': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846609, 'TimeEnd': 1712848244}}}}",*

 * * '2': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION': '2.2.3'}, 'Metadata': "*

 * *      "{'TimeStart': 1712846609, 'TimeEnd': 1712848244}}}}",*

 * * '3': "{0: {'results': {'property': {'SLDO_MEASUREMENT_VERSION […]*

```diff
@@ -466,21 +466,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip1",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709749176,
-                    "TimeStart": 1709746488,
+                    "TimeEnd": 1712848244,
+                    "TimeStart": 1712846609,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "SLDO_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip1",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -951,21 +951,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip2",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709749176,
-                    "TimeStart": 1709746488,
+                    "TimeEnd": 1712848244,
+                    "TimeStart": 1712846609,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "SLDO_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip2",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1436,21 +1436,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip3",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709749176,
-                    "TimeStart": 1709746488,
+                    "TimeEnd": 1712848244,
+                    "TimeStart": 1712846609,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "SLDO_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip3",
             "subtestType": "",
             "testType": "SLDO"
         }
     ],
@@ -1921,21 +1921,21 @@
                     "FirmwareIdentifier": "",
                     "FirmwareVersion": "",
                     "Institution": "TEST",
                     "ModuleSN": "20UPGXM1234567",
                     "Name": "dummy_chip4",
                     "SoftwareType": "",
                     "SoftwareVersion": "",
-                    "TimeEnd": 1709749176,
-                    "TimeStart": 1709746488,
+                    "TimeEnd": 1712848244,
+                    "TimeStart": 1712846609,
                     "useCalibAdc": false
                 },
                 "comment": "",
                 "property": {
-                    "SLDO_MEASUREMENT_VERSION": "2.2.2rc3"
+                    "SLDO_MEASUREMENT_VERSION": "2.2.3"
                 }
             },
             "serialNumber": "dummy_chip4",
             "subtestType": "",
             "testType": "SLDO"
         }
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/emulator/README.md` & `module_qc_tools-2.2.3/emulator/README.md`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/ADC_CALIBRATION.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/ADC_CALIBRATION.py`

 * *Files 3% similar despite different names*

```diff
@@ -77,14 +77,28 @@
         adc_calib_config["Range"]["step"],
     ]
     DACs = np.arange(start=Range[0], stop=Range[1], step=Range[2])
 
     # Check ADC ground
     check_adc_ground(yr, adc_calib_config)
 
+    # Measure ground
+    vmux_value_GNDA = adc_calib_config["MonitorV_GND"]
+    gnd_vmux = read_vmux(
+        meter, yr, adc_calib_config, v_mux=vmux_value_GNDA, use_adc=False
+    )
+    gnd_adc = read_vmux(
+        meter,
+        yr,
+        adc_calib_config,
+        v_mux=vmux_value_GNDA,
+        use_adc=True,
+        raw_adc_counts=True,
+    )
+
     for DAC in DACs:
         yr.write_register("InjVcalMed", DAC)  # write DAC values
         v_mea = [{} for _ in range(yr._number_of_chips)]
 
         for _i, vmux_value in enumerate(MonitorV):
             mea_chips_vmux = read_vmux(
                 meter, yr, adc_calib_config, v_mux=vmux_value, use_adc=False
@@ -100,14 +114,16 @@
 
             for chip in range(yr._number_of_chips):
                 if chip in yr._disabled_chip_positions:
                     continue
 
                 v_mea[chip][f"Vmux{vmux_value}"] = [mea_chips_vmux[chip]]
                 v_mea[chip][f"ADC_Vmux{vmux_value}"] = [mea_chips_adc[chip]]
+                v_mea[chip][f"Vmux{vmux_value_GNDA}"] = [gnd_vmux[chip]]
+                v_mea[chip][f"ADC_Vmux{vmux_value_GNDA}"] = [gnd_adc[chip]]
 
         # Add data to frame
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
             v_mea[chip]["DACs_input"] = [float(DAC)]
             data[chip].add_data(v_mea[chip])
@@ -200,19 +216,35 @@
 
     InjVcalRange = adc_calib_config["InjVcalRange"]
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
             columns=["DACs_input"]
-            + [f"Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]]
-            + [f"ADC_Vmux{v_mux}" for v_mux in adc_calib_config["MonitorV"]],
+            + [
+                f"Vmux{v_mux}"
+                for v_mux in adc_calib_config["MonitorV"]
+                + [adc_calib_config["MonitorV_GND"]]
+            ]
+            + [
+                f"ADC_Vmux{v_mux}"
+                for v_mux in adc_calib_config["MonitorV"]
+                + [adc_calib_config["MonitorV_GND"]]
+            ],
             units=["Count"]
-            + ["V" for v_mux in adc_calib_config["MonitorV"]]
-            + ["Count" for v_mux in adc_calib_config["MonitorV"]],
+            + [
+                "V"
+                for v_mux in adc_calib_config["MonitorV"]
+                + [adc_calib_config["MonitorV_GND"]]
+            ]
+            + [
+                "Count"
+                for v_mux in adc_calib_config["MonitorV"]
+                + [adc_calib_config["MonitorV_GND"]]
+            ],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/ANALOG_READBACK.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/ANALOG_READBACK.py`

 * *Files 10% similar despite different names*

```diff
@@ -70,14 +70,37 @@
             analog_readback_config["i_config"][layer],
         )  # Only for emulator do the emulation of power on/off.
         # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
 
     # Set and measure current for power supply
     i_mea = [{} for _ in range(yr._number_of_chips)]
 
+    # Measure ground once.
+    vmux_value_gnd = analog_readback_config["v_mux_gnd"]
+    vmux_gnd = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        v_mux=vmux_value_gnd,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+    imux_value_gnd = analog_readback_config["i_mux_gnd"]
+    imux_gnd = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        i_mux=imux_value_gnd,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+    for chip in range(yr._number_of_chips):
+        if chip in yr._disabled_chip_positions:
+            continue
+        i_mea[chip][f"Vmux{vmux_value_gnd}"] = [vmux_gnd[chip]]
+        i_mea[chip][f"Imux{imux_value_gnd}"] = [imux_gnd[chip]]
+
     # measure v_mux
     for v_mux in analog_readback_config["v_mux"]:
         mea_chips = read_vmux(
             meter,
             yr,
             analog_readback_config,
             v_mux=v_mux,
@@ -154,16 +177,31 @@
     }
     dem_maps = {
         14: "MonSensSldoAnaDem",
         16: "MonSensSldoDigDem",
         18: "MonSensAcbDem",
     }
 
-    # Measure external external NTC
-    mea_ntc, _status = nt.read()
+    # Measure ground once.
+    vmux_value_gnd = analog_readback_config["v_mux_gnd"]
+    vmux_gnd = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        v_mux=vmux_value_gnd,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+    imux_value_gnd = analog_readback_config["i_mux_gnd"]
+    imux_gnd = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        i_mux=imux_value_gnd,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
 
     i_mea = [{} for _ in range(yr._number_of_chips)]
     # Measure v_mux_tempmeas
     for v_mux in analog_readback_config["v_mux_tempsens"]:
         yr.enable_tempsens(v_mux=v_mux)
         for bias in analog_readback_config[bias_maps[v_mux]]:
             yr.set_tempsens_bias(v_mux=v_mux, bias=bias)
@@ -189,53 +227,50 @@
                     # Record vmux, bias, and dem.
                     i_mea[chip][f"Vmux{v_mux}"] = [mea_chips[chip]]
                     i_mea[chip][bias_maps[v_mux]] = [bias]
                     i_mea[chip][dem_maps[v_mux]] = [dem]
 
                     data[chip].add_data(i_mea[chip])
     yr.reset_tempsens()
-    # Measure v_mux_ntc 32 times.
+
+    # Measure NTCs
+    # Measure external external (flex) NTC
+    mea_ntc, _status = nt.read()
+    # Measure external (chip) NTCs
+    v_mux_value_ntc = analog_readback_config["v_mux_ntc"]
+    v_mux_ntc = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        v_mux=v_mux_value_ntc,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+    i_mux_value_ntc = analog_readback_config["i_mux_ntc"]
+    i_mux_ntc = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        i_mux=i_mux_value_ntc,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+
     max_n_measure = max(len(d["Vmux14"]) if d else 0 for d in data)
     n_measure = 0
-    log.debug(f"Measuring v_mux_ntc {max_n_measure} times")
     while n_measure < max_n_measure:
         # Clear dictionary to hold data
         i_mea = [{} for _ in range(yr._number_of_chips)]
-        for v_mux in analog_readback_config["v_mux_ntc"]:
-            mea_chips = read_vmux(
-                meter,
-                yr,
-                analog_readback_config,
-                v_mux=v_mux,
-                use_adc=analog_readback_config["use_calib_adc"],
-            )
-            for chip in range(yr._number_of_chips):
-                if chip in yr._disabled_chip_positions:
-                    continue
-                i_mea[chip][f"Vmux{v_mux}"] = [mea_chips[chip]]
-
-        for i_mux in analog_readback_config["i_mux_ntc"]:
-            mea_chips = read_vmux(
-                meter,
-                yr,
-                analog_readback_config,
-                i_mux=i_mux,
-                use_adc=analog_readback_config["use_calib_adc"],
-            )
-            for chip in range(yr._number_of_chips):
-                if chip in yr._disabled_chip_positions:
-                    continue
-                i_mea[chip][f"Imux{i_mux}"] = [mea_chips[chip]]
-
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
+            i_mea[chip][f"Vmux{v_mux_value_ntc}"] = [v_mux_ntc[chip]]
+            i_mea[chip][f"Vmux{vmux_value_gnd}"] = [vmux_gnd[chip]]
+            i_mea[chip][f"Imux{i_mux_value_ntc}"] = [i_mux_ntc[chip]]
+            i_mea[chip][f"Imux{imux_value_gnd}"] = [imux_gnd[chip]]
             i_mea[chip]["TExtExtNTC"] = [mea_ntc]
             data[chip].add_data(i_mea[chip])
-
         n_measure += 1
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         log.info(
             "--------------------------------------------------------------------------"
@@ -277,14 +312,24 @@
 
     # Trim to Vmux mapping
     vmux_to_trim = {
         34: "SldoTrimA",
         38: "SldoTrimD",
     }
 
+    # Measure ground once.
+    vmux_value_gnd = analog_readback_config["v_mux_gnd"]
+    vmux_gnd = read_vmux(
+        meter,
+        yr,
+        analog_readback_config,
+        v_mux=vmux_value_gnd,
+        use_adc=analog_readback_config["use_calib_adc"],
+    )
+
     # Measure VDDA/VDDD and ROSC vs SldoTrimA/SldoTrimD
     for v_mux, trim_name in vmux_to_trim.items():
         # Reset i_mea
         i_mea = [{} for _ in range(yr._number_of_chips)]
 
         # Read initial Trim in chip config
         config_trim, _status = yr.read_register(name=trim_name)
@@ -337,30 +382,26 @@
                 f"[run_AnalogReadBack] Set VMUX{v_mux} back to default and re-running \U0001F441  diagram."
             )
             yr.write_register(
                 name=trim_name, value=config_trim[chip], chip_position=chip
             )
             _eye, _status = yr.eyeDiagram(skipconfig=True)
 
-    # Measure ground once.
-    mea_chips = read_vmux(
-        meter,
-        yr,
-        analog_readback_config,
-        v_mux=30,
-        use_adc=analog_readback_config["use_calib_adc"],
-    )
+    # Add ground measurements.
     max_n_measure = max(len(d["Vmux34"]) if d else 0 for d in data)
-    log.debug(f"Measuring Vmux30 for VDDA/VDDD measurement {max_n_measure} times")
-    for _nmeas in range(max_n_measure):
+    n_measure = 0
+    while n_measure < max_n_measure:
+        # Clear dictionary to hold data
+        i_mea = [{} for _ in range(yr._number_of_chips)]
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
-            i_mea[chip]["Vmux30"] = [mea_chips[chip]]
+            i_mea[chip][f"Vmux{vmux_value_gnd}"] = [vmux_gnd[chip]]
             data[chip].add_data(i_mea[chip])
+        n_measure += 1
 
     log.info("[run_AnalogReadBack] VDDA/VDDD measurement done!")
     log.info(
         f"[run_AnalogReadBack] TimeEnd: {datetime.now().strftime('%Y-%m-%d_%H%M%S')}"
     )
 
 
@@ -469,36 +510,76 @@
     output_dir.mkdir(parents=True, exist_ok=True)
     log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
 
     data = [
         qcDataFrame(
-            columns=[f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in analog_readback_config["i_mux"]],
-            units=["V" for v_mux in analog_readback_config["v_mux"]]
-            + ["V" for i_mux in analog_readback_config["i_mux"]],
+            columns=[
+                f"Vmux{v_mux}"
+                for v_mux in analog_readback_config["v_mux"]
+                + [analog_readback_config["v_mux_gnd"]]
+            ]
+            + [
+                f"Imux{i_mux}"
+                for i_mux in analog_readback_config["i_mux"]
+                + [analog_readback_config["i_mux_gnd"]]
+            ],
+            units=[
+                "V"
+                for v_mux in analog_readback_config["v_mux"]
+                + [analog_readback_config["v_mux_gnd"]]
+            ]
+            + [
+                "V"
+                for i_mux in analog_readback_config["i_mux"]
+                + [analog_readback_config["i_mux_gnd"]]
+            ],
         )
         for input_file in input_files
     ]
 
     data_tempmeas = [
         qcDataFrame(
-            columns=[f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux_ntc"]]
-            + [f"Imux{i_mux}" for i_mux in analog_readback_config["i_mux_ntc"]]
+            columns=[
+                f"Vmux{v_mux}"
+                for v_mux in [
+                    analog_readback_config["v_mux_ntc"],
+                    analog_readback_config["v_mux_gnd"],
+                ]
+            ]
+            + [
+                f"Imux{i_mux}"
+                for i_mux in [
+                    analog_readback_config["i_mux_ntc"],
+                    analog_readback_config["i_mux_gnd"],
+                ]
+            ]
             + [f"Vmux{v_mux}" for v_mux in analog_readback_config["v_mux_tempsens"]]
             + ["MonSensSldoAnaSelBias"]
             + ["MonSensSldoDigSelBias"]
             + ["MonSensAcbSelBias"]
             + ["MonSensSldoAnaDem"]
             + ["MonSensSldoDigDem"]
             + ["MonSensAcbDem"]
             + ["TExtExtNTC"],
-            units=["V" for v_mux in analog_readback_config["v_mux_ntc"]]
-            + ["V" for i_mux in analog_readback_config["i_mux_ntc"]]
+            units=[
+                "V"
+                for v_mux in [
+                    analog_readback_config["v_mux_ntc"],
+                    analog_readback_config["v_mux_gnd"],
+                ]
+            ]
+            + [
+                "V"
+                for i_mux in [
+                    analog_readback_config["i_mux_ntc"],
+                    analog_readback_config["i_mux_gnd"],
+                ]
+            ]
             + ["V" for v_mux in analog_readback_config["v_mux_tempsens"]]
             + ["-"]
             + ["-"]
             + ["-"]
             + ["-"]
             + ["-"]
             + ["-"]
@@ -507,15 +588,15 @@
         for input_file in input_files
     ]
 
     data_vdda_vddd_vs_trim = [
         qcDataFrame(
             columns=["Vmux34"]
             + ["Vmux38"]
-            + ["Vmux30"]
+            + [f"Vmux{analog_readback_config['v_mux_gnd']}"]
             + ["SldoTrimA"]
             + ["SldoTrimD"]
             + [f"ROSC{i}" for i in range(42)],
             units=["V"] + ["V"] + ["V"] + ["-"] + ["-"] + ["MHz" for i in range(42)],
         )
         for input_file in input_files
     ]
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/DATA_TRANSMISSION.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/DATA_TRANSMISSION.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 
 import numpy as np
 import pandas as pd
 import pkg_resources
 import typer
 from module_qc_data_tools import (
     get_env,
+    get_layer_from_sn,
     get_nlanes_from_sn,
     get_sn_from_connectivity,
     outputDataFrame,
     qcDataFrame,
     save_dict_list,
 )
 
@@ -27,28 +28,36 @@
 from module_qc_tools.utils.misc import (
     bcolors,
     check_meas_config,
     get_identifiers,
     get_meta_data,
 )
 from module_qc_tools.utils.ntc import ntc
+from module_qc_tools.utils.power_supply import power_supply
 from module_qc_tools.utils.yarr import yarr
 
 if sys.version_info >= (3, 9):
     from importlib import resources
 else:
     import importlib_resources as resources
 
 logging.basicConfig(level=logging.INFO)
 log = logging.getLogger("measurement")
 
 app = typer.Typer(context_settings=CONTEXT_SETTINGS)
 
 
-def run(data, metadata, DT_config, yr, nt, log_file, dryrun, n_lanes_per_chip):
+def run(
+    data, metadata, DT_config, ps, yr, nt, layer, log_file, dryrun, n_lanes_per_chip
+):
+    if yr.running_emulator():
+        ps.on(v=DT_config["v_max"], i=DT_config["i_config"][layer])
+        # Only for emulator do the emulation of power on/off
+        # For real measurements avoid turn on/off the chip by commands. Just leave the chip running.
+
     _status = yr.configure()
     meas = [{} for _ in range(yr._number_of_chips)]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
         for value in DT_config["MonitorV"]:
@@ -158,25 +167,27 @@
     # connectivity for emulator is defined in config, not true when running on module (on purpose)
     if "emulator" not in str(config_path) and not module_connectivity:
         typer.echo("must supply path to connectivity file [-m --module-connectivity]")
         raise typer.Exit(2)
 
     DT_config = config["tasks"]["GENERAL"]
     DT_config.update(config["tasks"]["DATA_TRANSMISSION"])
+    ps = power_supply(config["power_supply"])
     yr = yarr(config["yarr"])
 
     nt = ntc(config["ntc"])
 
     if not use_pixel_config:
         yr.omit_pixel_config("tmp")
 
     # Define identifires for the output files.
     # Taking the module SN from YARR path to config in the connectivity file.
     # Taking the test-type from the script name which is the test-code in ProdDB.
     module_serial = get_sn_from_connectivity(config["yarr"]["connectivity"])
+    layer = get_layer_from_sn(module_serial)
     test_type = Path(__file__).stem
     institution = get_env("INSTITUTION")
     if site and institution is not None:
         log.warning(
             bcolors.WARNING
             + f" Overwriting default institution {institution} with manual input {site}!"
             + bcolors.ENDC
@@ -189,14 +200,16 @@
         log.error(
             bcolors.ERROR
             + 'No institution found. Please specify your testing site as an environmental variable "INSTITUTION" or specify with the --site option. '
             + bcolors.ENDC
         )
         return
 
+    ps.set(v=DT_config["v_max"], i=DT_config["i_config"][layer])
+
     # # if -o option used, overwrite the default output directory
     output_dir = module_connectivity.parent if module_connectivity else base_output_dir
 
     if base_output_dir != Path("outputs"):
         output_dir = base_output_dir
 
     output_dir = output_dir.joinpath("Measurements", test_type, timestart)
@@ -239,16 +252,18 @@
         )
 
     try:
         run(
             data,
             metadata,
             DT_config,
+            ps,
             yr,
             nt,
+            layer,
             log_file,
             dryrun,
             n_lanes_per_chip,
         )
     except KeyboardInterrupt:
         log.info("KeyboardInterrupt")
         yr.remove_tmp_connectivity()
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/INJECTION_CAPACITANCE.py`

 * *Files 8% similar despite different names*

```diff
@@ -67,14 +67,32 @@
     status = yr.configure()
     assert status >= 0
 
     # Check ADC ground
     if inj_cap_config["use_calib_adc"]:
         check_adc_ground(yr, inj_cap_config)
 
+    # Measure ground
+    vmux_value_gnd = inj_cap_config["v_mux_gnd"]
+    vmux_gnd = read_vmux(
+        meter,
+        yr,
+        inj_cap_config,
+        v_mux=vmux_value_gnd,
+        use_adc=inj_cap_config["use_calib_adc"],
+    )
+    imux_value_gnd = inj_cap_config["i_mux_gnd"]
+    imux_gnd = read_vmux(
+        meter,
+        yr,
+        inj_cap_config,
+        i_mux=imux_value_gnd,
+        use_adc=inj_cap_config["use_calib_adc"],
+    )
+
     for _i in range(inj_cap_config["n_meas"]):
         v_mea = [{} for _ in range(yr._number_of_chips)]
 
         # Disable both capmeasure and parasitic circuits
         yr.write_register("CapMeasEn", 0)
         yr.write_register("CapMeasEnPar", 0)
 
@@ -113,14 +131,21 @@
                 use_adc=inj_cap_config["use_calib_adc"],
             )
             for chip in range(yr._number_of_chips):
                 if chip in yr._disabled_chip_positions:
                     continue
                 v_mea[chip][f"Imux{imux_value}"] = [mea_chips[chip]]
 
+        # Add ground values
+        for chip in range(yr._number_of_chips):
+            if chip in yr._disabled_chip_positions:
+                continue
+            v_mea[chip][f"Vmux{vmux_value_gnd}"] = [vmux_gnd[chip]]
+            v_mea[chip][f"Imux{imux_value_gnd}"] = [imux_gnd[chip]]
+
         for chip in range(yr._number_of_chips):
             if chip in yr._disabled_chip_positions:
                 continue
             data[chip].add_data(v_mea[chip])
 
     if yr.running_emulator():
         ps.off()
@@ -206,18 +231,28 @@
     # Make output directory and start log file
     output_dir.mkdir(parents=True, exist_ok=True)
     log.addHandler(logging.FileHandler(output_dir.joinpath("output.log")))
 
     input_files = [None] * yr._number_of_chips
     data = [
         qcDataFrame(
-            columns=[f"Vmux{v_mux}" for v_mux in inj_cap_config["v_mux"]]
-            + [f"Imux{i_mux}" for i_mux in inj_cap_config["i_mux"]],
-            units=["V" for v_mux in inj_cap_config["v_mux"]]
-            + ["V" for i_mux in inj_cap_config["i_mux"]],
+            columns=[
+                f"Vmux{v_mux}"
+                for v_mux in inj_cap_config["v_mux"] + [inj_cap_config["v_mux_gnd"]]
+            ]
+            + [
+                f"Imux{i_mux}"
+                for i_mux in inj_cap_config["i_mux"] + [inj_cap_config["i_mux_gnd"]]
+            ],
+            units=[
+                "V" for v_mux in inj_cap_config["v_mux"] + [inj_cap_config["v_mux_gnd"]]
+            ]
+            + [
+                "V" for i_mux in inj_cap_config["i_mux"] + [inj_cap_config["i_mux_gnd"]]
+            ],
         )
         for input_file in input_files
     ]
 
     for chip in range(yr._number_of_chips):
         if chip in yr._disabled_chip_positions:
             continue
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/IV_MEASURE.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/IV_MEASURE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/LP_MODE.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/LP_MODE.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/OVERVOLTAGE_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/SLDO.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/SLDO.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/UNDERSHUNT_PROTECTION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/VCAL_CALIBRATION.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/VCAL_CALIBRATION.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/globals.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/globals.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/hardware_emulator.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/hardware_emulator.py`

 * *Files 0% similar despite different names*

```diff
@@ -669,15 +669,24 @@
 
     T = module_state["temperature"]
     sys.stdout.write(f"{T}")
     raise typer.Exit(0)
 
 
 @app.command()
-def switchLPM(_: PSAction):
+def switchLPM(
+    _specNum: int = typer.Option(
+        0,
+        "-s",
+        help="Spec card number",
+    ),
+    _action: str = typer.Argument(
+        help="Action (on/off)",
+    ),
+):
     raise typer.Exit(0)
 
 
 def run_scanConsole():
     typer.run(scanConsole)
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/main.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/main.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/cli/upload_localdb.py` & `module_qc_tools-2.2.3/src/module_qc_tools/cli/upload_localdb.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,15 @@
             data = response.json()
 
             log.info(data)
 
         except Exception as err:
             log.error("failure in uploading!")
             log.error(err)
+            log.error(response.json())
             raise typer.Exit(1) from err
 
         log.info(
             f"\nDone! LocalDB has accepted the following {len(data)} TestRun results"
         )
         for testRun in data:
             if testRun is None:
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/emulator_merged_vmux.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/emulator_merged_vmux.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9921203703703704%*

 * *Differences: {"'tasks'": "{'ADC_CALIBRATION': {'MonitorV': {delete: [1]}, 'Range': {'step': 200}, "*

 * *            "'MonitorV_GND': 30}, 'SLDO': {'i_max': {'L1': 9.8}, 'n_points': {'L1': 17}}, "*

 * *            "'VCAL_CALIBRATION': {'Large_Range': {'step': 200}, 'Small_Range': {'step': 200}}, "*

 * *            "'ANALOG_READBACK': {'v_mux': {delete: [14]}, 'i_mux': {delete: [29]}, 'v_mux_ntc': 2, "*

 * *            "'i_mux_ntc': 9, 'v_mux_gnd': 30, 'i_mux_gnd': 63}, 'INJECTION_CAPACITANCE': {'v_mux': "*

 * *            "{delete: [1]}, 'i_mux […]*

```diff
@@ -34,20 +34,20 @@
         "success_code": 0,
         "timeout": 30
     },
     "tasks": {
         "ADC_CALIBRATION": {
             "InjVcalRange": 1,
             "MonitorV": [
-                8,
-                30
+                8
             ],
+            "MonitorV_GND": 30,
             "Range": {
                 "start": 500,
-                "step": 100,
+                "step": 200,
                 "stop": 3500
             }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
@@ -175,21 +175,18 @@
                 22,
                 23,
                 24,
                 25,
                 28,
                 29,
                 30,
-                31,
-                63
-            ],
-            "i_mux_ntc": [
-                9,
-                63
+                31
             ],
+            "i_mux_gnd": 63,
+            "i_mux_ntc": 9,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -197,30 +194,27 @@
                 9,
                 10,
                 11,
                 12,
                 13,
                 15,
                 17,
-                30,
                 31,
                 32,
                 33,
                 34,
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_ntc": [
-                2,
-                30
-            ],
+            "v_mux_gnd": 30,
+            "v_mux_ntc": 2,
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
         "DATA_TRANSMISSION": {
@@ -242,22 +236,22 @@
                 0,
                 0
             ]
         },
         "INJECTION_CAPACITANCE": {
             "i_mux": [
                 10,
-                11,
-                63
+                11
             ],
+            "i_mux_gnd": 63,
             "n_meas": 5,
             "v_mux": [
-                4,
-                30
-            ]
+                4
+            ],
+            "v_mux_gnd": 30
         },
         "IV_MEASURE": {
             "i_max": {
                 "L0": 0.0001,
                 "L1": 0.0001,
                 "L2": 0.0001
             },
@@ -328,15 +322,15 @@
                 37
             ]
         },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
-                "L1": 10.6,
+                "L1": 9.8,
                 "L2": 9.48
             },
             "i_min": {
                 "L0": 5.55,
                 "L1": 6.6,
                 "L2": 5.88
             },
@@ -346,15 +340,15 @@
                 29,
                 30,
                 31,
                 63
             ],
             "n_points": {
                 "L0": 22,
-                "L1": 21,
+                "L1": 17,
                 "L2": 19
             },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
@@ -391,32 +385,32 @@
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
             "Large_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             },
             "MonitorV": [
                 8,
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "connectivity": "src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json",
-        "controller": "configs/controller/emuCfg_rd53a.json",
+        "controller": "src/module_qc_tools/data/emulator/configs/controller/specCfg-rd53b.json",
         "eyeDiagram_exe": "emulator-eye-diagram",
         "lpm_digitalscan": "configs/scans/rd53b/lpm_digitalscan.json",
         "read_adc_exe": "emulator-read-adc",
         "read_register_exe": "emulator-read-register",
         "read_ringosc_exe": "emulator-read-ringosc",
         "run_dir": "emulator",
         "scanConsole_exe": "emulator-scanConsole",
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/example_merged_vmux.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_merged_vmux.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959082491582492%*

 * *Differences: {"'tasks'": "{'ADC_CALIBRATION': {'MonitorV': {delete: [1]}, 'Range': {'step': 200}, "*

 * *            "'MonitorV_GND': 30}, 'SLDO': {'i_max': {'L1': 9.8}, 'n_points': {'L1': 17}}, "*

 * *            "'VCAL_CALIBRATION': {'Large_Range': {'step': 200}, 'Small_Range': {'step': 200}}, "*

 * *            "'ANALOG_READBACK': {'v_mux': {delete: [14]}, 'i_mux': {delete: [29]}, 'v_mux_ntc': 2, "*

 * *            "'i_mux_ntc': 9, 'v_mux_gnd': 30, 'i_mux_gnd': 63}, 'INJECTION_CAPACITANCE': {'v_mux': "*

 * *            "{delete: [1]}, 'i_mux […]*

```diff
@@ -41,20 +41,20 @@
         "success_code": 0,
         "timeout": 30
     },
     "tasks": {
         "ADC_CALIBRATION": {
             "InjVcalRange": 1,
             "MonitorV": [
-                8,
-                30
+                8
             ],
+            "MonitorV_GND": 30,
             "Range": {
                 "start": 500,
-                "step": 100,
+                "step": 200,
                 "stop": 3500
             }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
@@ -182,21 +182,18 @@
                 22,
                 23,
                 24,
                 25,
                 28,
                 29,
                 30,
-                31,
-                63
-            ],
-            "i_mux_ntc": [
-                9,
-                63
+                31
             ],
+            "i_mux_gnd": 63,
+            "i_mux_ntc": 9,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -204,30 +201,27 @@
                 9,
                 10,
                 11,
                 12,
                 13,
                 15,
                 17,
-                30,
                 31,
                 32,
                 33,
                 34,
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_ntc": [
-                2,
-                30
-            ],
+            "v_mux_gnd": 30,
+            "v_mux_ntc": 2,
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
         "DATA_TRANSMISSION": {
@@ -249,22 +243,22 @@
                 0,
                 0
             ]
         },
         "INJECTION_CAPACITANCE": {
             "i_mux": [
                 10,
-                11,
-                63
+                11
             ],
+            "i_mux_gnd": 63,
             "n_meas": 5,
             "v_mux": [
-                4,
-                30
-            ]
+                4
+            ],
+            "v_mux_gnd": 30
         },
         "IV_MEASURE": {
             "i_max": {
                 "L0": 0.0001,
                 "L1": 0.0001,
                 "L2": 0.0001
             },
@@ -336,15 +330,15 @@
                 37
             ]
         },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
-                "L1": 10.6,
+                "L1": 9.8,
                 "L2": 9.48
             },
             "i_min": {
                 "L0": 5.55,
                 "L1": 6.6,
                 "L2": 5.88
             },
@@ -354,15 +348,15 @@
                 29,
                 30,
                 31,
                 63
             ],
             "n_points": {
                 "L0": 22,
-                "L1": 21,
+                "L1": 17,
                 "L2": 19
             },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
@@ -399,25 +393,25 @@
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
             "Large_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             },
             "MonitorV": [
                 8,
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
         "eyeDiagram_exe": "./bin/eyeDiagram",
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/configs/example_separate_vmux.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/configs/example_separate_vmux.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9959082491582492%*

 * *Differences: {"'tasks'": "{'ADC_CALIBRATION': {'MonitorV': {delete: [1]}, 'Range': {'step': 200}, "*

 * *            "'MonitorV_GND': 30}, 'SLDO': {'i_max': {'L1': 9.8}, 'n_points': {'L1': 17}}, "*

 * *            "'VCAL_CALIBRATION': {'Large_Range': {'step': 200}, 'Small_Range': {'step': 200}}, "*

 * *            "'ANALOG_READBACK': {'v_mux': {delete: [14]}, 'i_mux': {delete: [29]}, 'v_mux_ntc': 2, "*

 * *            "'i_mux_ntc': 9, 'v_mux_gnd': 30, 'i_mux_gnd': 63}, 'INJECTION_CAPACITANCE': {'v_mux': "*

 * *            "{delete: [1]}, 'i_mux […]*

```diff
@@ -44,20 +44,20 @@
         "success_code": 0,
         "timeout": 30
     },
     "tasks": {
         "ADC_CALIBRATION": {
             "InjVcalRange": 1,
             "MonitorV": [
-                8,
-                30
+                8
             ],
+            "MonitorV_GND": 30,
             "Range": {
                 "start": 500,
-                "step": 100,
+                "step": 200,
                 "stop": 3500
             }
         },
         "ANALOG_READBACK": {
             "MonSensAcbDem": [
                 0,
                 1,
@@ -185,21 +185,18 @@
                 22,
                 23,
                 24,
                 25,
                 28,
                 29,
                 30,
-                31,
-                63
-            ],
-            "i_mux_ntc": [
-                9,
-                63
+                31
             ],
+            "i_mux_gnd": 63,
+            "i_mux_ntc": 9,
             "v_mux": [
                 0,
                 3,
                 4,
                 5,
                 6,
                 7,
@@ -207,30 +204,27 @@
                 9,
                 10,
                 11,
                 12,
                 13,
                 15,
                 17,
-                30,
                 31,
                 32,
                 33,
                 34,
                 35,
                 36,
                 37,
                 38,
                 39,
                 63
             ],
-            "v_mux_ntc": [
-                2,
-                30
-            ],
+            "v_mux_gnd": 30,
+            "v_mux_ntc": 2,
             "v_mux_tempsens": [
                 14,
                 16,
                 18
             ]
         },
         "DATA_TRANSMISSION": {
@@ -252,22 +246,22 @@
                 2,
                 3
             ]
         },
         "INJECTION_CAPACITANCE": {
             "i_mux": [
                 10,
-                11,
-                63
+                11
             ],
+            "i_mux_gnd": 63,
             "n_meas": 5,
             "v_mux": [
-                4,
-                30
-            ]
+                4
+            ],
+            "v_mux_gnd": 30
         },
         "IV_MEASURE": {
             "i_max": {
                 "L0": 0.0001,
                 "L1": 0.0001,
                 "L2": 0.0001
             },
@@ -339,15 +333,15 @@
                 37
             ]
         },
         "SLDO": {
             "extra_i": [],
             "i_max": {
                 "L0": 9.75,
-                "L1": 10.6,
+                "L1": 9.8,
                 "L2": 9.48
             },
             "i_min": {
                 "L0": 5.55,
                 "L1": 6.6,
                 "L2": 5.88
             },
@@ -357,15 +351,15 @@
                 29,
                 30,
                 31,
                 63
             ],
             "n_points": {
                 "L0": 22,
-                "L1": 21,
+                "L1": 17,
                 "L2": 19
             },
             "v_mux": [
                 30,
                 33,
                 37,
                 34,
@@ -402,25 +396,25 @@
         "VCAL_CALIBRATION": {
             "InjVcalRange": [
                 1,
                 0
             ],
             "Large_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             },
             "MonitorV": [
                 8,
                 7
             ],
             "MonitorV_GND": 30,
             "Small_Range": {
                 "start": 100,
-                "step": 100,
+                "step": 200,
                 "stop": 4000
             }
         }
     },
     "yarr": {
         "controller": "configs/controller/specCfg-rd53b-16x1.json",
         "eyeDiagram_exe": "./bin/eyeDiagram",
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/module_state_template.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/module_state_template.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/20UPGXM1234567_Lx_dummy.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip1.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip2.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip3.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/emulator/configs/connectivity/chip/dummy_chip4.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ADC_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/ANALOG_READBACK.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/ANALOG_READBACK.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/DATA_TRANSMISSION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/INJECTION_CAPACITANCE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/IV_MEASURE.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/IV_MEASURE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/LP_MODE.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/LP_MODE.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/OVERVOLTAGE_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/SLDO.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/SLDO.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/UNDERSHUNT_PROTECTION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/VCAL_CALIBRATION.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/common.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/common.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/data/schema/config.json` & `module_qc_tools-2.2.3/src/module_qc_tools/data/schema/config.json`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/hardware_control_base.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/hardware_control_base.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/misc.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/misc.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,15 @@
 
 # Convert micro-amps to voltages using rImux
 # TODO: Decide if I should change read-adc script to return V instead
 def microItoV(read_uA, yr):
     read_V = []
     for r, chip in zip(read_uA, range(yr._number_of_chips)):
         if chip in yr._disabled_chip_positions:
+            read_V += [-999]
             continue
         try:
             rImux = yr.get_config(chip)["RD53B"]["Parameter"]["ADCcalPar"][2]
         except Exception:
             rImux = 4.99e3  # Default in YARR read-adc script
             log.warning(
                 bcolors.WARNING
@@ -163,24 +164,24 @@
                     reads = [int(x) for x in read.split()]
                 else:
                     reads = [float(x) for x in read.split()[0::2]]  # Remove units
             except Exception as e:
                 log.error(f"Unable to decode return from read_adc: {read}")
                 raise RuntimeError() from e
 
-            # If we read current, we need to convert back to V
-            if i_mux > -1:
-                reads = microItoV(reads, yr)
-
             #  Fill in values at disabled chip positions
             for i in yr._disabled_chip_positions:
                 if i != chip_position and chip_position is not None:
                     continue
                 reads.insert(i, -999)
 
+            # If we read current, we need to convert back to V
+            if i_mux > -1:
+                reads = microItoV(reads, yr)
+
     # Read through multimeter
     else:
         for chip in range(yr._number_of_chips):
             if chip != chip_position and chip_position is not None:
                 continue
             if chip in yr._disabled_chip_positions:
                 reads.append(-999)
```

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/multimeter.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/multimeter.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/ntc.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/ntc.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/power_supply.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/power_supply.py`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/src/module_qc_tools/utils/yarr.py` & `module_qc_tools-2.2.3/src/module_qc_tools/utils/yarr.py`

 * *Files 5% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 #    import importlib_resources as resources
 
 log = logging.getLogger("measurement")
 
 
 class yarr(hardware_control_base):
     def __init__(self, config, *args, name="yarr", **kwargs):
+        self.run_dir = ""
         self.controller = ""
         self.connectivity = ""
         self.scanConsole_exe = ""
         self.write_register_exe = ""
         self.read_register_exe = ""
         self.read_adc_exe = ""
         self.switchLPM_exe = ""
@@ -84,14 +85,25 @@
                                     bcolors.WARNING
                                     + "Attention! Module is in low-power mode. If this is not intended, you can turn it off by running `./bin/switchLPM off` in YARR directory"
                                     + bcolors.ENDC
                                 )
 
         return 0
 
+    # Reads controller file, returns spec number
+    def get_spec(self):
+        controller_path = self.run_dir / self.controller
+        with controller_path.open(encoding="utf-8") as file:
+            controller_params = json.load(file)
+        try:
+            return controller_params.get("ctrlCfg").get("cfg").get("specNum")
+        except Exception:
+            log.warning("Unable to read specNum from controller file. Assuming spec #0")
+            return 0
+
     def run_scan(self, scan, output=None, skip_reset=False):
         if output:
             cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} -s {scan} -o {output} {"--skip-reset" if skip_reset else ""}'
         else:
             cmd = f'{self.scanConsole_exe} -r {self.controller} -c {self.connectivity} -s {scan} {"--skip-reset" if skip_reset else ""}'
 
         log.info(f"Running YARR scan: {scan} ...")
@@ -348,15 +360,15 @@
         else:
             msg = "Incorrect VMUX value for setting trim!"
             raise RuntimeError(msg)
 
         return 0
 
     def switchLPM(self, position):
-        cmd = f"{self.switchLPM_exe} {position}"
+        cmd = f"{self.switchLPM_exe} -s {self.get_spec()} {position}"
         return self.send_command(cmd, purpose="switch LP mode on/off")
 
     def get_connectivity(self):
         with Path(self.connectivity).open(encoding="utf-8") as file:
             return json.load(file)
 
     def get_config(self, chip_position):
```

### Comparing `module_qc_tools-2.2.2rc3/.gitignore` & `module_qc_tools-2.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/LICENSE` & `module_qc_tools-2.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `module_qc_tools-2.2.2rc3/README.md` & `module_qc_tools-2.2.3/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# module-qc-tools v2.2.2rc3
+# module-qc-tools v2.2.3
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -70,15 +70,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 $ python -m venv venv
 $ source venv/bin/activate
 $ python -m pip install -U pip
-$ python -m pip install -U pip module-qc-tools==2.2.2rc3
+$ python -m pip install -U pip module-qc-tools==2.2.3
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

### Comparing `module_qc_tools-2.2.2rc3/pyproject.toml` & `module_qc_tools-2.2.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 requires-python = ">=3.7"
 dependencies = [
     "numpy",
     "pandas",
     "tabulate",
     "pre-commit",
     "check-jsonschema",
-    "module-qc-data-tools >= 1.0.11",
+    "module-qc-data-tools >= 1.0.14",
     'importlib_resources; python_version < "3.9"',
     "requests",
     'urllib3>=1.26.11,<2; "el7.x86_64" in platform_release',
     "typer>=0.9.0",
 ]
 classifiers = [
     "Programming Language :: Python :: 3",
```

### Comparing `module_qc_tools-2.2.2rc3/PKG-INFO` & `module_qc_tools-2.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: module_qc_tools
-Version: 2.2.2rc3
+Version: 2.2.3
 Summary: Module qc tools
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools/-/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <gstark@cern.ch>
 License: Copyright (c) 2018 ATLAS ITk Pixel Modules
@@ -29,25 +29,25 @@
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Requires-Dist: check-jsonschema
 Requires-Dist: importlib-resources; python_version < '3.9'
-Requires-Dist: module-qc-data-tools>=1.0.11
+Requires-Dist: module-qc-data-tools>=1.0.14
 Requires-Dist: numpy
 Requires-Dist: pandas
 Requires-Dist: pre-commit
 Requires-Dist: requests
 Requires-Dist: tabulate
 Requires-Dist: typer>=0.9.0
 Requires-Dist: urllib3<2,>=1.26.11; 'el7.x86_64' in platform_release
 Description-Content-Type: text/markdown
 
-# module-qc-tools v2.2.2rc3
+# module-qc-tools v2.2.3
 
 A general python tool for running ITkPixV1.1 module QC tests
 
 ## Table of contents
 
 1. [Requirements](#requirements)
 2. [Installation](#installation)
@@ -115,15 +115,15 @@
 Use this method if you want to use the latest stable (versioned) release of the
 package.
 
 ```
 $ python -m venv venv
 $ source venv/bin/activate
 $ python -m pip install -U pip
-$ python -m pip install -U pip module-qc-tools==2.2.2rc3
+$ python -m pip install -U pip module-qc-tools==2.2.3
 ```
 
 ## Usage
 
 After installation, one just needs to enter the virtual environment in each new
 session to use the scripts:
```

