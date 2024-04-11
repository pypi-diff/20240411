# Comparing `tmp/botocore-a-la-carte-payment-cryptography-1.34.81.tar.gz` & `tmp/botocore-a-la-carte-payment-cryptography-1.34.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botocore-a-la-carte-payment-cryptography-1.34.81.tar", last modified: Wed Apr 10 01:00:08 2024, max compression
+gzip compressed data, was "botocore-a-la-carte-payment-cryptography-1.34.9.tar", last modified: Thu Dec 28 01:06:57 2023, max compression
```

## Comparing `botocore-a-la-carte-payment-cryptography-1.34.81.tar` & `botocore-a-la-carte-payment-cryptography-1.34.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.324294 botocore-a-la-carte-payment-cryptography-1.34.81/
--rw-r--r--   0 runner    (1001) docker     (127)    10174 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 01:00:08.324294 botocore-a-la-carte-payment-cryptography-1.34.81/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.320294 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.320294 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.320294 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.320294 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/
--rw-r--r--   0 runner    (1001) docker     (127)    17732 2024-04-10 00:59:41.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json
--rw-r--r--   0 runner    (1001) docker     (127)      504 2024-04-10 00:59:41.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/paginators-1.json
--rw-r--r--   0 runner    (1001) docker     (127)   101492 2024-04-10 00:59:41.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/service-2.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 01:00:08.320294 botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      984 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 01:00:08.324294 botocore-a-la-carte-payment-cryptography-1.34.81/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1181 2024-04-10 01:00:08.000000 botocore-a-la-carte-payment-cryptography-1.34.81/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/
+-rw-r--r--   0 runner    (1001) docker     (127)    10174 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/
+-rw-r--r--   0 runner    (1001) docker     (127)    17732 2023-12-28 01:06:26.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      504 2023-12-28 01:06:26.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/paginators-1.json
+-rw-r--r--   0 runner    (1001) docker     (127)    95268 2023-12-28 01:06:26.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/service-2.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      983 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-28 01:06:57.298402 botocore-a-la-carte-payment-cryptography-1.34.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2023-12-28 01:06:57.000000 botocore-a-la-carte-payment-cryptography-1.34.9/setup.py
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/LICENSE.txt` & `botocore-a-la-carte-payment-cryptography-1.34.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-1.34.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography
-Version: 1.34.81
+Version: 1.34.9
 Summary: payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json` & `botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/endpoint-rule-set-1.json`

 * *Files identical despite different names*

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/botocore/data/payment-cryptography/2021-09-14/service-2.json` & `botocore-a-la-carte-payment-cryptography-1.34.9/botocore/data/payment-cryptography/2021-09-14/service-2.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9953202950808251%*

 * *Differences: {"'operations'": "{'ExportKey': {'documentation': '<p>Exports a key from Amazon Web Services "*

 * *                 'Payment Cryptography.</p> <p>Amazon Web Services Payment Cryptography simplifies '*

 * *                 'key exchange by replacing the existing paper-based approach with a modern '*

 * *                 'electronic approach. With <code>ExportKey</code> you can export symmetric keys '*

 * *                 'using either symmetric and asymmetric key exchange mechanisms. Using this '*

 * *                 'operation,  […]*

```diff
@@ -167,15 +167,15 @@
             },
             "name": "DeleteKey",
             "output": {
                 "shape": "DeleteKeyOutput"
             }
         },
         "ExportKey": {
-            "documentation": "<p>Exports a key from Amazon Web Services Payment Cryptography.</p> <p>Amazon Web Services Payment Cryptography simplifies key exchange by replacing the existing paper-based approach with a modern electronic approach. With <code>ExportKey</code> you can export symmetric keys using either symmetric and asymmetric key exchange mechanisms. Using this operation, you can share your Amazon Web Services Payment Cryptography generated keys with other service partners to perform cryptographic operations outside of Amazon Web Services Payment Cryptography </p> <p>For symmetric key exchange, Amazon Web Services Payment Cryptography uses the ANSI X9 TR-31 norm in accordance with PCI PIN guidelines. And for asymmetric key exchange, Amazon Web Services Payment Cryptography supports ANSI X9 TR-34 norm and RSA wrap and unwrap key exchange mechanism. Asymmetric key exchange methods are typically used to establish bi-directional trust between the two parties exhanging keys and are used for initial key exchange such as Key Encryption Key (KEK). After which you can export working keys using symmetric method to perform various cryptographic operations within Amazon Web Services Payment Cryptography.</p> <p>The TR-34 norm is intended for exchanging 3DES keys only and keys are imported in a WrappedKeyBlock format. Key attributes (such as KeyUsage, KeyAlgorithm, KeyModesOfUse, Exportability) are contained within the key block. With RSA wrap and unwrap, you can exchange both 3DES and AES-128 keys. The keys are imported in a WrappedKeyCryptogram format and you will need to specify the key attributes during import. </p> <p>You can also use <code>ExportKey</code> functionality to generate and export an IPEK (Initial Pin Encryption Key) from Amazon Web Services Payment Cryptography using either TR-31 or TR-34 export key exchange. IPEK is generated from BDK (Base Derivation Key) and <code>ExportDukptInitialKey</code> attribute KSN (<code>KeySerialNumber</code>). The generated IPEK does not persist within Amazon Web Services Payment Cryptography and has to be re-generated each time during export.</p> <p> <b>To export initial keys (KEK) or IPEK using TR-34</b> </p> <p>Using this operation, you can export initial key using TR-34 asymmetric key exchange. You can only export KEK generated within Amazon Web Services Payment Cryptography. In TR-34 terminology, the sending party of the key is called Key Distribution Host (KDH) and the receiving party of the key is called Key Receiving Device (KRD). During key export process, KDH is Amazon Web Services Payment Cryptography which initiates key export and KRD is the user receiving the key.</p> <p>To initiate TR-34 key export, the KRD must obtain an export token by calling <a>GetParametersForExport</a>. This operation also generates a key pair for the purpose of key export, signs the key and returns back the signing public key certificate (also known as KDH signing certificate) and root certificate chain. The KDH uses the private key to sign the the export payload and the signing public key certificate is provided to KRD to verify the signature. The KRD can import the root certificate into its Hardware Security Module (HSM), as required. The export token and the associated KDH signing certificate expires after 7 days. </p> <p>Next the KRD generates a key pair for the the purpose of encrypting the KDH key and provides the public key cerificate (also known as KRD wrapping certificate) back to KDH. The KRD will also import the root cerificate chain into Amazon Web Services Payment Cryptography by calling <a>ImportKey</a> for <code>RootCertificatePublicKey</code>. The KDH, Amazon Web Services Payment Cryptography, will use the KRD wrapping cerificate to encrypt (wrap) the key under export and signs it with signing private key to generate a TR-34 WrappedKeyBlock. For more information on TR-34 key export, see section <a href=\"https://docs.aws.amazon.com/payment-cryptography/latest/userguide/keys-export.html\">Exporting symmetric keys</a> in the <i>Amazon Web Services Payment Cryptography User Guide</i>. </p> <p>Set the following parameters:</p> <ul> <li> <p> <code>ExportAttributes</code>: Specify export attributes in case of IPEK export. This parameter is optional for KEK export.</p> </li> <li> <p> <code>ExportKeyIdentifier</code>: The <code>KeyARN</code> of the KEK or BDK (in case of IPEK) under export.</p> </li> <li> <p> <code>KeyMaterial</code>: Use <code>Tr34KeyBlock</code> parameters.</p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: The <code>KeyARN</code> of the certificate chain that signed the KRD wrapping key certificate.</p> </li> <li> <p> <code>ExportToken</code>: Obtained from KDH by calling <a>GetParametersForImport</a>.</p> </li> <li> <p> <code>WrappingKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the KRD wrapping key Amazon Web Services Payment Cryptography uses for encryption of the TR-34 export payload. This certificate must be signed by the root certificate (CertificateAuthorityPublicKeyIdentifier) imported into Amazon Web Services Payment Cryptography.</p> </li> </ul> <p>When this operation is successful, Amazon Web Services Payment Cryptography returns the KEK or IPEK as a TR-34 WrappedKeyBlock. </p> <p> <b>To export initial keys (KEK) or IPEK using RSA Wrap and Unwrap</b> </p> <p>Using this operation, you can export initial key using asymmetric RSA wrap and unwrap key exchange method. To initiate export, generate an asymmetric key pair on the receiving HSM and obtain the public key certificate in PEM format (base64 encoded) for the purpose of wrapping and the root certifiate chain. Import the root certificate into Amazon Web Services Payment Cryptography by calling <a>ImportKey</a> for <code>RootCertificatePublicKey</code>.</p> <p>Next call <code>ExportKey</code> and set the following parameters:</p> <ul> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: The <code>KeyARN</code> of the certificate chain that signed wrapping key certificate.</p> </li> <li> <p> <code>KeyMaterial</code>: Set to <code>KeyCryptogram</code>.</p> </li> <li> <p> <code>WrappingKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) obtained by the receiving HSM and signed by the root certificate (CertificateAuthorityPublicKeyIdentifier) imported into Amazon Web Services Payment Cryptography. The receiving HSM uses its private key component to unwrap the WrappedKeyCryptogram.</p> </li> </ul> <p>When this operation is successful, Amazon Web Services Payment Cryptography returns the WrappedKeyCryptogram. </p> <p> <b>To export working keys or IPEK using TR-31</b> </p> <p>Using this operation, you can export working keys or IPEK using TR-31 symmetric key exchange. In TR-31, you must use an initial key such as KEK to encrypt or wrap the key under export. To establish a KEK, you can use <a>CreateKey</a> or <a>ImportKey</a>. </p> <p>Set the following parameters:</p> <ul> <li> <p> <code>ExportAttributes</code>: Specify export attributes in case of IPEK export. This parameter is optional for KEK export.</p> </li> <li> <p> <code>ExportKeyIdentifier</code>: The <code>KeyARN</code> of the KEK or BDK (in case of IPEK) under export.</p> </li> <li> <p> <code>KeyMaterial</code>: Use <code>Tr31KeyBlock</code> parameters.</p> </li> </ul> <p>When this operation is successful, Amazon Web Services Payment Cryptography returns the working key or IPEK as a TR-31 WrappedKeyBlock.</p> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>GetParametersForExport</a> </p> </li> <li> <p> <a>ImportKey</a> </p> </li> </ul>",
+            "documentation": "<p>Exports a key from Amazon Web Services Payment Cryptography.</p> <p>Amazon Web Services Payment Cryptography simplifies key exchange by replacing the existing paper-based approach with a modern electronic approach. With <code>ExportKey</code> you can export symmetric keys using either symmetric and asymmetric key exchange mechanisms. Using this operation, you can share your Amazon Web Services Payment Cryptography generated keys with other service partners to perform cryptographic operations outside of Amazon Web Services Payment Cryptography </p> <p>For symmetric key exchange, Amazon Web Services Payment Cryptography uses the ANSI X9 TR-31 norm in accordance with PCI PIN guidelines. And for asymmetric key exchange, Amazon Web Services Payment Cryptography supports ANSI X9 TR-34 norm . Asymmetric key exchange methods are typically used to establish bi-directional trust between the two parties exhanging keys and are used for initial key exchange such as Key Encryption Key (KEK). After which you can export working keys using symmetric method to perform various cryptographic operations within Amazon Web Services Payment Cryptography.</p> <p>The TR-34 norm is intended for exchanging 3DES keys only and keys are imported in a WrappedKeyBlock format. Key attributes (such as KeyUsage, KeyAlgorithm, KeyModesOfUse, Exportability) are contained within the key block.</p> <p>You can also use <code>ExportKey</code> functionality to generate and export an IPEK (Initial Pin Encryption Key) from Amazon Web Services Payment Cryptography using either TR-31 or TR-34 export key exchange. IPEK is generated from BDK (Base Derivation Key) and <code>ExportDukptInitialKey</code> attribute KSN (<code>KeySerialNumber</code>). The generated IPEK does not persist within Amazon Web Services Payment Cryptography and has to be re-generated each time during export.</p> <p> <b>To export KEK or IPEK using TR-34</b> </p> <p>Using this operation, you can export initial key using TR-34 asymmetric key exchange. You can only export KEK generated within Amazon Web Services Payment Cryptography. In TR-34 terminology, the sending party of the key is called Key Distribution Host (KDH) and the receiving party of the key is called Key Receiving Device (KRD). During key export process, KDH is Amazon Web Services Payment Cryptography which initiates key export and KRD is the user receiving the key.</p> <p>To initiate TR-34 key export, the KRD must obtain an export token by calling <a>GetParametersForExport</a>. This operation also generates a key pair for the purpose of key export, signs the key and returns back the signing public key certificate (also known as KDH signing certificate) and root certificate chain. The KDH uses the private key to sign the the export payload and the signing public key certificate is provided to KRD to verify the signature. The KRD can import the root certificate into its Hardware Security Module (HSM), as required. The export token and the associated KDH signing certificate expires after 7 days. </p> <p>Next the KRD generates a key pair for the the purpose of encrypting the KDH key and provides the public key cerificate (also known as KRD wrapping certificate) back to KDH. The KRD will also import the root cerificate chain into Amazon Web Services Payment Cryptography by calling <a>ImportKey</a> for <code>RootCertificatePublicKey</code>. The KDH, Amazon Web Services Payment Cryptography, will use the KRD wrapping cerificate to encrypt (wrap) the key under export and signs it with signing private key to generate a TR-34 WrappedKeyBlock. For more information on TR-34 key export, see section <a href=\"https://docs.aws.amazon.com/payment-cryptography/latest/userguide/keys-export.html\">Exporting symmetric keys</a> in the <i>Amazon Web Services Payment Cryptography User Guide</i>. </p> <p>Set the following parameters:</p> <ul> <li> <p> <code>ExportAttributes</code>: Specify export attributes in case of IPEK export. This parameter is optional for KEK export.</p> </li> <li> <p> <code>ExportKeyIdentifier</code>: The <code>KeyARN</code> of the KEK or BDK (in case of IPEK) under export.</p> </li> <li> <p> <code>KeyMaterial</code>: Use <code>Tr34KeyBlock</code> parameters.</p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: The <code>KeyARN</code> of the certificate chain that signed the KRD wrapping key certificate.</p> </li> <li> <p> <code>ExportToken</code>: Obtained from KDH by calling <a>GetParametersForImport</a>.</p> </li> <li> <p> <code>WrappingKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the KRD wrapping key Amazon Web Services Payment Cryptography uses for encryption of the TR-34 export payload. This certificate must be signed by the root certificate (CertificateAuthorityPublicKeyIdentifier) imported into Amazon Web Services Payment Cryptography.</p> </li> </ul> <p>When this operation is successful, Amazon Web Services Payment Cryptography returns the KEK or IPEK as a TR-34 WrappedKeyBlock. </p> <p> <b>To export WK (Working Key) or IPEK using TR-31</b> </p> <p>Using this operation, you can export working keys or IPEK using TR-31 symmetric key exchange. In TR-31, you must use an initial key such as KEK to encrypt or wrap the key under export. To establish a KEK, you can use <a>CreateKey</a> or <a>ImportKey</a>. </p> <p>Set the following parameters:</p> <ul> <li> <p> <code>ExportAttributes</code>: Specify export attributes in case of IPEK export. This parameter is optional for KEK export.</p> </li> <li> <p> <code>ExportKeyIdentifier</code>: The <code>KeyARN</code> of the KEK or BDK (in case of IPEK) under export.</p> </li> <li> <p> <code>KeyMaterial</code>: Use <code>Tr31KeyBlock</code> parameters.</p> </li> </ul> <p>When this operation is successful, Amazon Web Services Payment Cryptography returns the WK or IPEK as a TR-31 WrappedKeyBlock.</p> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>GetParametersForExport</a> </p> </li> <li> <p> <a>ImportKey</a> </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ServiceUnavailableException"
                 },
                 {
                     "shape": "ValidationException"
                 },
@@ -312,15 +312,15 @@
             },
             "name": "GetParametersForExport",
             "output": {
                 "shape": "GetParametersForExportOutput"
             }
         },
         "GetParametersForImport": {
-            "documentation": "<p>Gets the import token and the wrapping key certificate in PEM format (base64 encoded) to initiate a TR-34 WrappedKeyBlock or a RSA WrappedKeyCryptogram import into Amazon Web Services Payment Cryptography.</p> <p>The wrapping key certificate wraps the key under import. The import token and wrapping key certificate must be in place and operational before calling <a>ImportKey</a>. The import token expires in 7 days. You can use the same import token to import multiple keys into your service account.</p> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>GetParametersForExport</a> </p> </li> <li> <p> <a>ImportKey</a> </p> </li> </ul>",
+            "documentation": "<p>Gets the import token and the wrapping key certificate in PEM format (base64 encoded) to initiate a TR-34 WrappedKeyBlock.</p> <p>The wrapping key certificate wraps the key under import. The import token and wrapping key certificate must be in place and operational before calling <a>ImportKey</a>. The import token expires in 7 days. You can use the same import token to import multiple keys into your service account.</p> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>GetParametersForExport</a> </p> </li> <li> <p> <a>ImportKey</a> </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
                 {
                     "shape": "ServiceUnavailableException"
                 },
@@ -386,15 +386,15 @@
             },
             "name": "GetPublicKeyCertificate",
             "output": {
                 "shape": "GetPublicKeyCertificateOutput"
             }
         },
         "ImportKey": {
-            "documentation": "<p>Imports symmetric keys and public key certificates in PEM format (base64 encoded) into Amazon Web Services Payment Cryptography.</p> <p>Amazon Web Services Payment Cryptography simplifies key exchange by replacing the existing paper-based approach with a modern electronic approach. With <code>ImportKey</code> you can import symmetric keys using either symmetric and asymmetric key exchange mechanisms.</p> <p>For symmetric key exchange, Amazon Web Services Payment Cryptography uses the ANSI X9 TR-31 norm in accordance with PCI PIN guidelines. And for asymmetric key exchange, Amazon Web Services Payment Cryptography supports ANSI X9 TR-34 norm and RSA wrap and unwrap key exchange mechanisms. Asymmetric key exchange methods are typically used to establish bi-directional trust between the two parties exhanging keys and are used for initial key exchange such as Key Encryption Key (KEK) or Zone Master Key (ZMK). After which you can import working keys using symmetric method to perform various cryptographic operations within Amazon Web Services Payment Cryptography.</p> <p>The TR-34 norm is intended for exchanging 3DES keys only and keys are imported in a WrappedKeyBlock format. Key attributes (such as KeyUsage, KeyAlgorithm, KeyModesOfUse, Exportability) are contained within the key block. With RSA wrap and unwrap, you can exchange both 3DES and AES-128 keys. The keys are imported in a WrappedKeyCryptogram format and you will need to specify the key attributes during import. </p> <p>You can also import a <i>root public key certificate</i>, used to sign other public key certificates, or a <i>trusted public key certificate</i> under an already established root public key certificate.</p> <p> <b>To import a public root key certificate</b> </p> <p>You can also import a <i>root public key certificate</i>, used to sign other public key certificates, or a <i>trusted public key certificate</i> under an already established root public key certificate.</p> <p> <b>To import a public root key certificate</b> </p> <p>Using this operation, you can import the public component (in PEM cerificate format) of your private root key. You can use the imported public root key certificate for digital signatures, for example signing wrapping key or signing key in TR-34, within your Amazon Web Services Payment Cryptography account.</p> <p>Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: <code>RootCertificatePublicKey</code> </p> </li> <li> <p> <code>KeyClass</code>: <code>PUBLIC_KEY</code> </p> </li> <li> <p> <code>KeyModesOfUse</code>: <code>Verify</code> </p> </li> <li> <p> <code>KeyUsage</code>: <code>TR31_S0_ASYMMETRIC_KEY_FOR_DIGITAL_SIGNATURE</code> </p> </li> <li> <p> <code>PublicKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the private root key under import.</p> </li> </ul> <p> <b>To import a trusted public key certificate</b> </p> <p>The root public key certificate must be in place and operational before you import a trusted public key certificate. Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: <code>TrustedCertificatePublicKey</code> </p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: <code>KeyArn</code> of the <code>RootCertificatePublicKey</code>.</p> </li> <li> <p> <code>KeyModesOfUse</code> and <code>KeyUsage</code>: Corresponding to the cryptographic operations such as wrap, sign, or encrypt that you will allow the trusted public key certificate to perform.</p> </li> <li> <p> <code>PublicKeyCertificate</code>: The trusted public key certificate in PEM format (base64 encoded) under import.</p> </li> </ul> <p> <b>To import initial keys (KEK or ZMK or similar) using TR-34</b> </p> <p>Using this operation, you can import initial key using TR-34 asymmetric key exchange. In TR-34 terminology, the sending party of the key is called Key Distribution Host (KDH) and the receiving party of the key is called Key Receiving Device (KRD). During the key import process, KDH is the user who initiates the key import and KRD is Amazon Web Services Payment Cryptography who receives the key.</p> <p>To initiate TR-34 key import, the KDH must obtain an import token by calling <a>GetParametersForImport</a>. This operation generates an encryption keypair for the purpose of key import, signs the key and returns back the wrapping key certificate (also known as KRD wrapping certificate) and the root certificate chain. The KDH must trust and install the KRD wrapping certificate on its HSM and use it to encrypt (wrap) the KDH key during TR-34 WrappedKeyBlock generation. The import token and associated KRD wrapping certificate expires after 7 days.</p> <p>Next the KDH generates a key pair for the purpose of signing the encrypted KDH key and provides the public certificate of the signing key to Amazon Web Services Payment Cryptography. The KDH will also need to import the root certificate chain of the KDH signing certificate by calling <code>ImportKey</code> for <code>RootCertificatePublicKey</code>. For more information on TR-34 key import, see section <a href=\"https://docs.aws.amazon.com/payment-cryptography/latest/userguide/keys-import.html\">Importing symmetric keys</a> in the <i>Amazon Web Services Payment Cryptography User Guide</i>.</p> <p>Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: Use <code>Tr34KeyBlock</code> parameters.</p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: The <code>KeyARN</code> of the certificate chain that signed the KDH signing key certificate.</p> </li> <li> <p> <code>ImportToken</code>: Obtained from KRD by calling <a>GetParametersForImport</a>.</p> </li> <li> <p> <code>WrappedKeyBlock</code>: The TR-34 wrapped key material from KDH. It contains the KDH key under import, wrapped with KRD wrapping certificate and signed by KDH signing private key. This TR-34 key block is typically generated by the KDH Hardware Security Module (HSM) outside of Amazon Web Services Payment Cryptography.</p> </li> <li> <p> <code>SigningKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the KDH signing key generated under the root certificate (CertificateAuthorityPublicKeyIdentifier) imported in Amazon Web Services Payment Cryptography.</p> </li> </ul> <p> <b>To import initial keys (KEK or ZMK or similar) using RSA Wrap and Unwrap</b> </p> <p>Using this operation, you can import initial key using asymmetric RSA wrap and unwrap key exchange method. To initiate import, call <a>GetParametersForImport</a> with <code>KeyMaterial</code> set to <code>KEY_CRYPTOGRAM</code> to generate an import token. This operation also generates an encryption keypair for the purpose of key import, signs the key and returns back the wrapping key certificate in PEM format (base64 encoded) and its root certificate chain. The import token and associated KRD wrapping certificate expires after 7 days. </p> <p>You must trust and install the wrapping certificate and its certificate chain on the sending HSM and use it to wrap the key under export for WrappedKeyCryptogram generation. Next call <code>ImportKey</code> with <code>KeyMaterial</code> set to <code>KEY_CRYPTOGRAM</code> and provide the <code>ImportToken</code> and <code>KeyAttributes</code> for the key under import.</p> <p> <b>To import working keys using TR-31</b> </p> <p>Amazon Web Services Payment Cryptography uses TR-31 symmetric key exchange norm to import working keys. A KEK must be established within Amazon Web Services Payment Cryptography by using TR-34 key import or by using <a>CreateKey</a>. To initiate a TR-31 key import, set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: Use <code>Tr31KeyBlock</code> parameters.</p> </li> <li> <p> <code>WrappedKeyBlock</code>: The TR-31 wrapped key material. It contains the key under import, encrypted using KEK. The TR-31 key block is typically generated by a HSM outside of Amazon Web Services Payment Cryptography. </p> </li> <li> <p> <code>WrappingKeyIdentifier</code>: The <code>KeyArn</code> of the KEK that Amazon Web Services Payment Cryptography uses to decrypt or unwrap the key under import.</p> </li> </ul> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>ExportKey</a> </p> </li> <li> <p> <a>GetParametersForImport</a> </p> </li> </ul>",
+            "documentation": "<p>Imports symmetric keys and public key certificates in PEM format (base64 encoded) into Amazon Web Services Payment Cryptography.</p> <p>Amazon Web Services Payment Cryptography simplifies key exchange by replacing the existing paper-based approach with a modern electronic approach. With <code>ImportKey</code> you can import symmetric keys using either symmetric and asymmetric key exchange mechanisms.</p> <p>For symmetric key exchange, Amazon Web Services Payment Cryptography uses the ANSI X9 TR-31 norm in accordance with PCI PIN guidelines. And for asymmetric key exchange, Amazon Web Services Payment Cryptography supports ANSI X9 TR-34 norm . Asymmetric key exchange methods are typically used to establish bi-directional trust between the two parties exhanging keys and are used for initial key exchange such as Key Encryption Key (KEK) or Zone Master Key (ZMK). After which you can import working keys using symmetric method to perform various cryptographic operations within Amazon Web Services Payment Cryptography.</p> <p>The TR-34 norm is intended for exchanging 3DES keys only and keys are imported in a WrappedKeyBlock format. Key attributes (such as KeyUsage, KeyAlgorithm, KeyModesOfUse, Exportability) are contained within the key block. </p> <p>You can also import a <i>root public key certificate</i>, used to sign other public key certificates, or a <i>trusted public key certificate</i> under an already established root public key certificate.</p> <p> <b>To import a public root key certificate</b> </p> <p>You can also import a <i>root public key certificate</i>, used to sign other public key certificates, or a <i>trusted public key certificate</i> under an already established root public key certificate.</p> <p> <b>To import a public root key certificate</b> </p> <p>Using this operation, you can import the public component (in PEM cerificate format) of your private root key. You can use the imported public root key certificate for digital signatures, for example signing wrapping key or signing key in TR-34, within your Amazon Web Services Payment Cryptography account.</p> <p>Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: <code>RootCertificatePublicKey</code> </p> </li> <li> <p> <code>KeyClass</code>: <code>PUBLIC_KEY</code> </p> </li> <li> <p> <code>KeyModesOfUse</code>: <code>Verify</code> </p> </li> <li> <p> <code>KeyUsage</code>: <code>TR31_S0_ASYMMETRIC_KEY_FOR_DIGITAL_SIGNATURE</code> </p> </li> <li> <p> <code>PublicKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the private root key under import.</p> </li> </ul> <p> <b>To import a trusted public key certificate</b> </p> <p>The root public key certificate must be in place and operational before you import a trusted public key certificate. Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: <code>TrustedCertificatePublicKey</code> </p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: <code>KeyArn</code> of the <code>RootCertificatePublicKey</code>.</p> </li> <li> <p> <code>KeyModesOfUse</code> and <code>KeyUsage</code>: Corresponding to the cryptographic operations such as wrap, sign, or encrypt that you will allow the trusted public key certificate to perform.</p> </li> <li> <p> <code>PublicKeyCertificate</code>: The trusted public key certificate in PEM format (base64 encoded) under import.</p> </li> </ul> <p> <b>To import KEK or ZMK using TR-34</b> </p> <p>Using this operation, you can import initial key using TR-34 asymmetric key exchange. In TR-34 terminology, the sending party of the key is called Key Distribution Host (KDH) and the receiving party of the key is called Key Receiving Device (KRD). During the key import process, KDH is the user who initiates the key import and KRD is Amazon Web Services Payment Cryptography who receives the key.</p> <p>To initiate TR-34 key import, the KDH must obtain an import token by calling <a>GetParametersForImport</a>. This operation generates an encryption keypair for the purpose of key import, signs the key and returns back the wrapping key certificate (also known as KRD wrapping certificate) and the root certificate chain. The KDH must trust and install the KRD wrapping certificate on its HSM and use it to encrypt (wrap) the KDH key during TR-34 WrappedKeyBlock generation. The import token and associated KRD wrapping certificate expires after 7 days.</p> <p>Next the KDH generates a key pair for the purpose of signing the encrypted KDH key and provides the public certificate of the signing key to Amazon Web Services Payment Cryptography. The KDH will also need to import the root certificate chain of the KDH signing certificate by calling <code>ImportKey</code> for <code>RootCertificatePublicKey</code>. For more information on TR-34 key import, see section <a href=\"https://docs.aws.amazon.com/payment-cryptography/latest/userguide/keys-import.html\">Importing symmetric keys</a> in the <i>Amazon Web Services Payment Cryptography User Guide</i>.</p> <p>Set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: Use <code>Tr34KeyBlock</code> parameters.</p> </li> <li> <p> <code>CertificateAuthorityPublicKeyIdentifier</code>: The <code>KeyARN</code> of the certificate chain that signed the KDH signing key certificate.</p> </li> <li> <p> <code>ImportToken</code>: Obtained from KRD by calling <a>GetParametersForImport</a>.</p> </li> <li> <p> <code>WrappedKeyBlock</code>: The TR-34 wrapped key material from KDH. It contains the KDH key under import, wrapped with KRD wrapping certificate and signed by KDH signing private key. This TR-34 key block is typically generated by the KDH Hardware Security Module (HSM) outside of Amazon Web Services Payment Cryptography.</p> </li> <li> <p> <code>SigningKeyCertificate</code>: The public key certificate in PEM format (base64 encoded) of the KDH signing key generated under the root certificate (CertificateAuthorityPublicKeyIdentifier) imported in Amazon Web Services Payment Cryptography.</p> </li> </ul> <p> <b>To import WK (Working Key) using TR-31</b> </p> <p>Amazon Web Services Payment Cryptography uses TR-31 symmetric key exchange norm to import working keys. A KEK must be established within Amazon Web Services Payment Cryptography by using TR-34 key import or by using <a>CreateKey</a>. To initiate a TR-31 key import, set the following parameters:</p> <ul> <li> <p> <code>KeyMaterial</code>: Use <code>Tr31KeyBlock</code> parameters.</p> </li> <li> <p> <code>WrappedKeyBlock</code>: The TR-31 wrapped key material. It contains the key under import, encrypted using KEK. The TR-31 key block is typically generated by a HSM outside of Amazon Web Services Payment Cryptography. </p> </li> <li> <p> <code>WrappingKeyIdentifier</code>: The <code>KeyArn</code> of the KEK that Amazon Web Services Payment Cryptography uses to decrypt or unwrap the key under import.</p> </li> </ul> <p> <b>Cross-account use:</b> This operation can't be used across different Amazon Web Services accounts.</p> <p> <b>Related operations:</b> </p> <ul> <li> <p> <a>ExportKey</a> </p> </li> <li> <p> <a>GetParametersForImport</a> </p> </li> </ul>",
             "errors": [
                 {
                     "shape": "ServiceQuotaExceededException"
                 },
                 {
                     "shape": "ServiceUnavailableException"
                 },
@@ -969,36 +969,14 @@
                 }
             },
             "required": [
                 "KeySerialNumber"
             ],
             "type": "structure"
         },
-        "ExportKeyCryptogram": {
-            "documentation": "<p>Parameter information for key material export using asymmetric RSA wrap and unwrap key exchange method.</p>",
-            "members": {
-                "CertificateAuthorityPublicKeyIdentifier": {
-                    "documentation": "<p>The <code>KeyARN</code> of the certificate chain that signs the wrapping key certificate during RSA wrap and unwrap key export.</p>",
-                    "shape": "KeyArnOrKeyAliasType"
-                },
-                "WrappingKeyCertificate": {
-                    "documentation": "<p>The wrapping key certificate in PEM format (base64 encoded). Amazon Web Services Payment Cryptography uses this certificate to wrap the key under export.</p>",
-                    "shape": "CertificateType"
-                },
-                "WrappingSpec": {
-                    "documentation": "<p>The wrapping spec for the key under export.</p>",
-                    "shape": "WrappingKeySpec"
-                }
-            },
-            "required": [
-                "CertificateAuthorityPublicKeyIdentifier",
-                "WrappingKeyCertificate"
-            ],
-            "type": "structure"
-        },
         "ExportKeyInput": {
             "members": {
                 "ExportAttributes": {
                     "documentation": "<p>The attributes for IPEK generation during export.</p>",
                     "shape": "ExportAttributes"
                 },
                 "ExportKeyIdentifier": {
@@ -1013,20 +991,16 @@
             "required": [
                 "ExportKeyIdentifier",
                 "KeyMaterial"
             ],
             "type": "structure"
         },
         "ExportKeyMaterial": {
-            "documentation": "<p>Parameter information for key material export from Amazon Web Services Payment Cryptography using TR-31 or TR-34 or RSA wrap and unwrap key exchange method.</p>",
+            "documentation": "<p>Parameter information for key material export from Amazon Web Services Payment Cryptography using TR-31 or TR-34 key exchange method.</p>",
             "members": {
-                "KeyCryptogram": {
-                    "documentation": "<p>Parameter information for key material export using asymmetric RSA wrap and unwrap key exchange method</p>",
-                    "shape": "ExportKeyCryptogram"
-                },
                 "Tr31KeyBlock": {
                     "documentation": "<p>Parameter information for key material export using symmetric TR-31 key exchange method.</p>",
                     "shape": "ExportTr31KeyBlock"
                 },
                 "Tr34KeyBlock": {
                     "documentation": "<p>Parameter information for key material export using the asymmetric TR-34 key exchange method.</p>",
                     "shape": "ExportTr34KeyBlock"
@@ -1034,15 +1008,15 @@
             },
             "type": "structure",
             "union": true
         },
         "ExportKeyOutput": {
             "members": {
                 "WrappedKey": {
-                    "documentation": "<p>The key material under export as a TR-34 WrappedKeyBlock or a TR-31 WrappedKeyBlock. or a RSA WrappedKeyCryptogram.</p>",
+                    "documentation": "<p>The key material under export as a TR-34 WrappedKeyBlock or a TR-31 WrappedKeyBlock. </p>",
                     "shape": "WrappedKey"
                 }
             },
             "type": "structure"
         },
         "ExportTokenId": {
             "pattern": "^export-token-[0-9a-zA-Z]{16,64}$",
@@ -1189,19 +1163,19 @@
                 "SigningKeyCertificateChain"
             ],
             "type": "structure"
         },
         "GetParametersForImportInput": {
             "members": {
                 "KeyMaterialType": {
-                    "documentation": "<p>The method to use for key material import. Import token is only required for TR-34 WrappedKeyBlock (<code>TR34_KEY_BLOCK</code>) and RSA WrappedKeyCryptogram (<code>KEY_CRYPTOGRAM</code>).</p> <p>Import token is not required for TR-31, root public key cerificate or trusted public key certificate.</p>",
+                    "documentation": "<p>The method to use for key material import. Import token is only required for TR-34 WrappedKeyBlock (<code>TR34_KEY_BLOCK</code>).</p> <p>Import token is not required for TR-31, root public key cerificate or trusted public key certificate.</p>",
                     "shape": "KeyMaterialType"
                 },
                 "WrappingKeyAlgorithm": {
-                    "documentation": "<p>The wrapping key algorithm to generate a wrapping key certificate. This certificate wraps the key under import.</p> <p>At this time, <code>RSA_2048</code> is the allowed algorithm for TR-34 WrappedKeyBlock import. Additionally, <code>RSA_2048</code>, <code>RSA_3072</code>, <code>RSA_4096</code> are the allowed algorithms for RSA WrappedKeyCryptogram import.</p>",
+                    "documentation": "<p>The wrapping key algorithm to generate a wrapping key certificate. This certificate wraps the key under import.</p> <p>At this time, <code>RSA_2048</code>, <code>RSA_3072</code>, <code>RSA_4096</code> are the only allowed algorithms for TR-34 WrappedKeyBlock import.</p>",
                     "shape": "KeyAlgorithm"
                 }
             },
             "required": [
                 "KeyMaterialType",
                 "WrappingKeyAlgorithm"
             ],
@@ -1214,15 +1188,15 @@
                     "shape": "ImportTokenId"
                 },
                 "ParametersValidUntilTimestamp": {
                     "documentation": "<p>The validity period of the import token.</p>",
                     "shape": "Timestamp"
                 },
                 "WrappingKeyAlgorithm": {
-                    "documentation": "<p>The algorithm of the wrapping key for use within TR-34 WrappedKeyBlock or RSA WrappedKeyCryptogram.</p>",
+                    "documentation": "<p>The algorithm of the wrapping key for use within TR-34 WrappedKeyBlock.</p>",
                     "shape": "KeyAlgorithm"
                 },
                 "WrappingKeyCertificate": {
                     "documentation": "<p>The wrapping key certificate in PEM format (base64 encoded) of the wrapping key for use within the TR-34 key block. The certificate expires in 7 days.</p>",
                     "shape": "CertificateType"
                 },
                 "WrappingKeyCertificateChain": {
@@ -1276,45 +1250,14 @@
         },
         "HexLength20Or24": {
             "max": 24,
             "min": 20,
             "pattern": "^[0-9A-F]{20}$|^[0-9A-F]{24}$",
             "type": "string"
         },
-        "ImportKeyCryptogram": {
-            "documentation": "<p>Parameter information for key material import using asymmetric RSA wrap and unwrap key exchange method.</p>",
-            "members": {
-                "Exportable": {
-                    "documentation": "<p>Specifies whether the key is exportable from the service.</p>",
-                    "shape": "Boolean"
-                },
-                "ImportToken": {
-                    "documentation": "<p>The import token that initiates key import using the asymmetric RSA wrap and unwrap key exchange method into AWS Payment Cryptography. It expires after 7 days. You can use the same import token to import multiple keys to the same service account.</p>",
-                    "shape": "ImportTokenId"
-                },
-                "KeyAttributes": {
-                    "shape": "KeyAttributes"
-                },
-                "WrappedKeyCryptogram": {
-                    "documentation": "<p>The RSA wrapped key cryptogram under import.</p>",
-                    "shape": "WrappedKeyCryptogram"
-                },
-                "WrappingSpec": {
-                    "documentation": "<p>The wrapping spec for the wrapped key cryptogram.</p>",
-                    "shape": "WrappingKeySpec"
-                }
-            },
-            "required": [
-                "Exportable",
-                "ImportToken",
-                "KeyAttributes",
-                "WrappedKeyCryptogram"
-            ],
-            "type": "structure"
-        },
         "ImportKeyInput": {
             "members": {
                 "Enabled": {
                     "documentation": "<p>Specifies whether import key is enabled.</p>",
                     "shape": "Boolean"
                 },
                 "KeyCheckValueAlgorithm": {
@@ -1332,20 +1275,16 @@
             },
             "required": [
                 "KeyMaterial"
             ],
             "type": "structure"
         },
         "ImportKeyMaterial": {
-            "documentation": "<p>Parameter information for key material import into Amazon Web Services Payment Cryptography using TR-31 or TR-34 or RSA wrap and unwrap key exchange method.</p>",
+            "documentation": "<p>Parameter information for key material import into Amazon Web Services Payment Cryptography using TR-31 or TR-34 key exchange method.</p>",
             "members": {
-                "KeyCryptogram": {
-                    "documentation": "<p>Parameter information for key material import using asymmetric RSA wrap and unwrap key exchange method.</p>",
-                    "shape": "ImportKeyCryptogram"
-                },
                 "RootCertificatePublicKey": {
                     "documentation": "<p>Parameter information for root public key certificate import.</p>",
                     "shape": "RootCertificatePublicKey"
                 },
                 "Tr31KeyBlock": {
                     "documentation": "<p>Parameter information for key material import using symmetric TR-31 key exchange method.</p>",
                     "shape": "ImportTr31KeyBlock"
@@ -1595,16 +1534,15 @@
             "type": "string"
         },
         "KeyMaterialType": {
             "enum": [
                 "TR34_KEY_BLOCK",
                 "TR31_KEY_BLOCK",
                 "ROOT_PUBLIC_KEY_CERTIFICATE",
-                "TRUSTED_PUBLIC_KEY_CERTIFICATE",
-                "KEY_CRYPTOGRAM"
+                "TRUSTED_PUBLIC_KEY_CERTIFICATE"
             ],
             "type": "string"
         },
         "KeyModesOfUse": {
             "documentation": "<p>The list of cryptographic operations that you can perform using the key. The modes of use are de\ufb01ned in section A.5.3 of the TR-31 spec.</p>",
             "members": {
                 "Decrypt": {
@@ -1720,15 +1658,14 @@
                 "TR31_E4_EMV_MKEY_DYNAMIC_NUMBERS",
                 "TR31_E5_EMV_MKEY_CARD_PERSONALIZATION",
                 "TR31_E6_EMV_MKEY_OTHER",
                 "TR31_K0_KEY_ENCRYPTION_KEY",
                 "TR31_K1_KEY_BLOCK_PROTECTION_KEY",
                 "TR31_K3_ASYMMETRIC_KEY_FOR_KEY_AGREEMENT",
                 "TR31_M3_ISO_9797_3_MAC_KEY",
-                "TR31_M1_ISO_9797_1_MAC_KEY",
                 "TR31_M6_ISO_9797_5_CMAC_KEY",
                 "TR31_M7_HMAC_KEY",
                 "TR31_P0_PIN_ENCRYPTION_KEY",
                 "TR31_P1_PIN_GENERATION_KEY",
                 "TR31_S0_ASYMMETRIC_KEY_FOR_DIGITAL_SIGNATURE",
                 "TR31_V1_IBM3624_PIN_VERIFICATION_KEY",
                 "TR31_V2_VISA_PIN_VERIFICATION_KEY",
@@ -2183,31 +2120,18 @@
             "required": [
                 "KeyMaterial",
                 "WrappedKeyMaterialFormat",
                 "WrappingKeyArn"
             ],
             "type": "structure"
         },
-        "WrappedKeyCryptogram": {
-            "max": 4096,
-            "min": 16,
-            "pattern": "^[0-9A-F]+$",
-            "type": "string"
-        },
         "WrappedKeyMaterialFormat": {
             "enum": [
                 "KEY_CRYPTOGRAM",
                 "TR31_KEY_BLOCK",
                 "TR34_KEY_BLOCK"
             ],
             "type": "string"
-        },
-        "WrappingKeySpec": {
-            "enum": [
-                "RSA_OAEP_SHA_256",
-                "RSA_OAEP_SHA_512"
-            ],
-            "type": "string"
         }
     },
     "version": "2.0"
 }
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO` & `botocore-a-la-carte-payment-cryptography-1.34.9/botocore_a_la_carte_payment_cryptography.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botocore-a-la-carte-payment-cryptography
-Version: 1.34.81
+Version: 1.34.9
 Summary: payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.
 Home-page: https://github.com/thejcannon/botocore-a-la-carte
 Author: Amazon Web Services
 License: Apache License 2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
```

### Comparing `botocore-a-la-carte-payment-cryptography-1.34.81/setup.py` & `botocore-a-la-carte-payment-cryptography-1.34.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!/usr/bin/env python
 from setuptools import setup
 
 setup(
     name='botocore-a-la-carte-payment-cryptography',
-    version="1.34.81",
+    version="1.34.9",
     description='payment-cryptography data for botocore. See the `botocore-a-la-carte` package for more info.',
     author='Amazon Web Services',
     url='https://github.com/thejcannon/botocore-a-la-carte',
     scripts=[],
     packages=["botocore"],
     package_data={
         'botocore': ['data/payment-cryptography/*/*.json'],
```

