# Comparing `tmp/sapysol-0.4.1.tar.gz` & `tmp/sapysol-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sapysol-0.4.1.tar", max compression
+gzip compressed data, was "sapysol-0.5.0.tar", max compression
```

## Comparing `sapysol-0.4.1.tar` & `sapysol-0.5.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.4.1/LICENSE
--rw-r--r--   0        0        0     4644 2024-04-08 12:29:18.740757 sapysol-0.4.1/README.md
--rw-r--r--   0        0        0      529 2024-04-08 19:05:00.614073 sapysol-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     2690 2024-04-08 12:49:12.656562 sapysol-0.4.1/sapysol/__init__.py
--rw-r--r--   0        0        0     9019 2024-04-08 12:48:28.490259 sapysol-0.4.1/sapysol/helpers.py
--rw-r--r--   0        0        0     7970 2024-04-08 07:21:58.647655 sapysol-0.4.1/sapysol/ix.py
--rw-r--r--   0        0        0     5921 2024-04-08 07:30:51.470374 sapysol-0.4.1/sapysol/jupag.py
--rw-r--r--   0        0        0     4775 2024-04-04 22:25:05.883961 sapysol-0.4.1/sapysol/snippets/batcher.py
--rw-r--r--   0        0        0     4668 2024-04-08 07:29:48.650854 sapysol-0.4.1/sapysol/snippets/token_selloff.py
--rw-r--r--   0        0        0     4454 2024-04-05 20:16:05.330344 sapysol-0.4.1/sapysol/snippets/wallets_balance.py
--rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.4.1/sapysol/sysvar/clock.py
--rw-r--r--   0        0        0     7102 2024-04-06 18:57:26.944570 sapysol-0.4.1/sapysol/token.py
--rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.4.1/sapysol/tokenMetadata2022.py
--rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.4.1/sapysol/tokenMetadataMetaplex.py
--rw-r--r--   0        0        0     7233 2024-04-05 20:08:23.397989 sapysol-0.4.1/sapysol/token_cache.py
--rw-r--r--   0        0        0    13796 2024-04-06 18:47:21.503484 sapysol-0.4.1/sapysol/tx.py
--rw-r--r--   0        0        0     4963 2024-04-08 07:29:31.640984 sapysol-0.4.1/sapysol/wallet.py
--rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 sapysol-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0     1080 2024-04-01 16:52:51.371732 sapysol-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4644 2024-04-09 17:19:46.025088 sapysol-0.5.0/README.md
+-rw-r--r--   0        0        0      529 2024-04-08 19:05:51.383703 sapysol-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     2744 2024-04-10 22:59:19.237955 sapysol-0.5.0/sapysol/__init__.py
+-rw-r--r--   0        0        0     9019 2024-04-08 12:48:28.490259 sapysol-0.5.0/sapysol/helpers.py
+-rw-r--r--   0        0        0     8082 2024-04-10 22:59:41.907791 sapysol-0.5.0/sapysol/ix.py
+-rw-r--r--   0        0        0     5921 2024-04-08 07:30:51.470374 sapysol-0.5.0/sapysol/jupag.py
+-rw-r--r--   0        0        0     4775 2024-04-04 22:25:05.883961 sapysol-0.5.0/sapysol/snippets/batcher.py
+-rw-r--r--   0        0        0     4668 2024-04-08 07:29:48.650854 sapysol-0.5.0/sapysol/snippets/token_selloff.py
+-rw-r--r--   0        0        0     4454 2024-04-05 20:16:05.330344 sapysol-0.5.0/sapysol/snippets/wallets_balance.py
+-rw-r--r--   0        0        0     3949 2024-04-08 10:17:13.391023 sapysol-0.5.0/sapysol/sysvar/clock.py
+-rw-r--r--   0        0        0     7102 2024-04-06 18:57:26.944570 sapysol-0.5.0/sapysol/token.py
+-rw-r--r--   0        0        0      847 2024-04-02 11:13:18.066218 sapysol-0.5.0/sapysol/tokenMetadata2022.py
+-rw-r--r--   0        0        0      845 2024-03-21 11:53:44.681342 sapysol-0.5.0/sapysol/tokenMetadataMetaplex.py
+-rw-r--r--   0        0        0     7233 2024-04-05 20:08:23.397989 sapysol-0.5.0/sapysol/token_cache.py
+-rw-r--r--   0        0        0    13796 2024-04-06 18:47:21.503484 sapysol-0.5.0/sapysol/tx.py
+-rw-r--r--   0        0        0     4963 2024-04-08 07:29:31.640984 sapysol-0.5.0/sapysol/wallet.py
+-rw-r--r--   0        0        0     5578 1970-01-01 00:00:00.000000 sapysol-0.5.0/PKG-INFO
```

### Comparing `sapysol-0.4.1/LICENSE` & `sapysol-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/README.md` & `sapysol-0.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Installation
 
 ```sh
 pip install sapysol
 ```
 
-Note: Requires Python >= 3.11.
+Note: Requires Python >= 3.10.
 
 # Usage
 
 `sapysol` uses `Client` instead of `AsyncClient` for few reasons:
 * First - without `async` you can put more logic to Python constructors and other non-async functions;
 * Second - what is the point of `async` if you really use `await` in 100% of cases?
```

### Comparing `sapysol-0.4.1/pyproject.toml` & `sapysol-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sapysol"
-version = "0.4.1"
+version = "0.5.0"
 description = "SuperArmor's Solana Python wrapper."
 authors = ["Anton Platonov <anton@platonov.io>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sapysol-0.4.1/sapysol/__init__.py` & `sapysol-0.5.0/sapysol/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                             GetPubkeysFromKeypairs, \
                             FetchAccount,           \
                             FetchAccounts,          \
                             DivmodJsBignumber
 
 from sapysol.ix import AtaInstruction,              \
                        GetAta,                      \
+                       CreateAtaIx,                 \
                        GetOrCreateAtaIx,            \
                        GetTransferTokenIxInternal,  \
                        GetTransferTokenIx,          \
                        WrapSolInstructions,         \
                        UnwrapSolInstruction,        \
                        ComputeBudgetIx,             \
                        ComputePriceIx
```

### Comparing `sapysol-0.4.1/sapysol/helpers.py` & `sapysol-0.5.0/sapysol/helpers.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/ix.py` & `sapysol-0.5.0/sapysol/ix.py`

 * *Files 12% similar despite different names*

```diff
@@ -37,35 +37,30 @@
 class AtaInstruction(NamedTuple):
     pubkey: Pubkey
     ix:     Instruction = None
 
 def GetAta(tokenMint: SapysolPubkey, owner: SapysolPubkey) -> Pubkey:
     return get_associated_token_address(owner=MakePubkey(owner), mint=MakePubkey(tokenMint))
 
+def CreateAtaIx(tokenMint: SapysolPubkey, owner: SapysolPubkey, payer: SapysolPubkey) -> Pubkey:
+    return create_associated_token_account(payer=MakePubkey(payer), owner=MakePubkey(owner), mint=MakePubkey(tokenMint))
+
 def GetOrCreateAtaIx(connection: Client,
                      tokenMint:  SapysolPubkey,
                      owner:      SapysolPubkey,
                      payer:      SapysolPubkey = None,
                      allowOwnerOffCurve: bool = True) -> AtaInstruction:
 
-    _tokenMint = MakePubkey(tokenMint)
-    _owner     = MakePubkey(owner)
-    _payer     = MakePubkey(payer)
-    _ix        = None
-
     if allowOwnerOffCurve == False and not owner.is_on_curve():
         raise("GetOrCreateATAInstruction(): allowOwnerOffCurve = False, but `owner` is off curve address!")
 
-    if _payer is None:
-        _payer = _owner
     ataAddress = GetAta(owner=owner, tokenMint=tokenMint)
     account    = connection.get_account_info(ataAddress)
-    if account.value is None:
-        _ix = create_associated_token_account(payer=_payer, owner=_owner, mint=_tokenMint)
-    return AtaInstruction(pubkey=ataAddress, ix=_ix)
+    return AtaInstruction(pubkey = ataAddress,
+                          ix     = None if account.value is not None else CreateAtaIx(payer=payer if payer else owner, owner=owner, tokenMint=tokenMint))
 
 # ===============================================================================
 # `transfer` is deprecated, using `transfer_checked`.
 # Transfering SPL tokens takes 114 bytes per instruction.
 # If the same sender address is used, each next transfer takes 50 bytes per instruction.
 # But also may vary, because it depends.
 #
@@ -117,45 +112,44 @@
                                             receiverAta    = get_associated_token_address(owner=MakePubkey(receiverWallet), mint=MakePubkey(tokenMint)),
                                             amountLamports = sendLamports)
     result.append(transferIx)
     return result
 
 # ===============================================================================
 #
-def WrapSolInstructions(source:   SapysolPubkey,
-                        dest:     SapysolPubkey,
-                        lamports: int) -> List[Instruction]:
-
-    _source = MakePubkey(source) # preserve original `source`
-    _dest   = MakePubkey(dest)   # preserve original `dest`
-    return [
-        transfer({
-            "from_pubkey": _source,
-            "to_pubkey":   _dest,
-            "lamports":    lamports
-        }),
-        sync_native(SyncNativeParams(program_id=TOKEN_PROGRAM_ID, account=_dest))
-    ]
+def WrapSolInstructions(connection: Client,
+                        lamports:   int,
+                        owner:      SapysolPubkey,
+                        payer:      SapysolPubkey = None) -> List[Instruction]:
+
+    wsolAta = GetOrCreateAtaIx(connection=connection, tokenMint=NATIVE_MINT, owner=owner, payer=payer)
+    ixList: List[Instruction] = []
+    if wsolAta.ix:
+        ixList.append(wsolAta.ix)
+    ixList.append(transfer({
+        "from_pubkey": MakePubkey(owner),
+        "to_pubkey":   wsolAta.pubkey,
+        "lamports":    lamports
+    }))
+    ixList.append(sync_native(SyncNativeParams(program_id=TOKEN_PROGRAM_ID, account=wsolAta.pubkey)))
+    return ixList
 
 # ===============================================================================
 # 
 def UnwrapSolInstruction(owner:              SapysolPubkey,
                          allowOwnerOffCurve: bool = True) -> Instruction:
 
-    _owner = MakePubkey(owner) # preserve original `owner`
-    if allowOwnerOffCurve == False and not _owner.is_on_curve():
+    if allowOwnerOffCurve == False and not MakePubkey(owner).is_on_curve():
         raise("UnwrapSolInstruction(): allowOwnerOffCurve = False, but `owner` is off curve address!")
 
-    WSolAtaAccount = get_associated_token_address(owner=_owner, mint=NATIVE_MINT)
-    if WSolAtaAccount:
-        return close_account(params=CloseAccountParams(program_id = TOKEN_PROGRAM_ID,
-                                                       account    = WSolAtaAccount,
-                                                       dest       = _owner,
-                                                       owner      = _owner))
-    return None
+    wsolAta = GetAta(tokenMint=NATIVE_MINT, owner=owner)
+    return close_account(params=CloseAccountParams(program_id = TOKEN_PROGRAM_ID,
+                                                   account    = wsolAta,
+                                                   dest       = MakePubkey(owner),
+                                                   owner      = MakePubkey(owner)))
 
 # ===============================================================================
 #
 def ComputeBudgetIx(units=1_400_000) -> Instruction:
     return set_compute_unit_limit(units=units)
 
 def ComputePriceIx(microLamports=1) -> Instruction:
```

### Comparing `sapysol-0.4.1/sapysol/jupag.py` & `sapysol-0.5.0/sapysol/jupag.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/snippets/batcher.py` & `sapysol-0.5.0/sapysol/snippets/batcher.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/snippets/token_selloff.py` & `sapysol-0.5.0/sapysol/snippets/token_selloff.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/snippets/wallets_balance.py` & `sapysol-0.5.0/sapysol/snippets/wallets_balance.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/sysvar/clock.py` & `sapysol-0.5.0/sapysol/sysvar/clock.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/token.py` & `sapysol-0.5.0/sapysol/token.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/tokenMetadata2022.py` & `sapysol-0.5.0/sapysol/tokenMetadata2022.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/tokenMetadataMetaplex.py` & `sapysol-0.5.0/sapysol/tokenMetadataMetaplex.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/token_cache.py` & `sapysol-0.5.0/sapysol/token_cache.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/tx.py` & `sapysol-0.5.0/sapysol/tx.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/sapysol/wallet.py` & `sapysol-0.5.0/sapysol/wallet.py`

 * *Files identical despite different names*

### Comparing `sapysol-0.4.1/PKG-INFO` & `sapysol-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sapysol
-Version: 0.4.1
+Version: 0.5.0
 Summary: SuperArmor's Solana Python wrapper.
 License: MIT
 Author: Anton Platonov
 Author-email: anton@platonov.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -36,15 +36,15 @@
 
 # Installation
 
 ```sh
 pip install sapysol
 ```
 
-Note: Requires Python >= 3.11.
+Note: Requires Python >= 3.10.
 
 # Usage
 
 `sapysol` uses `Client` instead of `AsyncClient` for few reasons:
 * First - without `async` you can put more logic to Python constructors and other non-async functions;
 * Second - what is the point of `async` if you really use `await` in 100% of cases?
```

