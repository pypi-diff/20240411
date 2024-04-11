# Comparing `tmp/authsign-0.4.0.tar.gz` & `tmp/authsign-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/authsign-0.4.0.tar", last modified: Sun May 15 20:52:09 2022, max compression
+gzip compressed data, was "authsign-0.5.1.tar", last modified: Thu Apr 11 17:16:26 2024, max compression
```

## Comparing `authsign-0.4.0.tar` & `authsign-0.5.1.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2022-05-15 20:52:09.355547 authsign-0.4.0/
--rw-r--r--   0 ilya       (501) staff       (20)     5574 2022-05-15 20:52:09.349010 authsign-0.4.0/PKG-INFO
--rw-r--r--   0 ilya       (501) staff       (20)     4930 2022-01-18 00:28:06.000000 authsign-0.4.0/README.md
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2022-05-15 20:52:09.347573 authsign-0.4.0/authsign/
--rw-r--r--   0 ilya       (501) staff       (20)       22 2022-05-15 20:51:50.000000 authsign-0.4.0/authsign/__init__.py
--rw-r--r--   0 ilya       (501) staff       (20)     4238 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/acme_signer.py
--rw-r--r--   0 ilya       (501) staff       (20)     4942 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/crypto.py
--rw-r--r--   0 ilya       (501) staff       (20)      626 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/log.py
--rw-r--r--   0 ilya       (501) staff       (20)     3000 2022-05-15 20:51:50.000000 authsign-0.4.0/authsign/main.py
--rw-r--r--   0 ilya       (501) staff       (20)      477 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/model.py
--rw-r--r--   0 ilya       (501) staff       (20)    10560 2022-05-15 20:51:50.000000 authsign-0.4.0/authsign/signer.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2022-05-15 20:52:09.348802 authsign-0.4.0/authsign/trusted/
--rw-r--r--   0 ilya       (501) staff       (20)        0 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/trusted/__init__.py
--rw-r--r--   0 ilya       (501) staff       (20)      596 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/trusted/roots.yaml
--rw-r--r--   0 ilya       (501) staff       (20)     5670 2022-01-18 00:28:06.000000 authsign-0.4.0/authsign/trusted/ts-chain.pem
--rw-r--r--   0 ilya       (501) staff       (20)     1167 2022-05-15 20:51:50.000000 authsign-0.4.0/authsign/utils.py
--rw-r--r--   0 ilya       (501) staff       (20)     5604 2022-05-15 20:51:50.000000 authsign-0.4.0/authsign/verifier.py
-drwxr-xr-x   0 ilya       (501) staff       (20)        0 2022-05-15 20:52:09.348349 authsign-0.4.0/authsign.egg-info/
--rw-r--r--   0 ilya       (501) staff       (20)     5574 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/PKG-INFO
--rw-r--r--   0 ilya       (501) staff       (20)      525 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/SOURCES.txt
--rw-r--r--   0 ilya       (501) staff       (20)        1 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/dependency_links.txt
--rw-r--r--   0 ilya       (501) staff       (20)       31 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/entry_points.txt
--rw-r--r--   0 ilya       (501) staff       (20)       62 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/requires.txt
--rw-r--r--   0 ilya       (501) staff       (20)        9 2022-05-15 20:52:09.000000 authsign-0.4.0/authsign.egg-info/top_level.txt
--rw-r--r--   0 ilya       (501) staff       (20)        1 2022-01-18 01:33:28.000000 authsign-0.4.0/authsign.egg-info/zip-safe
--rw-r--r--   0 ilya       (501) staff       (20)      757 2022-01-18 00:28:06.000000 authsign-0.4.0/log.json
--rw-r--r--   0 ilya       (501) staff       (20)       62 2022-01-18 00:28:06.000000 authsign-0.4.0/requirements.txt
--rw-r--r--   0 ilya       (501) staff       (20)       38 2022-05-15 20:52:09.355638 authsign-0.4.0/setup.cfg
--rw-r--r--   0 ilya       (501) staff       (20)     1472 2022-04-17 23:32:09.000000 authsign-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:26.712630 authsign-0.5.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-11 17:16:26.712630 authsign-0.5.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4930 2024-04-11 17:16:18.000000 authsign-0.5.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:26.708630 authsign-0.5.1/authsign/
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/acme_signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4942 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)      914 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3096 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11273 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/signer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:26.708630 authsign-0.5.1/authsign/trusted/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/trusted/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/trusted/roots.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     5670 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/trusted/ts-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5563 2024-04-11 17:16:18.000000 authsign-0.5.1/authsign/verifier.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:16:26.708630 authsign-0.5.1/authsign.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5574 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:16:26.000000 authsign-0.5.1/authsign.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      757 2024-04-11 17:16:18.000000 authsign-0.5.1/log.json
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 17:16:18.000000 authsign-0.5.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:16:26.712630 authsign-0.5.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-04-11 17:16:18.000000 authsign-0.5.1/setup.py
```

### Comparing `authsign-0.4.0/PKG-INFO` & `authsign-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authsign
-Version: 0.4.0
+Version: 0.5.1
 Summary: Authenticating Data Signing + Verification Server
 Home-page: https://github.com/webrecorder/authsign
 Author: Webrecorder Software
 Author-email: info@webrecorder.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `authsign-0.4.0/README.md` & `authsign-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/authsign/acme_signer.py` & `authsign-0.5.1/authsign/acme_signer.py`

 * *Files 5% similar despite different names*

```diff
@@ -81,14 +81,15 @@
             # Choosing challenge.
             # authz.body.challenges is a set of ChallengeBody objects.
             for i in authz.body.challenges:
                 # Find the supported challenge.
                 if isinstance(i.chall, challenges.HTTP01):
                     return i
 
+        # pylint: disable=broad-exception-raised
         raise Exception("HTTP-01 challenge was not offered by the CA server.")
 
     @contextmanager
     def challenge_server(self, http_01_resources):
         """Manage standalone server set up and shutdown."""
 
         servers = None
@@ -97,15 +98,16 @@
                 ("", self.port), http_01_resources
             )
             # Start client standalone web server.
             servers.serve_forever()
             yield servers
         finally:
             # Shutdown client web server and unbind from PORT
-            servers.shutdown_and_server_close()
+            if servers:
+                servers.shutdown_and_server_close()
 
     def perform_http01(self, client_acme, challb, orderr):
         """Set up standalone webserver and perform HTTP-01 challenge."""
 
         response, validation = challb.response_and_validation(client_acme.net.key)
 
         resource = standalone.HTTP01RequestHandler.HTTP01Resource(
```

### Comparing `authsign-0.4.0/authsign/crypto.py` & `authsign-0.5.1/authsign/crypto.py`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/authsign/log.py` & `authsign-0.5.1/authsign/log.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,32 +1,42 @@
+""" multicolored logging utils """
+
 import logging
 
 logger = logging.getLogger("authsign")
 
 RESET_SEQ = "\033[0m"
 COLOR_SEQ = "\033[1;%dm"
 CHECK = "\u2713"
 X = "\u2717"
 
 
+# pylint: disable=logging-not-lazy
+
+
 def log_assert(test, msg):
+    """log and raise assertion error"""
     if test:
         log_success(msg)
     else:
         log_failure(msg)
     assert test
 
 
 def log_message(text):
+    """log message in neutral color"""
     logger.info("  " + (COLOR_SEQ % 33) + text + RESET_SEQ)
 
 
 def log_success(text):
+    """log message in success color"""
     logger.info("  " + (COLOR_SEQ % 32) + CHECK + " " + text + RESET_SEQ)
 
 
 def log_failure(text):
+    """log message in failure color"""
     logger.info("  " + (COLOR_SEQ % 31) + X + " " + text + RESET_SEQ)
 
 
 def debug_error(text):
+    """log message at debugging level in failure color"""
     logger.debug("  " + (COLOR_SEQ % 31) + X + " " + text + RESET_SEQ)
```

### Comparing `authsign-0.4.0/authsign/main.py` & `authsign-0.5.1/authsign/main.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+""" main entrypoint for authsign web server """
+
 import asyncio
 import os
 import datetime
 
 from fastapi import FastAPI, HTTPException, Header
 
 from authsign.signer import Signer
@@ -17,15 +19,16 @@
 app = FastAPI()
 
 signer = None
 verifier = None
 
 
 @app.on_event("startup")
-async def startup_event():
+async def load_certs():
+    """load existing certs or request new ones if expired don't exist"""
     configfile = os.environ.get("CONFIG", "config.yaml")
 
     global signer
     log_message("Loading config from: " + configfile)
 
     config = load_yaml(configfile)
 
@@ -71,32 +74,33 @@
     log_message("Verifier Init...")
     verifier = Verifier(config.get("trusted_roots"), cert_duration, stamp_duration)
     log_message("")
 
 
 @app.post("/sign", response_model=SignedHash, response_model_exclude_none=True)
 async def sign_data(sign_req: SignReq, authorization: str = Header(None)):
+    """sign data api"""
     log_message("Signing Request...")
     if not signer.validate_token(authorization):
         log_failure("Invalid Auth Token")
         raise HTTPException(status_code=403, detail="Invalid auth token")
 
     try:
         return signer(sign_req)
     except Exception as e:
         raise HTTPException(status_code=400, detail=str(e))
 
 
 @app.post("/verify")
 async def verify_data(signed_hash: SignedHash):
+    """verify data api"""
     log_message("Verifying Signed Request...")
-    # result = await loop.run_in_executor(None, verifier, signed_hash)
-    # if result:
-    #    return result
+
     try:
         result = verifier(signed_hash)
         if result:
             return result
-    except Exception as e:
+    except Exception:
+        # not adding details for security
         pass
 
     raise HTTPException(status_code=400, detail="Not verified")
```

### Comparing `authsign-0.4.0/authsign/signer.py` & `authsign-0.5.1/authsign/signer.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 """
-Generate Cert and Pub Key via ACME
+Generate or load certs and handle signing
 """
+
 from pathlib import Path
 
 import datetime
 import base64
 import random
 import asyncio
+import traceback
 
 from pyasn1.codec.der import encoder
 import rfc3161ng
 
 
 from authsign import crypto, __version__
 
 from authsign.acme_signer import AcmeSigner
 
 from authsign.model import SignedHash
 from authsign.utils import (
     CERT_DURATION,
     STAMP_DURATION,
     YEARS,
-    parse_date,
-    is_time_range_valid,
+    no_older_then,
     open_file,
 )
 
 from authsign.log import log_assert, log_message, log_failure, log_success
 
 
 PASSPHRASE = b"passphrase"
 
 renewing = False
 
 
 # ============================================================================
+# pylint: disable=too-few-public-methods
 class Timestamper:
+    """handle rfc3161 timestamp signing"""
+
     def __init__(self, certfile=None, url=None):
         self.cert_pem = None
         with open_file(certfile, "rb") as fh_in:
             self.cert_pem = fh_in.read()
 
         self._timestamper = rfc3161ng.RemoteTimestamper(
             url, certificate=self.cert_pem, hashname="sha256"
         )
 
     def __call__(self, text):
+        """perform signing op"""
         tsr = self._timestamper(data=text.encode("ascii"), return_tsr=True)
 
         tst = tsr.time_stamp_token
 
         result = encoder.encode(tsr)
 
         return base64.b64encode(result), rfc3161ng.get_timestamp(tst)
 
 
 # ============================================================================
+# pylint: disable=too-many-instance-attributes,too-many-arguments
 class CertKeyPair:
     """Loads a cert + private key from PEM, extracts public key from cert"""
 
     def __init__(self):
         self.cert_pem = None
         self.cert = None
 
@@ -67,14 +73,16 @@
         self.public_key_pem = None
 
         self.private_key = None
 
     def load(
         self, name, certfile, private_key, passphrase=PASSPHRASE, duration=CERT_DURATION
     ):
+        """load existing keypair and certs from file system. load public key from cert"""
+
         log_message("{0}: Loading Cert: {1}".format(name, str(certfile)))
         with open(certfile, "rb") as fh_in:
             self.set_cert(fh_in.read())
 
         self.public_key = self.cert.public_key()
         self.public_key_pem = crypto.get_public_key_pem(self.public_key)
 
@@ -84,42 +92,45 @@
             self.private_key = crypto.load_private_key(data, passphrase)
 
         now = datetime.datetime.utcnow()
 
         log_assert(self.test_keys("Data Signature Test"), "Validating key pair")
 
         log_assert(
-            is_time_range_valid(self.cert.not_valid_before, now, duration)
+            self.cert.not_valid_before <= now <= self.cert.not_valid_before + duration
             and now <= self.cert.not_valid_after,
             "Validating cert still valid",
         )
 
         return self
 
     def init_new(self):
+        """init new key pair for signing"""
         self.private_key = crypto.create_ecdsa_private_key()
 
         self.public_key = self.private_key.public_key()
         self.public_key_pem = crypto.get_public_key_pem(self.public_key)
 
         return self
 
     def set_cert(self, cert_pem):
+        """init cert via pem"""
         self.cert_pem = cert_pem
         if isinstance(cert_pem, str):
             cert_pem = cert_pem.encode("ascii")
         self.cert = crypto.load_cert(cert_pem)
 
     def test_keys(self, data):
         """Test key pair sign/verify to ensure its valid"""
         signature = crypto.sign(data, self.private_key)
         return crypto.verify(data, signature, self.public_key)
 
 
 # ============================================================================
+# pylint: disable=too-many-arguments
 class Signer:
     """Signing cert, private, public key generator"""
 
     def __init__(
         self,
         domain=None,
         email=None,
@@ -178,19 +189,21 @@
         except AssertionError:
             log_message(
                 "Signing cert expired or not valid, creating new signing key + cert"
             )
             self.update_signing_key_and_cert()
 
         if not self.domain_signing:
+            # pylint: disable=broad-exception-raised
             raise Exception("Could not load domain signing cert + keys")
 
         self.timestampers = [Timestamper(**ts_data) for ts_data in timestamping]
 
     def validate_token(self, auth_header):
+        """validate the passed in auth header token"""
         if not self.auth_token:
             return True
 
         if not auth_header or not auth_header.startswith("bearer "):
             return False
 
         return auth_header.split(" ")[1] == self.auth_token
@@ -201,16 +214,14 @@
         self.domain_signing = CertKeyPair().load(
             "Domain Auth",
             self.rootpath / "cert.pem",
             self.rootpath / "private-key.pem",
             duration=self.cert_duration,
         )
 
-        self.set_next_update_time(self.domain_signing.cert)
-
         if self.csca_signing:
             cross_signing = CertKeyPair().load(
                 "Cross-Signing Cert",
                 self.rootpath / "cs-cert.pem",
                 self.rootpath / "private-key.pem",
                 duration=self.cert_duration,
             )
@@ -219,14 +230,15 @@
 
             log_assert(
                 cross_signing.public_key_pem == self.domain_signing.public_key_pem,
                 "Cross-Signing Cert Public Key == Domain Cert Public Key",
             )
 
     def set_next_update_time(self, cert):
+        """store the time for next cert renew"""
         next_update = cert.not_valid_before + self.cert_duration
         log_message(
             "Certificate will be used from {0} to {1}".format(
                 cert.not_valid_before, next_update
             )
         )
         next_update = (next_update - datetime.datetime.utcnow()).total_seconds()
@@ -264,14 +276,15 @@
         try:
             self.domain_signing.set_cert(signer.get_acme_cert(csr_pem))
 
             log_success("Obtained new domain cert for: " + self.domain)
         except Exception as e:
             log_failure("Unable to retrieve cert for: " + self.domain)
             log_failure("Reason: " + repr(e))
+            log_failure(traceback.format_exc())
             self.domain_signing = None
             return
 
         if self.csca_signing:
             now = datetime.datetime.utcnow()
 
             cs_cert = crypto.create_signed_cert(
@@ -289,35 +302,40 @@
     def __call__(self, sign_req):
         signature = crypto.sign(sign_req.hash, self.domain_signing.private_key)
 
         timestamper = random.choice(self.timestampers)
 
         time_signature, timestamp = timestamper(signature)
 
-        created_dt = parse_date(sign_req.created)
+        created = sign_req.created
 
-        if not is_time_range_valid(created_dt, timestamp, self.stamp_duration):
-            msg = "Created timestamp is out of range: Must be between {0} and {1}, but is {2}".format(
-                timestamp, timestamp + self.stamp_duration, created_dt
+        if not no_older_then(created, timestamp, self.stamp_duration):
+            msg = "Created timestamp is out of range: Must be between between {0} and {1}, but is {2}".format(
+                timestamp - self.stamp_duration, timestamp, created
             )
+            print(msg)
+            # pylint: disable=broad-exception-raised
             raise Exception(msg)
 
         return SignedHash(
             software="authsigner " + __version__,
             hash=sign_req.hash,
-            created=sign_req.created,
+            created=created,
             signature=signature,
             timeSignature=time_signature,
             domain=self.domain,
             domainCert=self.domain_signing.cert_pem,
             timestampCert=timestamper.cert_pem,
             crossSignedCert=self.cs_cert_pem,
         )
 
     async def renew_loop(self):
+        """sleep and run cert renew process in a loop"""
+        self.set_next_update_time(self.domain_signing.cert)
+
         log_message(
             "Signer: Renewing domain certificate in {0}".format(
                 datetime.timedelta(seconds=self.next_update)
             )
         )
         loop = asyncio.get_event_loop()
         await asyncio.sleep(self.next_update)
```

### Comparing `authsign-0.4.0/authsign/trusted/roots.yaml` & `authsign-0.5.1/authsign/trusted/roots.yaml`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/authsign/trusted/ts-chain.pem` & `authsign-0.5.1/authsign/trusted/ts-chain.pem`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/authsign/utils.py` & `authsign-0.5.1/authsign/utils.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,40 +1,54 @@
+""" shared utils """
+
 import datetime
 import importlib
 import contextlib
 
 import yaml
+import dateutil.parser
 
 # no limit on CA cert validity
 YEARS = datetime.timedelta(weeks=1000)
 
 CERT_DURATION = datetime.timedelta(days=7)
 
 STAMP_DURATION = datetime.timedelta(minutes=10)
 
 ISO_FORMAT = "%Y-%m-%dT%H:%M:%SZ"
 
 
-def is_time_range_valid(base, thedate, duration):
-    return base <= thedate and thedate - base <= duration
+def no_older_then(thedate, base, duration):
+    """ensure thedate is no older than duration from base date, and also not newer"""
+    if thedate > base:
+        return False
+
+    if thedate < base - duration:
+        return False
+
+    return True
 
 
 def parse_date(datestr):
-    try:
-        return datetime.datetime.strptime(datestr, ISO_FORMAT)
-    except:
-        return None
+    """parse date using dateutil"""
+    if isinstance(datestr, datetime.datetime):
+        return datestr
+
+    return dateutil.parser.parse(datestr, ignoretz=True)
 
 
 def format_date(date):
+    """format date to iso format"""
     return date.strftime(ISO_FORMAT)
 
 
 @contextlib.contextmanager
 def open_file(filename_or_resource, mode):
+    """open file from either package or file system"""
+    # pylint: disable=deprecated-method
     res = None
     if filename_or_resource.startswith("pkg://"):
         pkg, resource = filename_or_resource[6:].split("/", 1)
         if "b" in mode:
             res = importlib.resources.open_binary(pkg, resource)
         else:
             res = importlib.resources.open_text(pkg, resource)
@@ -43,11 +57,12 @@
 
     yield res
 
     res.close()
 
 
 def load_yaml(filename):
+    """load yaml and parse to dict"""
     with open_file(filename, "rt") as fh:
         data = yaml.load(fh.read(), Loader=yaml.SafeLoader)
 
     return data
```

### Comparing `authsign-0.4.0/authsign/verifier.py` & `authsign-0.5.1/authsign/verifier.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 """ Verify signed responses api"""
 
-
 import base64
 import traceback
 
 import rfc3161ng
 
 from authsign.utils import (
     CERT_DURATION,
     STAMP_DURATION,
-    is_time_range_valid,
-    parse_date,
+    no_older_then,
+    format_date,
     load_yaml,
 )
 from authsign import crypto
 from authsign.log import log_assert, log_message, debug_error
 from authsign.model import SignedHash
-from authsign.utils import format_date
 
 
 DEFAULT_TRUSTED_ROOTS = "pkg://authsign.trusted/roots.yaml"
 
 
 # ============================================================================
 class Verifier:
@@ -110,35 +108,37 @@
             domain_fingerprint = crypto.get_fingerprint(cert)
 
             log_assert(
                 domain == signed_req.domain,
                 f"Domain Cert Matches Expected: '{domain}' (sha-256 fingerprint: {domain_fingerprint})",
             )
 
-            created = parse_date(signed_req.created)
+            created = signed_req.created
             log_assert(created, "Parsed signature date")
 
             log_assert(
-                is_time_range_valid(cert.not_valid_before, created, self.cert_duration),
-                f"Verify WACZ creation date '{created}' - cert creation date '{cert.not_valid_before}' <= '{self.cert_duration}'",
+                cert.not_valid_before
+                <= created
+                <= cert.not_valid_before + self.cert_duration,
+                f"Verify creation date '{created}' - cert creation date '{cert.not_valid_before}' <= '{self.cert_duration}'",
             )
 
             timestamp = self.timestamp_verify(
                 signed_req.signature, signed_req.timeSignature, signed_req.timestampCert
             )
 
             log_assert(
                 timestamp,
                 "Verify timeSignature is a valid timestamp signature of\
  hash signature with timestamp certificate",
             )
 
             log_assert(
-                is_time_range_valid(created, timestamp, self.stamp_duration),
-                f"Verify signed timestamp time '{timestamp}' - WACZ creation date '{created}' <= '{self.stamp_duration}'",
+                no_older_then(created, timestamp, self.stamp_duration),
+                f"Verify created date '{created}' is no older than {self.stamp_duration}' from '{timestamp}'",
             )
 
             timestamp_certs = crypto.validate_cert_chain(
                 signed_req.timestampCert.encode("ascii")
             )
 
             log_assert(
```

### Comparing `authsign-0.4.0/authsign.egg-info/PKG-INFO` & `authsign-0.5.1/authsign.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authsign
-Version: 0.4.0
+Version: 0.5.1
 Summary: Authenticating Data Signing + Verification Server
 Home-page: https://github.com/webrecorder/authsign
 Author: Webrecorder Software
 Author-email: info@webrecorder.net
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `authsign-0.4.0/authsign.egg-info/SOURCES.txt` & `authsign-0.5.1/authsign.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/log.json` & `authsign-0.5.1/log.json`

 * *Files identical despite different names*

### Comparing `authsign-0.4.0/setup.py` & `authsign-0.5.1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     url="https://github.com/webrecorder/authsign",
     packages=find_packages(exclude=["tests"]),
     install_requires=[
         line.strip()
         for line in read("requirements.txt").splitlines()
         if not line.strip().startswith("#")
     ],
-    test_requires=["pytest", "pytest-asyncio"],
+    tests_require=["pytest", "pytest-asyncio"],
     zip_safe=True,
     package_data={"authsign.trusted": ["*"]},
     data_files={
         "requirements.txt": "requirements.txt",
         "log.json": "log.json",
     },
     entry_points="""
```

