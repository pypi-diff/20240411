# Comparing `tmp/dexus-vault-0.1.6.tar.gz` & `tmp/dexus-vault-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dexus-vault-0.1.6.tar", last modified: Fri Mar 29 15:21:54 2024, max compression
+gzip compressed data, was "dexus-vault-0.2.0.tar", last modified: Thu Apr 11 17:21:58 2024, max compression
```

## Comparing `dexus-vault-0.1.6.tar` & `dexus-vault-0.2.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7914 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.202425 dexus-vault-0.1.6/dexus_vault/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      819 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/__version__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.202425 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/dexus_vault/src/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/src/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6064 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/src/dex_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5456 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/src/vault_processor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/dexus_vault/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1575 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/client_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     3205 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/files.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)     1331 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      386 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/dexus_vault/utils/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/dexus_vault.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9002 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      803 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 15:21:54.000000 dexus-vault-0.1.6/dexus_vault.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 15:21:54.206425 dexus-vault-0.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-03-29 15:21:44.000000 dexus-vault-0.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8104 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      819 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7929 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19894 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.612589 dexus-vault-0.2.0/dexus_vault/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5923 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/dex_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6169 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/src/vault_processor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/dexus_vault/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/client_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3277 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1265 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      386 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/dexus_vault/utils/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/dexus_vault.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9192 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      803 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-11 17:21:58.000000 dexus-vault-0.2.0/dexus_vault.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 17:21:58.616590 dexus-vault-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1674 2024-04-11 17:21:53.000000 dexus-vault-0.2.0/setup.py
```

### Comparing `dexus-vault-0.1.6/LICENSE` & `dexus-vault-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/PKG-INFO` & `dexus-vault-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.1.6
+Version: 0.2.0
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -52,15 +52,18 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
+> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
+
 ### How it works
+
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
 
 The recommended installation method is using `pip`:
@@ -70,23 +73,25 @@
 ```
 
 Using `docker`:
 
 ```bash
 docker run ifurs/dexus-vault
 ```
+
 you can find docker image [here](https://github.com/ifurs/dexus-vault/docker/image)
 
 ## 📙 Usage
 
 if you've installed `dexus-vault` using `pip`, you can execute it with the following command:
 
 ```bash
 dexus-vault
 ```
+
 or like a python module:
 
 ```bash
 python3 -m dexus_vault
 ```
 
 This will initiate a process that synchronizes Dex clients with the secrets stored in Vault.
@@ -95,50 +100,51 @@
 
 Currently dexus-vault support only Environment variables.
 
 ### General
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| SYNC_INTERVAL | false | 60    | Interval in seconds, dexus_vault will refresh in |
-| LOG_LEVEL | false | INFO | Set log level(logging lib) |
-| METRICS_ENABLE | false | True | Enable prometheus metrics publisher |
-| METRICS_PORT | false | 8000 | Set Metrics port, reuire METRICS_ENABLE to be enabled |
-| INTERNAL_METRICS | false | False | Enable the built-in metrics for Python (not application-specific) |
+| SYNC_INTERVAL | - | 60    | Interval in seconds, dexus_vault will refresh in |
+| LOG_LEVEL | - | INFO | Set log level(logging lib) |
+| METRICS_ENABLE | - | True | Enable prometheus metrics publisher |
+| METRICS_PORT | - | 8000 | Set Metrics port, require METRICS_ENABLE to be enabled |
+| INTERNAL_METRICS | - | False | Enable the built-in metrics for Python (not application-specific) |
 
 ### Dex client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| DEX_GRPC_URL | false | 127.0.0.1:5557 | url, with your dex grpc |
-| CLIENT_CRT | false | - | path to Dex GRPC client certificate |
-| CLIENT_KEY | false | - | path to Dex GRPC client certificate key |
-| CA_CRT | false | - | path to Dex GRPC client certificate autority |
-| DEX_MAX_RETRIES | false | 20 | How many retries need to wait for Dex to be reacheble |
-| DEX_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| DEX_GRPC_URL | - | 127.0.0.1:5557 | url, with your dex grpc |
+| CLIENT_CRT | - | - | path to Dex GRPC client certificate |
+| CLIENT_KEY | - | - | path to Dex GRPC client certificate key |
+| CA_CRT | - | - | path to Dex GRPC client certificate authority |
+| DEX_MAX_RETRIES | - | 20 | How many retries need to wait for Dex to be reachable |
+| DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| VAULT_ADDR | false | http://127.0.0.1:8200 | vault adress |
-| VAULT_CLIENTS_PATH | true | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | false | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
-| VAULT_TOKEN | false | - | used to auth to Vault via token |
-| VAULT_CERT | false | - | Vault client certificate path |
-| VAULT_CERT_KEY | false | - | Vault client certificate key path |
-| VAULT_CERT_CA | false | - | Vault certficate authority path or bool, `false` - do not validate, `true` - validate with internal trustore |
-| VAULT_LDAP_USERNAME | false | - | LDAP username used to auth to Vault |
-| VAULT_LDAP_PASSWORD | false | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | false | - | bool value, used to identify to use APPROLE auth |
-| VAULT_APPROLE_ROLE_ID | false | - | Vault approle role id |
-| VAULT_APPROLE_SECRET_ID | false | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | false | - | Vault approle path, use it if agent mount approle file in other than default directory |
-| VAULT_MAX_RETRIES | false | 20 | How many retries need to mark Vault unreacheble |
-| VAULT_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
+| VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
+| VAULT_TOKEN | - | - | used to auth to Vault via token |
+| VAULT_CERT | - | - | Vault client certificate path |
+| VAULT_CERT_KEY | - | - | Vault client certificate key path |
+| VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
+| VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
+| VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
+| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
+| VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
+| VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
+| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
+| VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
 
 #### About Vault auth
 
@@ -150,16 +156,17 @@
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
-client_create{client_id="my-first-dex-client", status="ok"} 1.0
+client_create{status="ok"} 1.0
 ```
+
 for "status" could be values "ok" and "failed"
 
 > **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
@@ -172,39 +179,41 @@
   "name": "My First Client",
   "public": false,
   "redirect_uris": ["http://127.0.0.1:5000/callback"],
   "trusted_peers": ["my-second-client"]
 }
 ```
 
-In the Vault configuration, `id` and `secret` are mandatory fields. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
+In the Vault configuration, `secret` are mandatory field same as `id`, but if you don't specify id, dexus-vault will use secret name for client id. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
 
 For defining lists in `redirect_uris` and `trusted_peers`, there are two methods:
 
 1. Use a native JSON list, e.g., `["value1", "value2"]`. Note that this will disable the non-JSON view for that secret in the Vault UI.
 2. Use a string with commas as delimiters, e.g., `"value1,value2"`. However, this method is not recommended and may be deprecated in future versions.
 
 ## 💻 Local Testing
 
 The `docker/tests` directory houses a `docker-compose.yaml` file, designed to facilitate local testing by running both Vault and Dex. However, this configuration is not suitable for production environments.
 
 For more details, please see the [README](docker/tests/README.md).
 
 ## 📓 Other notes
-- This projects uses pre-commit: https://pre-commit.com/
+
+- This projects uses pre-commit: <https://pre-commit.com/>
 
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
 - [ ] Redesign metrics concept to make it more Prometheus friendly
 - [ ] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
-- [ ] Redisign dexus-vault to work like cli and accepts params
+- [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
+
 - [Hurlenko](https://github.com/hurlenko) for references copied from your repos
```

### Comparing `dexus-vault-0.1.6/README.md` & `dexus-vault-0.2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -24,15 +24,18 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
+> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
+
 ### How it works
+
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
 
 The recommended installation method is using `pip`:
@@ -42,23 +45,25 @@
 ```
 
 Using `docker`:
 
 ```bash
 docker run ifurs/dexus-vault
 ```
+
 you can find docker image [here](https://github.com/ifurs/dexus-vault/docker/image)
 
 ## 📙 Usage
 
 if you've installed `dexus-vault` using `pip`, you can execute it with the following command:
 
 ```bash
 dexus-vault
 ```
+
 or like a python module:
 
 ```bash
 python3 -m dexus_vault
 ```
 
 This will initiate a process that synchronizes Dex clients with the secrets stored in Vault.
@@ -67,50 +72,51 @@
 
 Currently dexus-vault support only Environment variables.
 
 ### General
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| SYNC_INTERVAL | false | 60    | Interval in seconds, dexus_vault will refresh in |
-| LOG_LEVEL | false | INFO | Set log level(logging lib) |
-| METRICS_ENABLE | false | True | Enable prometheus metrics publisher |
-| METRICS_PORT | false | 8000 | Set Metrics port, reuire METRICS_ENABLE to be enabled |
-| INTERNAL_METRICS | false | False | Enable the built-in metrics for Python (not application-specific) |
+| SYNC_INTERVAL | - | 60    | Interval in seconds, dexus_vault will refresh in |
+| LOG_LEVEL | - | INFO | Set log level(logging lib) |
+| METRICS_ENABLE | - | True | Enable prometheus metrics publisher |
+| METRICS_PORT | - | 8000 | Set Metrics port, require METRICS_ENABLE to be enabled |
+| INTERNAL_METRICS | - | False | Enable the built-in metrics for Python (not application-specific) |
 
 ### Dex client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| DEX_GRPC_URL | false | 127.0.0.1:5557 | url, with your dex grpc |
-| CLIENT_CRT | false | - | path to Dex GRPC client certificate |
-| CLIENT_KEY | false | - | path to Dex GRPC client certificate key |
-| CA_CRT | false | - | path to Dex GRPC client certificate autority |
-| DEX_MAX_RETRIES | false | 20 | How many retries need to wait for Dex to be reacheble |
-| DEX_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| DEX_GRPC_URL | - | 127.0.0.1:5557 | url, with your dex grpc |
+| CLIENT_CRT | - | - | path to Dex GRPC client certificate |
+| CLIENT_KEY | - | - | path to Dex GRPC client certificate key |
+| CA_CRT | - | - | path to Dex GRPC client certificate authority |
+| DEX_MAX_RETRIES | - | 20 | How many retries need to wait for Dex to be reachable |
+| DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| VAULT_ADDR | false | http://127.0.0.1:8200 | vault adress |
-| VAULT_CLIENTS_PATH | true | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | false | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
-| VAULT_TOKEN | false | - | used to auth to Vault via token |
-| VAULT_CERT | false | - | Vault client certificate path |
-| VAULT_CERT_KEY | false | - | Vault client certificate key path |
-| VAULT_CERT_CA | false | - | Vault certficate authority path or bool, `false` - do not validate, `true` - validate with internal trustore |
-| VAULT_LDAP_USERNAME | false | - | LDAP username used to auth to Vault |
-| VAULT_LDAP_PASSWORD | false | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | false | - | bool value, used to identify to use APPROLE auth |
-| VAULT_APPROLE_ROLE_ID | false | - | Vault approle role id |
-| VAULT_APPROLE_SECRET_ID | false | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | false | - | Vault approle path, use it if agent mount approle file in other than default directory |
-| VAULT_MAX_RETRIES | false | 20 | How many retries need to mark Vault unreacheble |
-| VAULT_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
+| VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
+| VAULT_TOKEN | - | - | used to auth to Vault via token |
+| VAULT_CERT | - | - | Vault client certificate path |
+| VAULT_CERT_KEY | - | - | Vault client certificate key path |
+| VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
+| VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
+| VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
+| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
+| VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
+| VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
+| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
+| VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
 
 #### About Vault auth
 
@@ -122,16 +128,17 @@
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
-client_create{client_id="my-first-dex-client", status="ok"} 1.0
+client_create{status="ok"} 1.0
 ```
+
 for "status" could be values "ok" and "failed"
 
 > **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
@@ -144,39 +151,41 @@
   "name": "My First Client",
   "public": false,
   "redirect_uris": ["http://127.0.0.1:5000/callback"],
   "trusted_peers": ["my-second-client"]
 }
 ```
 
-In the Vault configuration, `id` and `secret` are mandatory fields. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
+In the Vault configuration, `secret` are mandatory field same as `id`, but if you don't specify id, dexus-vault will use secret name for client id. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
 
 For defining lists in `redirect_uris` and `trusted_peers`, there are two methods:
 
 1. Use a native JSON list, e.g., `["value1", "value2"]`. Note that this will disable the non-JSON view for that secret in the Vault UI.
 2. Use a string with commas as delimiters, e.g., `"value1,value2"`. However, this method is not recommended and may be deprecated in future versions.
 
 ## 💻 Local Testing
 
 The `docker/tests` directory houses a `docker-compose.yaml` file, designed to facilitate local testing by running both Vault and Dex. However, this configuration is not suitable for production environments.
 
 For more details, please see the [README](docker/tests/README.md).
 
 ## 📓 Other notes
-- This projects uses pre-commit: https://pre-commit.com/
+
+- This projects uses pre-commit: <https://pre-commit.com/>
 
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
 - [ ] Redesign metrics concept to make it more Prometheus friendly
 - [ ] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
-- [ ] Redisign dexus-vault to work like cli and accepts params
+- [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
+
 - [Hurlenko](https://github.com/hurlenko) for references copied from your repos
```

### Comparing `dexus-vault-0.1.6/dexus_vault/__main__.py` & `dexus-vault-0.2.0/dexus_vault/__main__.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/dexus_vault/client.py` & `dexus-vault-0.2.0/dexus_vault/client.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/api_pb2.py` & `dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py` & `dexus-vault-0.2.0/dexus_vault/grpc_dexidp/dexidp/api_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/dexus_vault/src/dex_processor.py` & `dexus-vault-0.2.0/dexus_vault/src/dex_processor.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,15 +60,15 @@
                 logger.info(f"Dex server version {self.get_dex_version()}")
                 return True
             except Exception as error:
                 if _retry >= self.config["DEX_MAX_RETRIES"]:
                     raise RuntimeError(f"Could not connect to Dex gRPC server: {error}")
                 else:
                     _retry += 1
-                    logger.debug(f"Dex gRPC is unavalable, retying...")
+                    logger.debug(f"Dex gRPC is unavailable, retying...")
                     time.sleep(self.config["DEX_RETRY_WAIT"])
 
     def get_dex_version(self) -> dict:
         """
         Get Dex version
         """
         dex_request = pb2.VersionReq()
@@ -110,24 +110,22 @@
             request.client.public = client.get("public", 0)
             request.client.name = client.get("name", "")
             request.client.logo_url = client.get("logo_url", "")
 
             response = MessageToDict(DexStub(self.channel).CreateClient(request))
             if response.get("client", None) is not None:
                 client_id = response.get("client").get("id")
-                client_create_metric.labels(client_id=client_id, status="ok").inc()
+                client_create_metric.labels(status="ok").inc()
                 logger.info(f"Created new Dex client '{client_id}'")
                 return client_id
             else:
                 logger.warning(f"RESPONSE FROM GRPC: {response}")
 
         except Exception as error:
-            client_create_metric.labels(
-                client_id=client.get("id"), status="failed"
-            ).inc()
+            client_create_metric.labels(status="failed").inc()
             logger.error(f"Failed to create client {client.get('id')}")
             logger.error(f"RESPONSE FROM GRPC: {error}")
 
     def delete_dex_client(self, client_id: str) -> None:
         """
         Delete OIDC client in Dex
         """
@@ -136,23 +134,23 @@
             dex_request.id = client_id
 
             # Because of Dex implementation, this request returns None
             # Or simple dict {'notFound': True} so it need to be processed
             response = MessageToDict(DexStub(self.channel).DeleteClient(dex_request))
 
             if response.get("notFound", None) is not None:
-                client_delete_metric.labels(client_id=client_id, status="failed").inc()
+                client_delete_metric.labels(status="failed").inc()
                 logger.warning(f"Client '{client_id}' not found")
             else:
-                client_create_metric.labels(client_id=client_id, status="ok").inc()
+                client_create_metric.labels(status="ok").inc()
                 logger.info(f"client {client_id} was deleted")
         except Exception as error:
-            client_delete_metric.labels(client_id=client_id, status="failed").inc()
+            client_delete_metric.labels(status="failed").inc()
             logger.error(f"Failed to delete client {client_id}")
             logger.error(f"RESPONSE FROM GRPC: {error}")
 
     def __del__(self):
         """
-        Everytime DexClient object delets, this will close gRPC connection
+        Every time DexClient object deletes, this will close gRPC connection
         """
         self.dex_grpc_close_connection()
         logger.debug(f"Dex connection closed")
```

### Comparing `dexus-vault-0.1.6/dexus_vault/src/vault_processor.py` & `dexus-vault-0.2.0/dexus_vault/src/vault_processor.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,14 +17,15 @@
         self.config = config
         self.client = self.login_to_client()
 
     def _check_vault_status(self, client: object) -> None:
         """
         Function validates if Vault is up and running
         """
+
         for _ in range(self.config["VAULT_MAX_RETRIES"]):
             try:
                 response = client.sys.read_health_status(method="GET")
                 if isinstance(response, requests.Response):
                     status = response.json()
                 else:
                     status = response
@@ -39,28 +40,30 @@
                 logger.warning(f"Vault {self.config['VAULT_ADDR']} connection failed")
             time.sleep(self.config["VAULT_RETRY_WAIT"])
         logger.error(f"Vault {self.config['VAULT_ADDR']} unreachable, exiting...")
         sys.exit(1)
 
     def _check_if_vault_auth(self, client: object, auth_method: str) -> None:
         """
-        Function validates if we sucessfuly authentificated to Vault
+        Function validates if we successfully authenticated to Vault
         """
+
         if client.is_authenticated():
             logger.debug(
-                f"Authentificated to Vault {self.config['VAULT_ADDR']} via {auth_method} auth method"
+                f"Authenticated to Vault {self.config['VAULT_ADDR']} via {auth_method} auth method"
             )
+
         else:
             raise RuntimeError(
-                f"Failed to authentificate to Vault {self.config['VAULT_ADDR']} via {auth_method} auth method "
+                f"Failed to authenticate to Vault {self.config['VAULT_ADDR']} via {auth_method} auth method "
             )
 
     def login_to_client(self) -> object:
         """
-        Define auth method for Vault and authentificate
+        Define auth method for Vault and authenticate
         """
         client = hvac.Client(url=self.config["VAULT_ADDR"])
         self._check_vault_status(client)
 
         if self.config["VAULT_APPROLE"] is not None:
             auth_method = "approle"
             client.sys.enable_auth_method(
@@ -105,39 +108,64 @@
         self._check_if_vault_auth(client, auth_method)
         return client
 
     def vault_list_secrets(self) -> list:
         """
         List secrets from Vault by path
         """
-        response = self.client.secrets.kv.v2.list_secrets(
-            self.config["VAULT_CLIENTS_PATH"],
-            mount_point=self.config["VAULT_MOUNT_POINT"],
-        )
+
+        if self.config["VAULT_ENGINE"] == "v1":
+            response = self.client.secrets.kv.v1.list_secrets(
+                self.config["VAULT_CLIENTS_PATH"],
+                mount_point=self.config["VAULT_MOUNT_POINT"],
+            )
+
+        elif self.config["VAULT_ENGINE"] == "v2":
+            response = self.client.secrets.kv.v2.list_secrets(
+                self.config["VAULT_CLIENTS_PATH"],
+                mount_point=self.config["VAULT_MOUNT_POINT"],
+            )
+
         return response["data"]["keys"]
 
     def vault_read_secret(self, secret_path: str):
         """
         Read specified secret from Vault
         """
-        response = self.client.secrets.kv.read_secret_version(
-            path=f"{self.config['VAULT_CLIENTS_PATH']}/{secret_path}",
-            mount_point=self.config["VAULT_MOUNT_POINT"],
-        )
-        return response["data"]["data"]
+
+        if self.config["VAULT_ENGINE"] == "v1":
+            response = self.client.secrets.kv.v1.read_secret(
+                path=f"{self.config['VAULT_CLIENTS_PATH']}/{secret_path}",
+                mount_point=self.config["VAULT_MOUNT_POINT"],
+            )
+            return response["data"]
+
+        elif self.config["VAULT_ENGINE"] == "v2":
+            response = self.client.secrets.kv.read_secret_version(
+                path=f"{self.config['VAULT_CLIENTS_PATH']}/{secret_path}",
+                mount_point=self.config["VAULT_MOUNT_POINT"],
+            )
+            return response["data"]["data"]
+        return None
 
     def vault_read_secrets(self) -> list:
         """
         Combine list_secrets with read_secret
         """
         _client_config = []
+
         for secret in self.vault_list_secrets():
-            config = normalize_config(self.vault_read_secret(secret_path=secret))
+            config = normalize_config(
+                self.vault_read_secret(secret_path=secret), secret
+            )
+
             if config is not None:
                 _client_config.append(config)
-                vault_client_secret.labels(secret_name=secret, status="ok").inc()
+                vault_client_secret.labels(status="ok").inc()
+
             else:
                 logger.warning(
-                    f"Secret '{secret}' in Vault, missing 'id' and 'secret' keys, or have incorrect structure"
+                    f"Secret '{secret}' in Vault, missing 'secret' key, or have incorrect structure"
                 )
-                vault_client_secret.labels(secret_name=secret, status="failed").inc()
+                vault_client_secret.labels(status="failed").inc()
+
         return _client_config
```

### Comparing `dexus-vault-0.1.6/dexus_vault/utils/client_parser.py` & `dexus-vault-0.2.0/dexus_vault/utils/client_parser.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,15 @@
     "name",
     "logo_url",
 ]
 
 
 def parse_list(list_from_vault: str | list) -> list:
     """
-    Nativly Vault can't support lists in UI(except json view), omg Hashicop:)
+    Natively Vault can't support lists in UI(except json view), omg Hashicorp:)
     """
     if isinstance(list_from_vault, list):
         return list_from_vault
 
     if isinstance(list_from_vault, str):
         return list_from_vault.split(",")
     else:
@@ -34,26 +34,31 @@
     for key in _config_keys:
         if key in ["redirect_uris", "trusted_peers"]:
             config[key] = parse_list(config.get(key))
         config["public"] = parse_bool(config.get("public", False))
     return config
 
 
-def _camel_case_to_undercore(config: dict) -> dict:
+def _camel_case_to_underscore(config: dict) -> dict:
     """
-    Tranform camel case response from Dex GRPC
+    Transform camel case response from Dex GRPC
     """
     return {
         "".join(["_" + i.lower() if i.isupper() else i for i in key]).lstrip("_"): value
         for key, value in config.items()
     }
 
 
-def normalize_config(client_config: dict) -> dict | None:
-    """
-    Normilize Dex config to one standart.
-    I know, re is better, but I don't like it
-    """
+def normalize_config(
+    client_config: dict, vault_secret: str | None = None
+) -> dict | None:
+    """
+    Normalize Dex config to one standard.
+    """
+    if "id" not in client_config and vault_secret is not None:
+        # Set Vault secret name as client Id
+        client_config["id"] = vault_secret
+
     if {"id", "secret"}.issubset(client_config.keys()):
-        config = _camel_case_to_undercore(client_config)
+        config = _camel_case_to_underscore(client_config)
         return _fill_missing_keys(config)
     return None
```

### Comparing `dexus-vault-0.1.6/dexus_vault/utils/config.py` & `dexus-vault-0.2.0/dexus_vault/utils/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,15 +42,15 @@
     }
 
 
 def get_vault_config() -> Dict[str, Any]:
     """
     Get the configuration as a dictionary, with type-checked values.
     """
-    # TODO: Check if it realy need assignment
+    # TODO: Check if it really need assignment
     config = {
         "VAULT_ADDR": _get_config_value("VAULT_ADDR", str, "http://127.0.0.1:8200"),
         "VAULT_APPROLE": _get_config_value("VAULT_APPROLE", str),
         "VAULT_APPROLE_ROLE_ID": _get_config_value("VAULT_APPROLE_ROLE_ID", str),
         "VAULT_APPROLE_SECRET_ID": _get_config_value("VAULT_APPROLE_SECRET_ID", str),
         "VAULT_APPROLE_PATH": _get_config_value("VAULT_APPROLE_PATH", str),
         "VAULT_TOKEN": _get_config_value("VAULT_TOKEN", str),
@@ -63,9 +63,10 @@
         "VAULT_MAX_RETRIES": _get_config_value("VAULT_MAX_RETRIES", int, 20),
         "VAULT_RETRY_WAIT": _get_config_value("VAULT_RETRY_WAIT", int, 3),
         "VAULT_ALLOW_REDIRECT": _get_config_value("VAULT_ALLOW_REDIRECT", bool, False),
         "VAULT_NAMESPACE": _get_config_value("VAULT_NAMESPACE", str),
         "VAULT_PROXIES": _get_config_value("VAULT_PROXIES", dict),
         "VAULT_MOUNT_POINT": _get_config_value("VAULT_MOUNT_POINT", str),
         "VAULT_CLIENTS_PATH": _get_config_value("VAULT_CLIENTS_PATH", str),
+        "VAULT_ENGINE": _get_config_value("VAULT_ENGINE", str, "v2"),
     }
     return config
```

### Comparing `dexus-vault-0.1.6/dexus_vault/utils/logger.py` & `dexus-vault-0.2.0/dexus_vault/utils/logger.py`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/dexus_vault/utils/metrics.py` & `dexus-vault-0.2.0/dexus_vault/utils/metrics.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,26 @@
 from prometheus_client import (
     start_http_server,
     Counter,
-    Summary,
     REGISTRY,
     PROCESS_COLLECTOR,
     PLATFORM_COLLECTOR,
 )
 from dexus_vault.utils.logger import logger
 
 """
 Define the Prometheus metrics and start the metrics server.
 """
 
-client_create_metric = Counter(
-    "client_create", "Client creation status", ["client_id", "status"]
-)
-client_delete_metric = Counter(
-    "client_delete", "Client deletion status", ["client_id", "status"]
-)
+client_create_metric = Counter("client_create", "Client creation status", ["status"])
+client_delete_metric = Counter("client_delete", "Client deletion status", ["status"])
 vault_client_secret = Counter(
     "vault_client_secret",
     "Number of wrong client specifications in Vault",
-    ["secret_name", "status"],
+    ["status"],
 )
 # SYNC_TIME = Summary("sync_time_seconds", "Time spent on synchronization")
 
 
 def start_metrics_server(
     disable_internal_metrics: bool, start_server: bool, port: int
 ) -> None:
```

### Comparing `dexus-vault-0.1.6/dexus_vault.egg-info/PKG-INFO` & `dexus-vault-0.2.0/dexus_vault.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dexus-vault
-Version: 0.1.6
+Version: 0.2.0
 Summary: Synchronizer of Dex clients with secrets in Vault
 Home-page: https://github.com/ifurs/dexus-vault
 Author: ifurs
 License: Apache License 2.0
 Project-URL: Source, https://github.com/ifurs/dexus-vault
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
@@ -52,15 +52,18 @@
 - [Thanks](#-thanks)
 
 ## 🚀 About the project
 
 Dexus Vault is utility designed to synchronize Dex client configurations with secrets stored in Hashicorp Vault.
 This tool simplifies the management of Dex clients by automating the process of keeping them in sync with Vault secrets.
 
+> As of the current release, dexus_vault is compatible only with version 2 of the Vault secrets engine.
+
 ### How it works
+
 When you execute `dexus-vault`, it establishes a connection to the specified Vault using the `hvac` library and retrieves secrets from the provided path. Following this, `dexus-vault` connects to Dex IdP via gRPC and creates or updates clients.
 
 > Please note that Dex does not currently support a native "Update" method. As a workaround, `dexus_vault` will recreate the client. Be aware of this behavior when using the tool.
 
 ## 💾 Installation
 
 The recommended installation method is using `pip`:
@@ -70,23 +73,25 @@
 ```
 
 Using `docker`:
 
 ```bash
 docker run ifurs/dexus-vault
 ```
+
 you can find docker image [here](https://github.com/ifurs/dexus-vault/docker/image)
 
 ## 📙 Usage
 
 if you've installed `dexus-vault` using `pip`, you can execute it with the following command:
 
 ```bash
 dexus-vault
 ```
+
 or like a python module:
 
 ```bash
 python3 -m dexus_vault
 ```
 
 This will initiate a process that synchronizes Dex clients with the secrets stored in Vault.
@@ -95,50 +100,51 @@
 
 Currently dexus-vault support only Environment variables.
 
 ### General
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| SYNC_INTERVAL | false | 60    | Interval in seconds, dexus_vault will refresh in |
-| LOG_LEVEL | false | INFO | Set log level(logging lib) |
-| METRICS_ENABLE | false | True | Enable prometheus metrics publisher |
-| METRICS_PORT | false | 8000 | Set Metrics port, reuire METRICS_ENABLE to be enabled |
-| INTERNAL_METRICS | false | False | Enable the built-in metrics for Python (not application-specific) |
+| SYNC_INTERVAL | - | 60    | Interval in seconds, dexus_vault will refresh in |
+| LOG_LEVEL | - | INFO | Set log level(logging lib) |
+| METRICS_ENABLE | - | True | Enable prometheus metrics publisher |
+| METRICS_PORT | - | 8000 | Set Metrics port, require METRICS_ENABLE to be enabled |
+| INTERNAL_METRICS | - | False | Enable the built-in metrics for Python (not application-specific) |
 
 ### Dex client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| DEX_GRPC_URL | false | 127.0.0.1:5557 | url, with your dex grpc |
-| CLIENT_CRT | false | - | path to Dex GRPC client certificate |
-| CLIENT_KEY | false | - | path to Dex GRPC client certificate key |
-| CA_CRT | false | - | path to Dex GRPC client certificate autority |
-| DEX_MAX_RETRIES | false | 20 | How many retries need to wait for Dex to be reacheble |
-| DEX_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| DEX_GRPC_URL | - | 127.0.0.1:5557 | url, with your dex grpc |
+| CLIENT_CRT | - | - | path to Dex GRPC client certificate |
+| CLIENT_KEY | - | - | path to Dex GRPC client certificate key |
+| CA_CRT | - | - | path to Dex GRPC client certificate authority |
+| DEX_MAX_RETRIES | - | 20 | How many retries need to wait for Dex to be reachable |
+| DEX_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 ### Vault client configuration
 
 | variable | required  | default | description |
 |:---------:|:---------:|:-------:|:------------:|
-| VAULT_ADDR | false | http://127.0.0.1:8200 | vault adress |
-| VAULT_CLIENTS_PATH | true | - | path in vault where clients could be found |
-| VAULT_MOUNT_POINT | false | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) |
-| VAULT_TOKEN | false | - | used to auth to Vault via token |
-| VAULT_CERT | false | - | Vault client certificate path |
-| VAULT_CERT_KEY | false | - | Vault client certificate key path |
-| VAULT_CERT_CA | false | - | Vault certficate authority path or bool, `false` - do not validate, `true` - validate with internal trustore |
-| VAULT_LDAP_USERNAME | false | - | LDAP username used to auth to Vault |
-| VAULT_LDAP_PASSWORD | false | - | LDAP password used to auth to Vault |
-| VAULT_APPROLE | false | - | bool value, used to identify to use APPROLE auth |
-| VAULT_APPROLE_ROLE_ID | false | - | Vault approle role id |
-| VAULT_APPROLE_SECRET_ID | false | - | Vault approle secret id |
-| VAULT_APPROLE_PATH | false | - | Vault approle path, use it if agent mount approle file in other than default directory |
-| VAULT_MAX_RETRIES | false | 20 | How many retries need to mark Vault unreacheble |
-| VAULT_RETRY_WAIT | false | 3 | How many seconds need to wait before next retry |
+| VAULT_CLIENTS_PATH | yes | - | path in vault where clients could be found |
+| VAULT_MOUNT_POINT | yes | - | vault [mount point](https://developer.hashicorp.com/vault/tutorials/enterprise/namespace-structure#understand-vault-s-mount-points) by default vault client uses "secret" |
+| VAULT_ENGINE | - | v2 | KV engine version, supported values v1 and v2 |
+| VAULT_ADDR | - | <http://127.0.0.1:8200> | vault address |
+| VAULT_TOKEN | - | - | used to auth to Vault via token |
+| VAULT_CERT | - | - | Vault client certificate path |
+| VAULT_CERT_KEY | - | - | Vault client certificate key path |
+| VAULT_CERT_CA | - | - | Vault certificate authority path or bool, `false` - do not validate, `true` - validate with internal truststore |
+| VAULT_LDAP_USERNAME | - | - | LDAP username used to auth to Vault |
+| VAULT_LDAP_PASSWORD | - | - | LDAP password used to auth to Vault |
+| VAULT_APPROLE | - | - | bool value, used to identify to use APPROLE auth |
+| VAULT_APPROLE_ROLE_ID | - | - | Vault approle role id |
+| VAULT_APPROLE_SECRET_ID | - | - | Vault approle secret id |
+| VAULT_APPROLE_PATH | - | - | Vault approle path, use it if agent mount approle file in other than default directory |
+| VAULT_MAX_RETRIES | - | 20 | How many retries need to mark Vault unreachable |
+| VAULT_RETRY_WAIT | - | 3 | How many seconds need to wait before next retry |
 
 #### About Dex auth
 
 If you don't specify certificates for Dex, the client will establish an insecure connection. Note that it's not necessary to use a certificate authority when you provide a client certificate and key.
 
 #### About Vault auth
 
@@ -150,16 +156,17 @@
 - AppRole authentication: To use this method, set `VAULT_APPROLE` to `true`. The HVAC client will then log into Vault using the default file mounted by the Vault agent by default, also there is possible to specify approle id and secret via env vars too.
 
 ### Metrics
 
 For now "dexus-vault" publish simplified metrics, like this:
 
 ```bash
-client_create{client_id="my-first-dex-client", status="ok"} 1.0
+client_create{status="ok"} 1.0
 ```
+
 for "status" could be values "ok" and "failed"
 
 > **NOTE:** We plan to redesign the metrics system in the near future. Any contributions to this effort are greatly appreciated.
 
 ## 🔒 Vault secret structure
 
 This example demonstrates all the parameters available for a client, which align with the Dex gRPC protocol message.
@@ -172,39 +179,41 @@
   "name": "My First Client",
   "public": false,
   "redirect_uris": ["http://127.0.0.1:5000/callback"],
   "trusted_peers": ["my-second-client"]
 }
 ```
 
-In the Vault configuration, `id` and `secret` are mandatory fields. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
+In the Vault configuration, `secret` are mandatory field same as `id`, but if you don't specify id, dexus-vault will use secret name for client id. The `public` field defaults to `False` at the `dexus_vault` level. If you wish to enable `public`, ensure that it is set as a boolean type in your Vault implementation, not as a string.
 
 For defining lists in `redirect_uris` and `trusted_peers`, there are two methods:
 
 1. Use a native JSON list, e.g., `["value1", "value2"]`. Note that this will disable the non-JSON view for that secret in the Vault UI.
 2. Use a string with commas as delimiters, e.g., `"value1,value2"`. However, this method is not recommended and may be deprecated in future versions.
 
 ## 💻 Local Testing
 
 The `docker/tests` directory houses a `docker-compose.yaml` file, designed to facilitate local testing by running both Vault and Dex. However, this configuration is not suitable for production environments.
 
 For more details, please see the [README](docker/tests/README.md).
 
 ## 📓 Other notes
-- This projects uses pre-commit: https://pre-commit.com/
+
+- This projects uses pre-commit: <https://pre-commit.com/>
 
 - All gRPC API methods dexus_vault use, defined in [api.proto](https://github.com/dexidp/dex/blob/v2.38.0/api/v2/api.proto)
 and compiled with `grpc_tools.protoc`
 
 ## Roadmap
 
 Plans for future:
 
 - [ ] Redesign metrics concept to make it more Prometheus friendly
 - [ ] Switch to pydantic
 - [ ] Implement functionality that tracks current clients state in Dex
 - [ ] Make logs more Fluent
-- [ ] Redisign dexus-vault to work like cli and accepts params
+- [ ] Redesign dexus-vault to work like cli and accepts params
 - [ ] Implement feature to use other storage options
 
 ## 🔥 Thanks
+
 - [Hurlenko](https://github.com/hurlenko) for references copied from your repos
```

### Comparing `dexus-vault-0.1.6/dexus_vault.egg-info/SOURCES.txt` & `dexus-vault-0.2.0/dexus_vault.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dexus-vault-0.1.6/setup.py` & `dexus-vault-0.2.0/setup.py`

 * *Files identical despite different names*

