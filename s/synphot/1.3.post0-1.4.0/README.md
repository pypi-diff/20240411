# Comparing `tmp/synphot-1.3.post0.tar.gz` & `tmp/synphot-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synphot-1.3.post0.tar", last modified: Tue Nov 28 20:43:49 2023, max compression
+gzip compressed data, was "synphot-1.4.0.tar", last modified: Thu Apr 11 18:08:07 2024, max compression
```

## Comparing `synphot-1.3.post0.tar` & `synphot-1.4.0.tar`

### file list

```diff
@@ -1,128 +1,129 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:49.000996 synphot-1.3.post0/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2023-11-28 20:43:31.000000 synphot-1.3.post0/.bandit.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.980996 synphot-1.3.post0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.980996 synphot-1.3.post0/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1985 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0 runner    (1001) docker     (127)      929 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/PULL_REQUEST_TEMPLATE.md
--rw-r--r--   0 runner    (1001) docker     (127)      127 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/dependabot.yml
--rw-r--r--   0 runner    (1001) docker     (127)      800 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.980996 synphot-1.3.post0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/workflows/ci_workflows.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2856 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/workflows/codeql-analysis.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2487 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/workflows/open_actions.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/workflows/predeps_workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2023-11-28 20:43:31.000000 synphot-1.3.post0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      604 2023-11-28 20:43:31.000000 synphot-1.3.post0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      425 2023-11-28 20:43:31.000000 synphot-1.3.post0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3801 2023-11-28 20:43:31.000000 synphot-1.3.post0/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (127)      413 2023-11-28 20:43:31.000000 synphot-1.3.post0/CITATION.md
--rw-r--r--   0 runner    (1001) docker     (127)     3207 2023-11-28 20:43:31.000000 synphot-1.3.post0/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2023-11-28 20:43:31.000000 synphot-1.3.post0/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (127)      316 2023-11-28 20:43:31.000000 synphot-1.3.post0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-28 20:43:49.000996 synphot-1.3.post0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2023-11-28 20:43:31.000000 synphot-1.3.post0/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-28 20:43:31.000000 synphot-1.3.post0/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.984996 synphot-1.3.post0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     4724 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.984996 synphot-1.3.post0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    19012 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/_static/stsci_logo.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.976996 synphot-1.3.post0/docs/_templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.984996 synphot-1.3.post0/docs/_templates/autosummary/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/_templates/autosummary/base.rst
--rw-r--r--   0 runner    (1001) docker     (127)      251 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/_templates/autosummary/class.rst
--rw-r--r--   0 runner    (1001) docker     (127)      252 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/_templates/autosummary/module.rst
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    12536 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4513 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.984996 synphot-1.3.post0/docs/synphot/
--rw-r--r--   0 runner    (1001) docker     (127)    10208 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/bandpass.rst
--rw-r--r--   0 runner    (1001) docker     (127)       97 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/c_ext.rst
--rw-r--r--   0 runner    (1001) docker     (127)      285 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/config.rst
--rw-r--r--   0 runner    (1001) docker     (127)     4737 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/filter_par.rst
--rw-r--r--   0 runner    (1001) docker     (127)    11039 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/formulae.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18230 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/from_pysyn_iraf.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.988996 synphot-1.3.post0/docs/synphot/images/
--rw-r--r--   0 runner    (1001) docker     (127)   142118 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/VegaPhotomSys.png
--rw-r--r--   0 runner    (1001) docker     (127)    49541 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/bb5000_lmcavg.png
--rw-r--r--   0 runner    (1001) docker     (127)    49043 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/bb5000_renorm.png
--rw-r--r--   0 runner    (1001) docker     (127)    32169 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/johnson_bi.png
--rw-r--r--   0 runner    (1001) docker     (127)    42702 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/tutorial_em_line.png
--rw-r--r--   0 runner    (1001) docker     (127)    58060 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/tutorial_fit_ab.png
--rw-r--r--   0 runner    (1001) docker     (127)    41626 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/images/vega_spec.png
--rw-r--r--   0 runner    (1001) docker     (127)     7307 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/observation.rst
--rw-r--r--   0 runner    (1001) docker     (127)    28630 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/overview.rst
--rw-r--r--   0 runner    (1001) docker     (127)    18778 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/spectrum.rst
--rw-r--r--   0 runner    (1001) docker     (127)    10097 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/tutorials.rst
--rw-r--r--   0 runner    (1001) docker     (127)     9992 2023-11-28 20:43:31.000000 synphot-1.3.post0/docs/synphot/units.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.988996 synphot-1.3.post0/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)      250 2023-11-28 20:43:31.000000 synphot-1.3.post0/licenses/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2023-11-28 20:43:31.000000 synphot-1.3.post0/licenses/TYNT_LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      146 2023-11-28 20:43:31.000000 synphot-1.3.post0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2351 2023-11-28 20:43:49.000996 synphot-1.3.post0/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (127)     1546 2023-11-28 20:43:31.000000 synphot-1.3.post0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.988996 synphot-1.3.post0/synphot/
--rw-r--r--   0 runner    (1001) docker     (127)      719 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16408 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/binning.py
--rw-r--r--   0 runner    (1001) docker     (127)     9377 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)      729 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)     3579 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2271 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.992996 synphot-1.3.post0/synphot/filter_parameterization/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/filter_parameterization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7528 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/filter_parameterization/filter_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.992996 synphot-1.3.post0/synphot/filter_parameterization/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/filter_parameterization/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.992996 synphot-1.3.post0/synphot/filter_parameterization/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)    11520 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/filter_parameterization/tests/data/fft_test_data.fits
--rw-r--r--   0 runner    (1001) docker     (127)     2783 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/filter_parameterization/tests/test_filter_fft.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.992996 synphot-1.3.post0/synphot/include/
--rw-r--r--   0 runner    (1001) docker     (127)      778 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/include/synphot_utils.h
--rw-r--r--   0 runner    (1001) docker     (127)    27606 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    24911 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/observation.py
--rw-r--r--   0 runner    (1001) docker     (127)    10216 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/reddening.py
--rw-r--r--   0 runner    (1001) docker     (127)    12708 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/specio.py
--rw-r--r--   0 runner    (1001) docker     (127)    69441 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/spectrum.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.992996 synphot-1.3.post0/synphot/src/
--rw-r--r--   0 runner    (1001) docker     (127)     3501 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/src/synphot_utils.c
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:48.996996 synphot-1.3.post0/synphot/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:49.000996 synphot-1.3.post0/synphot/tests/data/
--rw-r--r--   0 runner    (1001) docker     (127)   521280 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits
--rw-r--r--   0 runner    (1001) docker     (127)   120960 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/grw_70d5824_stisnic_005.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f555w.fits
--rw-r--r--   0 runner    (1001) docker     (127)    86400 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits
--rw-r--r--   0 runner    (1001) docker     (127)   118080 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f850lp.fits
--rw-r--r--   0 runner    (1001) docker     (127)    25920 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/k93_4500_0_5_rn_box.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8640 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/milkyway_diffuse_001.fits
--rw-r--r--   0 runner    (1001) docker     (127)    61614 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/qso_template_001.dat
--rw-r--r--   0 runner    (1001) docker     (127)    88008 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin
--rw-r--r--   0 runner    (1001) docker     (127)    46080 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits
--rw-r--r--   0 runner    (1001) docker     (127)     8988 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/us7.txt
--rw-r--r--   0 runner    (1001) docker     (127)    89280 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits
--rw-r--r--   0 runner    (1001) docker     (127)     9927 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_binning.py
--rw-r--r--   0 runner    (1001) docker     (127)      967 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_blackbody.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_integrator.py
--rw-r--r--   0 runner    (1001) docker     (127)     9433 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)    18003 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_observation.py
--rw-r--r--   0 runner    (1001) docker     (127)     6654 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_reddening.py
--rw-r--r--   0 runner    (1001) docker     (127)     5359 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_specio.py
--rw-r--r--   0 runner    (1001) docker     (127)    10482 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_spectrum_bandpass.py
--rw-r--r--   0 runner    (1001) docker     (127)    15792 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_spectrum_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25824 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_spectrum_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_thermal.py
--rw-r--r--   0 runner    (1001) docker     (127)     7512 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_units.py
--rw-r--r--   0 runner    (1001) docker     (127)     6192 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4800 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/thermal.py
--rw-r--r--   0 runner    (1001) docker     (127)    11151 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/units.py
--rw-r--r--   0 runner    (1001) docker     (127)    10421 2023-11-28 20:43:31.000000 synphot-1.3.post0/synphot/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-28 20:43:49.000996 synphot-1.3.post0/synphot.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1209 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3130 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      129 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2023-11-28 20:43:48.000000 synphot-1.3.post0/synphot.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2913 2023-11-28 20:43:31.000000 synphot-1.3.post0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.330965 synphot-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-11 18:07:55.000000 synphot-1.4.0/.bandit.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.310965 synphot-1.4.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.310965 synphot-1.4.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1985 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/PULL_REQUEST_TEMPLATE.md
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1532 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.310965 synphot-1.4.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/check_milestone.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3123 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/ci_workflows.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2859 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/codeql-analysis.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2350 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/open_actions.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1172 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/predeps_workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3599 2024-04-11 18:07:55.000000 synphot-1.4.0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      604 2024-04-11 18:07:55.000000 synphot-1.4.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 18:07:55.000000 synphot-1.4.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     4571 2024-04-11 18:07:55.000000 synphot-1.4.0/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-04-11 18:07:55.000000 synphot-1.4.0/CITATION.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3207 2024-04-11 18:07:55.000000 synphot-1.4.0/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-11 18:07:55.000000 synphot-1.4.0/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      316 2024-04-11 18:07:55.000000 synphot-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 18:08:07.330965 synphot-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-11 18:07:55.000000 synphot-1.4.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 18:07:55.000000 synphot-1.4.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.314965 synphot-1.4.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     4724 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.314965 synphot-1.4.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    19012 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/_static/stsci_logo.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.306965 synphot-1.4.0/docs/_templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.314965 synphot-1.4.0/docs/_templates/autosummary/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/_templates/autosummary/base.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      251 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/_templates/autosummary/class.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/_templates/autosummary/module.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12537 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4513 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.314965 synphot-1.4.0/docs/synphot/
+-rw-r--r--   0 runner    (1001) docker     (127)    10208 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/bandpass.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/c_ext.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/config.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     4737 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/filter_par.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    11039 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/formulae.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18230 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/from_pysyn_iraf.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.318965 synphot-1.4.0/docs/synphot/images/
+-rw-r--r--   0 runner    (1001) docker     (127)   142118 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/VegaPhotomSys.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49541 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/bb5000_lmcavg.png
+-rw-r--r--   0 runner    (1001) docker     (127)    49043 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/bb5000_renorm.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32169 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/johnson_bi.png
+-rw-r--r--   0 runner    (1001) docker     (127)    42702 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/tutorial_em_line.png
+-rw-r--r--   0 runner    (1001) docker     (127)    58060 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/tutorial_fit_ab.png
+-rw-r--r--   0 runner    (1001) docker     (127)    41626 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/images/vega_spec.png
+-rw-r--r--   0 runner    (1001) docker     (127)     7307 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/observation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    28483 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/overview.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    18778 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/spectrum.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    10097 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/tutorials.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     9992 2024-04-11 18:07:55.000000 synphot-1.4.0/docs/synphot/units.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.318965 synphot-1.4.0/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)      250 2024-04-11 18:07:55.000000 synphot-1.4.0/licenses/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-04-11 18:07:55.000000 synphot-1.4.0/licenses/TYNT_LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      150 2024-04-11 18:07:55.000000 synphot-1.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2232 2024-04-11 18:08:07.334965 synphot-1.4.0/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1546 2024-04-11 18:07:55.000000 synphot-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/
+-rw-r--r--   0 runner    (1001) docker     (127)      719 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16408 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9295 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3579 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2271 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/filter_parameterization/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/filter_parameterization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7528 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/filter_parameterization/filter_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/filter_parameterization/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/filter_parameterization/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/filter_parameterization/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)    11520 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/filter_parameterization/tests/data/fft_test_data.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     2783 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/filter_parameterization/tests/test_filter_fft.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/include/
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/include/synphot_utils.h
+-rw-r--r--   0 runner    (1001) docker     (127)    27396 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24911 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10260 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/reddening.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12987 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/specio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    69485 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/spectrum.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.322965 synphot-1.4.0/synphot/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     3501 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/src/synphot_utils.c
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.326965 synphot-1.4.0/synphot/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.330965 synphot-1.4.0/synphot/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   521280 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   120960 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/grw_70d5824_stisnic_005.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f555w.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    86400 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits
+-rw-r--r--   0 runner    (1001) docker     (127)   118080 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f850lp.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    25920 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/k93_4500_0_5_rn_box.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8640 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/milkyway_diffuse_001.fits
+-rw-r--r--   0 runner    (1001) docker     (127)    61614 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/qso_template_001.dat
+-rw-r--r--   0 runner    (1001) docker     (127)    88008 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin
+-rw-r--r--   0 runner    (1001) docker     (127)    46080 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     8988 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/us7.txt
+-rw-r--r--   0 runner    (1001) docker     (127)    89280 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits
+-rw-r--r--   0 runner    (1001) docker     (127)     9891 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_binning.py
+-rw-r--r--   0 runner    (1001) docker     (127)      967 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_blackbody.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_integrator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9433 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18003 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_observation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6374 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_reddening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8009 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_specio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10482 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_spectrum_bandpass.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15634 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_spectrum_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25824 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_spectrum_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_thermal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7512 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_units.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6219 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/thermal.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11635 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/units.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10421 2024-04-11 18:07:55.000000 synphot-1.4.0/synphot/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      411 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 18:08:07.330965 synphot-1.4.0/synphot.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1206 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3168 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      129 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-11 18:08:07.000000 synphot-1.4.0/synphot.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2910 2024-04-11 18:07:55.000000 synphot-1.4.0/tox.ini
```

### Comparing `synphot-1.3.post0/.github/ISSUE_TEMPLATE/bug_report.md` & `synphot-1.4.0/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/.github/ISSUE_TEMPLATE/feature_request.md` & `synphot-1.4.0/.github/ISSUE_TEMPLATE/feature_request.md`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/.github/ISSUE_TEMPLATE/question.md` & `synphot-1.4.0/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/.github/PULL_REQUEST_TEMPLATE.md` & `synphot-1.4.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/.github/workflows/ci_workflows.yml` & `synphot-1.4.0/.github/workflows/ci_workflows.yml`

 * *Files 5% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 jobs:
   initial_check:
     name: Mandatory checks before CI
     runs-on: ubuntu-latest
     steps:
     - name: Check base branch
-      uses: actions/github-script@v6
+      uses: actions/github-script@v7
       if: github.event_name == 'pull_request'
       with:
         script: |
           const allowed_basebranch = 'master';
           const pr = context.payload.pull_request;
           if (pr.base.ref !== allowed_basebranch) {
             core.setFailed(`PR opened against ${pr.base.ref}, not ${allowed_basebranch}`);
@@ -62,57 +62,57 @@
           - name: Link check
             os: ubuntu-latest
             python: 3.x
             toxenv: linkcheck
 
           - name: Test without optional deps
             os: ubuntu-latest
-            python: 3.9
-            toxenv: py39-test
+            python: '3.10'
+            toxenv: py310-test
 
           - name: Coverage test with remote data
             os: ubuntu-latest
-            python: '3.10'
-            toxenv: py310-test-alldeps-cov
+            python: '3.11'
+            toxenv: py311-test-alldeps-cov
             toxposargs: --remote-data
 
           - name: Test with dev dependencies
             os: ubuntu-latest
             python: '3.12'
             toxenv: py312-test-devdeps
 
           - name: Test with old dependencies
             os: ubuntu-20.04
-            python: 3.9
-            toxenv: py39-test-oldestdeps
+            python: '3.10'
+            toxenv: py310-test-oldestdeps
 
           - name: Test in OSX
             os: macos-latest
-            python: '3.10'
-            toxenv: py310-test-alldeps
+            python: '3.12'
+            toxenv: py312-test-alldeps
 
           # NOTE: If TRDS cannot take the hit, disable --remote-data
           - name: Test in Windows with remote data
             os: windows-latest
             python: '3.11'
             toxenv: py311-test-alldeps
             toxposargs: --remote-data
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python }}
     - name: Install Python dependencies
       run: |
         python -m pip install --upgrade pip tox
     - name: Run tests
       run: tox -e ${{ matrix.toxenv }} -- ${{ matrix.toxposargs }}
     - name: Upload coverage to codecov
       if: ${{ contains(matrix.toxenv,'-cov') }}
-      uses: codecov/codecov-action@v3
+      uses: codecov/codecov-action@v4
       with:
         file: ./coverage.xml
```

### Comparing `synphot-1.3.post0/.github/workflows/codeql-analysis.yml` & `synphot-1.4.0/.github/workflows/codeql-analysis.yml`

 * *Files 12% similar despite different names*

```diff
@@ -45,43 +45,43 @@
     - name: Checkout repository
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
 
     # Initializes the CodeQL tools for scanning.
     - name: Initialize CodeQL
-      uses: github/codeql-action/init@v2
+      uses: github/codeql-action/init@v3
       with:
         languages: ${{ matrix.language }}
         # If you wish to specify custom queries, you can do so here or in a config file.
         # By default, queries listed here will override any specified in a config file.
         # Prefix the list here with "+" to use these queries and those in the config file.
         # queries: ./path/to/local/query, your-org/your-repo/queries@main
 
     # Autobuild attempts to build any compiled languages  (C/C++, C#, or Java).
     # If this step fails, then you should remove it and run the build manually (see below)
     - name: Autobuild
       if: matrix.language != 'cpp'
-      uses: github/codeql-action/autobuild@v2
+      uses: github/codeql-action/autobuild@v3
 
     # ℹ️ Command-line programs to run using the OS shell.
     # 📚 https://git.io/JvXDl
 
     # ✏️ If the Autobuild fails above, remove it and uncomment the following three lines
     #    and modify them (or add more) to build your code if your project
     #    uses a compiled language
 
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       if: matrix.language == 'cpp'
       with:
-        python-version: 3.9
+        python-version: '3.12'
 
     - name: Manual build
       if: matrix.language == 'cpp'
       run: |
        pip install -U pip setuptools_scm wheel
        pip install numpy astropy
        python setup.py build_ext --inplace
 
     - name: Perform CodeQL Analysis
-      uses: github/codeql-action/analyze@v2
+      uses: github/codeql-action/analyze@v3
```

### Comparing `synphot-1.3.post0/.github/workflows/open_actions.yml` & `synphot-1.4.0/.github/workflows/open_actions.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,20 +9,20 @@
     - opened
 
 jobs:
   triage:
     runs-on: ubuntu-latest
     steps:
     - name: Label PR
-      uses: actions/labeler@v4
+      uses: actions/labeler@v5
       if: github.event_name == 'pull_request_target'
       with:
         repo-token: "${{ secrets.GITHUB_TOKEN }}"
     - name: 'Reviewer Checklist'
-      uses: actions/github-script@v6
+      uses: actions/github-script@v7
       if: github.event_name == 'pull_request_target'
       with:
         github-token: ${{ secrets.GITHUB_TOKEN }}
         script: |
           await github.rest.issues.createComment({
             issue_number: context.issue.number,
             owner: context.repo.owner,
@@ -32,25 +32,24 @@
             - [ ] Do the proposed changes actually accomplish desired goals?
             - [ ] Do the proposed changes follow the [STScI coding guidelines](https://github.com/spacetelescope/style-guides/blob/master/guides/python.md)?
             - [ ] Are tests added/updated as required? If so, do they follow the [STScI testing guidelines](https://github.com/spacetelescope/style-guides/blob/master/guides/python-testing.md)?
             - [ ] Are docs added/updated as required?
             - [ ] Is rebase and/or squash necessary? If so, please provide the author with appropriate instructions.
             - [ ] Did the CI pass? If no, are the failures related?
             - [ ] Is a change log needed?
-            - [ ] Is a milestone set? Milestone must be set but we cannot check for it on Actions; do not let the green checkmark fool you.`
           })
     - name: 'Comment Draft PR'
-      uses: actions/github-script@v6
+      uses: actions/github-script@v7
       if: github.event.pull_request.draft == true
       with:
         github-token: ${{ secrets.GITHUB_TOKEN }}
         script: |
           await github.rest.issues.createComment({
             issue_number: context.issue.number,
             owner: context.repo.owner,
             repo: context.repo.repo,
             body: '👋 Thank you for your draft pull request! Do you know that you can use `[ci skip]` or `[skip ci]` in your commit messages to skip running continuous integration tests until you are ready?'
           })
-    - name: Special comment
-      uses: pllim/action-special_pr_comment@main
-      with:
-        GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
+    #- name: Special comment
+    #  uses: pllim/action-special_pr_comment@main
+    #  with:
+    #    GITHUB_TOKEN: ${{ secrets.GITHUB_TOKEN }}
```

### Comparing `synphot-1.3.post0/.github/workflows/predeps_workflow.yml` & `synphot-1.4.0/.github/workflows/predeps_workflow.yml`

 * *Files 13% similar despite different names*

```diff
@@ -28,24 +28,24 @@
           - name: RC test on OSX
             os: macos-latest
             python: '3.10'
             toxenv: py310-test-predeps
 
           - name: RC test on Windows
             os: windows-latest
-            python: 3.9
-            toxenv: py39-test-predeps
+            python: '3.12'
+            toxenv: py312-test-predeps
 
     steps:
     - name: Checkout code
       uses: actions/checkout@v4
       with:
         fetch-depth: 0
     - name: Set up Python
-      uses: actions/setup-python@v4
+      uses: actions/setup-python@v5
       with:
         python-version: ${{ matrix.python }}
     - name: Install Python dependencies
       run: |
         python -m pip install --upgrade pip tox
     - name: Run tests
       run: tox -e ${{ matrix.toxenv }} -- ${{ matrix.toxposargs }}
```

### Comparing `synphot-1.3.post0/.github/workflows/publish-to-pypi.yml` & `synphot-1.4.0/.github/workflows/publish-to-pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,72 @@
 name: Release
 
 on:
   workflow_dispatch:
   release:
     types: [released]
+  pull_request:
+    # We also want this workflow triggered if the 'Build wheels'
+    # label is added or present when PR is updated
+    types:
+      - synchronize
+      - labeled
 
 concurrency:
   group: ${{ github.workflow }}-${{ github.ref }}
   cancel-in-progress: true
 
 jobs:
   build_wheels:
     name: Wheels on ${{ matrix.os }}
     runs-on: ${{ matrix.os }}
-    if: github.repository == 'spacetelescope/synphot_refactor'
+    if: (github.repository == 'spacetelescope/synphot_refactor' && ( github.event_name == 'release' || github.event_name == 'workflow_dispatch' || contains(github.event.pull_request.labels.*.name, 'Build wheels')))
     strategy:
       matrix:
         os: [ubuntu-latest, windows-latest, macos-latest]
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: |
         python -m pip install pip "twine>=3.3" -U
     - name: Build wheels
-      uses: pypa/cibuildwheel@v2.16.2
+      uses: pypa/cibuildwheel@v2.17.0
       env:
         CIBW_BUILD: 'cp39-* cp310-* cp311-* cp312-*'
         CIBW_SKIP: '*-musllinux_*'
         CIBW_ARCHS_LINUX: 'x86_64'
         CIBW_ARCHS_WINDOWS: 'AMD64'
         CIBW_ARCHS_MACOS: 'arm64'
         CIBW_TEST_SKIP: '*-macosx_arm64'
         CIBW_TEST_REQUIRES: 'pytest pytest-astropy'
         CIBW_TEST_COMMAND: 'python -c "import synphot; synphot.test()"'
     - name: Check wheels
       run: python -m twine check --strict wheelhouse/*
     # Upload artifacts because gh-action-pypi-publish Docker is only on Linux
     - name: Upload wheels
       if: github.event_name == 'release'
-      uses: actions/upload-artifact@v3
+      uses: actions/upload-artifact@v4
       with:
-        name: additional-pylons
+        name: additional-pylons-${{ matrix.os }}
         path: ./wheelhouse/*.whl
 
   build_dist:
-    name: Source dist and publish
+    name: Source dist
     runs-on: ubuntu-latest
-    needs: build_wheels
-    environment:
-      name: release
-      url: https://pypi.org/p/synphot
-    permissions:
-      id-token: write  # IMPORTANT: mandatory for trusted publishing
+    if: (github.repository == 'spacetelescope/synphot_refactor' && ( github.event_name == 'release' || github.event_name == 'workflow_dispatch' || contains(github.event.pull_request.labels.*.name, 'Build wheels')))
     steps:
     - uses: actions/checkout@v4
       with:
         fetch-depth: 0
-    - uses: actions/setup-python@v4
+    - uses: actions/setup-python@v5
       with:
         python-version: '3.x'
     - name: Install dependencies
       run: python -m pip install pip build "twine>=3.3" -U
     - name: Build package
       run: python -m build --sdist .
     - name: Check dist
@@ -74,16 +75,35 @@
       run: |
         cd ..
         python -m venv testenv
         testenv/bin/pip install -U pip
         testenv/bin/pip install pytest pytest-astropy
         testenv/bin/pip install synphot_refactor/dist/*.tar.gz
         testenv/bin/python -c "import synphot; synphot.test()"
-    - name: Download wheels
+    - name: Upload dist
       if: github.event_name == 'release'
-      uses: actions/download-artifact@v3
+      uses: actions/upload-artifact@v4
+      with:
+        name: additional-pylons-dist
+        path: ./dist/*.tar.gz
+
+  publish:
+    name: Publish to PyPI
+    needs: [build_wheels, build_dist]
+    if: github.repository == 'spacetelescope/synphot_refactor' && github.event_name == 'release'
+    runs-on: ubuntu-latest
+    environment:
+      name: release
+      url: https://pypi.org/p/synphot
+    permissions:
+      id-token: write  # IMPORTANT: mandatory for trusted publishing
+    steps:
+    - name: Download wheels
+      uses: actions/download-artifact@v4
       with:
-        name: additional-pylons
         path: dist
+        pattern: additional-pylons-*
+        merge-multiple: true
+    - name: Pylons inspection
+      run: ls dist/*
     - name: Publish package to PyPI
-      if: github.event_name == 'release'
       uses: pypa/gh-action-pypi-publish@release/v1
```

### Comparing `synphot-1.3.post0/.gitignore` & `synphot-1.4.0/.gitignore`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/CHANGES.rst` & `synphot-1.4.0/CHANGES.rst`

 * *Files 17% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+1.4.0 (2024-04-11)
+==================
+
+- ``read_fits_spec()`` now uses ``astropy.table.QTable.read`` for parsing to
+  ensure that the correct ``TUNITn`` is read. As a result, ``wave_unit`` and
+  ``flux_unit`` keywords are deprecated and no longer used in that function.
+  Additionally, if any ``TUNITn`` in the table is invalid, regardless whether
+  the column is used or not, an exception will now be raised. [#384]
+
+- ``read_spec()`` now detects whether given filename is FITS more consistently
+  w.r.t. ``astropy``. [#384]
+
+- Compatibility with ``numpy`` 2.0 and ``astropy`` 6.1 by building C-extension
+  against ``numpy`` 2.x ABI. [#387]
+
+- Bumped minimum supported versions for Python to 3.10,
+  ``numpy`` to 1.23, ``astropy`` to 6.0, and ``scipy`` to 1.9. [#387]
+
 1.3.0 (2023-11-28)
 ==================
 
 - Compatibility with ``numpy`` 2.0. [#363]
 
 - Bumped minimum supported versions for Python to 3.9,
   ``numpy`` to 1.20, ``astropy`` to 5.0, and ``scipy`` to 1.6. [#363]
```

### Comparing `synphot-1.3.post0/CODE_OF_CONDUCT.md` & `synphot-1.4.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/LICENSE.rst` & `synphot-1.4.0/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/PKG-INFO` & `synphot-1.4.0/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: synphot
-Version: 1.3.post0
+Version: 1.4.0
 Summary: Synthetic photometry
 Home-page: https://www.github.com/spacetelescope/synphot_refactor
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,synthetic,photometry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/plain
 License-File: LICENSE.rst
-Requires-Dist: numpy>=1.20
-Requires-Dist: astropy>=5
-Requires-Dist: scipy>=1.6
+Requires-Dist: numpy>=1.23
+Requires-Dist: astropy>=6
+Requires-Dist: scipy>=1.9
 Provides-Extra: all
 Requires-Dist: specutils>=0.7; extra == "all"
 Requires-Dist: dust-extinction; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
```

### Comparing `synphot-1.3.post0/README.rst` & `synphot-1.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/conftest.py` & `synphot-1.4.0/conftest.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/Makefile` & `synphot-1.4.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/_static/stsci_logo.png` & `synphot-1.4.0/docs/_static/stsci_logo.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/conf.py` & `synphot-1.4.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/index.rst` & `synphot-1.4.0/docs/index.rst`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 
 
 .. _synphot-installation-setup:
 
 Installation and Setup
 ======================
 
-**synphot** works for Python 3.9 or later only. It requires the following
+**synphot** works for Python 3.10 or later only. It requires the following
 packages:
 
 * numpy
 * astropy
 * scipy
 * matplotlib (optional for plotting)
 * specutils (optional)
```

### Comparing `synphot-1.3.post0/docs/make.bat` & `synphot-1.4.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/bandpass.rst` & `synphot-1.4.0/docs/synphot/bandpass.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/filter_par.rst` & `synphot-1.4.0/docs/synphot/filter_par.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/formulae.rst` & `synphot-1.4.0/docs/synphot/formulae.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/from_pysyn_iraf.rst` & `synphot-1.4.0/docs/synphot/from_pysyn_iraf.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/VegaPhotomSys.png` & `synphot-1.4.0/docs/synphot/images/VegaPhotomSys.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/bb5000_lmcavg.png` & `synphot-1.4.0/docs/synphot/images/bb5000_lmcavg.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/bb5000_renorm.png` & `synphot-1.4.0/docs/synphot/images/bb5000_renorm.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/johnson_bi.png` & `synphot-1.4.0/docs/synphot/images/johnson_bi.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/tutorial_em_line.png` & `synphot-1.4.0/docs/synphot/images/tutorial_em_line.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/tutorial_fit_ab.png` & `synphot-1.4.0/docs/synphot/images/tutorial_fit_ab.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/images/vega_spec.png` & `synphot-1.4.0/docs/synphot/images/vega_spec.png`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/observation.rst` & `synphot-1.4.0/docs/synphot/observation.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/overview.rst` & `synphot-1.4.0/docs/synphot/overview.rst`

 * *Files 2% similar despite different names*

```diff
@@ -392,17 +392,15 @@
 keywords (unless you overwrite them with non-default values in
 :func:`~synphot.specio.read_fits_spec`):
 
 * ``TTYPE1`` set to "WAVELENGTH".
 * ``TTYPE2`` set to "FLUX" (for source spectrum) or "THROUGHPUT"
   (for bandpass).
 
-While these were required in ASTROLIB PYSYNPHOT, they are optional here in that
-default units would be applied, where applicable, if they are missing from
-the header. Regardless, setting them is highly recommended:
+These were required in ASTROLIB PYSYNPHOT, as well as this package:
 
 * ``TUNIT1`` set to :ref:`supported wavelength unit name <synphot_units>`.
 * ``TUNIT2`` set to :ref:`supported flux unit name <synphot_units>`
   (source spectrum only).
 
 For writing out FITS table, many options can be set to non-default as
 acceptable by :func:`~synphot.specio.write_fits_spec`.
```

### Comparing `synphot-1.3.post0/docs/synphot/spectrum.rst` & `synphot-1.4.0/docs/synphot/spectrum.rst`

 * *Files 0% similar despite different names*

```diff
@@ -83,15 +83,15 @@
 +========+===========================+============+
 |mwavg   |Milky Way Diffuse, R(V)=3.1||mw_ext_ref||
 +--------+---------------------------+            |
 |mwdense |Milky Way Dense, R(V)=5.0  |            |
 +--------+---------------------------+            |
 |mwrv21  |Milky Way CCM, R(V)=2.1    |            |
 +--------+---------------------------+            |
-|mwrv4   |Milky Way CCM, R(V)=4.0    |            |
+|mwrv40  |Milky Way CCM, R(V)=4.0    |            |
 +--------+---------------------------+------------+
 |lmc30dor|LMC Supershell, R(V)=2.76  ||mc_ext_ref||
 +--------+---------------------------+            |
 |lmcavg  |LMC Average, R(V)=3.41     |            |
 +--------+---------------------------+            |
 |smcbar  |SMC Bar, R(V)=2.74         |            |
 +--------+---------------------------+------------+
```

### Comparing `synphot-1.3.post0/docs/synphot/tutorials.rst` & `synphot-1.4.0/docs/synphot/tutorials.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/docs/synphot/units.rst` & `synphot-1.4.0/docs/synphot/units.rst`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/licenses/TYNT_LICENSE.txt` & `synphot-1.4.0/licenses/TYNT_LICENSE.txt`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/setup.cfg` & `synphot-1.4.0/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 [tool:pytest]
 minversion = 6
 testpaths = "synphot" "docs"
 norecursedirs = build docs/_build synphot/src
 astropy_header = true
 doctest_plus = enabled
 doctest_subpackage_requires = 
-	docs/index.rst = astropy>=5.3
-	docs/synphot/spectrum.rst = astropy>=5.3
-	docs/synphot/tutorials.rst = astropy>=5.3
+	docs/synphot/filter_par.rst = numpy<2
 text_file_format = rst
 addopts = --doctest-rst --import-mode=append
 xfail_strict = true
 filterwarnings = 
 	error
 	ignore:can't resolve package from __spec__
 	ignore:numpy\.ndarray size changed:RuntimeWarning
 	ignore:numpy\.ufunc size changed:RuntimeWarning
 	ignore:distutils Version classes are deprecated:DeprecationWarning
 	ignore:Class CCM89 defines class attributes
-	ignore:.*numpy\.core.*:DeprecationWarning
 
 [metadata]
 name = synphot
 description = Synthetic photometry
 long_description = This is a package for doing synthetic photometry that relies on Astropy
 long_description_content_type = text/plain
 keywords = astronomy, astrophysics, synthetic, photometry
@@ -45,18 +42,18 @@
 
 [options]
 packages = find:
 zip_safe = False
 setup_requires = 
 	setuptools_scm
 install_requires = 
-	numpy>=1.20
-	astropy>=5
-	scipy>=1.6
-python_requires = >=3.9
+	numpy>=1.23
+	astropy>=6
+	scipy>=1.9
+python_requires = >=3.10
 
 [options.extras_require]
 all = 
 	specutils>=0.7
 	dust-extinction
 test = 
 	pytest-astropy
```

### Comparing `synphot-1.3.post0/setup.py` & `synphot-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/__init__.py` & `synphot-1.4.0/synphot/__init__.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/binning.py` & `synphot-1.4.0/synphot/binning.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/blackbody.py` & `synphot-1.4.0/synphot/blackbody.py`

 * *Files 6% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 from astropy.modeling.parameters import Parameter
 from astropy.utils.exceptions import AstropyUserWarning
 
 from synphot.units import FNU, FLAM
 
 __all__ = ['BlackBody1D', 'blackbody_nu', 'blackbody_lambda']
 
-# ASTROPY_LT_5_3
-__doctest_requires__ = {"BlackBody1D": ["astropy<5.3"]}
-
 with warnings.catch_warnings():
     warnings.simplefilter('ignore', RuntimeWarning)
     _has_buggy_expm1 = np.isnan(np.expm1(1000)) or np.isnan(np.expm1(1e10))
 
 
 class BlackBody1D(Fittable1DModel):
     """
@@ -55,15 +52,15 @@
 
     Examples
     --------
     >>> from astropy import units as u
     >>> from synphot.blackbody import BlackBody1D
     >>> bb = BlackBody1D()
     >>> bb(6000 * u.AA)  # doctest: +FLOAT_CMP
-    <Quantity 1.3585381201978953e-15 erg / (cm2 Hz s)>
+    <Quantity 1.35853828e-15 erg / (Hz s cm2)>
 
     .. plot::
         :include-source:
 
         import numpy as np
         import matplotlib.pyplot as plt
         from astropy import units as u
```

### Comparing `synphot-1.3.post0/synphot/config.py` & `synphot-1.4.0/synphot/config.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/exceptions.py` & `synphot-1.4.0/synphot/exceptions.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/filter_parameterization/filter_fft.py` & `synphot-1.4.0/synphot/filter_parameterization/filter_fft.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/filter_parameterization/tests/data/fft_test_data.fits` & `synphot-1.4.0/synphot/filter_parameterization/tests/data/fft_test_data.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/filter_parameterization/tests/test_filter_fft.py` & `synphot-1.4.0/synphot/filter_parameterization/tests/test_filter_fft.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/include/synphot_utils.h` & `synphot-1.4.0/synphot/include/synphot_utils.h`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/models.py` & `synphot-1.4.0/synphot/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,14 @@
                                      Tabular1D)
 from astropy.stats.funcs import gaussian_fwhm_to_sigma, gaussian_sigma_to_fwhm
 from astropy.utils import metadata
 from astropy.utils.exceptions import AstropyUserWarning
 
 # LOCAL
 from synphot import units
-from synphot.compat import ASTROPY_LT_5_0
 from synphot.exceptions import SynphotError
 from synphot.utils import merge_wavelengths
 
 __all__ = ['BlackBody1D', 'BlackBodyNorm1D', 'Box1D', 'ConstFlux1D',
            'Empirical1D', 'Gaussian1D', 'GaussianAbsorption1D',
            'GaussianFlux1D', 'Lorentz1D', 'MexicanHat1D', 'RickerWavelet1D',
            'PowerLawFlux1D', 'Trapezoid1D', 'get_waveset', 'get_metadata']
@@ -224,18 +223,15 @@
             Only return the minimal points needed to define the box;
             i.e., box edges and a point outside on each side.
 
         """
         if step is None:
             step = self.step
 
-        if ASTROPY_LT_5_0:
-            w1, w2 = self.bounding_box
-        else:
-            w1, w2 = tuple(self.bounding_box.bounding_box())
+        w1, w2 = tuple(self.bounding_box.bounding_box())
 
         if self._n_models == 1:
             w = self._calc_sampleset(w1, w2, step, minimal)
         else:
             w = list(map(partial(
                 self._calc_sampleset, step=step, minimal=minimal), w1, w2))
 
@@ -759,18 +755,15 @@
 class Trapezoid1D(_models.Trapezoid1D):
     """Same as `astropy.modeling.functional_models.Trapezoid1D`, except with
     ``sampleset`` defined.
 
     """
     def sampleset(self):
         """Return ``x`` array that samples the feature."""
-        if ASTROPY_LT_5_0:
-            x1, x4 = self.bounding_box
-        else:
-            x1, x4 = tuple(self.bounding_box.bounding_box())
+        x1, x4 = tuple(self.bounding_box.bounding_box())
         dw = self.width * 0.5
         x2 = self.x_0 - dw
         x3 = self.x_0 + dw
 
         if self._n_models == 1:
             w = [x1, x2, x3, x4]
         else:
```

### Comparing `synphot-1.3.post0/synphot/observation.py` & `synphot-1.4.0/synphot/observation.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/reddening.py` & `synphot-1.4.0/synphot/reddening.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 # STDLIB
 import numbers
 
 # THIRD-PARTY
 import numpy as np
 from astropy import units as u
+from astropy.io.fits.connect import is_fits
 
 # LOCAL
 from synphot import exceptions, specio, units
 from synphot.compat import HAS_DUST_EXTINCTION
 from synphot.config import Conf
 from synphot.models import Empirical1D
 from synphot.spectrum import BaseUnitlessSpectrum
@@ -133,16 +134,16 @@
 
         specio.write_fits_spec(filename, w, y, **kwargs)
 
     @classmethod
     def from_file(cls, filename, **kwargs):
         """Create a reddening law from file.
 
-        If filename has 'fits' or 'fit' suffix, it is read as FITS.
-        Otherwise, it is read as ASCII.
+        If filename is recognized by ``astropy.io.fits`` as FITS,
+        it is read as such. Otherwise, it is read as ASCII.
 
         Parameters
         ----------
         filename : str
             Reddening law filename.
 
         kwargs : dict
@@ -152,21 +153,20 @@
 
         Returns
         -------
         redlaw : `ReddeningLaw`
             Empirical reddening law.
 
         """
-        if 'flux_unit' not in kwargs:
+        if is_fits("", filename, None):
+            if 'flux_col' not in kwargs:
+                kwargs['flux_col'] = 'Av/E(B-V)'
+        elif 'flux_unit' not in kwargs:  # pragma: no cover
             kwargs['flux_unit'] = cls._internal_flux_unit
 
-        if ((filename.endswith('fits') or filename.endswith('fit')) and
-                'flux_col' not in kwargs):
-            kwargs['flux_col'] = 'Av/E(B-V)'
-
         header, wavelengths, rvs = specio.read_spec(filename, **kwargs)
 
         return cls(Empirical1D, points=wavelengths, lookup_table=rvs,
                    meta={'header': header})
 
     @classmethod
     def from_extinction_model(cls, modelname, **kwargs):
@@ -213,21 +213,20 @@
             cfgitem = Conf.xgal_file
         else:
             raise exceptions.SynphotError(
                 'Extinction model {0} is invalid.'.format(modelname))
 
         filename = cfgitem()
 
-        if 'flux_unit' not in kwargs:
+        if is_fits("", filename, None):
+            if 'flux_col' not in kwargs:
+                kwargs['flux_col'] = 'Av/E(B-V)'
+        elif 'flux_unit' not in kwargs:  # pragma: no cover
             kwargs['flux_unit'] = cls._internal_flux_unit
 
-        if ((filename.endswith('fits') or filename.endswith('fit')) and
-                'flux_col' not in kwargs):
-            kwargs['flux_col'] = 'Av/E(B-V)'
-
         header, wavelengths, rvs = specio.read_remote_spec(filename, **kwargs)
         header['filename'] = filename
         header['descrip'] = cfgitem.description
         meta = {'header': header, 'expr': modelname}
 
         return cls(Empirical1D, points=wavelengths, lookup_table=rvs,
                    meta=meta)
```

### Comparing `synphot-1.3.post0/synphot/specio.py` & `synphot-1.4.0/synphot/specio.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 # THIRD-PARTY
 import numpy as np
 
 # ASTROPY
 from astropy import log
 from astropy import units as u
 from astropy.io import ascii, fits
+from astropy.io.fits.connect import is_fits
+from astropy.table import QTable
 from astropy.utils.data import get_readable_fileobj
+from astropy.utils.decorators import deprecated_renamed_argument
 from astropy.utils.exceptions import AstropyUserWarning
 
 # LOCAL
 from synphot import __version__, exceptions, units
 
 __all__ = ['read_remote_spec', 'read_spec', 'read_ascii_spec',
            'read_fits_spec', 'write_fits_spec']
@@ -84,15 +87,15 @@
 
     """
     if isinstance(filename, str):
         fname = filename
     elif not fname:  # pragma: no cover
         raise exceptions.SynphotError('Cannot determine filename.')
 
-    if fname.endswith('fits') or fname.endswith('fit'):
+    if is_fits("", fname, None):
         read_func = read_fits_spec
     else:
         read_func = read_ascii_spec
 
     return read_func(filename, **kwargs)
 
 
@@ -139,20 +142,23 @@
 
     wavelengths = dat.columns[0].data.astype(np.float64) * wave_unit
     fluxes = dat.columns[1].data.astype(np.float64) * flux_unit
 
     return header, wavelengths, fluxes
 
 
+@deprecated_renamed_argument(
+    ["wave_unit", "flux_unit"], [None, None], ["1.4", "1.4"],
+    alternative='TUNITn as per FITS standards')
 def read_fits_spec(filename, ext=1, wave_col='WAVELENGTH', flux_col='FLUX',
                    wave_unit=u.AA, flux_unit=units.FLAM):
     """Read FITS spectrum.
 
-    Wavelength and flux units are extracted from ``TUNIT1`` and ``TUNIT2``
-    keywords, respectively, from data table (not primary) header.
+    Wavelength and flux units are extracted from respective ``TUNITn``
+    keywords, from data table (not primary) header.
     If these keywords are not present, units are taken from
     ``wave_unit`` and ``flux_unit`` instead.
 
     Parameters
     ----------
     filename : str or file pointer
         Spectrum file name or pointer.
@@ -160,58 +166,65 @@
     ext: int
         FITS extension with table data. Default is 1.
 
     wave_col, flux_col : str
         Wavelength and flux column names (case-insensitive).
 
     wave_unit, flux_unit : str or `~astropy.units.Unit`
-        Wavelength and flux units, which default to Angstrom and FLAM,
-        respectively. These are *only* used if ``TUNIT1`` and ``TUNIT2``
-        keywords are not present in table (not primary) header.
+        Wavelength and flux units. These are *no longer used*.
+        Define your units in the respective ``TUNITn``
+        keywords in table (not primary) header.
+
+        .. deprecated:: 1.4
 
     Returns
     -------
     header : dict
         Primary header only. Extension header is discarded.
 
     wavelengths, fluxes : `~astropy.units.quantity.Quantity`
         Wavelength and flux of the spectrum.
 
     """
+    wave_col = wave_col.lower()
+    flux_col = flux_col.lower()
+
     try:
         fs = fits.open(filename)
-        header = dict(fs[str('PRIMARY')].header)
-        wave_dat = fs[ext].data.field(wave_col).copy()
-        flux_dat = fs[ext].data.field(flux_col).copy()
-        fits_wave_unit = fs[ext].header.get('TUNIT1')
-        fits_flux_unit = fs[ext].header.get('TUNIT2')
-
-        if fits_wave_unit is not None:
-            try:
-                wave_unit = units.validate_unit(fits_wave_unit)
-            except (exceptions.SynphotError, ValueError) as e:  # pragma: no cover  # noqa: E501
-                warnings.warn(
-                    '{0} from FITS header is not valid wavelength unit, using '
-                    '{1}: {2}'.format(fits_wave_unit, wave_unit, e),
-                    AstropyUserWarning)
-
-        if fits_flux_unit is not None:
-            try:
-                flux_unit = units.validate_unit(fits_flux_unit)
-            except (exceptions.SynphotError, ValueError) as e:  # pragma: no cover  # noqa: E501
-                warnings.warn(
-                    '{0} from FITS header is not valid flux unit, using '
-                    '{1}: {2}'.format(fits_flux_unit, flux_unit, e),
-                    AstropyUserWarning)
+        subhdu = fs[ext]
 
-        wave_unit = units.validate_unit(wave_unit)
-        flux_unit = units.validate_unit(flux_unit)
+        # Need to fix table units
+        for key in subhdu.header["TUNIT*"]:
+            val = subhdu.header[key]
+            if not val:
+                continue
+            newval = units.validate_unit(val)
+            subhdu.header[key] = newval.to_string()  # Must be generic to handle mag  # noqa: E501
+
+        with warnings.catch_warnings():
+            warnings.filterwarnings("ignore", category=u.UnitsWarning,
+                                    message=".* did not parse as fits unit")
+            t = QTable.read(subhdu)
+        header = dict(fs["PRIMARY"].header)
+
+        # https://github.com/astropy/astropy/issues/16221
+        lower_colnames = [c.lower() for c in t.colnames]
+        t_col_wave = t.columns[lower_colnames.index(wave_col)]
+        if t_col_wave.unit:
+            t_col_wave_unit = units.validate_unit(t_col_wave.unit.to_string())
+        else:
+            t_col_wave_unit = u.dimensionless_unscaled
+        t_col_flux = t.columns[lower_colnames.index(flux_col)]
+        if t_col_flux.unit:
+            t_col_flux_unit = units.validate_unit(t_col_flux.unit.to_string())
+        else:
+            t_col_flux_unit = u.dimensionless_unscaled
+        wavelengths = t_col_wave.value * t_col_wave_unit
+        fluxes = t_col_flux.value * t_col_flux_unit
 
-        wavelengths = wave_dat * wave_unit
-        fluxes = flux_dat * flux_unit
     finally:
         if isinstance(filename, str):
             fs.close()
 
     return header, wavelengths, fluxes
```

### Comparing `synphot-1.3.post0/synphot/spectrum.py` & `synphot-1.4.0/synphot/spectrum.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 # THIRD-PARTY
 import numpy as np
 from scipy.integrate import trapezoid
 
 # ASTROPY
 from astropy import log
 from astropy import units as u
+from astropy.io.fits.connect import is_fits
 from astropy.modeling import Model
 from astropy.modeling.core import CompoundModel
 from astropy.modeling.models import RedshiftScaleFactor, Scale
 from astropy.utils.exceptions import AstropyUserWarning
 from astropy.utils import metadata
 
 # LOCAL
@@ -1917,16 +1918,16 @@
 
         specio.write_fits_spec(filename, w, y, **kwargs)
 
     @classmethod
     def from_file(cls, filename, **kwargs):
         """Creates a bandpass from file.
 
-        If filename has 'fits' or 'fit' suffix, it is read as FITS.
-        Otherwise, it is read as ASCII.
+        If filename is recognized by ``astropy.io.fits`` as FITS,
+        it is read as such. Otherwise, it is read as ASCII.
 
         Parameters
         ----------
         filename : str
             Bandpass filename.
 
         kwargs : dict
@@ -1936,21 +1937,20 @@
 
         Returns
         -------
         bp : `SpectralElement`
             Empirical bandpass.
 
         """
-        if 'flux_unit' not in kwargs:
+        if is_fits("", filename, None):
+            if 'flux_col' not in kwargs:
+                kwargs['flux_col'] = 'THROUGHPUT'
+        elif 'flux_unit' not in kwargs:  # pragma: no cover
             kwargs['flux_unit'] = cls._internal_flux_unit
 
-        if ((filename.endswith('fits') or filename.endswith('fit')) and
-                'flux_col' not in kwargs):
-            kwargs['flux_col'] = 'THROUGHPUT'
-
         header, wavelengths, throughput = specio.read_spec(filename, **kwargs)
         return cls(Empirical1D, points=wavelengths, lookup_table=throughput,
                    keep_neg=True, meta={'header': header})
 
     @classmethod
     def from_filter(cls, filtername, **kwargs):
         """Load :ref:`pre-defined filter bandpass <synphot-predefined-filter>`.
@@ -2005,21 +2005,20 @@
             cfgitem = Conf.johnson_k_file
         else:
             raise exceptions.SynphotError(
                 'Filter name {0} is invalid.'.format(filtername))
 
         filename = cfgitem()
 
-        if 'flux_unit' not in kwargs:
+        if is_fits("", filename, None):
+            if 'flux_col' not in kwargs:
+                kwargs['flux_col'] = 'THROUGHPUT'
+        elif 'flux_unit' not in kwargs:  # pragma: no cover
             kwargs['flux_unit'] = cls._internal_flux_unit
 
-        if ((filename.endswith('fits') or filename.endswith('fit')) and
-                'flux_col' not in kwargs):
-            kwargs['flux_col'] = 'THROUGHPUT'
-
         header, wavelengths, throughput = specio.read_remote_spec(
             filename, **kwargs)
         header['filename'] = filename
         header['descrip'] = cfgitem.description
         meta = {'header': header, 'expr': filtername}
         return cls(Empirical1D, points=wavelengths, lookup_table=throughput,
                    meta=meta)
```

### Comparing `synphot-1.3.post0/synphot/src/synphot_utils.c` & `synphot-1.4.0/synphot/src/synphot_utils.c`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits` & `synphot-1.4.0/synphot/tests/data/cos_fuv_g130m_c1309_psa.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/grw_70d5824_stisnic_005.fits` & `synphot-1.4.0/synphot/tests/data/grw_70d5824_stisnic_005.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f555w.fits` & `synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f555w.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits` & `synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f555w_x_grw70d5824.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/hst_acs_hrc_f850lp.fits` & `synphot-1.4.0/synphot/tests/data/hst_acs_hrc_f850lp.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/k93_4500_0_5_rn_box.fits` & `synphot-1.4.0/synphot/tests/data/k93_4500_0_5_rn_box.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/milkyway_diffuse_001.fits` & `synphot-1.4.0/synphot/tests/data/milkyway_diffuse_001.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/qso_template_001.dat` & `synphot-1.4.0/synphot/tests/data/qso_template_001.dat`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin` & `synphot-1.4.0/synphot/tests/data/stis_fuv_f25ndq2_binset.bin`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits` & `synphot-1.4.0/synphot/tests/data/stis_fuv_f25ndq2_mjd58300_0822774.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/us7.txt` & `synphot-1.4.0/synphot/tests/data/us7.txt`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits` & `synphot-1.4.0/synphot/tests/data/wfc3_ir_g141_src_003_th.fits`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_binning.py` & `synphot-1.4.0/synphot/tests/test_binning.py`

 * *Files 1% similar despite different names*

```diff
@@ -194,15 +194,15 @@
     """
     def setup_class(self):
         # Get bandpass data for interpolation.
         hdr, wave, thru = specio.read_fits_spec(
             get_pkg_data_filename(
                 os.path.join('data', 'hst_acs_hrc_f555w.fits'),
                 package='synphot.tests'),
-            flux_col='THROUGHPUT', flux_unit=u.dimensionless_unscaled)
+            flux_col='THROUGHPUT')
 
         # Binned data.
         bins = generate_wavelengths(
             minwave=6000, maxwave=6010, delta=1.0, log=False)[0]
         edges = binning.calculate_bin_edges(bins)
 
         # Merge bin edges and centers in with the natural waveset.
```

### Comparing `synphot-1.3.post0/synphot/tests/test_blackbody.py` & `synphot-1.4.0/synphot/tests/test_blackbody.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_integrator.py` & `synphot-1.4.0/synphot/tests/test_integrator.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_models.py` & `synphot-1.4.0/synphot/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_observation.py` & `synphot-1.4.0/synphot/tests/test_observation.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_reddening.py` & `synphot-1.4.0/synphot/tests/test_reddening.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """Test reddening.py module."""
 
 # STDLIB
 import os
-import shutil
-import tempfile
 
 # THIRD-PARTY
 import numpy as np
 import pytest
 
 # ASTROPY
 from astropy import units as u
@@ -152,36 +150,30 @@
 
 
 def test_redlaw_from_model_exception():
     with pytest.raises(exceptions.SynphotError):
         ReddeningLaw.from_extinction_model('foo')
 
 
-class TestWriteReddeningLaw:
+@pytest.mark.parametrize('ext_hdr', [None, {'foo': 'foo'}])
+def test_write_reddening_law(tmp_path, ext_hdr):
     """Test ReddeningLaw ``to_fits()`` method."""
-    def setup_class(self):
-        self.outdir = tempfile.mkdtemp()
-        self.x = np.linspace(1000, 5000, 5)
-        self.y = np.linspace(1, 5, 5) * 0.1
-        self.redlaw = ReddeningLaw(
-            Empirical1D, points=self.x, lookup_table=self.y)
-
-    @pytest.mark.parametrize('ext_hdr', [None, {'foo': 'foo'}])
-    def test_write(self, ext_hdr):
-        outfile = os.path.join(self.outdir, 'outredlaw.fits')
-
-        if ext_hdr is None:
-            self.redlaw.to_fits(outfile, overwrite=True)
-        else:
-            self.redlaw.to_fits(outfile, overwrite=True, ext_header=ext_hdr)
-
-        # Read it back in and check
-        redlaw2 = ReddeningLaw.from_file(outfile)
-        np.testing.assert_allclose(redlaw2.waveset.value, self.x)
-        np.testing.assert_allclose(redlaw2(self.x).value, self.y)
-
-        if ext_hdr is not None:
-            hdr = fits.getheader(outfile, 1)
-            assert 'foo' in hdr
-
-    def teardown_class(self):
-        shutil.rmtree(self.outdir)
+    x = np.linspace(1000, 5000, 5)
+    y = np.linspace(1, 5, 5) * 0.1
+    redlaw = ReddeningLaw(
+        Empirical1D, points=x, lookup_table=y, meta={"expr": "ebv(test)"})
+
+    outfile = str(tmp_path / 'outredlaw.fits')
+
+    if ext_hdr is None:
+        redlaw.to_fits(outfile, overwrite=True)
+    else:
+        redlaw.to_fits(outfile, overwrite=True, ext_header=ext_hdr)
+
+    # Read it back in and check
+    redlaw2 = ReddeningLaw.from_file(outfile)
+    np.testing.assert_allclose(redlaw2.waveset.value, x)
+    np.testing.assert_allclose(redlaw2(x).value, y)
+
+    if ext_hdr is not None:
+        hdr = fits.getheader(outfile, 1)
+        assert 'foo' in hdr
```

### Comparing `synphot-1.3.post0/synphot/tests/test_specio.py` & `synphot-1.4.0/synphot/tests/test_specio.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """Test specio.py module."""
 
 # STDLIB
 import os
-import shutil
-import tempfile
 
 # THIRD-PARTY
 import numpy as np
 import pytest
 
 # ASTROPY
 from astropy import units as u
 from astropy.io import fits
 from astropy.tests.helper import assert_quantity_allclose
 from astropy.utils.data import get_pkg_data_filename
-from astropy.utils.exceptions import AstropyUserWarning
+from astropy.utils.exceptions import (
+    AstropyUserWarning, AstropyDeprecationWarning)
 
 # LOCAL
 from synphot import exceptions, specio, units
+from synphot.spectrum import SpectralElement
 
 
 @pytest.mark.remote_data
 def test_read_remote_spec():
     """Test read remote spectrum.
 
     .. note:: This is just I/O test. No check on data quality.
@@ -51,36 +51,36 @@
     assert hdr == {}
 
 
 class TestReadWriteFITS:
     """Test read/write FITS spectrum."""
     def setup_class(self):
         self.epsilon = 0.00031
-        self.outdir = tempfile.mkdtemp()
         self.wave = np.array([1000.0, 2000.0, 2000.0 + self.epsilon, 3000.0,
                               4000.0, 5000.0], dtype=np.float64) * u.AA
         self.flux = np.array([0.1, 100.2, 10.0, 0.0, 6.5, 1.2],
                              dtype=np.float64) * units.PHOTLAM
         self.prihdr = {'PEDIGREE': 'DUMMY'}
         self.scihdr = {'SPEC_SRC': 'RANDOM'}
 
-    def test_array_data(self):
+    def test_array_data(self, tmp_path):
         """Data as Numpy array."""
-        outfile = os.path.join(self.outdir, 'outspec1.fits')
+        outfile = str(tmp_path / 'outspec1.fits')
 
         # Write it out
         with pytest.warns(AstropyUserWarning, match=r'rows are thrown out'):
             specio.write_fits_spec(
                 outfile, self.wave.value, self.flux.value,
                 pri_header=self.prihdr, ext_header=self.scihdr,
                 trim_zero=False, pad_zero_ends=False, precision='single',
                 wave_unit=self.wave.unit, flux_unit=self.flux.unit)
 
         # Read it back in and check values (flux_unit should be ignored)
-        hdr, wave, flux = specio.read_spec(outfile, flux_unit='foo')
+        with pytest.warns(AstropyDeprecationWarning, match=r"\"flux_unit\" was deprecated"):  # noqa: E501
+            hdr, wave, flux = specio.read_spec(outfile, flux_unit='foo')
 
         # Compare data
         np.testing.assert_allclose(
             wave.value,
             [1000.0, 2000.0 + self.epsilon, 3000.0, 4000.0, 5000.0],
             rtol=1e-06)
         np.testing.assert_allclose(flux.value, [0.1, 10.0, 0.0, 6.5, 1.2])
@@ -91,25 +91,26 @@
         assert hdr['PEDIGREE'] == 'DUMMY'
 
         # Compare science header
         sci_hdr = fits.getheader(outfile, 1)
         assert sci_hdr['SPEC_SRC'] == 'RANDOM'
         assert sci_hdr['TFORM2'].lower() == 'e'
 
-    def test_quantity_data(self):
+    def test_quantity_data(self, tmp_path):
         """Data as Quantity."""
-        outfile = os.path.join(self.outdir, 'outspec2.fits')
+        outfile = str(tmp_path / 'outspec2.fits')
 
         # Write it out (flux_unit should be ignored)
         specio.write_fits_spec(
             outfile, self.wave, self.flux, pri_header=self.prihdr,
             ext_header=self.scihdr, precision='double', flux_unit='foo')
 
         # Read it back in and check values (flux_unit should be ignored)
-        hdr, wave, flux = specio.read_spec(outfile, flux_unit='foo')
+        with pytest.warns(AstropyDeprecationWarning, match=r"\"flux_unit\" was deprecated"):  # noqa: E501
+            hdr, wave, flux = specio.read_spec(outfile, flux_unit='foo')
 
         # Compare data (trim_zero=True, pad_zero_ends=True)
         np.testing.assert_allclose(
             wave.value, [500.0, 1000.0, 2000.0, 2000.0 + self.epsilon, 4000.0,
                          5000.0, 6250.0],
             rtol=1e-06)
         np.testing.assert_allclose(
@@ -121,17 +122,17 @@
         assert hdr['PEDIGREE'] == 'DUMMY'
 
         # Compare science header
         sci_hdr = fits.getheader(outfile, 1)
         assert sci_hdr['SPEC_SRC'] == 'RANDOM'
         assert sci_hdr['TFORM2'].lower() == 'd'
 
-    def test_exceptions(self):
+    def test_exceptions(self, tmp_path):
         """Test for appropriate exceptions."""
-        outfile = os.path.join(self.outdir, 'outspec3.fits')
+        outfile = str(tmp_path / 'outspec3.fits')
 
         # Shape mismatch
         with pytest.raises(exceptions.SynphotError):
             specio.write_fits_spec(
                 outfile, self.wave, np.arange(3, dtype=np.float64))
 
         # Invalid precision keyword
@@ -145,9 +146,65 @@
                 outfile, np.arange(6), self.flux, overwrite=True)
 
         # Invalid flux precision
         with pytest.raises(exceptions.SynphotError):
             specio.write_fits_spec(
                 outfile, self.wave, np.arange(6), overwrite=True)
 
-    def teardown_class(self):
-        shutil.rmtree(self.outdir)
+
+def test_read_nonstandard_fits_cols_01(tmp_path):
+    """See https://github.com/spacetelescope/synphot_refactor/issues/372"""
+    pix = np.arange(5, dtype=int) + 1
+    wav = (pix * 0.1) * u.micron
+    trace = np.array([0, 0.5, 1, 0.9, 0])
+    coldefs = fits.ColDefs([
+        fits.Column(name="X", format="I", array=pix),
+        fits.Column(name="Wavelength", format="E",
+                    unit=wav.unit.to_string(format="fits"), array=wav.value),
+        fits.Column(name="Trace", format="E", array=trace)])
+    hdulist = fits.HDUList([
+        fits.PrimaryHDU(),
+        fits.BinTableHDU.from_columns(coldefs)])
+    outfile = str(tmp_path / "jwst_niriss_soss_trace.fits")
+    hdulist.writeto(outfile, overwrite=True)
+
+    # Make sure column names are still case insensitive.
+    for (wave_col, flux_col) in (
+            ("Wavelength", "Trace"),
+            ("WAVELENGTH", "TRACE"),
+            ("wavelength", "trace")):
+        tr = SpectralElement.from_file(
+            outfile, wave_col=wave_col, flux_col=flux_col)
+        assert_quantity_allclose(tr.waveset, wav)
+        assert_quantity_allclose(tr(wav), trace, atol=1e-7)
+
+
+def test_read_nonstandard_fits_cols_02(tmp_path):
+    """See https://github.com/spacetelescope/synphot_refactor/issues/372"""
+
+    wav = (np.arange(5) + 1) * u.nm
+    flux_unit_str = "ph/s/m2/micron/arcsec2"  # Invalid but should not matter.
+    flux = np.ones(5)
+    thru = np.array([0, 0.5, 1, 0.9, 0])
+    coldefs = fits.ColDefs([
+        fits.Column(name="lam", format="E",
+                    unit=wav.unit.to_string(format="fits"), array=wav.value),
+        fits.Column(name="flux", format="E",
+                    unit=flux_unit_str, array=flux),
+        fits.Column(name="dflux1", format="E",
+                    unit=flux_unit_str, array=flux),
+        fits.Column(name="dflux2", format="E",
+                    unit=flux_unit_str, array=flux),
+        fits.Column(name="trans", format="E", unit="1", array=thru)])
+    hdulist = fits.HDUList([
+        fits.PrimaryHDU(),
+        fits.BinTableHDU.from_columns(coldefs)])
+    outfile = str(tmp_path / "skytable.fits")
+    hdulist.writeto(outfile, overwrite=True)
+
+    with pytest.warns(u.UnitsWarning, match="'ph/s/m2/micron/arcsec2'"):  # noqa: E501
+        header, wavelengths, transmission = specio.read_spec(
+            outfile, wave_col="lam", flux_col="trans")
+
+    assert header["SIMPLE"]
+    assert_quantity_allclose(wavelengths, wav)
+    assert_quantity_allclose(transmission, thru)
```

### Comparing `synphot-1.3.post0/synphot/tests/test_spectrum_bandpass.py` & `synphot-1.4.0/synphot/tests/test_spectrum_bandpass.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_spectrum_misc.py` & `synphot-1.4.0/synphot/tests/test_spectrum_misc.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,11 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """Test spectrum.py module and related functionalities that are not covered
 by ``test_spectrum_source.py`` nor ``test_spectrum_bandpass.py``."""
 
-# STDLIB
-import os
-import shutil
-import tempfile
-
 # THIRD-PARTY
 import numpy as np
 import pytest
 
 # ASTROPY
 from astropy import units as u
 from astropy.io import fits
@@ -386,30 +381,29 @@
         with pytest.raises(exceptions.IncompatibleSources):
             self.bp_1 * (1 - 1j)
 
 
 class TestWriteSpec:
     """Test spectrum to_fits() method."""
     def setup_class(self):
-        self.outdir = tempfile.mkdtemp()
         self.sp = SourceSpectrum(
             Empirical1D, points=_wave, lookup_table=_flux_photlam,
             meta={'expr': 'Test source'})
         self.bp = SpectralElement(
             Empirical1D, points=_wave, lookup_table=np.ones(_wave.shape),
             meta={'expr': 'Test bandpass'})
 
     @pytest.mark.parametrize(
         ('is_sp', 'ext_hdr'),
         [(True, None),
          (True, {'foo': 'foo'}),
          (False, None),
          (False, {'foo': 'foo'})])
-    def test_write(self, is_sp, ext_hdr):
-        outfile = os.path.join(self.outdir, 'outspec.fits')
+    def test_write(self, tmp_path, is_sp, ext_hdr):
+        outfile = str(tmp_path / 'outspec.fits')
 
         if is_sp:
             sp1 = self.sp
         else:
             sp1 = self.bp
 
         if ext_hdr is None:
@@ -422,10 +416,7 @@
         # Read it back in and check
         sp2 = sp1.__class__.from_file(outfile)
         np.testing.assert_allclose(sp2(sp2.waveset), sp1(sp1.waveset))
         hdr = fits.getheader(outfile, 1)
         assert 'expr' in hdr
         if ext_hdr is not None:
             assert 'foo' in hdr
-
-    def teardown_class(self):
-        shutil.rmtree(self.outdir)
```

### Comparing `synphot-1.3.post0/synphot/tests/test_spectrum_source.py` & `synphot-1.4.0/synphot/tests/test_spectrum_source.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_thermal.py` & `synphot-1.4.0/synphot/tests/test_thermal.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_units.py` & `synphot-1.4.0/synphot/tests/test_units.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot/tests/test_utils.py` & `synphot-1.4.0/synphot/tests/test_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -112,33 +112,33 @@
         assert np.all(dw > self.thres)
 
     def test_merge_same(self):
         wave = utils.merge_wavelengths(self.wave, self.wave)
         np.testing.assert_array_equal(wave, self.wave)
 
 
-def test_download_bad_root(tmpdir):
+def test_download_bad_root(tmp_path):
     """Test data download helper when input dir is invalid."""
-    ptr = tmpdir.join('bad_cdbs')
-    ptr.write('content')
+    ptr = tmp_path / 'bad_cdbs'
+    ptr.write_text("something")
     cdbs_root = str(ptr)
 
-    with pytest.raises(OSError):
+    with pytest.raises(OSError, match=".* must be a directory"):
         utils.download_data(cdbs_root, verbose=False)
 
     with pytest.raises(FileNotFoundError):
         utils.download_data('', verbose=False)
 
 
-def test_download_data(tmpdir):
+def test_download_data(tmp_path):
     """Test data download helper in dry run mode."""
     from synphot.config import conf
 
     # Use case where user downloads all data into new dir.
-    cdbs_root = os.path.join(tmpdir.strpath, 'cdbs')
+    cdbs_root = str(tmp_path / 'cdbs')
     file_list_1 = utils.download_data(cdbs_root, verbose=False, dry_run=True)
     filename = file_list_1[0]
     assert len(file_list_1) == 21
     assert filename.startswith(cdbs_root)
     assert os.path.isdir(os.path.join(cdbs_root, 'calspec'))
 
     # Make dummy files for the next step.
```

### Comparing `synphot-1.3.post0/synphot/thermal.py` & `synphot-1.4.0/synphot/thermal.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # Licensed under a 3-clause BSD style license - see LICENSE.rst
 """This module defines thermal spectra."""
 
 # ASTROPY
 from astropy import units as u
 from astropy.io import fits
+from astropy.io.fits.connect import is_fits
 
 # LOCAL
 from synphot import exceptions, specio, units
 from synphot.models import BlackBody1D, Empirical1D
 from synphot.spectrum import BaseUnitlessSpectrum, SourceSpectrum
 
 __all__ = ['ThermalSpectralElement']
@@ -120,31 +121,28 @@
 
         Raises
         ------
         synphot.exceptions.SynphotError
             Invalid inputs.
 
         """
-        if not (filename.endswith('fits') or filename.endswith('fit')):
+        if not is_fits("", filename, None):
             raise exceptions.SynphotError('Only FITS format is supported.')
 
         # Extra info from table header
         ext = kwargs.get('ext', 1)
         tab_hdr = fits.getheader(filename, ext=ext)
 
         temperature = tab_hdr.get(temperature_key)
         if temperature is None:
             raise exceptions.SynphotError(
                 'Missing {0} keyword.'.format(temperature_key))
 
         beam_fill_factor = tab_hdr.get('BEAMFILL', 1)
 
-        if 'flux_unit' not in kwargs:
-            kwargs['flux_unit'] = cls._internal_flux_unit
-
         if 'flux_col' not in kwargs:
             kwargs['flux_col'] = 'EMISSIVITY'
 
         header, wavelengths, em = specio.read_spec(filename, **kwargs)
         return cls(
             Empirical1D, temperature, beam_fill_factor=beam_fill_factor,
             points=wavelengths, lookup_table=em, meta={'header': header})
```

### Comparing `synphot-1.3.post0/synphot/units.py` & `synphot-1.4.0/synphot/units.py`

 * *Files 3% similar despite different names*

```diff
@@ -287,18 +287,30 @@
 
         # Backward-compatibility
         if input_unit_lowcase == 'angstroms':
             output_unit = u.AA
         elif input_unit_lowcase == 'inversemicrons':
             output_unit = u.micron ** -1
         elif input_unit_lowcase in ('transmission', 'extinction',
-                                    'emissivity'):
+                                    'emissivity', 'throughput'):
             output_unit = THROUGHPUT
         elif input_unit_lowcase == 'jy':
             output_unit = u.Jy
+        elif input_unit_lowcase == "flam":
+            output_unit = FLAM
+        elif input_unit_lowcase == "fnu":
+            output_unit = FNU
+        elif input_unit_lowcase == "photlam":
+            output_unit = PHOTLAM
+        elif input_unit_lowcase == "photnu":
+            output_unit = PHOTNU
+        elif input_unit_lowcase == "none":
+            output_unit = u.dimensionless_unscaled
+        elif input_unit_lowcase == "sec":
+            output_unit = u.s
 
         # Work around mag unit limitations
         elif input_unit_lowcase in ('stmag', 'mag(st)'):
             output_unit = u.STmag
         elif input_unit_lowcase in ('abmag', 'mag(ab)'):
             output_unit = u.ABmag
         elif input_unit_lowcase in ('obmag', 'mag(ob)'):
```

### Comparing `synphot-1.3.post0/synphot/utils.py` & `synphot-1.4.0/synphot/utils.py`

 * *Files identical despite different names*

### Comparing `synphot-1.3.post0/synphot.egg-info/PKG-INFO` & `synphot-1.4.0/synphot.egg-info/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,30 +1,30 @@
 Metadata-Version: 2.1
 Name: synphot
-Version: 1.3.post0
+Version: 1.4.0
 Summary: Synthetic photometry
 Home-page: https://www.github.com/spacetelescope/synphot_refactor
 Author: STScI
 Author-email: help@stsci.edu
 License: BSD
 Keywords: astronomy,astrophysics,synthetic,photometry
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Scientific/Engineering :: Astronomy
 Classifier: Topic :: Scientific/Engineering :: Physics
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/plain
 License-File: LICENSE.rst
-Requires-Dist: numpy>=1.20
-Requires-Dist: astropy>=5
-Requires-Dist: scipy>=1.6
+Requires-Dist: numpy>=1.23
+Requires-Dist: astropy>=6
+Requires-Dist: scipy>=1.9
 Provides-Extra: all
 Requires-Dist: specutils>=0.7; extra == "all"
 Requires-Dist: dust-extinction; extra == "all"
 Provides-Extra: test
 Requires-Dist: pytest-astropy; extra == "test"
 Provides-Extra: docs
 Requires-Dist: matplotlib; extra == "docs"
```

### Comparing `synphot-1.3.post0/synphot.egg-info/SOURCES.txt` & `synphot-1.4.0/synphot.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 tox.ini
 .github/PULL_REQUEST_TEMPLATE.md
 .github/dependabot.yml
 .github/labeler.yml
 .github/ISSUE_TEMPLATE/bug_report.md
 .github/ISSUE_TEMPLATE/feature_request.md
 .github/ISSUE_TEMPLATE/question.md
+.github/workflows/check_milestone.yml
 .github/workflows/ci_workflows.yml
 .github/workflows/codeql-analysis.yml
 .github/workflows/open_actions.yml
 .github/workflows/predeps_workflow.yml
 .github/workflows/publish-to-pypi.yml
 docs/Makefile
 docs/conf.py
```

### Comparing `synphot-1.3.post0/tox.ini` & `synphot-1.4.0/tox.ini`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tox]
 envlist =
-    py{39,310,311,312}-test{,-alldeps,-oldestdeps,-devdeps,-predeps}{,-cov}
+    py{310,311,312}-test{,-alldeps,-oldestdeps,-devdeps,-predeps}{,-cov}
     codestyle
     twine
     bandit
     linkcheck
 
 [testenv]
 setenv =
@@ -32,17 +32,17 @@
     oldestdeps: with the oldest supported version of key dependencies
     cov: and test coverage
 
 deps =
 
     # The oldestdeps factor is intended to be used to install the oldest versions of all
     # dependencies that have a minimum version.
-    oldestdeps: numpy==1.20.*
-    oldestdeps: scipy==1.6.*
-    oldestdeps: astropy==5.0.*
+    oldestdeps: numpy==1.23.*
+    oldestdeps: scipy==1.9.*
+    oldestdeps: astropy==6.0.*
 
     # The devdeps factor is intended to be used to install the latest developer version
     # or nightly wheel of key dependencies.
     devdeps: numpy>=0.0.dev0
     devdeps: scipy>=0.0.dev0
     devdeps: pyerfa>=0.0.dev0
     devdeps: astropy>=0.0.dev0
```

