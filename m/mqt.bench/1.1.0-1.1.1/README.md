# Comparing `tmp/mqt.bench-1.1.0.tar.gz` & `tmp/mqt.bench-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mqt.bench-1.1.0.tar", last modified: Wed Mar 20 14:52:38 2024, max compression
+gzip compressed data, was "mqt.bench-1.1.1.tar", last modified: Thu Apr 11 12:11:54 2024, max compression
```

## Comparing `mqt.bench-1.1.0.tar` & `mqt.bench-1.1.1.tar`

### file list

```diff
@@ -1,165 +1,166 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.348006 mqt.bench-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)      125 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.308006 mqt.bench-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.308006 mqt.bench-1.1.0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/ISSUE_TEMPLATE/bug-report.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/ISSUE_TEMPLATE/feature-request.yml
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/codecov.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      567 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/support.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.308006 mqt.bench-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/codeql.yml
--rw-r--r--   0 runner    (1001) docker     (127)      890 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/coverage.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/deploy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/mypy.yml
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/release-drafter.yml
--rw-r--r--   0 runner    (1001) docker     (127)      665 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.github/workflows/test_pregenerated_zip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/CITATION.bib
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-03-20 14:52:38.348006 mqt.bench-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.308006 mqt.bench-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Abstraction_levels.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Benchmark_selection.rst
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/DevelopmentGuide.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3202 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Parameter.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Quickstart.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/References.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Support.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/Usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.312006 mqt.bench-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/arch.png
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/custom.css
--rw-r--r--   0 runner    (1001) docker     (127)   100569 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/erc_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)   102052 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/erc_light.svg
--rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/level_1.png
--rw-r--r--   0 runner    (1001) docker     (127)    84500 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/level_2.png
--rw-r--r--   0 runner    (1001) docker     (127)    76051 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/level_3.png
--rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/level_4.png
--rw-r--r--   0 runner    (1001) docker     (127)   184498 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/logo-bavaria.svg
--rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/logo-mqv.svg
--rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/mqt_light.png
--rw-r--r--   0 runner    (1001) docker     (127)   196044 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/mqtbench.png
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/tum_dark.svg
--rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_static/tum_light.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.312006 mqt.bench-1.1.0/docs/_templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/_templates/page.html
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      815 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/docs/refs.bib
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-20 14:52:38.348006 mqt.bench-1.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.304006 mqt.bench-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.304006 mqt.bench-1.1.0/src/mqt/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.316006 mqt.bench-1.1.0/src/mqt/bench/
--rw-r--r--   0 runner    (1001) docker     (127)      496 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmark_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.316006 mqt.bench-1.1.0/src/mqt/bench/benchmarks/
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1988 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/ae.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/dj.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/ghz.py
--rw-r--r--   0 runner    (1001) docker     (127)      693 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/graphstate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1414 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/grover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qaoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      608 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qft.py
--rw-r--r--   0 runner    (1001) docker     (127)      692 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qftentangled.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
--rw-r--r--   0 runner    (1001) docker     (127)     2081 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
--rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
--rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_ml/
--rw-r--r--   0 runner    (1001) docker     (127)     1027 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_nature/
--rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_optimization/
--rw-r--r--   0 runner    (1001) docker     (127)     5114 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     1500 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qpeexact.py
--rw-r--r--   0 runner    (1001) docker     (127)     1535 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qpeinexact.py
--rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/qwalk.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/random.py
--rw-r--r--   0 runner    (1001) docker     (127)      738 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/realamprandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     8876 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/shor.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/su2random.py
--rw-r--r--   0 runner    (1001) docker     (127)      733 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/twolocalrandom.py
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/vqe.py
--rw-r--r--   0 runner    (1001) docker     (127)      868 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/benchmarks/wstate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/calibration_files/
--rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/ibm_montreal_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    58070 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/ibm_washington_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/ionq_aria1_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/ionq_harmony_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/oqc_lucy_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)    55310 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json
--rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/config.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.320006 mqt.bench-1.1.0/src/mqt/bench/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9172 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/calibration.py
--rw-r--r--   0 runner    (1001) docker     (127)     7600 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     9620 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/ibm.py
--rw-r--r--   0 runner    (1001) docker     (127)     3256 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/ionq.py
--rw-r--r--   0 runner    (1001) docker     (127)     3161 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/oqc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2771 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     2637 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/quantinuum.py
--rw-r--r--   0 runner    (1001) docker     (127)     7663 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/devices/rigetti.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.340006 mqt.bench-1.1.0/src/mqt/bench/evaluation/
--rw-r--r--   0 runner    (1001) docker     (127)      369 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (127) 15925096 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation_data.pkl
--rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.340006 mqt.bench-1.1.0/src/mqt/bench/evaluation/results/
--rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/results/pie.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/results/qubit_dist.pdf
--rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/evaluation/results/violins.pdf
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     7071 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/qiskit_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9707 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/tket_helper.py
--rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/bench/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.340006 mqt.bench-1.1.0/src/mqt/benchviewer/
--rw-r--r--   0 runner    (1001) docker     (127)      233 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26382 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     6258 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.340006 mqt.bench-1.1.0/src/mqt/benchviewer/static/
--rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/src/mqt/benchviewer/static/files/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/static/files/MQTBench_all.zip
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/src/mqt/benchviewer/static/files/qasm_output/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/static/files/qasm_output/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/static/mqt_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/static/tum_logo.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/src/mqt/benchviewer/templates/
--rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/templates/benchmark_description.html
--rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/templates/description.html
--rw-r--r--   0 runner    (1001) docker     (127)    28601 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/src/mqt/benchviewer/templates/legal.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/src/mqt.bench.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4706 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      179 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        4 2024-03-20 14:52:38.000000 mqt.bench-1.1.0/src/mqt.bench.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-20 14:52:38.344006 mqt.bench-1.1.0/tests/devices/
--rw-r--r--   0 runner    (1001) docker     (127)     6011 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_devices.py
--rw-r--r--   0 runner    (1001) docker     (127)     8094 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_ibm_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2934 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_ionq_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_oqc_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2045 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_quantinuum_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/devices/test_rigetti_device_support.py
--rw-r--r--   0 runner    (1001) docker     (127)    30979 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/test_bench.py
--rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/test_benchviewer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-03-20 14:52:32.000000 mqt.bench-1.1.0/tests/test_pregenerated_zip.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      125 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/bug-report.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1015 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/feature-request.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/codecov.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5852 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      567 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1040 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/support.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.755949 mqt.bench-1.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/codeql.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      890 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/coverage.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/deploy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/mypy.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/release-drafter.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      665 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.github/workflows/test_pregenerated_zip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     5010 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     3041 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/CITATION.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4718 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.759949 mqt.bench-1.1.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Abstraction_levels.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2732 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Benchmark_selection.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/DevelopmentGuide.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3216 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Parameter.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3195 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Quickstart.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/References.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Support.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2155 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/Usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    21005 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/arch.png
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/custom.css
+-rw-r--r--   0 runner    (1001) docker     (127)   100569 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/erc_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   102052 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/erc_light.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    40262 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)    84500 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_2.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76051 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_3.png
+-rw-r--r--   0 runner    (1001) docker     (127)   112485 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/level_4.png
+-rw-r--r--   0 runner    (1001) docker     (127)   184498 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/logo-bavaria.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    17368 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/logo-mqv.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)    57266 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqt_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)   196044 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/mqtbench.png
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/tum_dark.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    12257 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_static/tum_light.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/docs/_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2210 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/_templates/page.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      815 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/docs/refs.bib
+-rw-r--r--   0 runner    (1001) docker     (127)     1805 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/noxfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5949 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 12:11:54.795949 mqt.bench-1.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.751949 mqt.bench-1.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.751949 mqt.bench-1.1.1/src/mqt/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.763949 mqt.bench-1.1.1/src/mqt/bench/
+-rw-r--r--   0 runner    (1001) docker     (127)      496 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18948 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmark_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/ae.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1942 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/dj.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/ghz.py
+-rw-r--r--   0 runner    (1001) docker     (127)      692 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/graphstate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/grover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1164 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qaoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qft.py
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qftentangled.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/
+-rw-r--r--   0 runner    (1001) docker     (127)     1966 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2080 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2362 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2907 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/
+-rw-r--r--   0 runner    (1001) docker     (127)     1928 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/
+-rw-r--r--   0 runner    (1001) docker     (127)     5129 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeexact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeinexact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2950 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/qwalk.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/realamprandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9704 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/shor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/su2random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/twolocalrandom.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1289 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/vqe.py
+-rw-r--r--   0 runner    (1001) docker     (127)      867 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/benchmarks/wstate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.767949 mqt.bench-1.1.1/src/mqt/bench/calibration_files/
+-rw-r--r--   0 runner    (1001) docker     (127)    12189 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_montreal_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    58070 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_washington_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     8302 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_aria1_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_harmony_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/oqc_lucy_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13528 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)    55310 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4270 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/config.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.771949 mqt.bench-1.1.1/src/mqt/bench/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     2851 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8996 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/calibration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7523 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9512 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/ibm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3191 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/ionq.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3055 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/oqc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2576 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/quantinuum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7564 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/devices/rigetti.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.787949 mqt.bench-1.1.1/src/mqt/bench/evaluation/
+-rw-r--r--   0 runner    (1001) docker     (127)      369 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (127) 15925096 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_data.pkl
+-rw-r--r--   0 runner    (1001) docker     (127)     8242 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/
+-rw-r--r--   0 runner    (1001) docker     (127)    16461 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/pie.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    19421 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/qubit_dist.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)    24774 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/evaluation/results/violins.pdf
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/qiskit_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9705 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/tket_helper.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9703 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/bench/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/
+-rw-r--r--   0 runner    (1001) docker     (127)      233 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26385 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6263 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/
+-rw-r--r--   0 runner    (1001) docker     (127)    15406 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/MQTBench_all.zip
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/qasm_output/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/files/qasm_output/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    61137 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/mqt_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/static/tum_logo.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt/benchviewer/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)    16436 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/benchmark_description.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7436 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/description.html
+-rw-r--r--   0 runner    (1001) docker     (127)    28601 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/src/mqt/benchviewer/templates/legal.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/src/mqt.bench.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8706 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4717 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      179 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2024-04-11 12:11:54.000000 mqt.bench-1.1.1/src/mqt.bench.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 12:11:54.791949 mqt.bench-1.1.1/tests/devices/
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_devices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8050 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_ibm_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_ionq_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_oqc_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_quantinuum_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2073 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/devices/test_rigetti_device_support.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30958 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_bench.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15211 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_benchviewer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1595 2024-04-11 12:11:44.000000 mqt.bench-1.1.1/tests/test_pregenerated_zip.py
```

### Comparing `mqt.bench-1.1.0/.github/ISSUE_TEMPLATE/bug-report.yml` & `mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/bug-report.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/ISSUE_TEMPLATE/feature-request.yml` & `mqt.bench-1.1.1/.github/ISSUE_TEMPLATE/feature-request.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/contributing.rst` & `mqt.bench-1.1.1/.github/contributing.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/dependabot.yml` & `mqt.bench-1.1.1/.github/dependabot.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/release-drafter.yml` & `mqt.bench-1.1.1/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/support.rst` & `mqt.bench-1.1.1/.github/support.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/workflows/codeql.yml` & `mqt.bench-1.1.1/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/workflows/coverage.yml` & `mqt.bench-1.1.1/.github/workflows/coverage.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/workflows/deploy.yml` & `mqt.bench-1.1.1/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.github/workflows/test_pregenerated_zip.yml` & `mqt.bench-1.1.1/.github/workflows/test_pregenerated_zip.yml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.gitignore` & `mqt.bench-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/.pre-commit-config.yaml` & `mqt.bench-1.1.1/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -11,34 +11,42 @@
   autoupdate_commit_msg: "⬆️🪝 update pre-commit hooks"
   autofix_commit_msg: "🎨 pre-commit fixes"
   skip: [mypy]
 
 repos:
   # Standard hooks
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: "v4.5.0"
+    rev: "v4.6.0"
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-docstring-first
       - id: check-merge-conflict
       - id: check-toml
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: trailing-whitespace
 
   # Handling unwanted unicode characters
   - repo: https://github.com/sirosen/texthooks
-    rev: "0.6.4"
+    rev: "0.6.6"
     hooks:
       - id: fix-ligatures
       - id: fix-smartquotes
 
+  # Check for common mistakes
+  - repo: https://github.com/pre-commit/pygrep-hooks
+    rev: v1.10.0
+    hooks:
+      - id: rst-backticks
+      - id: rst-directive-colons
+      - id: rst-inline-touching-normal
+
   # Clean jupyter notebooks
   - repo: https://github.com/srstevenson/nb-clean
     rev: "3.2.0"
     hooks:
       - id: nb-clean
   # Check for spelling
   - repo: https://github.com/codespell-project/codespell
@@ -52,15 +60,15 @@
   - repo: https://github.com/pre-commit/mirrors-prettier
     rev: "v4.0.0-alpha.8"
     hooks:
       - id: prettier
         types_or: [yaml, markdown, html, css, javascript, json]
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.3.3
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: ["--fix", "--show-fixes"]
         types_or: [python, pyi, jupyter]
       - id: ruff-format
         types_or: [python, pyi, jupyter]
 
@@ -71,20 +79,36 @@
       - id: blacken-docs
         additional_dependencies: [black==23.*]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: v1.9.0
     hooks:
       - id: mypy
-        files: ^(src|tests|setup.py)
+        files: ^(src|tests)
         args: []
         additional_dependencies:
           - pytket_qiskit
           - qiskit_optimization
           - qiskit_nature
           - qiskit_finance
           - importlib_resources
           - pytest
           - types-setuptools
           - types-requests
           - types-tqdm
           - types-flask
+
+  # Catch common capitalization mistakes
+  - repo: local
+    hooks:
+      - id: disallow-caps
+        name: Disallow improper capitalization
+        language: pygrep
+        entry: PyBind|Numpy|Cmake|CCache|Github|PyTest|Mqt|Tum
+        exclude: .pre-commit-config.yaml
+
+  # Check best practices for scientific Python code
+  - repo: https://github.com/scientific-python/cookie
+    rev: 2024.03.10
+    hooks:
+      - id: sp-repo-review
+        additional_dependencies: ["repo-review[cli]"]
```

### Comparing `mqt.bench-1.1.0/.readthedocs.yaml` & `mqt.bench-1.1.1/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/LICENSE` & `mqt.bench-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/PKG-INFO` & `mqt.bench-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.1.0
+Version: 1.1.1
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@tum.de>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket-qiskit<0.51.0,>=0.50.0
+Requires-Dist: pytket-qiskit<0.53.0,>=0.50.0
 Requires-Dist: qiskit_optimization
 Requires-Dist: qiskit_nature
 Requires-Dist: qiskit_finance
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: flask>=2.0.0
 Requires-Dist: networkx>=2.0.0
 Requires-Dist: pyscf>=2.3.0
```

### Comparing `mqt.bench-1.1.0/README.md` & `mqt.bench-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/Abstraction_levels.rst` & `mqt.bench-1.1.1/docs/Abstraction_levels.rst`

 * *Files 2% similar despite different names*

```diff
@@ -48,36 +48,36 @@
 .. image:: /_static/level_3.png
    :width: 50%
    :alt: Illustration of the target-dependent native gates level
    :align: center
 
 Different quantum computer realizations support
 different native gate-sets. In our example, we consider the
-`ibmq_manila` device as the target device which natively supports I, X, √X, Rz and CX gates.
+``ibmq_manila`` device as the target device which natively supports I, X, √X, Rz and CX gates.
 Consequently, the Ry gates in the previous figure have to be converted using only these native gates. In this case,
 they are substituted by a sequence of X and Rz gates (denoted as • with a phase of −π).
 
 
 4. Target-dependent Mapped Level
 ---------------------------------
 
 
 .. image:: /_static/arch.png
    :width: 15%
-   :alt: Illustration of the `ibmq_manila` device
+   :alt: Illustration of the ``ibmq_manila`` device
    :align: center
 
-The architecture of the `ibmq_manila` device is shown above on the right and it defines between which qubits a two-qubit operation may be performed.
+The architecture of the ``ibmq_manila`` device is shown above on the right and it defines between which qubits a two-qubit operation may be performed.
 Since the circuit shown in the previous figure contains CX gates operating between all combination of qubits,
 there is no mapping directly matching the target architecture's layout. As a consequence,
 a non-trivial mapping followed by a round of optimization leads to the resulting circuit
 shown below.
 
 .. image:: /_static/level_4.png
    :width: 50%
    :alt: Illustration of the target-dependent mapped level
    :align: center
 
 This is also the reason for the different sequence of CX gates compared
 to the previous example.
 
-This circuit is now executable on the `ibmq_manila` device, since all hardware induced requirements are fulfilled.
+This circuit is now executable on the ``ibmq_manila`` device, since all hardware induced requirements are fulfilled.
```

### Comparing `mqt.bench-1.1.0/docs/Benchmark_selection.rst` & `mqt.bench-1.1.1/docs/Benchmark_selection.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/DevelopmentGuide.rst` & `mqt.bench-1.1.1/docs/DevelopmentGuide.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/Parameter.rst` & `mqt.bench-1.1.1/docs/Parameter.rst`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
   ``"qwalk-noancilla"``\ , ``"qwalk-v-chain"``\ , ``"random"``\ , ``"realamprandom"``\ , ``"su2random"``\ , ``"twolocalrandom"``\ , ``"vqe"``\ ,
   ``"wstate"``\ , ``"shor"``\ , ``"pricingcall"``\ , ``"pricingput"``\ , ``"groundstate"``\ , ``"routing"``\ ,
   ``"tsp"``
 * ``level``\ : ``0`` or ``"alg"``\ , ``1`` or ``"indep"``\ , ``2`` or ``"nativegates"``\ , ``3`` or ``"mapped"``
 * ``circuit_size``\ : for most of the cases this is equal to number of qubits
   (all scalable benchmarks except ``"qwalk-v-chain"`` and ``"grover-v-chain"``\ ) while for all other the qubit number is higher
 * ``compiler``\ : ``"qiskit"`` or ``"tket"``
-* `compiler_settings`: Optimization level for `"qiskit"` (`0`-`3`), placement for `"tket"` (`lineplacement` or `graphplacement`), exemplary shown:
+* ``compiler_settings``: Optimization level for ``"qiskit"`` (``0``-``3``), placement for ``"tket"`` (``lineplacement`` or ``graphplacement``), exemplary shown:
 
 .. code-block:: python
 
    from mqt.bench import CompilerSettings, QiskitSettings, TKETSettings
 
    compiler_settings = CompilerSettings(
        qiskit=QiskitSettings(optimization_level=1),
```

### Comparing `mqt.bench-1.1.0/docs/Quickstart.ipynb` & `mqt.bench-1.1.1/docs/Quickstart.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/Usage.rst` & `mqt.bench-1.1.1/docs/Usage.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/arch.png` & `mqt.bench-1.1.1/docs/_static/arch.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/erc_dark.svg` & `mqt.bench-1.1.1/docs/_static/erc_dark.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/erc_light.svg` & `mqt.bench-1.1.1/docs/_static/erc_light.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/level_1.png` & `mqt.bench-1.1.1/docs/_static/level_1.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/level_2.png` & `mqt.bench-1.1.1/docs/_static/level_2.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/level_3.png` & `mqt.bench-1.1.1/docs/_static/level_3.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/level_4.png` & `mqt.bench-1.1.1/docs/_static/level_4.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/logo-bavaria.svg` & `mqt.bench-1.1.1/docs/_static/logo-bavaria.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/logo-mqv.svg` & `mqt.bench-1.1.1/docs/_static/logo-mqv.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/mqt_dark.png` & `mqt.bench-1.1.1/docs/_static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/mqt_light.png` & `mqt.bench-1.1.1/docs/_static/mqt_light.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/mqtbench.png` & `mqt.bench-1.1.1/docs/_static/mqtbench.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/tum_dark.svg` & `mqt.bench-1.1.1/docs/_static/tum_dark.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_static/tum_light.svg` & `mqt.bench-1.1.1/docs/_static/tum_light.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/_templates/page.html` & `mqt.bench-1.1.1/docs/_templates/page.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/conf.py` & `mqt.bench-1.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/index.rst` & `mqt.bench-1.1.1/docs/index.rst`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/docs/refs.bib` & `mqt.bench-1.1.1/docs/refs.bib`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/pyproject.toml` & `mqt.bench-1.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 ]
 keywords = ["MQT",  "quantum computing", "benchmarking", "performance", "testing"]
 license = { file = "LICENSE" }
 requires-python = ">=3.10"
 dynamic = ["version"]
 
 dependencies = [
-    "pytket-qiskit>=0.50.0,<0.51.0",  #  manages the dependencies for qiskit and tket in a combined fashion
+    "pytket-qiskit>=0.50.0,<0.53.0",  #  manages the dependencies for qiskit and tket in a combined fashion
     "qiskit_optimization",
     "qiskit_nature",
     "qiskit_finance",
     "pandas>=1.0.0",
     "flask>=2.0.0",
     "networkx>=2.0.0",
     "pyscf>=2.3.0",
@@ -85,14 +85,21 @@
 
 [tool.pytest.ini_options]
 minversion = "7.2"
 testpaths = ["tests"]
 addopts = ["-ra", "--strict-markers", "--strict-config", "--showlocals"]
 log_cli_level = "INFO"
 xfail_strict = true
+filterwarnings = [
+    "error",
+    "ignore:.*pkg_resources.*:DeprecationWarning:",
+    "ignore:.*sre_.*:DeprecationWarning:",
+    "ignore:.*Rigetti.*:UserWarning:",
+    "ignore:.*Values in x.*:RuntimeWarning:",
+]
 
 [tool.coverage]
 run.source = ["mqt.bench", "mqt.benchviewer"]
 report.exclude_also = [
     '\.\.\.',
     'if TYPE_CHECKING:',
     'raise AssertionError',
@@ -104,15 +111,14 @@
 precision = 1
 
 [tool.mypy]
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src"
 files = ["src", "tests", "setup.py"]
 python_version = "3.10"
 strict = true
-show_error_codes = true
 enable_error_code = ["ignore-without-code", "redundant-expr", "truthy-bool"]
 warn_unreachable = true
 explicit_package_bases = true
 pretty = true
 
 [[tool.mypy.overrides]]
 module = ["pytket.*", "qiskit_finance.*"]
@@ -122,34 +128,37 @@
 module = ["qiskit.*", "qiskit_finance.*", "joblib.*", "networkx.*", "pandas.*", "qiskit_algorithms.*", "qiskit_ibm_runtime.*"]
 ignore_missing_imports = true
 
 [tool.ruff]
 line-length = 120
 extend-include = ["*.ipynb"]
 src = ["src"]
+preview = true
 unsafe-fixes = true
 
 [tool.ruff.lint]
 extend-select = [
     "A",           # flake8-builtins
-#    "ANN",         # flake8-annotations
+    "ANN",         # flake8-annotations
     "ARG",         # flake8-unused-arguments
     "ASYNC",       # flake8-async
     "B",  "B904",  # flake8-bugbear
     "C4",          # flake8-comprehensions
 #    "D",           # pydocstyle
     "EM",          # flake8-errmsg
     "EXE",         # flake8-executable
     "FA",          # flake8-future-annotations
     "FLY",         # flynt
+    "FURB",        # refurb
     "I",           # isort
     "ICN",         # flake8-import-conventions
     "ISC",         # flake8-implicit-str-concat
-  #  "N",           # flake8-naming
-  #  "NPY",         # numpy
+    "LOG",         # flake8-logging-format
+    "N",           # flake8-naming
+    "NPY",         # numpy
     "PERF",        # perflint
     "PGH",         # pygrep-hooks
     "PIE",         # flake8-pie
     "PL",          # pylint
     "PT",          # flake8-pytest-style
     "PTH",         # flake8-use-pathlib
     "PYI",         # flake8-pyi
@@ -162,23 +171,28 @@
     "SIM",         # flake8-simplify
     "TCH",         # flake8-type-checking
     "TID",         # flake8-tidy-imports
     "TRY",         # tryceratops
     "UP",          # pyupgrade
     "YTT",         # flake8-2020
 ]
-extend-ignore = [
-    "PLR",  # Design related pylint codes
-    "ISC001", # Added because of ruff-format warning
+ignore = [
+    "ANN101",  # Missing type annotation for self in method
+    "ANN102",  # Missing type annotation for cls in classmethod
+    "ISC001",  # Conflicts with formatter
+    "E501",    # Line too long (Black is enough)
+    "PLR",     # Design related pylint codes
+    "S101",    # Use of assert detected
 ]
+flake8-unused-arguments.ignore-variadic-names = true
 isort.required-imports = ["from __future__ import annotations"]
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "*.pyi" = ["D"]  # pydocstyle
 "*.ipynb" = [
     "D",    # pydocstyle
     "E402", # Allow imports to appear anywhere in Jupyter notebooks
     "I002", # Allow missing `from __future__ import annotations` import
 ]
 
-[tool.ruff.pydocstyle]
+[tool.ruff.lint.pydocstyle]
 convention = "google"
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmark_generator.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmark_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -328,15 +328,14 @@
         CompilerSettings: Data class containing the respective compiler settings for the specified compiler (e.g., optimization level for Qiskit or placement for TKET)
         provider_name: "ibm", "rigetti", "ionq", "oqc", or "quantinuum" (required for "nativegates" level)
         device_name: "ibm_washington", "ibm_montreal", "rigetti_aspen_m3", "ionq_harmony", "ionq_aria1", "oqc_lucy", "quantinuum_h2" (required for "mapped" level)
 
     Returns:
         Quantum Circuit Object representing the benchmark with the selected options, either as Qiskit::QuantumCircuit or Pytket::Circuit object (depending on the chosen compiler---while the algorithm level is always provided using Qiskit)
     """
-
     if "gate_set_name" in kwargs:
         msg = "gate_set_name is deprecated and will be removed in a future release. Use provider_name instead."
         warn(msg, DeprecationWarning, stacklevel=2)
         provider_name = kwargs["gate_set_name"]
 
     if benchmark_name not in utils.get_supported_benchmarks():
         msg = f"Selected benchmark is not supported. Valid benchmarks are {utils.get_supported_benchmarks()}."
@@ -462,26 +461,26 @@
 
 
 def timeout_watcher(
     func: Callable[..., bool | QuantumCircuit],
     timeout: int,
     args: list[Any] | int | tuple[int, str] | str,
 ) -> bool | QuantumCircuit | Circuit:
-    class TimeoutException(Exception):  # Custom exception class
+    class TimeoutExceptionError(Exception):  # Custom exception class
         pass
 
-    def timeout_handler(_signum: Any, _frame: Any) -> None:  # Custom signal handler
-        raise TimeoutException
+    def timeout_handler(_signum: int, _frame: Any) -> None:  # noqa: ANN401
+        raise TimeoutExceptionError
 
     # Change the behavior of SIGALRM
     signal.signal(signal.SIGALRM, timeout_handler)
     signal.alarm(timeout)
     try:
         res = func(*args) if isinstance(args, tuple | list) else func(args)
-    except TimeoutException:
+    except TimeoutExceptionError:
         print(
             "Calculation/Generation exceeded timeout limit for ",
             func.__name__,
             func.__module__.split(".")[-1],
         )
         if isinstance(args, list) and isinstance(args[0], QuantumCircuit):
             print(args[0].name, args[1:])
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/__init__.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/__init__.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -7,16 +7,16 @@
     pricingput,
 )
 from mqt.bench.benchmarks.qiskit_application_ml import qnn
 from mqt.bench.benchmarks.qiskit_application_nature import groundstate
 from mqt.bench.benchmarks.qiskit_application_optimization import routing, tsp
 
 __all__ = [
-    "pricingput",
-    "pricingcall",
+    "groundstate",
     "portfolioqaoa",
     "portfoliovqe",
-    "groundstate",
+    "pricingcall",
+    "pricingput",
+    "qnn",
     "routing",
     "tsp",
-    "qnn",
 ]
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/ae.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/ae.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,18 +6,17 @@
 from qiskit import QuantumCircuit
 from qiskit_algorithms import AmplitudeEstimation, EstimationProblem
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing Quantum Amplitude Estimation.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     ae = AmplitudeEstimation(
         num_eval_qubits=num_qubits - 1,  # -1 because of the to be estimated qubit
     )
     problem = get_estimation_problem()
 
     qc = ae.construct_circuit(problem)
     qc.name = "ae"
@@ -34,24 +33,26 @@
 
         self._theta_p = 2 * np.arcsin(np.sqrt(probability))
         self.ry(2 * self._theta_p, 0)
 
     def __eq__(self, other: object) -> bool:
         return isinstance(other, BernoulliQ) and self._theta_p == other._theta_p
 
+    def __hash__(self) -> int:
+        return hash(self._theta_p)
+
     def power(self, power: float, _matrix_power: bool = True) -> QuantumCircuit:
         # implement the efficient power of Q
         q_k = QuantumCircuit(1)
         q_k.ry(2 * power * self._theta_p, 0)
         return q_k
 
 
 def get_estimation_problem() -> EstimationProblem:
     """Returns a estimation problem instance for a fixed p value."""
-
     p = 0.2
 
     """A circuit representing the Bernoulli A operator."""
     a = QuantumCircuit(1)
     theta_p = 2 * np.arcsin(np.sqrt(p))
     a.ry(theta_p, 0)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/dj.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/dj.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 import numpy as np
 from qiskit import QuantumCircuit
 
 
 def dj_oracle(case: str, n: int) -> QuantumCircuit:
     # plus one output qubit
     oracle_qc = QuantumCircuit(n + 1)
+    rng = np.random.default_rng(10)
 
     if case == "balanced":
-        np.random.seed(10)
         b_str = ""
         for _ in range(n):
-            b = np.random.randint(0, 2)
+            b = rng.integers(0, 2)
             b_str = b_str + str(b)
 
         for qubit in range(len(b_str)):
             if b_str[qubit] == "1":
                 oracle_qc.x(qubit)
 
         for qubit in range(n):
             oracle_qc.cx(qubit, n)
 
         for qubit in range(len(b_str)):
             if b_str[qubit] == "1":
                 oracle_qc.x(qubit)
 
     if case == "constant":
-        output = np.random.randint(2)
+        output = rng.integers(2)
         if output == 1:
             oracle_qc.x(n)
 
     oracle_gate = oracle_qc.to_gate()
     oracle_gate.name = "Oracle"  # To show when we display the circuit
     return oracle_gate
 
@@ -58,19 +58,18 @@
 
     return dj_circuit
 
 
 def create_circuit(n: int, balanced: bool = True) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Deutsch-Josza algorithm.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     balanced -- True for a balanced and False for a constant oracle
     """
-
     oracle_mode = "balanced" if balanced else "constant"
     n = n - 1  # because of ancilla qubit
     oracle_gate = dj_oracle(oracle_mode, n)
     qc = dj_algorithm(oracle_gate, n)
     qc.name = "dj"
 
     return qc
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/ghz.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/ghz.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,18 +2,17 @@
 
 from qiskit import QuantumCircuit, QuantumRegister
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the GHZ state.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     q = QuantumRegister(num_qubits, "q")
     qc = QuantumCircuit(q, name="ghz")
     qc.h(q[-1])
     for i in range(1, num_qubits):
         qc.cx(q[num_qubits - i], q[num_qubits - i - 1])
     qc.measure_all()
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/graphstate.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/graphstate.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,19 +4,18 @@
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.library import GraphState
 
 
 def create_circuit(num_qubits: int, degree: int = 2) -> QuantumCircuit:
     """Returns a quantum circuit implementing a graph state.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     degree -- number of edges per node
     """
-
     q = QuantumRegister(num_qubits, "q")
     qc = QuantumCircuit(q, name="graphstate")
 
     g = nx.random_regular_graph(degree, num_qubits)
     a = nx.convert_matrix.to_numpy_array(g)
     qc.compose(GraphState(a), inplace=True)
     qc.measure_all()
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/grover.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/grover.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,19 +5,18 @@
 from qiskit.circuit.library import GroverOperator
 from qiskit_algorithms import Grover
 
 
 def create_circuit(num_qubits: int, ancillary_mode: str = "noancilla") -> QuantumCircuit:
     """Returns a quantum circuit implementing Grover's algorithm.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     ancillary_mode -- defining the decomposition scheme
     """
-
     num_qubits = num_qubits - 1  # -1 because of the flag qubit
     q = QuantumRegister(num_qubits, "q")
     flag = AncillaRegister(1, "flag")
 
     state_preparation = QuantumCircuit(q, flag)
     state_preparation.h(q)
     state_preparation.x(flag)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qaoa.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qaoa.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,17 @@
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Approximation Optimization Algorithm for a specific max-cut
      example.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     qp = get_examplary_max_cut_qp(num_qubits)
     assert isinstance(qp, QuadraticProgram)
 
     qaoa = QAOA(sampler=Sampler(), reps=2, optimizer=SLSQP(maxiter=25))
     qaoa_result = qaoa.compute_minimum_eigenvalue(qp.to_ising()[0])
     qc = qaoa.ansatz.assign_parameters(qaoa_result.optimal_point)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qft.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qft.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,18 @@
 from __future__ import annotations
 
-from qiskit import ClassicalRegister, QuantumCircuit, QuantumRegister
+from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.library import QFT
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Fourier Transform algorithm.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     q = QuantumRegister(num_qubits, "q")
-    c = ClassicalRegister(num_qubits, "c")
-    qc = QuantumCircuit(q, c, name="qft")
+    qc = QuantumCircuit(q, name="qft")
     qc.compose(QFT(num_qubits=num_qubits), inplace=True)
     qc.measure_all()
 
     return qc
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qftentangled.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qftentangled.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 from qiskit import QuantumCircuit, QuantumRegister
 from qiskit.circuit.library import QFT
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Fourier Transform algorithm using entangled qubits.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     q = QuantumRegister(num_qubits, "q")
     qc = QuantumCircuit(q)
     qc.h(q[-1])
     for i in range(1, num_qubits):
         qc.cx(q[num_qubits - i], q[num_qubits - i - 1])
 
     qc.compose(QFT(num_qubits=num_qubits), inplace=True)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfolioqaoa.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,18 +15,17 @@
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit of QAOA applied to a specific portfolio optimization task.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     # set number of assets (= number of qubits)
     num_assets = num_qubits
 
     # Generate expected return and covariance matrix from (random) time-series
     stocks = [("TICKER%s" % i) for i in range(num_assets)]
     data = RandomDataProvider(
         tickers=stocks,
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/portfoliovqe.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,18 +16,17 @@
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit of VQE applied to a specific portfolio optimization task.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     # set number of assets (= number of qubits)
     num_assets = num_qubits
 
     # Generate expected return and covariance matrix from (random) time-series
     stocks = [("TICKER%s" % i) for i in range(num_assets)]
     data = RandomDataProvider(
         tickers=stocks,
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingcall.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_uncertainty_qubits: int = 5) -> QuantumCircuit:
     """Returns a quantum circuit of Iterative Amplitude Estimation applied to a problem instance of
     pricing call options.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_uncertainty_qubits -- number of qubits to measure uncertainty
     """
     # parameters for considered random distribution
     s = 2.0  # initial spot price
     vol = 0.4  # volatility of 40%
     r = 0.05  # annual interest rate of 4%
     t = 40 / 365  # 40 days to maturity
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_finance/pricingput.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_uncertainty_qubits: int = 5) -> QuantumCircuit:
     """Returns a quantum circuit of Iterative Amplitude Estimation applied to a problem instance of pricing put options.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_uncertainty_qubits -- number of qubits to measure uncertainty
     """
     # parameters for considered random distribution
     s = 2.0  # initial spot price
     vol = 0.4  # volatility of 40%
     r = 0.05  # annual interest rate of 4%
     t = 40 / 365  # 40 days to maturity
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_ml/qnn.py`

 * *Files 5% similar despite different names*

```diff
@@ -5,22 +5,24 @@
 from qiskit import QuantumCircuit
 from qiskit.circuit.library import RealAmplitudes, ZZFeatureMap
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing a Quantum Neural Network (QNN) with a ZZ FeatureMap and a RealAmplitudes ansatz.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
     feature_map = ZZFeatureMap(feature_dimension=num_qubits)
     ansatz = RealAmplitudes(num_qubits=num_qubits, reps=1)
 
     qc = QuantumCircuit(num_qubits)
     feature_map = feature_map.assign_parameters([1 for _ in range(feature_map.num_parameters)])
-    ansatz = ansatz.assign_parameters(np.random.rand(ansatz.num_parameters))
+
+    rng = np.random.default_rng(10)
+    ansatz = ansatz.assign_parameters(rng.random(ansatz.num_parameters) * 2 * np.pi)
     qc.compose(feature_map, inplace=True)
     qc.compose(ansatz, inplace=True)
 
     qc.name = "qnn"
     qc.measure_all()
     return qc
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_nature/groundstate.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(choice: str) -> QuantumCircuit:
     """Returns a quantum circuit implementing Ground State Estimation.
 
-    Keyword arguments:
+    Keyword Arguments:
     molecule -- Molecule for which the ground state shall be estimated.
     """
     molecule = get_molecule(choice)
     driver = PySCFDriver(atom=molecule)
     es_problem = driver.run()
 
     mapper = JordanWignerMapper()
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/routing.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,104 +20,104 @@
 class Initializer:
     def __init__(self, n: int) -> None:
         self.n = n
 
     def generate_instance(
         self,
     ) -> tuple[
-        NDArray[np.float_],
-        NDArray[np.float_],
-        NDArray[np.float_],
+        NDArray[np.float64],
+        NDArray[np.float64],
+        NDArray[np.float64],
     ]:
         n = self.n
-        np.random.seed(10)
+        rng = np.random.default_rng(10)
 
-        xc = (np.random.rand(n) - 0.5) * 10
-        yc = (np.random.rand(n) - 0.5) * 10
+        xc = (rng.random(n) - 0.5) * 10
+        yc = (rng.random(n) - 0.5) * 10
 
         instance = np.zeros([n, n])
         for ii in range(n):
             for jj in range(ii + 1, n):
                 instance[ii, jj] = (xc[ii] - xc[jj]) ** 2 + (yc[ii] - yc[jj]) ** 2
                 instance[jj, ii] = instance[ii, jj]
 
         return xc, yc, instance
 
 
 class QuantumOptimizer:
-    def __init__(self, instance: NDArray[np.float_], n: int, K: int) -> None:
+    def __init__(self, instance: NDArray[np.float64], n: int, k: int) -> None:
         self.instance = instance
         self.n = n
-        self.K = K
+        self.k = k
 
     def binary_representation(
-        self, x_sol: NDArray[np.float_]
-    ) -> tuple[NDArray[np.float_], NDArray[np.float_], float, float]:
+        self, x_sol: NDArray[np.float64]
+    ) -> tuple[NDArray[np.float64], NDArray[np.float64], float, float]:
         instance = self.instance
         n = self.n
-        K = self.K
+        k = self.k
 
-        A = np.max(instance) * 100  # A parameter of cost function
+        a = np.max(instance) * 100  # A parameter of cost function
 
         # Determine the weights w
         instance_vec = instance.reshape(n**2)
         w_list = [instance_vec[x] for x in range(n**2) if instance_vec[x] > 0]
         w = np.zeros(n * (n - 1))
         for ii in range(len(w_list)):
             w[ii] = w_list[ii]
 
         # Some variables I will use
-        Id_n = np.eye(n)
-        Im_n_1 = np.ones([n - 1, n - 1])
-        Iv_n_1 = np.ones(n)
-        Iv_n_1[0] = 0
-        Iv_n = np.ones(n - 1)
-        neg_Iv_n_1 = np.ones(n) - Iv_n_1
+        id_n = np.eye(n)
+        im_n_1 = np.ones([n - 1, n - 1])
+        iv_n_1 = np.ones(n)
+        iv_n_1[0] = 0
+        iv_n = np.ones(n - 1)
+        neg_iv_n_1 = np.ones(n) - iv_n_1
 
         v = np.zeros([n, n * (n - 1)])
         for ii in range(n):
             count = ii - 1
             for jj in range(n * (n - 1)):
                 if jj // (n - 1) == ii:
                     count = ii
 
                 if jj // (n - 1) != ii and jj % (n - 1) == count:
                     v[ii][jj] = 1.0
 
         vn = np.sum(v[1:], axis=0)
 
         # Q defines the interactions between variables
-        Q = A * (np.kron(Id_n, Im_n_1) + np.dot(v.T, v))
+        q = a * (np.kron(id_n, im_n_1) + np.dot(v.T, v))
 
         # g defines the contribution from the individual variables
-        g = w - 2 * A * (np.kron(Iv_n_1, Iv_n) + vn.T) - 2 * A * K * (np.kron(neg_Iv_n_1, Iv_n) + v[0].T)
+        g = w - 2 * a * (np.kron(iv_n_1, iv_n) + vn.T) - 2 * a * k * (np.kron(neg_iv_n_1, iv_n) + v[0].T)
 
         # c is the constant offset
-        c = 2 * A * (n - 1) + 2 * A * (K**2)
+        c = 2 * a * (n - 1) + 2 * a * (k**2)
 
         try:
             # Evaluates the cost distance from a binary representation of a path
-            def fun(x: NDArray[np.float_]) -> float:
+            def fun(x: NDArray[np.float64]) -> float:
                 return cast(
                     float,
-                    np.dot(np.around(x), np.dot(Q, np.around(x))) + np.dot(g, np.around(x)) + c,
+                    np.dot(np.around(x), np.dot(q, np.around(x))) + np.dot(g, np.around(x)) + c,
                 )
 
             cost = fun(x_sol)
         except Exception:
             cost = 0
 
-        return Q, g, cast(float, c), cost
+        return q, g, cast(float, c), cost
 
-    def construct_problem(self, Q: QuadraticExpression, g: LinearExpression, c: float) -> QuadraticProgram:
+    def construct_problem(self, q: QuadraticExpression, g: LinearExpression, c: float) -> QuadraticProgram:
         qp = QuadraticProgram()
         for i in range(self.n * (self.n - 1)):
             qp.binary_var(str(i))
 
-        qp.objective.quadratic = Q
+        qp.objective.quadratic = q
         qp.objective.linear = g
         qp.objective.constant = c
         return qp
 
     def solve_problem(self, qp: QuadraticProgram) -> QuantumCircuit:
         ansatz = RealAmplitudes(self.n)
         vqe = VQE(estimator=Estimator(), optimizer=SLSQP(maxiter=25), ansatz=ansatz)
@@ -125,28 +125,27 @@
         vqe_result = vqe.compute_minimum_eigenvalue(qp.to_ising()[0])
         return vqe.ansatz.assign_parameters(vqe_result.optimal_point)
 
 
 def create_circuit(num_nodes: int = 3, num_vehs: int = 2) -> QuantumCircuit:
     """Returns a quantum circuit solving a routing problem.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_nodes -- number of to be visited nodes
     num_vehs -- number of used vehicles
     """
-
     # Initialize the problem by defining the parameters
     n = num_nodes  # number of nodes + depot (n+1)
     k = num_vehs  # number of vehicles
     # Initialize the problem by randomly generating the instance
     initializer = Initializer(n)
-    xc, yc, instance = initializer.generate_instance()
+    _xc, _yc, instance = initializer.generate_instance()
 
     quantum_optimizer = QuantumOptimizer(instance, n, k)
-    q, g, c, binary_cost = quantum_optimizer.binary_representation(x_sol=np.array(0.0, dtype=float))
+    q, g, c, _binary_cost = quantum_optimizer.binary_representation(x_sol=np.array(0.0, dtype=float))
     q_casted = cast(QuadraticExpression, q)
     g_casted = cast(LinearExpression, g)
     qp = quantum_optimizer.construct_problem(q_casted, g_casted, c)
     # Instantiate the quantum optimizer class with parameters:
     qc = quantum_optimizer.solve_problem(qp)
 
     qc.measure_all()
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qiskit_application_optimization/tsp.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,27 +14,26 @@
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_nodes: int) -> QuantumCircuit:
     """Returns a quantum circuit solving the Travelling Salesman Problem (TSP).
 
-    Keyword arguments:
+    Keyword Arguments:
     num_nodes -- number of to be visited nodes
     """
-
     # Generating a graph of 3 nodes
     n = num_nodes
     tsp = Tsp.create_random_instance(n, seed=10)
 
     qp = tsp.to_quadratic_program()
 
     qp2qubo = QuadraticProgramToQubo()
     qubo = qp2qubo.convert(qp)
-    qubit_op, offset = qubo.to_ising()
+    qubit_op, _offset = qubo.to_ising()
 
     spsa = SPSA(maxiter=25)
     ry = TwoLocal(qubit_op.num_qubits, "ry", "cz", reps=5, entanglement="linear")
     vqe = VQE(ansatz=ry, optimizer=spsa, estimator=Estimator())
     vqe.random_seed = 10
 
     vqe_result = vqe.compute_minimum_eigenvalue(qubit_op)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qpeexact.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeexact.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from qiskit.circuit.library import QFT
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Phase Estimation algorithm for a phase which can be
     exactly estimated.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     num_qubits = num_qubits - 1  # because of ancilla qubit
     q = QuantumRegister(num_qubits, "q")
     psi = QuantumRegister(1, "psi")
     c = ClassicalRegister(num_qubits, "c")
     qc = QuantumCircuit(q, psi, c, name="qpeexact")
 
     # get random n-bit string as target phase
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qpeinexact.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qpeinexact.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,18 +8,17 @@
 from qiskit.circuit.library import QFT
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Phase Estimation algorithm for a phase which cannot be
     exactly estimated.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     num_qubits = num_qubits - 1  # because of ancilla qubit
     q = QuantumRegister(num_qubits, "q")
     psi = QuantumRegister(1, "psi")
     c = ClassicalRegister(num_qubits, "c")
     qc = QuantumCircuit(q, psi, c, name="qpeinexact")
 
     # get random n+1-bit string as target phase
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/qwalk.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/qwalk.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     n: int,
     ancillary_mode: str = "noancilla",
     depth: int = 3,
     coin_state_preparation: QuantumCircuit | None = None,
 ) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Quantum Walk algorithm.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     depth -- number of quantum steps
     coin_state_preparation -- optional quantum circuit for state preparation
     ancillary_mode -- defining the decomposition scheme
     """
     n = n - 1  # because one qubit is needed for the coin
     coin = QuantumRegister(1, "coin")
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/random.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/random.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from mqt.bench import utils
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a random quantum circuit twice as deep as wide. The random gate span over four qubits maximum.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
     qc = random_circuit(num_qubits, num_qubits * 2, measure=False, seed=10)
     gates = list(set(utils.get_openqasm_gates()) - {"rccx", "csx", "cu"})
     qc = transpile(
         qc,
         basis_gates=gates,
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/realamprandom.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/realamprandom.py`

 * *Files 14% similar despite different names*

```diff
@@ -9,19 +9,18 @@
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the RealAmplitudes ansatz with random parameter
     values.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
-    np.random.seed(10)
+    rng = np.random.default_rng(10)
     qc = RealAmplitudes(num_qubits, entanglement="full", reps=3)
     num_params = qc.num_parameters
-    qc = qc.assign_parameters(2 * np.pi * np.random.rand(num_params))
+    qc = qc.assign_parameters(2 * np.pi * rng.random(num_params))
     qc.measure_all()
     qc.name = "realamprandom"
 
     return qc
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/shor.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/shor.py`

 * *Files 16% similar despite different names*

```diff
@@ -25,19 +25,18 @@
 from qiskit.circuit.library import QFT
 from qiskit_algorithms.utils.validation import validate_min
 
 
 def create_circuit(num_to_be_factorized: int, a: int = 2) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Shor's algorithm.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_to_be_factorized -- number which shall be factorized
     a -- any integer that satisfies 1 < a < num_to_be_factorized and gcd(a, num_to_be_factorized) = 1
     """
-
     qc = Shor().construct_circuit(num_to_be_factorized, a)
     qc.measure_all()
     qc.name = "shor_" + str(num_to_be_factorized) + "_" + str(a)
 
     return qc
 
 
@@ -50,40 +49,40 @@
         "xlarge": [201209, 4],  # 74 qubits
     }
     return instances[choice]
 
 
 class Shor:
     @staticmethod
-    def _get_angles(a: int, n: int) -> NDArray[np.float_]:
+    def _get_angles(a: int, n: int) -> NDArray[np.float64]:
         """Calculates the array of angles to be used in the addition in Fourier Space."""
         bits_little_endian = (bin(int(a))[2:].zfill(n))[::-1]
 
         angles = np.zeros(n)
         for i in range(n):
             for j in range(i + 1):
                 k = i - j
                 if bits_little_endian[j] == "1":
                     angles[i] += pow(2, -k)
 
         return angles * np.pi
 
     @staticmethod
-    def _phi_add_gate(angles: NDArray[np.float_] | ParameterVector) -> Gate:
+    def _phi_add_gate(angles: NDArray[np.float64] | ParameterVector) -> Gate:
         """Gate that performs addition by a in Fourier Space."""
         circuit = QuantumCircuit(len(angles), name="phi_add_a")
         for i, angle in enumerate(angles):
             circuit.p(angle, i)
         return circuit.to_gate()
 
-    def _double_controlled_phi_add_mod_N(
+    def _double_controlled_phi_add_mod_n(
         self,
-        angles: NDArray[np.float_] | ParameterVector,
-        c_phi_add_N: Gate,
-        iphi_add_N: Gate,
+        angles: NDArray[np.float64] | ParameterVector,
+        c_phi_add_n: Gate,
+        iphi_add_n: Gate,
         qft: Gate,
         iqft: Gate,
     ) -> QuantumCircuit:
         """Creates a circuit which implements double-controlled modular addition by a."""
         ctrl_qreg = QuantumRegister(2, "ctrl")
         b_qreg = QuantumRegister(len(angles), "b")
         flag_qreg = QuantumRegister(1, "flag")
@@ -91,167 +90,168 @@
         circuit = QuantumCircuit(ctrl_qreg, b_qreg, flag_qreg, name="ccphi_add_a_mod_N")
 
         cc_phi_add_a = self._phi_add_gate(angles).control(2)
         cc_iphi_add_a = cc_phi_add_a.inverse()
 
         circuit.append(cc_phi_add_a, [*ctrl_qreg, *b_qreg])
 
-        circuit.append(iphi_add_N, b_qreg)
+        circuit.append(iphi_add_n, b_qreg)
 
         circuit.append(iqft, b_qreg)
         circuit.cx(b_qreg[-1], flag_qreg[0])
         circuit.append(qft, b_qreg)
 
-        circuit.append(c_phi_add_N, [*flag_qreg, *b_qreg])
+        circuit.append(c_phi_add_n, [*flag_qreg, *b_qreg])
 
         circuit.append(cc_iphi_add_a, [*ctrl_qreg, *b_qreg])
 
         circuit.append(iqft, b_qreg)
         circuit.x(b_qreg[-1])
         circuit.cx(b_qreg[-1], flag_qreg[0])
         circuit.x(b_qreg[-1])
         circuit.append(qft, b_qreg)
 
         circuit.append(cc_phi_add_a, [*ctrl_qreg, *b_qreg])
 
         return circuit
 
-    def _controlled_multiple_mod_N(
+    def _controlled_multiple_mod_n(
         self,
-        n: int,
-        N: int,
+        num_bits_necessary: int,
+        to_be_factored_number: int,
         a: int,
-        c_phi_add_N: Gate,
-        iphi_add_N: Gate,
+        c_phi_add_n: Gate,
+        iphi_add_n: Gate,
         qft: Gate,
         iqft: Gate,
     ) -> Instruction:
         """Implements modular multiplication by a as an instruction."""
         ctrl_qreg = QuantumRegister(1, "ctrl")
-        x_qreg = QuantumRegister(n, "x")
-        b_qreg = QuantumRegister(n + 1, "b")
+        x_qreg = QuantumRegister(num_bits_necessary, "x")
+        b_qreg = QuantumRegister(num_bits_necessary + 1, "b")
         flag_qreg = QuantumRegister(1, "flag")
 
         circuit = QuantumCircuit(ctrl_qreg, x_qreg, b_qreg, flag_qreg, name="cmult_a_mod_N")
 
-        angle_params = ParameterVector("angles", length=n + 1)
-        modulo_adder = self._double_controlled_phi_add_mod_N(angle_params, c_phi_add_N, iphi_add_N, qft, iqft)
+        angle_params = ParameterVector("angles", length=num_bits_necessary + 1)
+        modulo_adder = self._double_controlled_phi_add_mod_n(angle_params, c_phi_add_n, iphi_add_n, qft, iqft)
 
         def append_adder(adder: QuantumCircuit, constant: int, idx: int) -> None:
-            partial_constant = (pow(2, idx, N) * constant) % N
-            angles = self._get_angles(partial_constant, n + 1)
+            partial_constant = (pow(2, idx, to_be_factored_number) * constant) % to_be_factored_number
+            angles = self._get_angles(partial_constant, num_bits_necessary + 1)
             bound = adder.assign_parameters({angle_params: angles})
             circuit.append(bound, [*ctrl_qreg, x_qreg[idx], *b_qreg, *flag_qreg])
 
         circuit.append(qft, b_qreg)
 
         # perform controlled addition by a on the aux register in Fourier space
-        for i in range(n):
+        for i in range(num_bits_necessary):
             append_adder(modulo_adder, a, i)
 
         circuit.append(iqft, b_qreg)
 
         # perform controlled subtraction by a in Fourier space on both the aux and down register
-        for i in range(n):
+        for i in range(num_bits_necessary):
             circuit.cswap(ctrl_qreg, x_qreg[i], b_qreg[i])
 
         circuit.append(qft, b_qreg)
 
-        a_inv = pow(a, -1, mod=N)
+        a_inv = pow(a, -1, mod=to_be_factored_number)
 
         modulo_adder_inv = modulo_adder.inverse()
-        for i in reversed(range(n)):
+        for i in reversed(range(num_bits_necessary)):
             append_adder(modulo_adder_inv, a_inv, i)
 
         circuit.append(iqft, b_qreg)
 
         return circuit.to_instruction()
 
-    def _power_mod_N(self, n: int, N: int, a: int) -> Instruction:
+    def _power_mod_n(self, num_bits_necessary: int, to_be_factored_number: int, a: int) -> Instruction:
         """Implements modular exponentiation a^x as an instruction."""
-        up_qreg = QuantumRegister(2 * n, name="up")
-        down_qreg = QuantumRegister(n, name="down")
-        aux_qreg = QuantumRegister(n + 2, name="aux")
+        up_qreg = QuantumRegister(2 * num_bits_necessary, name="up")
+        down_qreg = QuantumRegister(num_bits_necessary, name="down")
+        aux_qreg = QuantumRegister(num_bits_necessary + 2, name="aux")
 
-        circuit = QuantumCircuit(up_qreg, down_qreg, aux_qreg, name=f"{a}^x mod {N}")
+        circuit = QuantumCircuit(up_qreg, down_qreg, aux_qreg, name=f"{a}^x mod {to_be_factored_number}")
 
-        qft = QFT(n + 1, do_swaps=False).to_gate()
+        qft = QFT(num_bits_necessary + 1, do_swaps=False).to_gate()
         iqft = qft.inverse()
 
         # Create gates to perform addition/subtraction by N in Fourier Space
-        phi_add_N = self._phi_add_gate(self._get_angles(N, n + 1))
-        iphi_add_N = phi_add_N.inverse()
-        c_phi_add_N = phi_add_N.control(1)
+        phi_add_n = self._phi_add_gate(self._get_angles(to_be_factored_number, num_bits_necessary + 1))
+        iphi_add_n = phi_add_n.inverse()
+        c_phi_add_n = phi_add_n.control(1)
 
         # Apply the multiplication gates as showed in
         # the report in order to create the exponentiation
-        for i in range(2 * n):
-            partial_a = pow(a, pow(2, i), N)
-            modulo_multiplier = self._controlled_multiple_mod_N(n, N, partial_a, c_phi_add_N, iphi_add_N, qft, iqft)
+        for i in range(2 * num_bits_necessary):
+            partial_a = pow(a, pow(2, i), to_be_factored_number)
+            modulo_multiplier = self._controlled_multiple_mod_n(
+                num_bits_necessary, to_be_factored_number, partial_a, c_phi_add_n, iphi_add_n, qft, iqft
+            )
             circuit.append(modulo_multiplier, [up_qreg[i], *down_qreg, *aux_qreg])
 
         return circuit.to_instruction()
 
     @staticmethod
-    def _validate_input(N: int, a: int) -> None:
+    def _validate_input(to_be_factored_number: int, a: int) -> None:
         """Check parameters of the algorithm.
 
         Args:
-            N: The odd integer to be factored, has a min. value of 3.
+            to_be_factored_number: The odd integer to be factored, has a min. value of 3.
             a: Any integer that satisfies 1 < a < N and gcd(a, N) = 1.
 
         Raises:
             ValueError: Invalid input
 
         """
-
-        validate_min("N", N, 3)
+        validate_min("N", to_be_factored_number, 3)
         validate_min("a", a, 2)
 
-        if N < 1 or N % 2 == 0:
+        if to_be_factored_number < 1 or to_be_factored_number % 2 == 0:
             msg = "The input needs to be an odd integer greater than 1."
             raise ValueError(msg)
 
-        if a >= N or math.gcd(a, N) != 1:
+        if a >= to_be_factored_number or math.gcd(a, to_be_factored_number) != 1:
             msg = "The integer a needs to satisfy a < N and gcd(a, N) = 1."
             raise ValueError(msg)
 
-    def construct_circuit(self, N: int, a: int = 2) -> QuantumCircuit:
+    def construct_circuit(self, to_be_factored_number: int, a: int = 2) -> QuantumCircuit:
         """Construct quantum part of the algorithm.
 
         Args:
-            N: The odd integer to be factored, has a min. value of 3.
+            to_be_factored_number: The odd integer to be factored, has a min. value of 3.
             a: Any integer that satisfies 1 < a < N and gcd(a, N) = 1.
 
         Returns:
             Quantum circuit.
 
         """
-        self._validate_input(N, a)
+        self._validate_input(to_be_factored_number, a)
 
         # Get n value used in Shor's algorithm, to know how many qubits are used
-        n = N.bit_length()
+        num_bits_necessary = to_be_factored_number.bit_length()
 
         # quantum register where the sequential QFT is performed
-        up_qreg = QuantumRegister(2 * n, name="up")
+        up_qreg = QuantumRegister(2 * num_bits_necessary, name="up")
         # quantum register where the multiplications are made
-        down_qreg = QuantumRegister(n, name="down")
+        down_qreg = QuantumRegister(num_bits_necessary, name="down")
         # auxiliary quantum register used in addition and multiplication
-        aux_qreg = QuantumRegister(n + 2, name="aux")
+        aux_qreg = QuantumRegister(num_bits_necessary + 2, name="aux")
 
         # Create Quantum Circuit
-        circuit = QuantumCircuit(up_qreg, down_qreg, aux_qreg, name=f"Shor(N={N}, a={a})")
+        circuit = QuantumCircuit(up_qreg, down_qreg, aux_qreg, name=f"Shor(N={to_be_factored_number}, a={a})")
 
         # Create maximal superposition in top register
         circuit.h(up_qreg)
 
         # Initialize down register to 1
         circuit.x(down_qreg[0])
 
         # Apply modulo exponentiation
-        modulo_power = self._power_mod_N(n, N, a)
+        modulo_power = self._power_mod_n(num_bits_necessary, to_be_factored_number, a)
         circuit.append(modulo_power, circuit.qubits)
 
         # Apply inverse QFT
         iqft = QFT(len(up_qreg)).inverse().to_gate()
         circuit.append(iqft, up_qreg)
         return circuit
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/su2random.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/twolocalrandom.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,27 +1,26 @@
 from __future__ import annotations
 
 from typing import TYPE_CHECKING
 
 import numpy as np
-from qiskit.circuit.library import EfficientSU2
+from qiskit.circuit.library import TwoLocal
 
 if TYPE_CHECKING:  # pragma: no cover
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
-    """Returns a quantum circuit implementing EfficientSU2 ansatz with random parameter
+    """Returns a quantum circuit implementing the TwoLocal ansatz with random parameter
     values.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
-    np.random.seed(10)
-    qc = EfficientSU2(num_qubits, entanglement="full", reps=3)
+    rng = np.random.default_rng(10)
+    qc = TwoLocal(num_qubits, "ry", "cx", entanglement="full", reps=3)
     num_params = qc.num_parameters
-    qc = qc.assign_parameters(2 * np.pi * np.random.rand(num_params))
+    qc = qc.assign_parameters(2 * np.pi * rng.random(num_params))
     qc.measure_all()
-    qc.name = "su2random"
+    qc.name = "twolocalrandom"
 
     return qc
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/vqe.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/vqe.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,18 +16,17 @@
     from qiskit import QuantumCircuit
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the Variational Quantum Eigensolver Algorithm for a specific max-cut
      example.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     qp = get_examplary_max_cut_qp(num_qubits)
     assert isinstance(qp, QuadraticProgram)
 
     ansatz = RealAmplitudes(num_qubits, reps=2)
     vqe = VQE(ansatz=ansatz, optimizer=SLSQP(maxiter=25), estimator=Estimator())
     vqe_result = vqe.compute_minimum_eigenvalue(qp.to_ising()[0])
     qc = vqe.ansatz.assign_parameters(vqe_result.optimal_point)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/benchmarks/wstate.py` & `mqt.bench-1.1.1/src/mqt/bench/benchmarks/wstate.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,17 @@
 import numpy as np
 from qiskit import QuantumCircuit, QuantumRegister
 
 
 def create_circuit(num_qubits: int) -> QuantumCircuit:
     """Returns a quantum circuit implementing the W state.
 
-    Keyword arguments:
+    Keyword Arguments:
     num_qubits -- number of qubits of the returned quantum circuit
     """
-
     q = QuantumRegister(num_qubits, "q")
     qc = QuantumCircuit(q, name="wstate")
 
     def f_gate(qc: QuantumCircuit, q: QuantumRegister, i: int, j: int, n: int, k: int) -> None:
         theta = np.arccos(np.sqrt(1 / (n - k + 1)))
         qc.ry(-theta, q[j])
         qc.cz(q[i], q[j])
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/ibm_montreal_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_montreal_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/ibm_washington_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ibm_washington_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/ionq_aria1_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_aria1_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/ionq_harmony_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/ionq_harmony_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/oqc_lucy_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/oqc_lucy_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/quantinuum_h2_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json` & `mqt.bench-1.1.1/src/mqt/bench/calibration_files/rigetti_aspen_m3_calibration.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/config.json` & `mqt.bench-1.1.1/src/mqt/bench/config.json`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/__init__.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,30 +13,25 @@
 
 
 class NotFoundError(Exception):
     """Raised when a device or provider is not found within the available ones."""
 
 
 def get_available_providers() -> list[Provider]:
-    """
-    Get a list of all available providers
-    """
+    """Get a list of all available providers."""
     return [IBMProvider(), IonQProvider(), OQCProvider(), RigettiProvider(), QuantinuumProvider()]
 
 
 def get_available_provider_names() -> list[str]:
-    """
-    Get a list of all available provider names
-    """
+    """Get a list of all available provider names."""
     return [prov.provider_name for prov in get_available_providers()]
 
 
 def get_provider_by_name(provider_name: str) -> Provider:
-    """
-    Get a provider by its name
+    """Get a provider by its name.
 
     Args:
         provider_name: the name of the provider
     """
     provider = None
     for prov in get_available_providers():
         if prov.provider_name == provider_name:
@@ -47,35 +42,31 @@
         msg = f"Provider '{provider_name}' not found among available providers."
         raise NotFoundError(msg)
 
     return provider
 
 
 def get_available_devices(sanitize_device: bool = False) -> list[Device]:
-    """
-    Get a list of all available devices
+    """Get a list of all available devices.
 
     Args:
         sanitize_device: whether to sanitize the device calibration data
     """
     return [
         dev for prov in get_available_providers() for dev in prov.get_available_devices(sanitize_device=sanitize_device)
     ]
 
 
 def get_available_device_names() -> list[str]:
-    """
-    Get a list of all available device names
-    """
+    """Get a list of all available device names."""
     return [name for prov in get_available_providers() for name in prov.get_available_device_names()]
 
 
 def get_device_by_name(device_name: str) -> Device:
-    """
-    Get a device by its name
+    """Get a device by its name.
 
     Args:
         device_name: the name of the device
     """
     device = None
     for provider in get_available_providers():
         try:
@@ -88,22 +79,22 @@
         msg = f"Device '{device_name}' not found among available providers."
         raise NotFoundError(msg)
 
     return device
 
 
 __all__ = [
-    "Provider",
     "Device",
     "DeviceCalibration",
     "IBMProvider",
     "IonQProvider",
     "OQCProvider",
-    "RigettiProvider",
+    "Provider",
     "QuantinuumProvider",
-    "get_available_providers",
-    "get_available_provider_names",
-    "get_provider_by_name",
-    "get_available_devices",
+    "RigettiProvider",
     "get_available_device_names",
+    "get_available_devices",
+    "get_available_provider_names",
+    "get_available_providers",
     "get_device_by_name",
+    "get_provider_by_name",
 ]
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/calibration.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/calibration.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 from __future__ import annotations
 
 from dataclasses import dataclass, field
 
 
 @dataclass
 class DeviceCalibration:
-    """
-    Calibration data for a (generic) device.
+    """Calibration data for a (generic) device.
 
-    Attributes
+    Attributes:
     single_qubit_gate_fidelity: single-qubit fidelity for each qubit and gate
     single_qubit_gate_duration: single-qubit gate duration for each qubit and gate
     two_qubit_gate_fidelity: two-qubit fidelity for each qubit pair and gate
     two_qubit_gate_duration: two-qubit gate duration for each qubit pair and gate
     readout_fidelity: readout fidelity for each qubit
     readout_duration: readout duration for each qubit
     t1: T1 time for each qubit
@@ -26,54 +25,51 @@
     two_qubit_gate_duration: dict[tuple[int, ...], dict[str, float]] = field(default_factory=dict)
     readout_fidelity: dict[int, float] = field(default_factory=dict)
     readout_duration: dict[int, float] = field(default_factory=dict)
     t1: dict[int, float] = field(default_factory=dict)
     t2: dict[int, float] = field(default_factory=dict)
 
     def get_single_qubit_gate_fidelity(self, gate_type: str, qubit: int) -> float:
-        """
-        Get the single-qubit fidelity for a given gate type and qubit.
+        """Get the single-qubit fidelity for a given gate type and qubit.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit: index of the qubit
         """
         if not self.single_qubit_gate_fidelity:
             msg = "Single-qubit gate fidelity values not available."
             raise ValueError(msg)
 
         try:
             return self.single_qubit_gate_fidelity[qubit][gate_type]
         except KeyError:
             msg = f"Single-qubit fidelity for gate {gate_type} and qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def get_single_qubit_gate_duration(self, gate_type: str, qubit: int) -> float:
-        """
-        Get the single-qubit duration for a given gate type and qubit.
+        """Get the single-qubit duration for a given gate type and qubit.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit: index of the qubit
         """
         if not self.single_qubit_gate_duration:
             msg = "Single-qubit gate duration values not available."
             raise ValueError(msg)
 
         try:
             return self.single_qubit_gate_duration[qubit][gate_type]
         except KeyError:
             msg = f"Single-qubit duration for gate {gate_type} and qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def get_two_qubit_gate_fidelity(self, gate_type: str, qubit1: int, qubit2: int) -> float:
-        """
-        Get the two-qubit fidelity for a given gate type and qubit pair.
+        """Get the two-qubit fidelity for a given gate type and qubit pair.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit1: index of the first qubit
         qubit2: index of the second qubit
         """
         if not self.two_qubit_gate_fidelity:
             msg = "Two-qubit gate fidelity values not available."
             raise ValueError(msg)
@@ -81,18 +77,17 @@
         try:
             return self.two_qubit_gate_fidelity[(qubit1, qubit2)][gate_type]
         except KeyError:
             msg = f"Two-qubit fidelity for gate {gate_type} and qubits {qubit1} and {qubit2} not available."
             raise ValueError(msg) from None
 
     def get_two_qubit_gate_duration(self, gate_type: str, qubit1: int, qubit2: int) -> float:
-        """
-        Get the two-qubit duration for a given gate type and qubit pair.
+        """Get the two-qubit duration for a given gate type and qubit pair.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit1: index of the first qubit
         qubit2: index of the second qubit
         """
         if not self.two_qubit_gate_duration:
             msg = "Two-qubit gate duration values not available."
             raise ValueError(msg)
@@ -100,157 +95,141 @@
         try:
             return self.two_qubit_gate_duration[(qubit1, qubit2)][gate_type]
         except KeyError:
             msg = f"Two-qubit duration for gate {gate_type} and qubits {qubit1} and {qubit2} not available."
             raise ValueError(msg) from None
 
     def get_readout_fidelity(self, qubit: int) -> float:
-        """
-        Get the readout fidelity for a given qubit.
+        """Get the readout fidelity for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if not self.readout_fidelity:
             msg = "Readout fidelity values not available."
             raise ValueError(msg)
 
         try:
             return self.readout_fidelity[qubit]
         except KeyError:
             msg = f"Readout fidelity for qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def get_readout_duration(self, qubit: int) -> float:
-        """
-        Get the readout duration for a given qubit.
+        """Get the readout duration for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if not self.readout_duration:
             msg = "Readout duration values not available."
             raise ValueError(msg)
 
         try:
             return self.readout_duration[qubit]
         except KeyError:
             msg = f"Readout duration for qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def get_t1(self, qubit: int) -> float:
-        """
-        Get the T1 time for a given qubit.
+        """Get the T1 time for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if not self.t1:
             msg = "T1 values not available."
             raise ValueError(msg)
 
         try:
             return self.t1[qubit]
         except KeyError:
             msg = f"T1 for qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def get_t2(self, qubit: int) -> float:
-        """
-        Get the T2 time for a given qubit.
+        """Get the T2 time for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if not self.t2:
             msg = "T2 values not available."
             raise ValueError(msg)
 
         try:
             return self.t2[qubit]
         except KeyError:
             msg = f"T2 for qubit {qubit} not available."
             raise ValueError(msg) from None
 
     def compute_average_single_qubit_gate_fidelity(self, gate: str) -> float:
-        """
-        Compute the average single-qubit fidelity.
-        """
+        """Compute the average single-qubit fidelity."""
         if not self.single_qubit_gate_fidelity:
             msg = "Single-qubit gate fidelity values not available."
             raise ValueError(msg)
 
         avg_single_qubit_gate_fidelity = 0.0
         entries = 0
         for fidelity in self.single_qubit_gate_fidelity.values():
             if gate in fidelity:
                 avg_single_qubit_gate_fidelity += fidelity[gate]
                 entries += 1
         return avg_single_qubit_gate_fidelity / entries
 
     def compute_average_single_qubit_gate_duration(self, gate: str) -> float:
-        """
-        Compute the average single-qubit duration.
-        """
+        """Compute the average single-qubit duration."""
         if not self.single_qubit_gate_duration:
             msg = "Single-qubit gate duration values not available."
             raise ValueError(msg)
 
         avg_single_qubit_gate_duration = 0.0
         entries = 0
         for duration in self.single_qubit_gate_duration.values():
             if gate in duration:
                 avg_single_qubit_gate_duration += duration[gate]
                 entries += 1
         return avg_single_qubit_gate_duration / entries
 
     def compute_average_two_qubit_gate_fidelity(self, gate: str) -> float:
-        """
-        Compute the average two-qubit gate fidelity.
-        """
+        """Compute the average two-qubit gate fidelity."""
         if not self.two_qubit_gate_fidelity:
             msg = "Two-qubit gate fidelity values not available."
             raise ValueError(msg)
 
         avg_two_qubit_gate_fidelity = 0.0
         entries = 0
         for fidelity in self.two_qubit_gate_fidelity.values():
             if gate in fidelity:
                 avg_two_qubit_gate_fidelity += fidelity[gate]
                 entries += 1
         return avg_two_qubit_gate_fidelity / entries
 
     def compute_average_two_qubit_gate_duration(self, gate: str) -> float:
-        """
-        Compute the average two-qubit duration.
-        """
+        """Compute the average two-qubit duration."""
         if not self.two_qubit_gate_duration:
             msg = "Two-qubit gate duration values not available."
             raise ValueError(msg)
 
         avg_two_qubit_gate_duration = 0.0
         entries = 0
         for duration in self.two_qubit_gate_duration.values():
             if gate in duration:
                 avg_two_qubit_gate_duration += duration[gate]
                 entries += 1
         return avg_two_qubit_gate_duration / entries
 
     def compute_average_readout_fidelity(self) -> float:
-        """
-        Compute the average readout fidelity.
-        """
+        """Compute the average readout fidelity."""
         if not self.readout_fidelity:
             msg = "Readout fidelity values not available."
             raise ValueError(msg)
 
         return sum(self.readout_fidelity.values()) / len(self.readout_fidelity)
 
     def compute_average_readout_duration(self) -> float:
-        """
-        Compute the average readout duration.
-        """
+        """Compute the average readout duration."""
         if not self.readout_duration:
             msg = "Readout duration values not available."
             raise ValueError(msg)
 
         return sum(self.readout_duration.values()) / len(self.readout_duration)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/device.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/device.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,72 +5,68 @@
 
 if TYPE_CHECKING:
     from mqt.bench.devices import DeviceCalibration
 
 
 @dataclass
 class Device:
-    """
-    A class to represent a (generic) quantum device.
+    """A class to represent a (generic) quantum device.
 
-    Attributes
+    Attributes:
     name: name of the device
     num_qubits: number of qubits
     basis_gates: list of basis gates supported by the device
     coupling_map: coupling map of the device's qubits
     calibration: calibration information for the device
     """
 
     name: str = ""
     num_qubits: int = 0
     basis_gates: list[str] = field(default_factory=list)
     coupling_map: list[list[int]] = field(default_factory=list)
     calibration: DeviceCalibration | None = None
 
     def get_single_qubit_gate_fidelity(self, gate_type: str, qubit: int) -> float:
-        """
-        Get the single-qubit fidelity for a given gate type and qubit.
+        """Get the single-qubit fidelity for a given gate type and qubit.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit: index of the qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
 
         if gate_type not in self.basis_gates:
             msg = f"Gate {gate_type} not supported by device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_single_qubit_gate_fidelity(gate_type, qubit)
 
     def get_single_qubit_gate_duration(self, gate_type: str, qubit: int) -> float:
-        """
-        Get the single-qubit gate duration for a given gate type and qubit.
+        """Get the single-qubit gate duration for a given gate type and qubit.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit: index of the qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
 
         if gate_type not in self.basis_gates:
             msg = f"Gate {gate_type} not supported by device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_single_qubit_gate_duration(gate_type, qubit)
 
     def get_two_qubit_gate_fidelity(self, gate_type: str, qubit1: int, qubit2: int) -> float:
-        """
-        Get the two-qubit fidelity for a given gate type and qubit pair.
+        """Get the two-qubit fidelity for a given gate type and qubit pair.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit1: index of the first qubit
         qubit2: index of the second qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
@@ -78,18 +74,17 @@
         if gate_type not in self.basis_gates:
             msg = f"Gate {gate_type} not supported by device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_two_qubit_gate_fidelity(gate_type, qubit1, qubit2)
 
     def get_two_qubit_gate_duration(self, gate_type: str, qubit1: int, qubit2: int) -> float:
-        """
-        Get the two-qubit gate duration for a given gate type and qubit pair.
+        """Get the two-qubit gate duration for a given gate type and qubit pair.
 
-        Args
+        Args:
         gate_type: name of the gate
         qubit1: index of the first qubit
         qubit2: index of the second qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
@@ -97,66 +92,61 @@
         if gate_type not in self.basis_gates:
             msg = f"Gate {gate_type} not supported by device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_two_qubit_gate_duration(gate_type, qubit1, qubit2)
 
     def get_readout_fidelity(self, qubit: int) -> float:
-        """
-        Get the readout fidelity for a given qubit.
+        """Get the readout fidelity for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_readout_fidelity(qubit)
 
     def get_readout_duration(self, qubit: int) -> float:
-        """
-        Get the readout duration for a given qubit.
+        """Get the readout duration for a given qubit.
 
-        Args
+        Args:
         qubit: index of the qubit
         """
         if self.calibration is None:
             msg = f"Calibration data not available for device {self.name}."
             raise ValueError(msg)
 
         return self.calibration.get_readout_duration(qubit)
 
     def get_single_qubit_gates(self) -> set[str]:
-        """
-        Get the set of single-qubit gates supported by the device.
+        """Get the set of single-qubit gates supported by the device.
 
-        Returns
+        Returns:
         list of single-qubit gates
         """
         assert self.calibration is not None
         return {gate for qubit in range(self.num_qubits) for gate in self.calibration.single_qubit_gate_fidelity[qubit]}
 
     def get_two_qubit_gates(self) -> set[str]:
-        """
-        Get the set of two-qubit gates supported by the device.
+        """Get the set of two-qubit gates supported by the device.
 
-        Returns
+        Returns:
         list of two-qubit gates
         """
         assert self.calibration is not None
         return {
             gate
             for qubit1, qubit2 in self.coupling_map
             for gate in self.calibration.two_qubit_gate_fidelity[(qubit1, qubit2)]
         }
 
     def sanitize_device(self) -> None:
-        """
-        Tries to sanitize the device information so that it produces the least amount of problems when used.
+        """Tries to sanitize the device information so that it produces the least amount of problems when used.
 
         It is assumed that any edge, where the average two-qubit gate fidelity is 0, is not a valid edge.
         Thus, such edges are removed from the coupling map.
 
         It is ensured that
          * all single-qubit gates have fidelity data for all qubits in the device
          * all two-qubit gates have fidelity data for all qubit pairs in the coupling map.
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/ibm.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/ibm.py`

 * *Files 7% similar despite different names*

```diff
@@ -11,68 +11,58 @@
 
 from qiskit.providers import BackendV1, BackendV2
 
 from mqt.bench.devices import Device, DeviceCalibration, Provider
 
 
 class QubitProperties(TypedDict):
-    """
-    Class to store the properties of a single qubit.
-    """
+    """Class to store the properties of a single qubit."""
 
     T1: float  # us
     T2: float  # us
     eRO: float
     tRO: float  # ns
     eID: float
     eSX: float
     eX: float
     eCX: dict[str, float]
     tCX: dict[str, float]  # ns
 
 
 class IBMCalibration(TypedDict):
-    """
-    Class to store the calibration data of an IBM device.
-    """
+    """Class to store the calibration data of an IBM device."""
 
     name: str
     basis_gates: list[str]
     num_qubits: int
     connectivity: list[list[int]]
     properties: dict[str, QubitProperties]
 
 
 class IBMProvider(Provider):
-    """
-    Class to manage IBM devices.
-    """
+    """Class to manage IBM devices."""
 
     provider_name = "ibm"
 
     @classmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get the names of all available IBM devices.
-        """
+        """Get the names of all available IBM devices."""
         return ["ibm_washington", "ibm_montreal"]  # NOTE: update when adding new devices
 
     @classmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
         return ["id", "rz", "sx", "x", "cx", "measure", "barrier"]  # washington, montreal
 
     @classmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import an IBM backend.
+        """Import an IBM backend.
+
         Args:
-            path: the path to the JSON file containing the calibration data
+            path: the path to the JSON file containing the calibration data.
 
         Returns: the Device object
         """
         with path.open() as json_file:
             ibm_calibration = cast(IBMCalibration, json.load(json_file))
 
         device = Device()
@@ -104,18 +94,18 @@
             calibration.two_qubit_gate_duration[(qubit1, qubit2)] = {"cx": duration}
 
         device.calibration = calibration
         return device
 
     @classmethod
     def __import_backend_properties(cls, backend_properties: BackendProperties) -> DeviceCalibration:
-        """
-        Import calibration data from a Qiskit `BackendProperties` object.
+        """Import calibration data from a Qiskit `BackendProperties` object.
+
         Args:
-            backend_properties: the Qiskit `BackendProperties` object
+            backend_properties: the Qiskit `BackendProperties` object.
 
         Returns: Collection of calibration data
         """
         calibration = DeviceCalibration()
         num_qubits = len(backend_properties.qubits)
 
         for qubit in range(num_qubits):
@@ -147,35 +137,35 @@
                     calibration.two_qubit_gate_duration[(qubit1, qubit2)] = {}
                 calibration.two_qubit_gate_duration[(qubit1, qubit2)][gate.gate] = duration
 
         return calibration
 
     @classmethod
     def __import_backend_v1(cls, backend: BackendV1) -> Device:
-        """
-        Import device data from a Qiskit `BackendV1` object.
+        """Import device data from a Qiskit `BackendV1` object.
+
         Args:
-            backend: the Qiskit `BackendV1` object
+            backend: the Qiskit `BackendV1` object.
 
         Returns: Collection of device data
         """
         device = Device()
         device.name = backend.name()
         device.num_qubits = backend.configuration().n_qubits
         device.basis_gates = backend.configuration().basis_gates
         device.coupling_map = list(backend.configuration().coupling_map)
         device.calibration = cls.__import_backend_properties(backend.properties())
         return device
 
     @classmethod
     def __import_target(cls, target: Target) -> DeviceCalibration:
-        """
-        Import calibration data from a Qiskit `Target` object.
+        """Import calibration data from a Qiskit `Target` object.
+
         Args:
-            target: the Qiskit `Target` object
+            target: the Qiskit `Target` object.
 
         Returns: Collection of calibration data
         """
         calibration = DeviceCalibration()
         num_qubits = len(target.qubit_properties)
 
         for qubit in range(num_qubits):
@@ -208,35 +198,35 @@
                 calibration.two_qubit_gate_fidelity[(qubit1, qubit2)][instruction.name] = 1 - error
                 calibration.two_qubit_gate_duration[(qubit1, qubit2)][instruction.name] = duration
 
         return calibration
 
     @classmethod
     def __import_backend_v2(cls, backend: BackendV2) -> Device:
-        """
-        Import device data from a Qiskit `BackendV2` object.
+        """Import device data from a Qiskit `BackendV2` object.
+
         Args:
-            backend: the Qiskit `BackendV2` object
+            backend: the Qiskit `BackendV2` object.
 
         Returns: Collection of device data
         """
         device = Device()
         device.name = backend.name
         device.num_qubits = backend.num_qubits
         device.basis_gates = backend.operation_names
         device.coupling_map = backend.coupling_map.get_edges()
         device.calibration = cls.__import_target(backend.target)
         return device
 
     @classmethod
     def import_qiskit_backend(cls, backend: BackendV1 | BackendV2) -> Device:
-        """
-        Import device data from a Qiskit `Backend` object.
+        """Import device data from a Qiskit `Backend` object.
+
         Args:
-            backend: the Qiskit `Backend` object
+            backend: the Qiskit `Backend` object.
 
         Returns: Collection of device data
         """
         if isinstance(backend, BackendV1):
             return cls.__import_backend_v1(backend)
         if isinstance(backend, BackendV2):
             return cls.__import_backend_v2(backend)
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/ionq.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/ionq.py`

 * *Files 7% similar despite different names*

```diff
@@ -14,74 +14,67 @@
 
 
 Fidelity = TypedDict("Fidelity", {"1q": Statistics, "2q": Statistics, "spam": Statistics})
 Timing = TypedDict("Timing", {"t1": float, "t2": float, "1q": float, "2q": float, "readout": float, "reset": float})
 
 
 class IonQCalibration(TypedDict):
-    """
-    Class to store the calibration data of an IonQ device.
-    Follows https://docs.ionq.com/#tag/characterizations
+    """Class to store the calibration data of an IonQ device.
+    Follows https://docs.ionq.com/#tag/characterizations.
     """
 
     name: str
     basis_gates: list[str]
     connectivity: list[list[int]]
     fidelity: Fidelity
     num_qubits: int
     timing: Timing
 
 
 class IonQProvider(Provider):
-    """
-    Class to manage IonQ devices.
-    """
+    """Class to manage IonQ devices."""
 
     provider_name = "ionq"
 
     @classmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get the names of all available IonQ devices.
-        """
+        """Get the names of all available IonQ devices."""
         return ["ionq_harmony", "ionq_aria1"]  # NOTE: update when adding new devices
 
     @classmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
         return ["rxx", "rz", "ry", "rx", "measure", "barrier"]  # harmony, aria1
 
     @classmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import an IonQ backend as a Device object.
+        """Import an IonQ backend as a Device object.
+
         Args:
-            path: the path to the JSON file containing the calibration data
+            path: the path to the JSON file containing the calibration data.
 
         Returns: the Device object
         """
         with path.open() as json_file:
             ionq_calibration = cast(IonQCalibration, json.load(json_file))
 
         device = Device()
         device.name = ionq_calibration["name"]
         device.num_qubits = ionq_calibration["num_qubits"]
         device.basis_gates = ionq_calibration["basis_gates"]
         device.coupling_map = list(ionq_calibration["connectivity"])
         calibration = DeviceCalibration()
         for qubit in range(device.num_qubits):
-            calibration.single_qubit_gate_fidelity[qubit] = {
-                gate: ionq_calibration["fidelity"]["1q"]["mean"] for gate in ["ry", "rx"]
-            }
+            calibration.single_qubit_gate_fidelity[qubit] = dict.fromkeys(
+                ["ry", "rx"], ionq_calibration["fidelity"]["1q"]["mean"]
+            )
             calibration.single_qubit_gate_fidelity[qubit]["rz"] = 1  # rz is always perfect
-            calibration.single_qubit_gate_duration[qubit] = {
-                gate: ionq_calibration["timing"]["1q"] for gate in ["ry", "rx"]
-            }
+            calibration.single_qubit_gate_duration[qubit] = dict.fromkeys(
+                ["ry", "rx"], ionq_calibration["timing"]["1q"]
+            )
             calibration.single_qubit_gate_duration[qubit]["rz"] = 0  # rz is always instantaneous
             calibration.readout_fidelity[qubit] = ionq_calibration["fidelity"]["spam"]["mean"]
             calibration.readout_duration[qubit] = ionq_calibration["timing"]["readout"]
             calibration.t1[qubit] = ionq_calibration["timing"]["t1"]
             calibration.t2[qubit] = ionq_calibration["timing"]["t2"]
 
         for qubit1, qubit2 in device.coupling_map:
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/oqc.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/oqc.py`

 * *Files 18% similar despite different names*

```diff
@@ -6,91 +6,75 @@
 if TYPE_CHECKING:
     from pathlib import Path
 
 from mqt.bench.devices import Device, DeviceCalibration, Provider
 
 
 class QubitProperties(TypedDict):
-    """
-    Class to store the properties of a single qubit.
-    """
+    """Class to store the properties of a single qubit."""
 
     T1: float
     T2: float
     fRB: float
     fRO: float
     qubit: float
 
 
 class Coupling(TypedDict):
-    """
-    Class to store the connectivity of a two-qubit gate.
-    """
+    """Class to store the connectivity of a two-qubit gate."""
 
     control_qubit: float
     target_qubit: float
 
 
 class TwoQubitProperties(TypedDict):
-    """
-    Class to store the properties of a two-qubit gate.
-    """
+    """Class to store the properties of a two-qubit gate."""
 
     coupling: Coupling
     fCX: float
 
 
 class Properties(TypedDict):
-    """
-    Class to store the properties of a device.
-    """
+    """Class to store the properties of a device."""
 
     one_qubit: dict[str, QubitProperties]
     two_qubit: dict[str, TwoQubitProperties]
 
 
 class OQCCalibration(TypedDict):
-    """
-    Class to store the calibration data of an OQC device.
-    """
+    """Class to store the calibration data of an OQC device."""
 
     name: str
     basis_gates: list[str]
     num_qubits: int
     connectivity: list[list[int]]
     properties: Properties
 
 
 class OQCProvider(Provider):
-    """
-    Class to manage OQC devices
-    """
+    """Class to manage OQC devices."""
 
     provider_name = "oqc"
 
     @classmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get the names of all available OQC devices.
-        """
+        """Get the names of all available OQC devices."""
         return ["oqc_lucy"]  # NOTE: update when adding new devices
 
     @classmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
         return ["rz", "sx", "x", "ecr", "measure", "barrier"]  # lucy
 
     @classmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import an OQC backend.
+        """Import an OQC backend.
+
         Args:
-            path: the path to the JSON file containing the calibration data
+            path: the path to the JSON file containing the calibration data.
 
         Returns: the Device object
         """
         with path.open() as json_file:
             oqc_calibration = cast(OQCCalibration, json.load(json_file))
 
         device = Device()
@@ -105,12 +89,12 @@
                 gate: oqc_calibration["properties"]["one_qubit"][str(qubit)]["fRB"] for gate in ["rz", "sx", "x"]
             }
             calibration.readout_fidelity[qubit] = oqc_calibration["properties"]["one_qubit"][str(qubit)]["fRO"]
             calibration.t1[qubit] = oqc_calibration["properties"]["one_qubit"][str(qubit)]["T1"]
             calibration.t2[qubit] = oqc_calibration["properties"]["one_qubit"][str(qubit)]["T2"]
 
         for qubit1, qubit2 in device.coupling_map:
-            calibration.two_qubit_gate_fidelity[(qubit1, qubit2)] = {
-                gate: oqc_calibration["properties"]["two_qubit"][f"{qubit1}-{qubit2}"]["fCX"] for gate in ["ecr"]
-            }
+            calibration.two_qubit_gate_fidelity[(qubit1, qubit2)] = dict.fromkeys(
+                ["ecr"], oqc_calibration["properties"]["two_qubit"][f"{qubit1}-{qubit2}"]["fCX"]
+            )
         device.calibration = calibration
         return device
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/provider.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,75 +15,59 @@
     from mqt.bench.devices import Device
 
 from abc import ABC, abstractmethod
 
 
 @dataclass
 class Provider(ABC):
-    """
-    Abstract class for a quantum device provider.
-    """
+    """Abstract class for a quantum device provider."""
 
     @property
     @abstractmethod
     def provider_name(self) -> str:
-        """
-        Get the name of the provider.
-        """
+        """Get the name of the provider."""
 
     @classmethod
     def get_available_devices(cls, sanitize_device: bool = False) -> list[Device]:
-        """
-        Get a list of all available devices.
+        """Get a list of all available devices.
 
         Args:
             sanitize_device: whether to sanitize the device calibration data
         """
         return [cls.get_device(name, sanitize_device=sanitize_device) for name in cls.get_available_device_names()]
 
     @classmethod
     @abstractmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get a list of all available device names.
-        """
+        """Get a list of all available device names."""
 
     @classmethod
     @abstractmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
 
     @classmethod
     def get_available_basis_gates(cls) -> list[list[str]]:
-        """
-        Get a list of all available basis gates.
-        """
+        """Get a list of all available basis gates."""
         unique_basis_gates = {tuple(device.basis_gates) for device in cls.get_available_devices()}
         return [list(basis_gates) for basis_gates in unique_basis_gates]
 
     @classmethod
     def get_max_qubits(cls) -> int:
-        """
-        Get the maximum number of qubits offered by a device from the provider.
-        """
+        """Get the maximum number of qubits offered by a device from the provider."""
         return max([device.num_qubits for device in cls.get_available_devices()])
 
     @classmethod
     @abstractmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import a device from a file containing calibration data.
-        """
+        """Import a device from a file containing calibration data."""
 
     @classmethod
     def get_device(cls, name: str, sanitize_device: bool = False) -> Device:
-        """
-        Get a device by name.
+        """Get a device by name.
 
         Args:
             name: the name of the device
             sanitize_device: whether to sanitize the device calibration data
         """
         if name not in cls.get_available_device_names():
             msg = f"Device {name} not found."
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/quantinuum.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/quantinuum.py`

 * *Files 10% similar despite different names*

```diff
@@ -13,69 +13,62 @@
     mean: float
 
 
 Fidelity = TypedDict("Fidelity", {"1q": Statistics, "2q": Statistics, "spam": Statistics})
 
 
 class QuantinuumCalibration(TypedDict):
-    """
-    Class to store the calibration data of an Quantinuum device.
-    Follows https://docs.quantinuum.com/#tag/characterizations
+    """Class to store the calibration data of an Quantinuum device.
+    Follows https://docs.quantinuum.com/#tag/characterizations.
     """
 
     name: str
     basis_gates: list[str]
     connectivity: list[list[int]]
     fidelity: Fidelity
     num_qubits: int
 
 
 class QuantinuumProvider(Provider):
-    """
-    Class to manage Quantinuum devices.
-    """
+    """Class to manage Quantinuum devices."""
 
     provider_name = "quantinuum"
 
     @classmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get the names of all available Quantinuum devices.
-        """
+        """Get the names of all available Quantinuum devices."""
         return ["quantinuum_h2"]  # NOTE: update when adding new devices
 
     @classmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
         return ["rzz", "rz", "ry", "rx", "measure", "barrier"]  # h2
 
     @classmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import an Quantinuum backend as a Device object.
+        """Import an Quantinuum backend as a Device object.
+
         Args:
-            path: the path to the JSON file containing the calibration data
+            path: the path to the JSON file containing the calibration data.
 
         Returns: the Device object
         """
         with path.open() as json_file:
             quantinuum_calibration = cast(QuantinuumCalibration, json.load(json_file))
 
         device = Device()
         device.name = quantinuum_calibration["name"]
         device.num_qubits = quantinuum_calibration["num_qubits"]
         device.basis_gates = quantinuum_calibration["basis_gates"]
         device.coupling_map = list(quantinuum_calibration["connectivity"])
         calibration = DeviceCalibration()
         for qubit in range(device.num_qubits):
-            calibration.single_qubit_gate_fidelity[qubit] = {
-                gate: quantinuum_calibration["fidelity"]["1q"]["mean"] for gate in ["ry", "rx"]
-            }
+            calibration.single_qubit_gate_fidelity[qubit] = dict.fromkeys(
+                ["ry", "rx"], quantinuum_calibration["fidelity"]["1q"]["mean"]
+            )
             calibration.single_qubit_gate_fidelity[qubit]["rz"] = 1  # rz is always perfect
             calibration.readout_fidelity[qubit] = quantinuum_calibration["fidelity"]["spam"]["mean"]
 
         for qubit1, qubit2 in device.coupling_map:
             calibration.two_qubit_gate_fidelity[(qubit1, qubit2)] = {
                 "rzz": quantinuum_calibration["fidelity"]["2q"]["mean"]
             }
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/devices/rigetti.py` & `mqt.bench-1.1.1/src/mqt/bench/devices/rigetti.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,81 +7,68 @@
 if TYPE_CHECKING:
     from pathlib import Path
 
 from mqt.bench.devices import Device, DeviceCalibration, Provider
 
 
 class QubitProperties(TypedDict):
-    """
-    Class to store the properties of a single qubit.
-    """
+    """Class to store the properties of a single qubit."""
 
     fActiveReset: float
     fRO: float
     f1QRB: float
     f1QRB_std_err: float
     f1Q_simultaneous_RB: float
     f1Q_simultaneous_RB_std_err: float
     T1: float
     T2: float
 
 
 class TwoQubitProperties(TypedDict):
-    """
-    Class to store the properties of a two-qubit gate.
-    """
+    """Class to store the properties of a two-qubit gate."""
 
     fCZ: float
     fCZ_std_err: float
     fCPHASE: float
     fCPHASE_std_err: float
     fXY: float
     fXY_std_err: float
 
 
 Properties = TypedDict("Properties", {"1Q": dict[str, QubitProperties], "2Q": dict[str, TwoQubitProperties]})
 
 
 class RigettiCalibration(TypedDict):
-    """
-    Class to store the calibration data of a Rigetti device.
-    """
+    """Class to store the calibration data of a Rigetti device."""
 
     name: str
     num_qubits: int
     basis_gates: list[str]
     connectivity: list[tuple[int, int]]
     properties: Properties
 
 
 class RigettiProvider(Provider):
-    """
-    Class to manage Rigetti devices.
-    """
+    """Class to manage Rigetti devices."""
 
     provider_name = "rigetti"
 
     @classmethod
     def get_available_device_names(cls) -> list[str]:
-        """
-        Get the names of all available Rigetti devices.
-        """
+        """Get the names of all available Rigetti devices."""
         return ["rigetti_aspen_m3"]  # NOTE: update when adding new devices
 
     @classmethod
     def get_native_gates(cls) -> list[str]:
-        """
-        Get a list of provider specific native gates.
-        """
+        """Get a list of provider specific native gates."""
         return ["rx", "rz", "cz", "cp", "xx_plus_yy", "measure", "barrier"]  # aspen_m3
 
     @classmethod
     def __from_rigetti_index(cls, rigetti_index: int) -> int:
-        """
-        Convert the Rigetti qubit index to a consecutive index.
+        """Convert the Rigetti qubit index to a consecutive index.
         The Rigetti architectures consist of 8-qubit rings arranged in a two-dimensional grid.
         Each qubit is identified by a three digit number, where:
           * the first digit is the row index,
           * the second digit is the column index, and
           * the third digit is the ring index.
 
         Args:
@@ -99,18 +86,18 @@
         # rigetti_index: 136 = qubit_indx: 70
         if qubit_indx >= 70:
             qubit_indx = qubit_indx - 1
         return qubit_indx
 
     @classmethod
     def __to_rigetti_index(cls, index: int) -> int:
-        """
-        Convert the consecutive index to the Rigetti qubit index.
+        """Convert the consecutive index to the Rigetti qubit index.
+
         Args:
-            index: the consecutive index
+            index: the consecutive index.
 
         Returns: the Rigetti qubit index
         """
         # Account for missing qubit in Aspen-M3
         # rigetti_index: 136 = qubit_indx: 70
         if index >= 70:
             index = index + 1
@@ -119,18 +106,18 @@
         row = index // (ring_size * columns)
         column = (index % (ring_size * columns)) // ring_size
         ring = (index % (ring_size * columns)) % ring_size
         return row * 100 + column * 10 + ring
 
     @classmethod
     def import_backend(cls, path: Path) -> Device:
-        """
-        Import a Rigetti backend.
+        """Import a Rigetti backend.
+
         Args:
-            path: the path to the JSON file containing the calibration data
+            path: the path to the JSON file containing the calibration data.
 
         Returns: the Device object
         """
         with path.open() as json_file:
             rigetti_calibration = cast(RigettiCalibration, json.load(json_file))
 
         device = Device()
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation.py` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation_data.pkl` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_data.pkl`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/evaluation_visualization.ipynb` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/evaluation_visualization.ipynb`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/results/pie.pdf` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/pie.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/results/qubit_dist.pdf` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/qubit_dist.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/evaluation/results/violins.pdf` & `mqt.bench-1.1.1/src/mqt/bench/evaluation/results/violins.pdf`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/bench/qiskit_helper.py` & `mqt.bench-1.1.1/src/mqt/bench/qiskit_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,26 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | QuantumCircuit:
     """Handles the creation of the benchmark on the target-independent level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     num_qubits -- number of qubits
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-
     filename_indep = target_filename if target_filename else qc.name + "_indep_qiskit_" + str(num_qubits)
 
     path = Path(target_directory, filename_indep + ".qasm")
     if file_precheck and path.is_file():
         return True
     openqasm_gates = utils.get_openqasm_gates()
     target_independent = transpile(qc, basis_gates=openqasm_gates, optimization_level=1, seed_transpiler=10)
@@ -110,29 +109,28 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | QuantumCircuit:
     """Handles the creation of the benchmark on the target-dependent native gates level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     provider -- determines the native gate set
     num_qubits -- number of qubits
     opt_level -- optimization level
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-
     if not target_filename:
         filename_native = (
             qc.name + "_nativegates_" + provider.provider_name + "_qiskit_opt" + str(opt_level) + "_" + str(num_qubits)
         )
     else:
         filename_native = target_filename
 
@@ -188,29 +186,28 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | QuantumCircuit:
     """Handles the creation of the benchmark on the target-dependent mapped level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     num_qubits -- number of qubits
     device -- target device
     opt_level -- optimization level
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-
     if not target_filename:
         filename_mapped = qc.name + "_mapped_" + device.name + "_qiskit_opt" + str(opt_level) + "_" + str(num_qubits)
     else:
         filename_mapped = target_filename
 
     path = Path(target_directory, filename_mapped + ".qasm")
     if file_precheck and path.is_file():
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/tket_helper.py` & `mqt.bench-1.1.1/src/mqt/bench/tket_helper.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | Circuit:
     """Handles the creation of the benchmark on the target-independent level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     num_qubits -- number of qubits
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
@@ -147,28 +147,27 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | Circuit:
     """Handles the creation of the benchmark on the target-dependent native gates level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     provider -- determines the native gate set
     num_qubits -- number of qubits
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-
     if not target_filename:
         filename_native = qc.name + "_nativegates_" + provider.provider_name + "_tket_" + str(num_qubits)
     else:
         filename_native = target_filename
 
     path = Path(target_directory, filename_native + ".qasm")
     if file_precheck and path.is_file():
@@ -237,29 +236,28 @@
     file_precheck: bool,
     return_qc: bool = False,
     target_directory: str = "./",
     target_filename: str = "",
 ) -> bool | Circuit:
     """Handles the creation of the benchmark on the target-dependent mapped level.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc -- quantum circuit which the to be created benchmark circuit is based on
     num_qubits -- number of qubits
     device -- target device
     lineplacement -- if true line placement is used, else graph placement
     file_precheck -- flag indicating whether to check whether the file already exists before creating it (again)
     return_qc -- flag if the actual circuit shall be returned
     target_directory -- alternative directory to the default one to store the created circuit
     target_filename -- alternative filename to the default one
 
     Return values:
     if return_qc == True -- quantum circuit object
     else -- True/False indicating whether the function call was successful or not
     """
-
     placement = "line" if lineplacement else "graph"
 
     if not target_filename:
         filename_mapped = qc.name + "_mapped_" + device.name + "_tket_" + placement + "_" + str(num_qubits)
     else:
         filename_mapped = target_filename
```

### Comparing `mqt.bench-1.1.0/src/mqt/bench/utils.py` & `mqt.bench-1.1.1/src/mqt/bench/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,15 +104,15 @@
     """Returns the path where the zip file is stored."""
     return str(resources.files("mqt.benchviewer") / "static/files/MQTBench_all.zip")
 
 
 def get_examplary_max_cut_qp(n_nodes: int, degree: int = 2) -> QuadraticProgram:
     """Returns a quadratic problem formulation of a max cut problem of a random graph.
 
-    Keyword arguments:
+    Keyword Arguments:
     n_nodes -- number of graph nodes (and also number of qubits)
     degree -- edges per node
     """
     graph = nx.random_regular_graph(d=degree, n=n_nodes, seed=111)
     maxcut = Maxcut(graph)
     return maxcut.to_quadratic_program()
 
@@ -172,22 +172,21 @@
     gate_set: list[str] | None = None,
     mapped: bool = False,
     c_map: list[list[int]] | None = None,
     target_directory: str = "",
 ) -> bool:
     """Saves a quantum circuit as a qasm file.
 
-    Keyword arguments:
+    Keyword Arguments:
     qc_str -- Quantum circuit to be stored as a string
     filename -- filename
     gate_set -- set of used gates
     mapped -- boolean indicating whether the quantum circuit is mapped to a specific hardware layout
     c_map -- coupling map of used hardware layout
     """
-
     if c_map is None:
         c_map = []
 
     file = Path(target_directory, filename + ".qasm")
 
     try:
         mqtbench_module_version = metadata.version("mqt.bench")
@@ -234,15 +233,15 @@
         qasm_path = get_default_qasm_output_path()
     return subprocess.call(f"zip -rj {zip_path} {qasm_path}", shell=True)
 
 
 def calc_supermarq_features(
     qc: QuantumCircuit,
 ) -> SupermarqFeatures:
-    """Calculates the Supermarq features for a given quantum circuit. Code adapted from https://github.com/Infleqtion/client-superstaq/blob/91d947f8cc1d99f90dca58df5248d9016e4a5345/supermarq-benchmarks/supermarq/converters.py"""
+    """Calculates the Supermarq features for a given quantum circuit. Code adapted from https://github.com/Infleqtion/client-superstaq/blob/91d947f8cc1d99f90dca58df5248d9016e4a5345/supermarq-benchmarks/supermarq/converters.py."""
     num_qubits = qc.num_qubits
     dag = circuit_to_dag(qc)
     dag.remove_all_ops_named("barrier")
 
     # Program communication = circuit's average qubit degree / degree of a complete graph.
     graph = nx.Graph()
     for op in dag.two_qubit_ops():
```

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/backend.py` & `mqt.bench-1.1.1/src/mqt/benchviewer/backend.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,15 @@
 
         self.database: pd.DataFrame | None = None
         self.mqtbench_all_zip: ZipFile | None = None
 
     def filter_database(self, benchmark_config: BenchmarkConfiguration) -> list[str]:
         """Filters the database according to the filter criteria.
 
-        Keyword arguments:
+        Keyword Arguments:
         filterCriteria -- list of all filter criteria
         database -- database containing all available benchmarks
 
 
         Return values:
         db_filtered["path"].to_list() -- list of all file paths of the selected benchmark files
         """
@@ -247,15 +247,15 @@
 
     def generate_zip_ephemeral_chunks(
         self,
         filenames: list[str],
     ) -> Iterable[bytes]:
         """Generates the zip file for the selected benchmarks and returns a generator of the chunks.
 
-        Keyword arguments:
+        Keyword Arguments:
         paths -- list of file paths for all selected benchmarks
 
         Return values:
             Generator of bytes to send to the browser
         """
         fileobj = NoSeekBytesIO(io.BytesIO())
 
@@ -276,25 +276,24 @@
         fileobj.hidden_seek(0)
         yield fileobj.read()
         fileobj.close()
 
     def get_selected_file_paths(self, prepared_data: BenchmarkConfiguration) -> list[str]:
         """Extracts all file paths according to the prepared user's filter criteria.
 
-        Keyword arguments:
+        Keyword Arguments:
         prepared_data -- user's filter criteria after preparation step
 
         Return values:
         file_paths -- list of filter criteria for each selected benchmark
         """
         return self.filter_database(prepared_data)
 
     def init_database(self) -> bool:
         """Generates the database and saves it into a global variable."""
-
         assert self.mqtbench_all_zip is not None
 
         print("Initiating database...")
         self.database = create_database(self.mqtbench_all_zip)
         print(f"... done: {len(self.database)} benchmarks.")
 
         if not self.database.empty:
@@ -461,15 +460,15 @@
                 bar.update(size)
         print(f"Download completed to {fname}. Server is starting now.")
 
 
 def parse_data(filename: str) -> ParsedBenchmarkName:
     """Extracts the necessary information from a given filename.
 
-    Keyword arguments:
+    Keyword Arguments:
     filename -- name of file
 
     Return values:
     parsed_data -- parsed data extracted from filename
     """
     benchmark = filename.split("_")[0].lower()
     num_qubits = get_num_qubits(filename)
@@ -538,34 +537,34 @@
     if m:
         return int(m.group()[1:])
     return False
 
 
 def get_opt_level(filename: str) -> int:
     """Extracts the optimization level based on a filename.
-    Keyword arguments:
+
+    Keyword Arguments:
     filename -- filename of a benchmark
     Return values:
-    num -- optimization level
+    num -- optimization level.
     """
-
     pat = re.compile(r"opt\d")
     m = pat.search(filename)
     num = m.group()[-1:] if m else -1
     return int(cast(str, num))
 
 
 def get_num_qubits(filename: str) -> int:
     """Extracts the number of qubits based on a filename.
-    Keyword arguments:
+
+    Keyword Arguments:
     filename -- filename of a benchmark
     Return values:
-    num -- number of qubits
+    num -- number of qubits.
     """
-
     pat = re.compile(r"(\d+)\.")
     m = pat.search(filename)
     num = m.group()[0:-1] if m else -1
     return int(cast(str, num))
 
 
 def get_tket_settings(filename: str) -> str | None:
@@ -615,18 +614,19 @@
     if "tket" in filename:
         return "tket", get_tket_settings(filename)
     raise ValueError("Unknown compiler: " + filename)
 
 
 def create_database(zip_file: ZipFile) -> pd.DataFrame:
     """Creates the database based on the provided directories.
-    Keyword arguments:
+
+    Keyword Arguments:
     qasm_path -- zip containing all .qasm files
     Return values:
-    database -- database containing all available benchmarks
+    database -- database containing all available benchmarks.
     """
     rows_list = []
 
     for filename in zip_file.namelist():
         if filename.endswith(".qasm"):
             parsed_data = parse_data(filename)
             rows_list.append(parsed_data)
```

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/main.py` & `mqt.bench-1.1.1/src/mqt/benchviewer/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 class Server:
     def __init__(
         self,
         target_location: str,
         skip_question: bool = False,
         activate_logging: bool = False,
-    ):
+    ) -> None:
         self.backend = Backend()
 
         self.target_location = target_location
         if not os.access(self.target_location, os.W_OK):
             msg = "target_location is not writable. Please specify a different path."
             raise RuntimeError(msg)
 
@@ -122,31 +122,28 @@
         nonscalable_benchmarks=SERVER.backend.nonscalable_benchmarks,
     )
 
 
 @app.route(f"{PREFIX}/legal")
 def legal() -> str:
     """Return the legal.html file."""
-
     return render_template("legal.html")
 
 
 @app.route(f"{PREFIX}/description")
 def description() -> str:
     """Return the description.html file in which the file formats are described."""
-
     return render_template("description.html")
 
 
 @app.route(f"{PREFIX}/benchmark_description")
 def benchmark_description() -> str:
     """Return the benchmark_description.html file together in which all benchmark algorithms
     are described in detail.
     """
-
     return render_template("benchmark_description.html")
 
 
 @app.route(f"{PREFIX}/get_num_benchmarks", methods=["POST"])
 def get_num_benchmarks() -> Response:
     if request.method == "POST":
         data = request.form
```

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/static/favicon.ico` & `mqt.bench-1.1.1/src/mqt/benchviewer/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/static/mqt_dark.png` & `mqt.bench-1.1.1/src/mqt/benchviewer/static/mqt_dark.png`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/static/tum_logo.svg` & `mqt.bench-1.1.1/src/mqt/benchviewer/static/tum_logo.svg`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/templates/benchmark_description.html` & `mqt.bench-1.1.1/src/mqt/benchviewer/templates/benchmark_description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/templates/description.html` & `mqt.bench-1.1.1/src/mqt/benchviewer/templates/description.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/templates/index.html` & `mqt.bench-1.1.1/src/mqt/benchviewer/templates/index.html`

 * *Files 1% similar despite different names*

```diff
@@ -638,15 +638,15 @@
       <p class="text-justify">
         For a more detailed description of MQT Bench, we are referring to the
         corresponding paper
         <a href="https://arxiv.org/pdf/2204.13719.pdf" target="_blank"
           >"MQT Bench: Benchmarking Software and Design Automation Tools for
           Quantum Computing"</a
         >. Our implementation is available on
-        <a href="https://github.com/cda-tum/MQTBench" target="_blank">Github</a
+        <a href="https://github.com/cda-tum/MQTBench" target="_blank">GitHub</a
         >.
 
         <strong
           >In case you are using MQT Bench in your work, we would be thankful if
           you referred to it by citing the following publication:</strong
         >
       </p>
```

#### html2text {}

```diff
@@ -79,15 +79,15 @@
 After the download button is clicked, all benchmarks provided as ..qqaassmm files
 are downloaded as a ..zziipp archive. Details of the _f_i_l_e_ _f_o_r_m_a_t are provided.
 Alternatively, a pre-generated archive with aallll benchmarks can be _d_o_w_n_l_o_a_d_e_d.
 Download selected Benchmarks
 ****** RReeffeerreennccee ******
 For a more detailed description of MQT Bench, we are referring to the
 corresponding paper _"_M_Q_T_ _B_e_n_c_h_:_ _B_e_n_c_h_m_a_r_k_i_n_g_ _S_o_f_t_w_a_r_e_ _a_n_d_ _D_e_s_i_g_n_ _A_u_t_o_m_a_t_i_o_n
-_T_o_o_l_s_ _f_o_r_ _Q_u_a_n_t_u_m_ _C_o_m_p_u_t_i_n_g_". Our implementation is available on _G_i_t_h_u_b. IInn
+_T_o_o_l_s_ _f_o_r_ _Q_u_a_n_t_u_m_ _C_o_m_p_u_t_i_n_g_". Our implementation is available on _G_i_t_H_u_b. IInn
 ccaassee yyoouu aarree uussiinngg MMQQTT BBeenncchh iinn yyoouurr wwoorrkk,, wwee wwoouulldd bbee tthhaannkkffuull iiff yyoouu rreeffeerrrreedd
 ttoo iitt bbyy cciittiinngg tthhee ffoolllloowwiinngg ppuubblliiccaattiioonn::
 @article{quetschlich2023mqtbench,
   title={{{MQT Bench}}: Benchmarking Software and Design Automation Tools for
 Quantum Computing},
   shorttitle = {{MQT Bench}},
   journal = {{Quantum}},
```

### Comparing `mqt.bench-1.1.0/src/mqt/benchviewer/templates/legal.html` & `mqt.bench-1.1.1/src/mqt/benchviewer/templates/legal.html`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/src/mqt.bench.egg-info/PKG-INFO` & `mqt.bench-1.1.1/src/mqt.bench.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mqt.bench
-Version: 1.1.0
+Version: 1.1.1
 Summary: MQT Bench - A MQT tool for Benchmarking Quantum Software Tools
 Author-email: Nils Quetschlich <nils.quetschlich@tum.de>, Lukas Burgholzer <lukas.burgholzer@tum.de>
 License: MIT License
         
         Copyright (c) 2022 Nils Quetschlich, Lukas Burgholzer, and Robert Wille
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -42,15 +42,15 @@
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Intended Audience :: Science/Research
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pytket-qiskit<0.51.0,>=0.50.0
+Requires-Dist: pytket-qiskit<0.53.0,>=0.50.0
 Requires-Dist: qiskit_optimization
 Requires-Dist: qiskit_nature
 Requires-Dist: qiskit_finance
 Requires-Dist: pandas>=1.0.0
 Requires-Dist: flask>=2.0.0
 Requires-Dist: networkx>=2.0.0
 Requires-Dist: pyscf>=2.3.0
```

### Comparing `mqt.bench-1.1.0/src/mqt.bench.egg-info/SOURCES.txt` & `mqt.bench-1.1.1/src/mqt.bench.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 .gitignore
 .pre-commit-config.yaml
 .readthedocs.yaml
 CITATION.bib
 LICENSE
 MANIFEST.in
 README.md
+noxfile.py
 pyproject.toml
 .github/codecov.yml
 .github/contributing.rst
 .github/dependabot.yml
 .github/release-drafter.yml
 .github/support.rst
 .github/ISSUE_TEMPLATE/bug-report.yml
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_devices.py` & `mqt.bench-1.1.1/tests/devices/test_devices.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,17 +14,15 @@
 )
 
 
 @pytest.mark.parametrize(
     "device", get_available_devices(sanitize_device=True), ids=lambda device: cast(str, device.name)
 )
 def test_sanitized_devices(device: Device) -> None:
-    """
-    Test that all devices can be sanitized and provide complete fidelity data.
-    """
+    """Test that all devices can be sanitized and provide complete fidelity data."""
     assert device.calibration is not None
     for qubit in range(device.num_qubits):
         assert qubit in device.calibration.single_qubit_gate_fidelity
         for gate in device.get_single_qubit_gates():
             assert gate in device.calibration.single_qubit_gate_fidelity[qubit]
             assert device.calibration.single_qubit_gate_fidelity[qubit][gate] > 0
         assert qubit in device.calibration.readout_fidelity
@@ -33,17 +31,15 @@
         assert (qubit1, qubit2) in device.calibration.two_qubit_gate_fidelity
         for gate in device.get_two_qubit_gates():
             assert gate in device.calibration.two_qubit_gate_fidelity[(qubit1, qubit2)]
             assert device.calibration.two_qubit_gate_fidelity[(qubit1, qubit2)][gate] > 0
 
 
 def test_device_calibration_errors() -> None:
-    """
-    Test that all device calibration methods raise errors when no calibration data is available.
-    """
+    """Test that all device calibration methods raise errors when no calibration data is available."""
     device = Device(name="test", num_qubits=1, basis_gates=[], coupling_map=[], calibration=None)
 
     # Test all methods with no calibration
     with pytest.raises(ValueError, match="Calibration data not available for device test."):
         device.get_single_qubit_gate_fidelity("gate1", 0)
     with pytest.raises(ValueError, match="Calibration data not available for device test."):
         device.get_single_qubit_gate_duration("gate1", 0)
@@ -99,15 +95,13 @@
     with pytest.raises(ValueError, match="Readout fidelity values not available."):
         device.calibration.compute_average_readout_fidelity()
     with pytest.raises(ValueError, match="Readout duration values not available."):
         device.calibration.compute_average_readout_duration()
 
 
 def test_provider() -> None:
-    """
-    Test that all providers can be imported.
-    """
+    """Test that all providers can be imported."""
     for provider in get_available_providers():
         assert provider.provider_name in ["ibm", "rigetti", "oqc", "ionq", "quantinuum"]
 
     with pytest.raises(NotFoundError, match="Provider 'test' not found among available providers."):
         get_provider_by_name("test")
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_ibm_device_support.py` & `mqt.bench-1.1.1/tests/devices/test_ibm_device_support.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,33 +3,30 @@
 import pytest
 from qiskit_ibm_runtime.fake_provider import FakeMontreal, FakeMontrealV2
 
 from mqt.bench.devices import IBMProvider
 
 
 def test_ibm_provider_methods() -> None:
-    """
-    Test the methods of the IBMProvider class:
+    """Test the methods of the IBMProvider class:
     - get_available_device_names
     - get_available_basis_gates
     - get_native_gates
-    - get_max_qubits
+    - get_max_qubits.
     """
     assert IBMProvider.get_available_device_names() == ["ibm_washington", "ibm_montreal"]
     assert IBMProvider.get_available_basis_gates() == [["id", "rz", "sx", "x", "cx", "measure", "barrier"]]
     assert IBMProvider.get_native_gates() == ["id", "rz", "sx", "x", "cx", "measure", "barrier"]
     assert IBMProvider.get_max_qubits() == 127
     with pytest.raises(ValueError, match="Device ibm_unknown not found."):
         IBMProvider.get_device("ibm_unknown")
 
 
 def test_import_v1_backend() -> None:
-    """
-    Test importing a Qiskit `BackendV1` object.
-    """
+    """Test importing a Qiskit `BackendV1` object."""
     backend = FakeMontreal()
     device = IBMProvider.import_qiskit_backend(backend)
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == backend.name()
     assert device.num_qubits == backend.configuration().n_qubits
@@ -62,17 +59,15 @@
                 assert isinstance(device.calibration.compute_average_two_qubit_gate_fidelity(gate), float | int)
     if device.calibration is not None:
         assert isinstance(device.calibration.compute_average_readout_fidelity(), float | int)
         assert isinstance(device.calibration.compute_average_readout_duration(), float | int)
 
 
 def test_import_v2_backend() -> None:
-    """
-    Test importing a Qiskit `BackendV2` object.
-    """
+    """Test importing a Qiskit `BackendV2` object."""
     backend = FakeMontrealV2()
     device = IBMProvider.import_qiskit_backend(backend)
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == backend.name
     assert device.num_qubits == backend.num_qubits
@@ -105,17 +100,15 @@
                 assert isinstance(device.calibration.compute_average_two_qubit_gate_fidelity(gate), float | int)
     if device.calibration is not None:
         assert isinstance(device.calibration.compute_average_readout_fidelity(), float | int)
         assert isinstance(device.calibration.compute_average_readout_duration(), float | int)
 
 
 def test_get_ibm_washington_device() -> None:
-    """
-    Test getting the IBM Washington device.
-    """
+    """Test getting the IBM Washington device."""
     device = IBMProvider.get_device("ibm_washington")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "ibm_washington"
     assert device.num_qubits == 127
 
@@ -133,17 +126,15 @@
     for q0, q1 in device.coupling_map:
         for gate in two_qubit_gates:
             assert isinstance(device.get_two_qubit_gate_fidelity(gate, q0, q1), float | int)
             assert isinstance(device.get_two_qubit_gate_duration(gate, q0, q1), float | int)
 
 
 def test_get_ibmq_montreal_device() -> None:
-    """
-    Test getting the IBM Montreal device.
-    """
+    """Test getting the IBM Montreal device."""
     device = IBMProvider.get_device("ibm_montreal")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "ibm_montreal"
     assert device.num_qubits == 27
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_ionq_device_support.py` & `mqt.bench-1.1.1/tests/devices/test_ionq_device_support.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,30 +1,27 @@
 from __future__ import annotations
 
 from mqt.bench.devices import IonQProvider
 
 
 def test_ionq_provider_methods() -> None:
-    """
-    Test the methods of the IonQProvider class:
+    """Test the methods of the IonQProvider class:
     - get_available_device_names
     - get_available_basis_gates
     - get_native_gates
-    - get_max_qubits
+    - get_max_qubits.
     """
     assert IonQProvider.get_available_device_names() == ["ionq_harmony", "ionq_aria1"]
     assert IonQProvider.get_available_basis_gates() == [["rxx", "rz", "ry", "rx", "measure", "barrier"]]
     assert IonQProvider.get_native_gates() == ["rxx", "rz", "ry", "rx", "measure", "barrier"]
     assert IonQProvider.get_max_qubits() == 25
 
 
 def test_ionq_harmony_device() -> None:
-    """
-    Test the import of the IonQ Harmony quantum computer.
-    """
+    """Test the import of the IonQ Harmony quantum computer."""
     device = IonQProvider.get_device("ionq_harmony")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "ionq_harmony"
     assert device.num_qubits == 11
 
@@ -41,17 +38,15 @@
     for q0, q1 in device.coupling_map:
         for gate in two_qubit_gates:
             assert isinstance(device.get_two_qubit_gate_fidelity(gate, q0, q1), float | int)
             assert isinstance(device.get_two_qubit_gate_duration(gate, q0, q1), float | int)
 
 
 def test_ionq_aria1_device() -> None:
-    """
-    Test the import of the IonQ Aria quantum computer.
-    """
+    """Test the import of the IonQ Aria quantum computer."""
     device = IonQProvider.get_device("ionq_aria1")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "ionq_aria1"
     assert device.num_qubits == 25
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_oqc_device_support.py` & `mqt.bench-1.1.1/tests/devices/test_oqc_device_support.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 
 import pytest
 
 from mqt.bench.devices import OQCProvider
 
 
 def test_oqc_provider_methods() -> None:
-    """
-    Test the methods of the OQCrovider class:
+    """Test the methods of the OQCrovider class:
     - get_available_device_names
     - get_available_basis_gates
     - get_native_gates
-    - get_max_qubits
+    - get_max_qubits.
     """
     assert OQCProvider.get_available_device_names() == ["oqc_lucy"]
     assert OQCProvider.get_available_basis_gates() == [["rz", "sx", "x", "ecr", "measure", "barrier"]]
     assert OQCProvider.get_native_gates() == ["rz", "sx", "x", "ecr", "measure", "barrier"]
     assert OQCProvider.get_max_qubits() == 8
 
 
 def test_oqc_lucy_device() -> None:
-    """
-    Test the import of the OQC Lucy quantum computer.
-    """
+    """Test the import of the OQC Lucy quantum computer."""
     device = OQCProvider.get_device("oqc_lucy")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "oqc_lucy"
     assert device.num_qubits == 8
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_quantinuum_device_support.py` & `mqt.bench-1.1.1/tests/devices/test_quantinuum_device_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 
 import pytest
 
 from mqt.bench.devices import QuantinuumProvider
 
 
 def test_quantinuum_provider_methods() -> None:
-    """
-    Test the methods of the QuantinuumProvider class:
+    """Test the methods of the QuantinuumProvider class:
     - get_available_device_names
     - get_available_basis_gates
     - get_native_gates
-    - get_max_qubits
+    - get_max_qubits.
     """
     assert QuantinuumProvider.get_available_device_names() == ["quantinuum_h2"]
     assert QuantinuumProvider.get_available_basis_gates() == [["rzz", "rz", "ry", "rx", "measure", "barrier"]]
     assert QuantinuumProvider.get_native_gates() == ["rzz", "rz", "ry", "rx", "measure", "barrier"]
     assert QuantinuumProvider.get_max_qubits() == 32
 
 
 def test_quantinuum_h2_device() -> None:
-    """
-    Test the import of the Quantinuum H2 quantum computer.
-    """
+    """Test the import of the Quantinuum H2 quantum computer."""
     device = QuantinuumProvider.get_device("quantinuum_h2")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "quantinuum_h2"
     assert device.num_qubits == 32
```

### Comparing `mqt.bench-1.1.0/tests/devices/test_rigetti_device_support.py` & `mqt.bench-1.1.1/tests/devices/test_rigetti_device_support.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,31 +2,28 @@
 
 import pytest
 
 from mqt.bench.devices import RigettiProvider
 
 
 def test_rigetti_provider_methods() -> None:
-    """
-    Test the methods of the RigettiProvider class:
+    """Test the methods of the RigettiProvider class:
     - get_available_device_names
     - get_available_basis_gates
     - get_native_gates
-    - get_max_qubits
+    - get_max_qubits.
     """
     assert RigettiProvider.get_available_device_names() == ["rigetti_aspen_m3"]
     assert RigettiProvider.get_available_basis_gates() == [["rx", "rz", "cz", "cp", "xx_plus_yy", "measure", "barrier"]]
     assert RigettiProvider.get_native_gates() == ["rx", "rz", "cz", "cp", "xx_plus_yy", "measure", "barrier"]
     assert RigettiProvider.get_max_qubits() == 79
 
 
 def test_rigetti_aspen_m3_device() -> None:
-    """
-    Test the import of the Rigetti Aspen-M3 quantum computer.
-    """
+    """Test the import of the Rigetti Aspen-M3 quantum computer."""
     device = RigettiProvider.get_device("rigetti_aspen_m3")
     single_qubit_gates = device.get_single_qubit_gates()
     two_qubit_gates = device.get_two_qubit_gates()
 
     assert device.name == "rigetti_aspen_m3"
     assert device.num_qubits == 79
```

### Comparing `mqt.bench-1.1.0/tests/test_bench.py` & `mqt.bench-1.1.1/tests/test_bench.py`

 * *Files 0% similar despite different names*

```diff
@@ -330,28 +330,26 @@
             compiler="tket",
             device_name="oqc_lucy",
             gate_set_name="oqc",
         )
 
 
 def test_unidirectional_coupling_map() -> None:
-    from pytket.architecture import Architecture
-
     qc = get_benchmark(
         benchmark_name="dj",
         level="mapped",
         circuit_size=3,
         compiler="tket",
         compiler_settings=CompilerSettings(tket=TKETSettings(placement="graphplacement")),
         provider_name="oqc",
         device_name="oqc_lucy",
     )
     # check that all gates in the circuit are in the coupling map
     cmap = utils.convert_cmap_to_tuple_list(OQCProvider.get_device("oqc_lucy").coupling_map)
-    assert qc.valid_connectivity(arch=Architecture(cmap), directed=True)
+    assert qc.valid_connectivity(arch=pytket.architecture.Architecture(cmap), directed=True)
 
 
 @pytest.mark.parametrize(
     (
         "benchmark_name",
         "level",
         "circuit_size",
@@ -1088,30 +1086,30 @@
     assert 0 < regular_features.parallelism < 1
     assert 0 < regular_features.entanglement_ratio < 1
     assert 0 < regular_features.critical_depth < 1
     assert 0 < regular_features.program_communication < 1
     assert 0 < regular_features.liveness < 1
 
 
-def test_BenchmarkGenerator() -> None:
+def test_benchmark_generator() -> None:
     generator = BenchmarkGenerator(qasm_output_path="test")
     assert generator.qasm_output_path == "test"
     assert generator.timeout > 0
     assert generator.cfg is not None
 
 
 # This function is used to test the timeout watchers and needs two parameters since those values are logged when a timeout occurs.
 def endless_loop(arg1: SampleObject, run_forever: bool) -> bool:  # noqa: ARG001
     while run_forever:
         pass
     return True
 
 
 class SampleObject:
-    def __init__(self, name: str):
+    def __init__(self, name: str) -> None:
         self.name = name
 
 
 def test_timeout_watchers() -> None:
     timeout = 1
     assert not timeout_watcher(endless_loop, timeout, [SampleObject("test"), True])
     assert timeout_watcher(endless_loop, timeout, [SampleObject("test"), False])
```

### Comparing `mqt.bench-1.1.0/tests/test_benchviewer.py` & `mqt.bench-1.1.1/tests/test_benchviewer.py`

 * *Files identical despite different names*

### Comparing `mqt.bench-1.1.0/tests/test_pregenerated_zip.py` & `mqt.bench-1.1.1/tests/test_pregenerated_zip.py`

 * *Files identical despite different names*

