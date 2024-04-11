# Comparing `tmp/olas_operate_middleware-0.1.0rc2.tar.gz` & `tmp/olas_operate_middleware-0.1.0rc3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "olas_operate_middleware-0.1.0rc2.tar", max compression
+gzip compressed data, was "olas_operate_middleware-0.1.0rc3.tar", max compression
```

## Comparing `olas_operate_middleware-0.1.0rc2.tar` & `olas_operate_middleware-0.1.0rc3.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc2/LICENSE
--rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc2/README.md
--rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc2/operate/__init__.py
--rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc2/operate/account/__init__.py
--rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc2/operate/account/user.py
--rw-r--r--   0        0        0    17459 2024-04-05 14:54:43.349665 olas_operate_middleware-0.1.0rc2/operate/cli.py
--rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc2/operate/constants.py
--rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc2/operate/data/__init__.py
--rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc2/operate/data/contracts/__init__.py
--rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/__init__.py
--rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
--rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.py
--rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.yaml
--rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/__init__.py
--rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
--rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.py
--rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.yaml
--rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc2/operate/http/__init__.py
--rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc2/operate/http/exceptions.py
--rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc2/operate/keys.py
--rw-r--r--   0        0        0     2849 2024-04-05 14:54:43.350001 olas_operate_middleware-0.1.0rc2/operate/ledger/__init__.py
--rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc2/operate/ledger/base.py
--rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc2/operate/ledger/ethereum.py
--rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc2/operate/ledger/profiles.py
--rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc2/operate/ledger/solana.py
--rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc2/operate/resource.py
--rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc2/operate/services/__init__.py
--rw-r--r--   0        0        0    16022 2024-04-05 14:54:43.350907 olas_operate_middleware-0.1.0rc2/operate/services/manage.py
--rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc2/operate/services/protocol.py
--rw-r--r--   0        0        0    13179 2024-03-28 09:54:27.542688 olas_operate_middleware-0.1.0rc2/operate/services/service.py
--rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc2/operate/types.py
--rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc2/operate/utils/__init__.py
--rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc2/operate/utils/gnosis.py
--rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc2/operate/wallet/__init__.py
--rw-r--r--   0        0        0     8292 2024-04-05 14:54:43.354467 olas_operate_middleware-0.1.0rc2/operate/wallet/master.py
--rw-r--r--   0        0        0      803 2024-04-05 15:15:29.231331 olas_operate_middleware-0.1.0rc2/pyproject.toml
--rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11339 2024-02-06 05:22:56.471559 olas_operate_middleware-0.1.0rc3/LICENSE
+-rw-r--r--   0        0        0     4282 2024-03-05 05:48:41.164427 olas_operate_middleware-0.1.0rc3/README.md
+-rw-r--r--   0        0        0      803 2024-02-27 08:48:06.011840 olas_operate_middleware-0.1.0rc3/operate/__init__.py
+-rw-r--r--   0        0        0      804 2024-04-05 14:54:43.348635 olas_operate_middleware-0.1.0rc3/operate/account/__init__.py
+-rw-r--r--   0        0        0     2109 2024-04-05 14:54:43.349000 olas_operate_middleware-0.1.0rc3/operate/account/user.py
+-rw-r--r--   0        0        0    17481 2024-04-11 14:01:32.694321 olas_operate_middleware-0.1.0rc3/operate/cli.py
+-rw-r--r--   0        0        0     1091 2024-02-27 08:48:06.012404 olas_operate_middleware-0.1.0rc3/operate/constants.py
+-rw-r--r--   0        0        0      864 2024-03-08 10:47:59.399920 olas_operate_middleware-0.1.0rc3/operate/data/__init__.py
+-rw-r--r--   0        0        0      809 2024-02-27 08:48:06.013275 olas_operate_middleware-0.1.0rc3/operate/data/contracts/__init__.py
+-rw-r--r--   0        0        0      866 2024-02-27 08:48:06.013458 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/__init__.py
+-rw-r--r--   0        0        0    82730 2024-02-27 08:48:06.014051 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json
+-rw-r--r--   0        0        0     5847 2024-02-27 08:48:06.014506 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.py
+-rw-r--r--   0        0        0      724 2024-02-27 08:48:06.014716 olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.yaml
+-rw-r--r--   0        0        0      868 2024-02-28 14:31:11.754886 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/__init__.py
+-rw-r--r--   0        0        0    14169 2024-02-28 14:31:11.755175 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json
+-rw-r--r--   0        0        0     6985 2024-03-08 10:47:59.400374 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.py
+-rw-r--r--   0        0        0      741 2024-02-28 14:31:11.755543 olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.yaml
+-rw-r--r--   0        0        0     4646 2024-03-14 12:31:10.592254 olas_operate_middleware-0.1.0rc3/operate/http/__init__.py
+-rw-r--r--   0        0        0     1232 2024-02-27 08:48:06.014903 olas_operate_middleware-0.1.0rc3/operate/http/exceptions.py
+-rw-r--r--   0        0        0     2809 2024-03-27 11:16:42.979679 olas_operate_middleware-0.1.0rc3/operate/keys.py
+-rw-r--r--   0        0        0     2849 2024-04-05 14:54:43.350001 olas_operate_middleware-0.1.0rc3/operate/ledger/__init__.py
+-rw-r--r--   0        0        0     1154 2024-03-08 10:47:59.401479 olas_operate_middleware-0.1.0rc3/operate/ledger/base.py
+-rw-r--r--   0        0        0     1510 2024-03-08 10:47:59.401635 olas_operate_middleware-0.1.0rc3/operate/ledger/ethereum.py
+-rw-r--r--   0        0        0     1610 2024-03-08 10:47:59.401789 olas_operate_middleware-0.1.0rc3/operate/ledger/profiles.py
+-rw-r--r--   0        0        0     1199 2024-03-08 10:47:59.401953 olas_operate_middleware-0.1.0rc3/operate/ledger/solana.py
+-rw-r--r--   0        0        0     3880 2024-04-05 14:54:43.350296 olas_operate_middleware-0.1.0rc3/operate/resource.py
+-rw-r--r--   0        0        0      855 2024-03-27 11:16:42.980219 olas_operate_middleware-0.1.0rc3/operate/services/__init__.py
+-rw-r--r--   0        0        0    16425 2024-04-11 14:01:32.695097 olas_operate_middleware-0.1.0rc3/operate/services/manage.py
+-rw-r--r--   0        0        0    21677 2024-04-05 14:54:43.352503 olas_operate_middleware-0.1.0rc3/operate/services/protocol.py
+-rw-r--r--   0        0        0    13412 2024-04-11 14:01:32.695617 olas_operate_middleware-0.1.0rc3/operate/services/service.py
+-rw-r--r--   0        0        0     5357 2024-04-05 14:54:43.352823 olas_operate_middleware-0.1.0rc3/operate/types.py
+-rw-r--r--   0        0        0      808 2024-04-05 14:54:43.353285 olas_operate_middleware-0.1.0rc3/operate/utils/__init__.py
+-rw-r--r--   0        0        0     6082 2024-04-05 14:54:43.353744 olas_operate_middleware-0.1.0rc3/operate/utils/gnosis.py
+-rw-r--r--   0        0        0      813 2024-04-05 14:54:43.353950 olas_operate_middleware-0.1.0rc3/operate/wallet/__init__.py
+-rw-r--r--   0        0        0     8662 2024-04-11 14:01:32.695981 olas_operate_middleware-0.1.0rc3/operate/wallet/master.py
+-rw-r--r--   0        0        0      803 2024-04-11 14:03:40.857830 olas_operate_middleware-0.1.0rc3/pyproject.toml
+-rw-r--r--   0        0        0     5092 1970-01-01 00:00:00.000000 olas_operate_middleware-0.1.0rc3/PKG-INFO
```

### Comparing `olas_operate_middleware-0.1.0rc2/LICENSE` & `olas_operate_middleware-0.1.0rc3/LICENSE`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/README.md` & `olas_operate_middleware-0.1.0rc3/README.md`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/account/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/account/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/account/user.py` & `olas_operate_middleware-0.1.0rc3/operate/account/user.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/cli.py` & `olas_operate_middleware-0.1.0rc3/operate/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -432,29 +432,29 @@
         deployment = (
             operate.service_manager()
             .create_or_load(
                 request.path_params["service"],
             )
             .deployment
         )
-        deployment.build()
+        deployment.build(force=False)
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/start")
     @with_retries
     async def _start_service_locally(request: Request) -> JSONResponse:
         """Create a service."""
         deployment = (
             operate.service_manager()
             .create_or_load(
                 request.path_params["service"],
             )
             .deployment
         )
-        deployment.build()
+        deployment.build(force=False)
         operate.service_manager().fund_service(hash=request.path_params["service"])
         deployment.start()
         return JSONResponse(content=deployment.json)
 
     @app.post("/api/services/{service}/deployment/stop")
     @with_retries
     async def _stop_service_locally(request: Request) -> JSONResponse:
```

### Comparing `olas_operate_middleware-0.1.0rc2/operate/constants.py` & `olas_operate_middleware-0.1.0rc3/operate/constants.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/data/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/build/ServiceStakingToken.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.py` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/service_staking_token/contract.yaml` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/service_staking_token/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/build/IUniswapV2ERC20.json`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.py` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/data/contracts/uniswap_v2_erc20/contract.yaml` & `olas_operate_middleware-0.1.0rc3/operate/data/contracts/uniswap_v2_erc20/contract.yaml`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/http/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/http/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/http/exceptions.py` & `olas_operate_middleware-0.1.0rc3/operate/http/exceptions.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/keys.py` & `olas_operate_middleware-0.1.0rc3/operate/keys.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/ledger/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/ledger/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/ledger/base.py` & `olas_operate_middleware-0.1.0rc3/operate/ledger/base.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/ledger/ethereum.py` & `olas_operate_middleware-0.1.0rc3/operate/ledger/ethereum.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/ledger/profiles.py` & `olas_operate_middleware-0.1.0rc3/operate/ledger/profiles.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/ledger/solana.py` & `olas_operate_middleware-0.1.0rc3/operate/ledger/solana.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/resource.py` & `olas_operate_middleware-0.1.0rc3/operate/resource.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/services/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/services/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/services/manage.py` & `olas_operate_middleware-0.1.0rc3/operate/services/manage.py`

 * *Files 2% similar despite different names*

```diff
@@ -358,39 +358,45 @@
     def fund_service(self, hash: str) -> None:
         """Fund service if required."""
         service = self.create_or_load(hash=hash)
         wallet = self.wallet_manager.load(ledger_type=service.ledger_config.type)
         ledger_api = wallet.ledger_api(chain_type=service.ledger_config.chain)
         agent_fund_requirement = service.chain_data.user_params.fund_requirements.agent
 
-        self.logger.info("Funding agents")
         for key in service.keys:
             agent_balance = ledger_api.get_balance(address=key.address)
+            self.logger.info(f"Agent {key.address} balance: {agent_balance}")
+            self.logger.info(f"Required balance: {agent_fund_requirement}")
             if agent_balance < agent_fund_requirement:
+                self.logger.info("Funding agents")
                 to_transfer = agent_fund_requirement - agent_balance
                 self.logger.info(f"Transferring {to_transfer} units to {key.address}")
                 wallet.transfer(
                     to=key.address,
                     amount=to_transfer,
                     chain_type=service.ledger_config.chain,
                 )
 
-        self.logger.info("Funding safe")
+        safe_balanace = ledger_api.get_balance(service.chain_data.multisig)
         safe_fund_requirement = service.chain_data.user_params.fund_requirements.safe
-        safe_balanace = ledger_api.get_balance(wallet.safe)
+        self.logger.info(f"Safe {service.chain_data.multisig} balance: {safe_balanace}")
+        self.logger.info(f"Required balance: {safe_fund_requirement}")
         if safe_balanace < safe_fund_requirement:
+            self.logger.info("Funding safe")
             to_transfer = safe_fund_requirement - safe_balanace
-            self.logger.info(f"Transferring {to_transfer} units to {wallet.safe}")
+            self.logger.info(
+                f"Transferring {to_transfer} units to {service.chain_data.multisig}"
+            )
             wallet.transfer(
-                to=t.cast(str, wallet.safe),
+                to=t.cast(str, service.chain_data.multisig),
                 amount=to_transfer,
                 chain_type=service.ledger_config.chain,
             )
 
-    def deploy_service_locally(self, hash: str, force: bool = False) -> Deployment:
+    def deploy_service_locally(self, hash: str, force: bool = True) -> Deployment:
         """
         Deploy service locally
 
         :param hash: Service hash
         :param force: Remove previous deployment and start a new one.
         """
         deployment = self.create_or_load(hash=hash).deployment
```

### Comparing `olas_operate_middleware-0.1.0rc2/operate/services/protocol.py` & `olas_operate_middleware-0.1.0rc3/operate/services/protocol.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/services/service.py` & `olas_operate_middleware-0.1.0rc3/operate/services/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,24 +86,30 @@
         path.mkdir()
         try:
             os.chown(path, 1000, 1000)
         except (PermissionError, AttributeError):
             continue
 
 
-def remove_service_network(service_name: str) -> None:
+def remove_service_network(service_name: str, force: bool = True) -> None:
     """Remove service network cache."""
     client = from_env()
     network_names = (
         f"deployment_service_{service_name}_localnet",
         f"abci_build_service_{service_name}_localnet",
     )
-    for network in client.networks.list():
+    for network in client.networks.list(greedy=True):
         if network.attrs["Name"] not in network_names:
             continue
+
+        if force:
+            for container in network.attrs["Containers"]:
+                print(f"Killing {container}")
+                client.api.kill(container=container)
+
         print("Deleting network: " + network.attrs["Name"])
         client.api.remove_network(net_id=network.attrs["Id"])
 
 
 # TODO: Backport to autonomy
 class ServiceBuilder(BaseServiceBuilder):
     """Service builder patch."""
@@ -212,14 +218,15 @@
         :return: Deployment object
         """
         service = Service.load(path=self.path)
         # Remove network from cache if exists, this will raise an error
         # if the service is still running so we can do an early exit
         remove_service_network(
             service_name=service.helper.config.name,
+            force=force,
         )
 
         build = self.path / DEPLOYMENT
         if build.exists() and not force:
             return
         if build.exists() and force:
             shutil.rmtree(build)
```

### Comparing `olas_operate_middleware-0.1.0rc2/operate/types.py` & `olas_operate_middleware-0.1.0rc3/operate/types.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/utils/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/utils/gnosis.py` & `olas_operate_middleware-0.1.0rc3/operate/utils/gnosis.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/wallet/__init__.py` & `olas_operate_middleware-0.1.0rc3/operate/wallet/__init__.py`

 * *Files identical despite different names*

### Comparing `olas_operate_middleware-0.1.0rc2/operate/wallet/master.py` & `olas_operate_middleware-0.1.0rc3/operate/wallet/master.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 import json
 import typing as t
 from dataclasses import dataclass
 from pathlib import Path
 
 from aea.crypto.base import Crypto, LedgerApi
 from aea.crypto.registries import make_ledger_api
-from aea_ledger_ethereum.ethereum import EthereumCrypto
+from aea_ledger_ethereum.ethereum import EthereumApi, EthereumCrypto
+from autonomy.chain.config import ChainType as ChainProfile
+from autonomy.chain.tx import TxSettler
 from web3 import Account
 
 from operate.ledger import get_default_rpc
 from operate.resource import LocalResource
 from operate.types import ChainType, LedgerType
 from operate.utils.gnosis import create_safe as create_gnosis_safe
 
@@ -81,32 +83,15 @@
             self.ledger_type.name.lower(),
             address=(rpc or get_default_rpc(chain=chain_type)),
             chain_id=chain_type.id,
         )
 
     def transfer(self, to: str, amount: int, chain_type: ChainType) -> None:
         """Transfer funds to the given account."""
-        ledger_api = self.ledger_api(chain_type=chain_type)
-        tx = ledger_api.get_transfer_transaction(
-            sender_address=self.crypto.address,
-            destination_address=to,
-            amount=amount,
-            tx_fee=50000,
-            tx_nonce=ledger_api.generate_tx_nonce(
-                seller=self.crypto.address,
-                client=to,
-            ),
-        )
-        tx = ledger_api.update_with_gas_estimate(tx)
-        tx = self.crypto.sign_transaction(tx)
-        ledger_api.get_transaction_receipt(
-            tx_digest=ledger_api.send_signed_transaction(
-                tx_signed=tx,
-            )
-        )
+        raise NotImplementedError()
 
     @staticmethod
     def new(password: str, path: Path) -> t.Tuple["MasterWallet", t.List[str]]:
         """Create a new master wallet."""
         raise NotImplementedError()
 
     def create_safe(
@@ -131,21 +116,44 @@
     safe: t.Optional[str] = None
     safe_nonce: t.Optional[int] = None  # For cross-chain reusability
 
     _file = ledger_type.config_file
     _key = ledger_type.key_file
     _crypto_cls = EthereumCrypto
 
-    def get_crypto_obj(self, password: str) -> EthereumCrypto:
-        """Load ethereum crypto object."""
-        return EthereumCrypto(
-            private_key_path=self.path / self._key,
-            password=password,
+    def transfer(self, to: str, amount: int, chain_type: ChainType) -> None:
+        """Transfer funds to the given account."""
+        ledger_api = t.cast(EthereumApi, self.ledger_api(chain_type=chain_type))
+        tx_helper = TxSettler(
+            ledger_api=ledger_api,
+            crypto=self.crypto,
+            chain_type=ChainProfile.CUSTOM,
         )
 
+        def _build_tx(  # pylint: disable=unused-argument
+            *args: t.Any, **kwargs: t.Any
+        ) -> t.Dict:
+            """Build transaction"""
+            tx = ledger_api.get_transfer_transaction(
+                sender_address=self.crypto.address,
+                destination_address=to,
+                amount=amount,
+                tx_fee=50000,
+                tx_nonce="0x",
+                chain_id=chain_type.id,
+                raise_on_try=True,
+            )
+            return ledger_api.update_with_gas_estimate(
+                transaction=tx,
+                raise_on_try=True,
+            )
+
+        setattr(tx_helper, "build", _build_tx)  # noqa: B010
+        tx_helper.transact(lambda x: x, "", kwargs={})
+
     @classmethod
     def new(
         cls, password: str, path: Path
     ) -> t.Tuple["EthereumMasterWallet", t.List[str]]:
         """Create a new master wallet."""
         # Backport support on aea
         account = Account()
```

### Comparing `olas_operate_middleware-0.1.0rc2/pyproject.toml` & `olas_operate_middleware-0.1.0rc3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "olas-operate-middleware"
-version = "0.1.0-rc2"
+version = "0.1.0-rc3"
 description = ""
 authors = ["David Vilela <dvilelaf@gmail.com>", "Viraj Patel <vptl185@gmail.com>"]
 readme = "README.md"
 packages = [
     { include = "operate" }
 ]
 include = [
```

### Comparing `olas_operate_middleware-0.1.0rc2/PKG-INFO` & `olas_operate_middleware-0.1.0rc3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: olas-operate-middleware
-Version: 0.1.0rc2
+Version: 0.1.0rc3
 Summary: 
 Author: David Vilela
 Author-email: dvilelaf@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

