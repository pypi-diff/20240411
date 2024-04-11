# Comparing `tmp/auto-sdk-0.1.4.tar.gz` & `tmp/auto-sdk-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-sdk-0.1.4.tar", last modified: Tue Apr  9 00:49:41 2024, max compression
+gzip compressed data, was "auto-sdk-0.1.5.tar", last modified: Thu Apr 11 20:21:08 2024, max compression
```

## Comparing `auto-sdk-0.1.4.tar` & `auto-sdk-0.1.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.4/README.md
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.241440 auto-sdk-0.1.4/auto_identity/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      960 2024-04-09 00:49:31.000000 auto-sdk-0.1.4/auto_identity/__init__.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     6346 2024-04-09 00:48:34.000000 auto-sdk-0.1.4/auto_identity/certificate_manager.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5824 2024-04-09 00:48:45.000000 auto-sdk-0.1.4/auto_identity/key_management.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     4040 2024-04-04 00:32:25.000000 auto-sdk-0.1.4/auto_identity/registry.py
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1232 2024-04-04 00:32:25.000000 auto-sdk-0.1.4/auto_identity/utils.py
-drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/auto_sdk.egg-info/
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/PKG-INFO
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      321 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/requires.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-09 00:49:41.000000 auto-sdk-0.1.4/auto_sdk.egg-info/top_level.txt
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-09 00:49:41.251440 auto-sdk-0.1.4/setup.cfg
--rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-09 00:49:31.000000 auto-sdk-0.1.4/setup.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-11 20:21:08.976578 auto-sdk-0.1.5/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-11 20:21:08.976578 auto-sdk-0.1.5/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      274 2024-03-20 21:08:12.000000 auto-sdk-0.1.5/README.md
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-11 20:21:08.976578 auto-sdk-0.1.5/auto_identity/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      992 2024-04-11 20:15:16.000000 auto-sdk-0.1.5/auto_identity/__init__.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     9877 2024-04-11 20:07:12.000000 auto-sdk-0.1.5/auto_identity/certificate_manager.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     5824 2024-04-09 00:48:45.000000 auto-sdk-0.1.5/auto_identity/key_management.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     3542 2024-04-11 19:13:18.000000 auto-sdk-0.1.5/auto_identity/registry.py
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)     1553 2024-04-11 19:44:01.000000 auto-sdk-0.1.5/auto_identity/utils.py
+drwxr-xr-x   0 jeremy    (1000) jeremy    (1000)        0 2024-04-11 20:21:08.976578 auto-sdk-0.1.5/auto_sdk.egg-info/
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      218 2024-04-11 20:21:08.000000 auto-sdk-0.1.5/auto_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      321 2024-04-11 20:21:08.000000 auto-sdk-0.1.5/auto_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)        1 2024-04-11 20:21:08.000000 auto-sdk-0.1.5/auto_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       84 2024-04-11 20:21:08.000000 auto-sdk-0.1.5/auto_sdk.egg-info/requires.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       14 2024-04-11 20:21:08.000000 auto-sdk-0.1.5/auto_sdk.egg-info/top_level.txt
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)       38 2024-04-11 20:21:08.976578 auto-sdk-0.1.5/setup.cfg
+-rw-r--r--   0 jeremy    (1000) jeremy    (1000)      389 2024-04-11 20:15:23.000000 auto-sdk-0.1.5/setup.py
```

### Comparing `auto-sdk-0.1.4/auto_identity/__init__.py` & `auto-sdk-0.1.5/auto_identity/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,26 +14,27 @@
     pem_to_private_key,
     load_private_key,
     pem_to_public_key,
     load_public_key,
     save_key)
 from .certificate_manager import CertificateManager
 from .registry import Registry
-from .utils import der_encode_signature_algorithm_oid
+from .utils import der_encode_signature_algorithm_oid, blake2b_256
 
-__version__ = '0.1.4'
+__version__ = '0.1.5'
 
 __all__ = [
     "generate_rsa_key_pair",
     "generate_ed25519_key_pair",
     "key_to_hex",
     "load_private_key",
     "load_public_key",
     "save_key",
     "pem_to_private_key",
     "pem_to_public_key",
     "key_to_pem",
     "CertificateManager",
     "der_encode_signature_algorithm_oid",
+    "blake2b_256",
     "Registry",
     "Keypair",
 ]
```

### Comparing `auto-sdk-0.1.4/auto_identity/certificate_manager.py` & `auto-sdk-0.1.5/auto_identity/certificate_manager.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,185 +1,284 @@
 from datetime import datetime, timedelta, timezone
 from cryptography import x509
 from cryptography.x509.oid import NameOID
-from cryptography.hazmat.backends import default_backend
 from cryptography.hazmat.primitives import hashes, serialization
 from cryptography.hazmat.primitives.asymmetric import ed25519, rsa
 from .key_management import do_public_keys_match
+from .utils import blake2b_256
 
 
 class CertificateManager:
     """
     Certificate management class.
     """
 
     def __init__(self,  certificate=None, private_key=None):
         """
-        Initializes a certificate issuer.
+        Initializes a certificate manager.
 
         Args:
             certificate(Certificate): Certificate.
             private_key(PrivateKey): Private key.
         """
         self.private_key = private_key
         self.certificate = certificate
 
+    def _prepare_signing_params(self):
+        """
+        Prepares the signing parameters based on the key type.
+
+        Returns:
+            dict: Signing parameters.
+        """
+        private_key = self.private_key
+        if isinstance(private_key, ed25519.Ed25519PrivateKey):
+            return {"private_key": private_key, "algorithm": None}
+        if isinstance(private_key, rsa.RSAPrivateKey):
+            return {"private_key": private_key, "algorithm": hashes.SHA256()}
+
+        raise ValueError("Unsupported key type for signing.")
+
     @staticmethod
     def _to_common_name(subject_name):
         """
         Converts a subject name to a common name.
 
         Args:
             subject_name(str): Subject name for the certificate(common name).
 
         Returns:
             str: Common name.
         """
         return x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, subject_name)])
 
-    def _prepare_signing_params(self):
+    @staticmethod
+    def pretty_print_certificate(cert):
         """
-        Prepares the signing parameters based on the key type.
+        Prints the details of an X.509 Certificate in a readable format.
+
+        Args:
+            cert (x509.Certificate): The certificate to print.
+        """
+        print("Certificate:")
+        print("============")
+        print("Subject:", cert.subject.rfc4514_string())
+        print("Issuer:", cert.issuer.rfc4514_string())
+        print("Serial Number:", cert.serial_number)
+        print("Not Valid Before:", cert.not_valid_before_utc)
+        print("Not Valid After:", cert.not_valid_after_utc)
+
+        print("\nExtensions:")
+        for ext in cert.extensions:
+            print(
+                f" - {ext.oid._name if ext.oid._name else ext.oid.dotted_string}: {ext.value}")
+
+        # Optionally, print the public key details
+        print("\nPublic Key:")
+        print(cert.public_key().public_bytes(
+            encoding=serialization.Encoding.PEM,
+            format=serialization.PublicFormat.SubjectPublicKeyInfo
+        ).decode('utf-8'))
+
+    @staticmethod
+    def certificate_to_pem(certificate: x509.Certificate):
+        """
+        Converts an x509 certificate to PEM format.
 
         Returns:
-            dict: Signing parameters.
+            bytes: PEM encoded certificate.
         """
-        private_key = self.private_key
-        if isinstance(private_key, ed25519.Ed25519PrivateKey):
-            return {"private_key": private_key, "algorithm": None}
-        if isinstance(private_key, rsa.RSAPrivateKey):
-            return {"private_key": private_key, "algorithm": hashes.SHA256()}
+        return certificate.public_bytes(serialization.Encoding.PEM)
 
-        raise ValueError("Unsupported key type for signing.")
+    @staticmethod
+    def pem_to_certificate(pem_bytes: bytes) -> x509.Certificate:
+        """
+        Converts PEM bytes to an x509 Certificate object.
+
+        Args:
+            pem_bytes (bytes): The PEM-encoded certificate as bytes.
+
+        Returns:
+            An x509.Certificate object.
+        """
+        certificate = x509.load_pem_x509_certificate(pem_bytes)
+        return certificate
+
+    @staticmethod
+    def get_subject_common_name(subject: x509.Name):
+        """
+        Retrieves the common name from the subject of the certificate.
 
-    def create_csr(self, subject_name):
+        Args:
+            certificate(x509.Certificate): Certificate to retrieve the common name from .
+
+        Returns:
+            str: Common name of the certificate.
         """
-        Creates a Certificate Signing Request(CSR).
+        return subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
+
+    @staticmethod
+    def get_certificate_auto_id(certificate: x509.Certificate):
+        """
+        Retrieves the autoid from the certificate.
+
+        Args:
+            certificate(x509.Certificate): Certificate to retrieve the autoid from.
+
+        Returns:
+            str: Autoid of the certificate.
+        """
+        san = certificate.extensions.get_extension_for_oid(
+            x509.ExtensionOID.SUBJECT_ALTERNATIVE_NAME).value
+        for name in san:
+            if isinstance(name, x509.UniformResourceIdentifier) and name.value.startswith("autoid:auto:"):
+                return name.value.split(":")[-1]
+
+    @staticmethod
+    def create_csr(subject_name):
+        """
+        Creates an unsigned Certificate Signing Request(CSR).
 
         Args:
             subject_name(str): Subject name for the CSR(common name).
 
         Returns:
-            CertificateSigningRequest: Created X.509 CertificateSigningRequest.
+            CertificateSigningRequestBuilder: Created X.509 CertificateSigningRequestBuilder.
         """
-        signing_params = self._prepare_signing_params()
+        common_name = x509.Name(
+            [x509.NameAttribute(NameOID.COMMON_NAME, subject_name)])
+
         csr = x509.CertificateSigningRequestBuilder().subject_name(
-            x509.Name([x509.NameAttribute(NameOID.COMMON_NAME, subject_name)])
-        ).sign(**signing_params)
+            common_name)
 
         return csr
 
-    def issue_certificate(self, csr, validity_period_days=365):
+    def sign_csr(self, csr):
         """
-        Issues a certificate for Certificate Signing Request(CSR).
+        Signs a Certificate Signing Request(CSR).
 
         Args:
             csr(CertificateSigningRequest): Certificate Signing Request.
-            issuer_certificate(Certificate): Issuer certificate.
-            issuer_private_key(PrivateKey): Private key to sign the certificate with .
-            validity_period_days(int, optional): Number of days the certificate is valid. Defaults to 365.
 
         Returns:
-            Certificate: Created X.509 certificate.
+            CertificateSigningRequest: Created X.509 CertificateSigningRequest.
         """
-        if self.certificate is None:
-            raise ValueError("Certificate is not set.")
         if self.private_key is None:
             raise ValueError("Private key is not set.")
 
-        issuer_certificate = self.certificate
+        signing_params = self._prepare_signing_params()
 
-        # Verify that the public key derived from the private key matches the one in the issuer's certificate
-        if not do_public_keys_match(issuer_certificate.public_key(), self.private_key.public_key()):
-            raise ValueError(
-                "Issuer certificate public key does not match the private key used for signing.")
+        return csr.sign(**signing_params)
 
-        signing_params = self._prepare_signing_params()
+    def create_and_sign_csr(self, subject_name):
+        """
+        Creates and signs a Certificate Signing Request(CSR).
 
-        certificate = x509.CertificateBuilder().subject_name(
-            csr.subject,
-        ).issuer_name(
-            issuer_certificate.subject,
-        ).public_key(
-            csr.public_key(),
-        ).serial_number(
-            x509.random_serial_number(),
-        ).not_valid_before(
-            datetime.now(timezone.utc),
-        ).not_valid_after(
-            datetime.now(timezone.utc) + timedelta(days=validity_period_days),
-        ).sign(**signing_params)
+        Args:
+            subject_name(str): Subject name for the CSR(common name).
 
-        return certificate
+        Returns:
+            CertificateSigningRequest: Created X.509 CertificateSigningRequest.
+        """
+        csr = self.create_csr(subject_name)
+        return self.sign_csr(csr)
 
-    def self_issue_certificate(self, subject_name: str, validity_period_days=365):
+    def issue_certificate(self, csr: x509.CertificateSigningRequest, validity_period_days=365):
         """
-        Issues a self-signed certificate for the identity.
+        Issues a certificate for Certificate Signing Request(CSR).
 
         Args:
-            subject_name(str): Subject name for the certificate(common name).
-            private_key(PrivateKey): Private key to sign the certificate with .
+            csr(CertificateSigningRequest): Certificate Signing Request.
+            issuer_certificate(Certificate): Issuer certificate.
+            issuer_private_key(PrivateKey): Private key to sign the certificate with .
             validity_period_days(int, optional): Number of days the certificate is valid. Defaults to 365.
 
         Returns:
             Certificate: Created X.509 certificate.
         """
         if self.private_key is None:
             raise ValueError("Private key is not set.")
 
-        signing_params = self._prepare_signing_params()
-        common_name = self._to_common_name(subject_name)
-
-        certificate = x509.CertificateBuilder().subject_name(
-            common_name,
+        if self.certificate is None:
+            issuer_name = csr.subject
+            auto_id = blake2b_256(
+                self.get_subject_common_name(issuer_name).encode())
+        else:
+            if not do_public_keys_match(self.certificate.public_key(), self.private_key.public_key()):
+                raise ValueError(
+                    "Issuer certificate public key does not match the private key used for signing.")
+            issuer_name = self.certificate.subject
+            auto_id = blake2b_256((self.get_subject_common_name(
+                issuer_name)+self.get_subject_common_name(csr.subject)).encode())
+
+        # Prepare the certificate builder with information from the CSR
+        certificate_builder = x509.CertificateBuilder().subject_name(
+            csr.subject
         ).issuer_name(
-            common_name,
+            issuer_name
         ).public_key(
-            self.private_key.public_key(),
+            csr.public_key()
         ).serial_number(
-            x509.random_serial_number(),
+            x509.random_serial_number()
         ).not_valid_before(
-            datetime.now(timezone.utc),
+            datetime.utcnow()
         ).not_valid_after(
-            datetime.now(timezone.utc) + timedelta(days=validity_period_days),
-        ).sign(**signing_params)
+            datetime.utcnow() + timedelta(days=validity_period_days)
+        )
 
-        self.certificate = certificate
-        return certificate
+        auto_id_san = x509.UniformResourceIdentifier(
+            f"autoid:auto:{auto_id.hex()}")
+        san_extensions = [ext for ext in csr.extensions if isinstance(
+            ext.value, x509.SubjectAlternativeName)]
+        if san_extensions:
+            existing_san = san_extensions[0].value
+            new_san = existing_san.add(auto_id_san)
+            certificate_builder = certificate_builder.add_extension(
+                new_san, critical=False)
+        else:
+            certificate_builder = certificate_builder.add_extension(
+                x509.SubjectAlternativeName([auto_id_san]),
+                critical=False
+            )
+        # Copy all extensions from the CSR to the certificate
+        for extension in csr.extensions:
+            certificate_builder = certificate_builder.add_extension(
+                extension.value, extension.critical
+            )
 
-    @staticmethod
-    def certificate_to_pem(certificate: x509.Certificate):
-        """
-        Converts an x509 certificate to PEM format.
+        certificate = certificate_builder.sign(
+            **self._prepare_signing_params())
 
-        Returns:
-            bytes: PEM encoded certificate.
-        """
-        return certificate.public_bytes(serialization.Encoding.PEM)
+        return certificate
 
-    @staticmethod
-    def pem_to_certificate(pem_bytes: bytes) -> x509.Certificate:
+    def self_issue_certificate(self, subject_name: str, validity_period_days=365):
         """
-        Converts PEM bytes to an x509 Certificate object.
+        Issues a self-signed certificate for the identity.
 
         Args:
-            pem_bytes (bytes): The PEM-encoded certificate as bytes.
+            subject_name(str): Subject name for the certificate(common name).
+            private_key(PrivateKey): Private key to sign the certificate with .
+            validity_period_days(int, optional): Number of days the certificate is valid. Defaults to 365.
 
         Returns:
-            An x509.Certificate object.
+            Certificate: Created X.509 certificate.
         """
-        certificate = x509.load_pem_x509_certificate(
-            pem_bytes, default_backend())
+        if self.private_key is None:
+            raise ValueError("Private key is not set.")
+
+        csr = self.sign_csr(self.create_csr(subject_name))
+        certificate = self.issue_certificate(csr, validity_period_days)
+
+        self.certificate = certificate
         return certificate
 
-    @staticmethod
-    def get_subject_common_name(certificate: x509.Certificate):
+    def save_certificate(self, file_path: str):
         """
-        Retrieves the common name from the subject of the certificate.
+        Saves the certificate to a file.
 
         Args:
-            certificate(x509.Certificate): Certificate to retrieve the common name from .
-
-        Returns:
-            str: Common name of the certificate.
+            file_path (str): Path to the file where the certificate should be saved.
         """
-        return certificate.subject.get_attributes_for_oid(NameOID.COMMON_NAME)[0].value
+        certificate_data = self.certificate.public_bytes(
+            serialization.Encoding.PEM)
+        with open(file_path, "wb") as cert_file:
+            cert_file.write(certificate_data)
```

### Comparing `auto-sdk-0.1.4/auto_identity/key_management.py` & `auto-sdk-0.1.5/auto_identity/key_management.py`

 * *Files identical despite different names*

### Comparing `auto-sdk-0.1.4/auto_identity/registry.py` & `auto-sdk-0.1.5/auto_identity/registry.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,14 +1,19 @@
-from typing import Optional
+from typing import Optional, NamedTuple
 from cryptography import x509
 from cryptography.hazmat.primitives.asymmetric import ed25519
 from substrateinterface import ExtrinsicReceipt, Keypair, SubstrateInterface, exceptions
 from .utils import der_encode_signature_algorithm_oid
 
 
+class RegistrationResult(NamedTuple):
+    receipt: Optional[ExtrinsicReceipt]
+    identifier: Optional[int]
+
+
 class Registry():
     """
     Registry class for managing identities on Autonomys identity domains.
     """
 
     def __init__(self, rpc_url: str = "ws://127.0.0.1:9944", signer=None):
         """
@@ -47,24 +52,25 @@
         try:
             return self.registry.submit_extrinsic(extrinsic, wait_for_inclusion=True)
 
         except exceptions.SubstrateRequestException as e:
             print("Failed to send: {}".format(e))
             return None
 
-    def register_auto_id(self, certificate: x509.Certificate, issuer_id=None):
+    def register_auto_id(self, certificate: x509.Certificate, issuer_id=None) -> RegistrationResult:
         """
         Register a certificate in the registry.
 
         Args:            
             certificate (x509.Certificate): The certificate to register.
             issuer_id: The issuer ID. If None, the ID will be self-issued.
 
         Returns:
-            Optional[ExtrinsicReceipt]: The receipt of the extrinsic if successful, None otherwise.
+            RegistrationResult: A named tuple containing the receipt of the extrinsic and the identifier if successful,
+                                or None for both fields if unsuccessful.
         """
 
         base_certificate = {
             "certificate": certificate.tbs_certificate_bytes,
             "signature_algorithm": der_encode_signature_algorithm_oid(certificate.signature_algorithm_oid),
             "signature": certificate.signature,
         }
@@ -78,49 +84,16 @@
                 }
             }
 
         req = {"req": {"X509": certificate_param}}
 
         receipt = self._compose_call(
             call_function="register_auto_id", call_params=req)
-        return receipt
-
-    def get_auto_id(self, identifier):
-        """
-        Get an auto identity from the registry.
-
-        Args:
-            subject_name (str): The subject name of the certificate.
-
-        Returns:
-            The auto entity with the provided subject name.
-        """
-
-        result = self.registry.query('auto-id', 'AutoIds', [identifier])
-
-        if result is None:
-            return None
-
-        # TODO map result to AutoEntity type
-        auto_entity = result
-
-        return auto_entity
-
-    def verify(self, subject_name: str, public_key: ed25519.Ed25519PublicKey):
-        """
-        Verify a certificate from the registry.
-
-        Args:
-            subject_name (str): The subject name of the certificate.
-            public_key (ed25519.Ed25519PublicKey): The public key to verify.
-
-        Returns:
-            bool: True if the certificate is valid, False otherwise.
-        """
-        entity = self.get_auto_id(subject_name)
-
-        if entity is None:
-            return False
 
-        # TODO check public key and subject name match certificate, and that it is within the validity period
+        if receipt.is_success:
+            for event in receipt.triggered_events:
+                event_data = event['event'].serialize()
+                if event_data.get('event_id') == 'NewAutoIdRegistered':
+                    identifier = event_data['attributes']
+                    return RegistrationResult(receipt=receipt, identifier=identifier)
 
-        return True
+        return RegistrationResult(receipt=receipt, identifier=None)
```

### Comparing `auto-sdk-0.1.4/auto_identity/utils.py` & `auto-sdk-0.1.5/auto_identity/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from hashlib import blake2b
 from cryptography.x509.oid import ObjectIdentifier
 from pyasn1.type import namedtype, univ
 from pyasn1.codec.der.encoder import encode
 
 
 class AlgorithmIdentifier(univ.Sequence):
     """
@@ -31,7 +32,23 @@
     """
     algorithm_identifier = AlgorithmIdentifier()
     algorithm_identifier.setComponentByName('algorithm', oid.dotted_string)
     algorithm_identifier.setComponentByName('parameters', univ.Null())
 
     der_encoded_oid = encode(algorithm_identifier)
     return der_encoded_oid
+
+
+def blake2b_256(data: bytes) -> bytes:
+    """
+    Hashes the given data using BLAKE2b-256.
+
+    Args:
+        data (bytes): The data to be hashed.
+
+    Returns:
+        bytes: The BLAKE2b-256 hash of the data.
+
+    """
+    hasher = blake2b(data, digest_size=32)
+
+    return hasher.digest()
```

