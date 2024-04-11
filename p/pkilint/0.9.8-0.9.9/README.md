# Comparing `tmp/pkilint-0.9.8.tar.gz` & `tmp/pkilint-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pkilint-0.9.8.tar", last modified: Tue Nov 21 14:43:14 2023, max compression
+gzip compressed data, was "pkilint-0.9.9.tar", last modified: Mon Dec 18 14:00:04 2023, max compression
```

## Comparing `pkilint-0.9.8.tar` & `pkilint-0.9.9.tar`

### file list

```diff
@@ -1,134 +1,134 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-11-21 14:43:08.000000 pkilint-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24241 2023-11-21 14:43:14.311923 pkilint-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23015 2023-11-21 14:43:08.000000 pkilint-0.9.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-11-21 14:43:08.000000 pkilint-0.9.8/VERSION.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.295922 pkilint-0.9.8/pkilint/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.299922 pkilint-0.9.8/pkilint/adobe/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/adobe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      783 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/adobe/adobe_validator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.299922 pkilint-0.9.8/pkilint/adobe/asn1/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/adobe/asn1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.299922 pkilint-0.9.8/pkilint/bin/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      587 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/convert_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_crl.py
--rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_pkix_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.299922 pkilint-0.9.8/pkilint/cabf/
--rw-r--r--   0 runner    (1001) docker     (127)      542 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.299922 pkilint-0.9.8/pkilint/cabf/asn1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/asn1/ev_guidelines.py
--rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)      701 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_crl.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    14151 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/cabf_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/cabf/serverauth/
--rw-r--r--   0 runner    (1001) docker     (127)    16501 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14477 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     3786 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_cross_ca.py
--rw-r--r--   0 runner    (1001) docker     (127)     8691 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_finding_filter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    20337 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4136 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_ocsp.py
--rw-r--r--   0 runner    (1001) docker     (127)     5358 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_root.py
--rw-r--r--   0 runner    (1001) docker     (127)    27763 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_subscriber.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/cabf/smime/
--rw-r--r--   0 runner    (1001) docker     (127)     9623 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/smime/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/smime/smime_constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    24625 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/smime/smime_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/smime/smime_key.py
--rw-r--r--   0 runner    (1001) docker     (127)    19429 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/cabf/smime/smime_name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/common/
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13903 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/document.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/etsi/
--rw-r--r--   0 runner    (1001) docker     (127)      605 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/etsi/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/etsi/asn1/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/etsi/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/etsi/asn1/en_319_412_5.py
--rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/etsi/asn1/ts_119_495.py
--rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/finding_filter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.303923 pkilint-0.9.8/pkilint/iso/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/iso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/iso/lei.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/itu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/itu/bitstring.py
--rw-r--r--   0 runner    (1001) docker     (127)      899 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/itu/string.py
--rw-r--r--   0 runner    (1001) docker     (127)     3930 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/itu/x520_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/msft/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/msft/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/msft/asn1/
--rw-r--r--   0 runner    (1001) docker     (127)      243 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/msft/asn1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      740 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/msft/msft_name.py
--rw-r--r--   0 runner    (1001) docker     (127)      180 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/oid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/pkix/
--rw-r--r--   0 runner    (1001) docker     (127)     2744 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/algorithm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/pkix/certificate/
--rw-r--r--   0 runner    (1001) docker     (127)    14631 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27443 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     7751 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_transparency.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      592 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/certificate/certificate_validity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.307923 pkilint-0.9.8/pkilint/pkix/crl/
--rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/crl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3853 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/crl/crl_extension.py
--rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/crl/crl_validator.py
--rw-r--r--   0 runner    (1001) docker     (127)      578 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/crl/crl_validity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8611 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/extension.py
--rw-r--r--   0 runner    (1001) docker     (127)    10144 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/general_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     7481 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/name.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/pkilint/pkix/ocsp/
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/ocsp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_basic_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_response.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_validity.py
--rw-r--r--   0 runner    (1001) docker     (127)     8757 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/pkix/time.py
--rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/report.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/pkilint/rest/
--rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/rest/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/rest/cabf_serverauth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/rest/cabf_smime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/rest/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2540 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/util.py
--rw-r--r--   0 runner    (1001) docker     (127)    11289 2023-11-21 14:43:08.000000 pkilint-0.9.8/pkilint/validation.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/pkilint.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24241 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      382 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      141 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-21 14:43:14.000000 pkilint-0.9.8/pkilint.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-11-21 14:43:14.315923 pkilint-0.9.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-11-21 14:43:08.000000 pkilint-0.9.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/tests/integration_certificate/
--rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/integration_certificate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/integration_certificate/test_cabf_serverauth_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/integration_certificate/test_cabf_smime_cert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/integration_certificate/test_pkix_cert.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:14.311923 pkilint-0.9.8/tests/itu/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/itu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/itu/test_bitstring.py
--rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/itu/test_string.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/test_cli_smoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (127)    14584 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/test_server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/test_validation_report.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-11-21 14:43:08.000000 pkilint-0.9.8/tests/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.277481 pkilint-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1076 2023-12-18 13:59:57.000000 pkilint-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24241 2023-12-18 14:00:04.277481 pkilint-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23015 2023-12-18 13:59:57.000000 pkilint-0.9.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-12-18 13:59:57.000000 pkilint-0.9.9/VERSION.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.261481 pkilint-0.9.9/pkilint/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.261481 pkilint-0.9.9/pkilint/adobe/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/adobe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/adobe/adobe_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.261481 pkilint-0.9.9/pkilint/adobe/asn1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/adobe/asn1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.261481 pkilint-0.9.9/pkilint/bin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      587 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/convert_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4215 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6399 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2926 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_crl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1528 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_pkix_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4308 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/bin/lint_pkix_signer_signee_cert_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.265481 pkilint-0.9.9/pkilint/cabf/
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.265481 pkilint-0.9.9/pkilint/cabf/asn1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4103 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/asn1/ev_guidelines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2793 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_crl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4849 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14151 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/cabf_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.265481 pkilint-0.9.9/pkilint/cabf/serverauth/
+-rw-r--r--   0 runner    (1001) docker     (127)    16501 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14477 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3786 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3838 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_cross_ca.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8691 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_finding_filter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20337 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4136 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_ocsp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5358 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_root.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27763 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_subscriber.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/cabf/smime/
+-rw-r--r--   0 runner    (1001) docker     (127)     9547 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/smime/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/smime/smime_constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24625 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/smime/smime_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3923 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/smime/smime_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19429 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/cabf/smime/smime_name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/common/
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13903 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/document.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/etsi/
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/etsi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/etsi/asn1/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/etsi/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2445 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/etsi/asn1/en_319_412_5.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1779 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/etsi/asn1/ts_119_495.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2220 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/finding_filter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/iso/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/iso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2074 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/iso/lei.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/itu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1351 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/itu/bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)      899 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/itu/string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3930 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/itu/x520_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4831 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/msft/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/msft/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/msft/asn1/
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/msft/asn1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      740 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/msft/msft_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/oid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.269481 pkilint-0.9.9/pkilint/pkix/
+-rw-r--r--   0 runner    (1001) docker     (127)     2744 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2021 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/algorithm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.273481 pkilint-0.9.9/pkilint/pkix/certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)    14631 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27443 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9440 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3986 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_transparency.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/certificate/certificate_validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.273481 pkilint-0.9.9/pkilint/pkix/crl/
+-rw-r--r--   0 runner    (1001) docker     (127)     4353 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/crl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3853 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/crl/crl_extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1479 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/crl/crl_validator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      578 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/crl/crl_validity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8611 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/extension.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10144 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/general_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7481 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/name.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.273481 pkilint-0.9.9/pkilint/pkix/ocsp/
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/ocsp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_basic_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2639 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_validity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8840 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/pkix/time.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5667 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/report.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.273481 pkilint-0.9.9/pkilint/rest/
+-rw-r--r--   0 runner    (1001) docker     (127)     3431 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/rest/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/rest/cabf_serverauth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1746 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/rest/cabf_smime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4997 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/rest/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2592 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11289 2023-12-18 13:59:57.000000 pkilint-0.9.9/pkilint/validation.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.277481 pkilint-0.9.9/pkilint.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24241 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3320 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      382 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-18 14:00:04.000000 pkilint-0.9.9/pkilint.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)     1457 2023-12-18 14:00:04.277481 pkilint-0.9.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-12-18 13:59:57.000000 pkilint-0.9.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.273481 pkilint-0.9.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.277481 pkilint-0.9.9/tests/integration_certificate/
+-rw-r--r--   0 runner    (1001) docker     (127)     2958 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/integration_certificate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/integration_certificate/test_cabf_serverauth_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/integration_certificate/test_cabf_smime_cert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/integration_certificate/test_pkix_cert.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-18 14:00:04.277481 pkilint-0.9.9/tests/itu/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/itu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2061 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/itu/test_bitstring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/itu/test_string.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/test_cli_smoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14584 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/test_server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1476 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/test_validation_report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2023-12-18 13:59:57.000000 pkilint-0.9.9/tests/util.py
```

### Comparing `pkilint-0.9.8/LICENSE` & `pkilint-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/PKG-INFO` & `pkilint-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.9.8
+Version: 0.9.9
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.9.8/README.md` & `pkilint-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/adobe/adobe_validator.py` & `pkilint-0.9.9/pkilint/adobe/adobe_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/adobe/asn1/__init__.py` & `pkilint-0.9.9/pkilint/adobe/asn1/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/convert_cert.py` & `pkilint-0.9.9/pkilint/bin/convert_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_cabf_serverauth_cert.py` & `pkilint-0.9.9/pkilint/bin/lint_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_cabf_smime_cert.py` & `pkilint-0.9.9/pkilint/bin/lint_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_crl.py` & `pkilint-0.9.9/pkilint/bin/lint_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_ocsp_response.py` & `pkilint-0.9.9/pkilint/bin/lint_ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_pkix_cert.py` & `pkilint-0.9.9/pkilint/bin/lint_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/bin/lint_pkix_signer_signee_cert_chain.py` & `pkilint-0.9.9/pkilint/bin/lint_pkix_signer_signee_cert_chain.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/__init__.py` & `pkilint-0.9.9/pkilint/cabf/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/asn1/ev_guidelines.py` & `pkilint-0.9.9/pkilint/cabf/asn1/ev_guidelines.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_ca.py` & `pkilint-0.9.9/pkilint/cabf/cabf_ca.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_constants.py` & `pkilint-0.9.9/pkilint/cabf/cabf_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_crl.py` & `pkilint-0.9.9/pkilint/cabf/cabf_crl.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_extension.py` & `pkilint-0.9.9/pkilint/cabf/cabf_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_key.py` & `pkilint-0.9.9/pkilint/cabf/cabf_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/cabf_name.py` & `pkilint-0.9.9/pkilint/cabf/cabf_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/__init__.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_ca.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_ca.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_constants.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_cross_ca.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_cross_ca.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_extension.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_finding_filter.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_finding_filter.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_key.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_name.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_ocsp.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_ocsp.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_root.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_root.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/serverauth/serverauth_subscriber.py` & `pkilint-0.9.9/pkilint/cabf/serverauth/serverauth_subscriber.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/smime/__init__.py` & `pkilint-0.9.9/pkilint/cabf/smime/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 import operator
 from typing import Mapping, Tuple
 
-from cryptography import x509
 from dateutil.relativedelta import relativedelta
 from pyasn1.type import univ
-from pyasn1.type.univ import ObjectIdentifier
 from pyasn1_alt_modules import rfc8398, rfc5280, rfc4262
 
 import pkilint.adobe.asn1 as adobe_asn1
 import pkilint.cabf.cabf_extension
 import pkilint.cabf.smime.smime_extension
 import pkilint.common
 import pkilint.pkix.certificate
```

### Comparing `pkilint-0.9.8/pkilint/cabf/smime/smime_constants.py` & `pkilint-0.9.9/pkilint/cabf/smime/smime_constants.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/smime/smime_extension.py` & `pkilint-0.9.9/pkilint/cabf/smime/smime_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/smime/smime_key.py` & `pkilint-0.9.9/pkilint/cabf/smime/smime_key.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/cabf/smime/smime_name.py` & `pkilint-0.9.9/pkilint/cabf/smime/smime_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/common/__init__.py` & `pkilint-0.9.9/pkilint/common/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/document.py` & `pkilint-0.9.9/pkilint/document.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/etsi/__init__.py` & `pkilint-0.9.9/pkilint/etsi/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from pkilint.etsi.asn1 import en_319_412_5, ts_119_495
+from pkilint import document
 
 
 ETSI_QC_STATEMENTS_MAPPINGS = {
-    en_319_412_5.id_etsi_qcs_QcCompliance: None,
+    en_319_412_5.id_etsi_qcs_QcCompliance: document.ValueDecoder.VALUE_NODE_ABSENT,
     en_319_412_5.id_etsi_qcs_QcLimitValue: en_319_412_5.QcEuLimitValue(),
     en_319_412_5.id_etsi_qcs_QcRetentionPeriod: en_319_412_5.QcEuRetentionPeriod(),
-    en_319_412_5.id_etsi_qcs_QcSSCD: None,
+    en_319_412_5.id_etsi_qcs_QcSSCD: document.ValueDecoder.VALUE_NODE_ABSENT,
     en_319_412_5.id_etsi_qcs_QcPDS: en_319_412_5.QcEuPDS(),
     en_319_412_5.id_etsi_qcs_QcType: en_319_412_5.QcType(),
     en_319_412_5.id_etsi_qcs_QcCClegislation: en_319_412_5.QcCClegislation(),
     ts_119_495.id_etsi_psd2_qcStatement: ts_119_495.PSD2QcType(),
 }
```

### Comparing `pkilint-0.9.8/pkilint/etsi/asn1/en_319_412_5.py` & `pkilint-0.9.9/pkilint/etsi/asn1/en_319_412_5.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/etsi/asn1/ts_119_495.py` & `pkilint-0.9.9/pkilint/etsi/asn1/ts_119_495.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/finding_filter.py` & `pkilint-0.9.9/pkilint/finding_filter.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/iso/lei.py` & `pkilint-0.9.9/pkilint/iso/lei.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/itu/bitstring.py` & `pkilint-0.9.9/pkilint/itu/bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/itu/string.py` & `pkilint-0.9.9/pkilint/itu/string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/itu/x520_name.py` & `pkilint-0.9.9/pkilint/itu/x520_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/loader.py` & `pkilint-0.9.9/pkilint/loader.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/msft/msft_name.py` & `pkilint-0.9.9/pkilint/msft/msft_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/__init__.py` & `pkilint-0.9.9/pkilint/pkix/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/algorithm.py` & `pkilint-0.9.9/pkilint/pkix/algorithm.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/__init__.py` & `pkilint-0.9.9/pkilint/pkix/certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_extension.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_key.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_key.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import binascii
 
 from cryptography.exceptions import InvalidSignature
+from cryptography.hazmat.primitives import hashes
 from cryptography.hazmat.primitives.asymmetric import padding, rsa, ec
 from pyasn1.codec.der.encoder import encode
 from pyasn1.type import univ
 from pyasn1_alt_modules import rfc5280, rfc3279, rfc5480, rfc8410
 
 from pkilint import validation, util, document
 from pkilint.document import PDUNode
@@ -98,65 +99,100 @@
     def __init__(self, *, decode_func, **kwargs):
         super().__init__(pdu_class=rfc5280.SubjectPublicKeyInfo,
                          decode_func=decode_func,
                          **kwargs
                          )
 
 
-def _calculate_method2_hash(sha1_hash):
-    last_8_octets = bytearray(sha1_hash[12:])
-    last_8_octets[0] = 0x40 | (last_8_octets[0] & 0xF)
-
-    return bytes(last_8_octets)
-
-
 class SubjectKeyIdentifierValidator(validation.Validator):
     VALIDATION_UNKNOWN_METHOD = validation.ValidationFinding(
         validation.ValidationFindingSeverity.NOTICE,
         'pkix.unknown_subject_key_identifier_calculation_method'
     )
 
+    # TODO: consider renaming the finding code after weighing risk of user breakage
     VALIDATION_METHOD_1 = validation.ValidationFinding(
         validation.ValidationFindingSeverity.INFO,
         'pkix.subject_key_identifier_method_1_identified'
     )
 
+    # TODO: consider renaming the finding code after weighing risk of user breakage
     VALIDATION_METHOD_2 = validation.ValidationFinding(
         validation.ValidationFindingSeverity.INFO,
         'pkix.subject_key_identifier_method_2_identified'
     )
 
+    VALIDATION_RFC7093_METHOD_1 = validation.ValidationFinding(
+        validation.ValidationFindingSeverity.INFO,
+        'pkix.subject_key_identifier_rfc7093_method_1_identified'
+    )
+
+    VALIDATION_RFC7093_METHOD_2 = validation.ValidationFinding(
+        validation.ValidationFindingSeverity.INFO,
+        'pkix.subject_key_identifier_rfc7093_method_2_identified'
+    )
+
+    VALIDATION_RFC7093_METHOD_3 = validation.ValidationFinding(
+        validation.ValidationFindingSeverity.INFO,
+        'pkix.subject_key_identifier_rfc7093_method_3_identified'
+    )
+
     def __init__(self):
         super().__init__(
             validations=[
                 self.VALIDATION_UNKNOWN_METHOD,
                 self.VALIDATION_METHOD_1,
                 self.VALIDATION_METHOD_2,
+                self.VALIDATION_RFC7093_METHOD_1,
+                self.VALIDATION_RFC7093_METHOD_2,
+                self.VALIDATION_RFC7093_METHOD_3,
             ],
             pdu_class=rfc5280.SubjectKeyIdentifier
         )
 
+    @staticmethod
+    def _calculate_rfc5280_method2_id(sha1_hash):
+        last_8_octets = bytearray(sha1_hash[12:])
+        last_8_octets[0] = 0x40 | (last_8_octets[0] & 0xF)
+
+        return bytes(last_8_octets)
+
+    _RFC7093_HASH_CLS_TO_FINDINGS = {
+        hashes.SHA256: VALIDATION_RFC7093_METHOD_1,
+        hashes.SHA384: VALIDATION_RFC7093_METHOD_2,
+        hashes.SHA512: VALIDATION_RFC7093_METHOD_3,
+    }
+
+    # TODO: support RFC 7093 method 4
+    @staticmethod
+    def _calculate_rfc7093_method_hash(public_key_octets, hash_cls):
+        h = util.calculate_hash(public_key_octets, hash_cls())
+
+        # leftmost 160 bits (i.e., 20 octets)
+        return h[:20]
+
     def validate(self, node):
         public_key_node = node.document.root.navigate(
             'tbsCertificate.subjectPublicKeyInfo.subjectPublicKey'
         )
 
-        public_key_bytes = public_key_node.pdu.asOctets()
-        public_key_sha1 = util.calculate_sha1_hash(public_key_bytes)
-
-        method2_hash = _calculate_method2_hash(public_key_sha1)
+        public_key_octets = public_key_node.pdu.asOctets()
 
         identifier_octets = bytes(node.pdu)
 
-        if public_key_sha1 == identifier_octets:
+        public_key_sha1 = util.calculate_sha1_hash(public_key_octets)
+
+        if identifier_octets == public_key_sha1:
             finding = self.VALIDATION_METHOD_1
-        elif method2_hash == identifier_octets:
+        elif identifier_octets == SubjectKeyIdentifierValidator._calculate_rfc5280_method2_id(public_key_sha1):
             finding = self.VALIDATION_METHOD_2
         else:
-            finding = self.VALIDATION_UNKNOWN_METHOD
+            finding = next((f for h, f in SubjectKeyIdentifierValidator._RFC7093_HASH_CLS_TO_FINDINGS.items() if
+                           SubjectKeyIdentifierValidator._calculate_rfc7093_method_hash(
+                               public_key_octets, h) == identifier_octets), self.VALIDATION_UNKNOWN_METHOD)
 
         raise validation.ValidationFindingEncountered(finding)
 
 
 def _verify_signature(public_key, message, signature,
                       signature_algorithm):
     try:
```

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_name.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_transparency.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_transparency.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_validator.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/certificate/certificate_validity.py` & `pkilint-0.9.9/pkilint/pkix/certificate/certificate_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/crl/__init__.py` & `pkilint-0.9.9/pkilint/pkix/crl/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/crl/crl_extension.py` & `pkilint-0.9.9/pkilint/pkix/crl/crl_extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/crl/crl_validator.py` & `pkilint-0.9.9/pkilint/pkix/crl/crl_validator.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/crl/crl_validity.py` & `pkilint-0.9.9/pkilint/pkix/crl/crl_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/extension.py` & `pkilint-0.9.9/pkilint/pkix/extension.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/general_name.py` & `pkilint-0.9.9/pkilint/pkix/general_name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/name.py` & `pkilint-0.9.9/pkilint/pkix/name.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/ocsp/__init__.py` & `pkilint-0.9.9/pkilint/pkix/ocsp/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_basic_response.py` & `pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_basic_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_response.py` & `pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_response.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/ocsp/ocsp_validity.py` & `pkilint-0.9.9/pkilint/pkix/ocsp/ocsp_validity.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/pkix/time.py` & `pkilint-0.9.9/pkilint/pkix/time.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,24 +154,26 @@
 
     def validate_date_range(self, start_datetime, end_datetime):
         pass
 
 
 class SaneValidityPeriodValidator(ValidityPeriodDifferenceValidator):
     def __init__(self, *, end_validity_node_retriever, validation, **kwargs):
+        self._invalid_validity_period_validation = validation
+
         super().__init__(
             end_validity_node_retriever=end_validity_node_retriever,
             validations=[validation],
             **kwargs
         )
 
     def validate_date_range(self, start_datetime, end_datetime):
         if start_datetime > end_datetime:
             raise validation.ValidationFindingEncountered(
-                self._validations[0],
+                self._invalid_validity_period_validation,
                 f'Start of validity period "{start_datetime}" is greater than '
                 f'end of validity period "{end_datetime}"'
             )
 
 
 class ValidityPeriodThresholdsValidator(ValidityPeriodDifferenceValidator):
     def __init__(self, *, end_validity_node_retriever, inclusive_second=False,
```

### Comparing `pkilint-0.9.8/pkilint/report.py` & `pkilint-0.9.9/pkilint/report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/rest/__init__.py` & `pkilint-0.9.9/pkilint/rest/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/rest/cabf_serverauth.py` & `pkilint-0.9.9/pkilint/rest/cabf_serverauth.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/rest/cabf_smime.py` & `pkilint-0.9.9/pkilint/rest/cabf_smime.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/rest/model.py` & `pkilint-0.9.9/pkilint/rest/model.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint/util.py` & `pkilint-0.9.9/pkilint/util.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 
 from cryptography.hazmat.primitives import hashes
 
 from pkilint import validation, report
 from pkilint.report import report_wrapper, REPORT_FORMATS
 
 
-def _calculate_hash(octets, hash_algo):
+def calculate_hash(octets: bytes, hash_algo: hashes.HashAlgorithm) -> bytes:
     h = hashes.Hash(hash_algo)
     h.update(octets)
 
     return h.finalize()
 
 
-def calculate_sha1_hash(octets):
-    return _calculate_hash(octets, hashes.SHA1())
+def calculate_sha1_hash(octets: bytes) -> bytes:
+    return calculate_hash(octets, hashes.SHA1())
 
 
 def argparse_enum_type_parser(enum_type):
     def _parse(value):
         value = value.upper()
 
         try:
```

### Comparing `pkilint-0.9.8/pkilint/validation.py` & `pkilint-0.9.9/pkilint/validation.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/pkilint.egg-info/PKG-INFO` & `pkilint-0.9.9/pkilint.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pkilint
-Version: 0.9.8
+Version: 0.9.9
 Summary: A framework for verifying PKI structures
 Home-page: https://github.com/digicert/pkilint
 Author: DigiCert, Inc.
 Author-email: corey.bonnell@digicert.com
 License: MIT
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

### Comparing `pkilint-0.9.8/pkilint.egg-info/SOURCES.txt` & `pkilint-0.9.9/pkilint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/setup.cfg` & `pkilint-0.9.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/integration_certificate/__init__.py` & `pkilint-0.9.9/tests/integration_certificate/__init__.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/integration_certificate/test_cabf_serverauth_cert.py` & `pkilint-0.9.9/tests/integration_certificate/test_cabf_serverauth_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/integration_certificate/test_cabf_smime_cert.py` & `pkilint-0.9.9/tests/integration_certificate/test_cabf_smime_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/integration_certificate/test_pkix_cert.py` & `pkilint-0.9.9/tests/integration_certificate/test_pkix_cert.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/itu/test_bitstring.py` & `pkilint-0.9.9/tests/itu/test_bitstring.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/itu/test_string.py` & `pkilint-0.9.9/tests/itu/test_string.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/test_cli_smoke.py` & `pkilint-0.9.9/tests/test_cli_smoke.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/test_report.py` & `pkilint-0.9.9/tests/test_report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/test_server.py` & `pkilint-0.9.9/tests/test_server.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/test_validation_report.py` & `pkilint-0.9.9/tests/test_validation_report.py`

 * *Files identical despite different names*

### Comparing `pkilint-0.9.8/tests/util.py` & `pkilint-0.9.9/tests/util.py`

 * *Files identical despite different names*

