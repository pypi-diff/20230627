# Comparing `tmp/huma_signals-0.4.1.tar.gz` & `tmp/huma_signals-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "huma_signals-0.4.1.tar", max compression
+gzip compressed data, was "huma_signals-0.5.0.tar", max compression
```

## Comparing `huma_signals-0.4.1.tar` & `huma_signals-0.5.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0    34523 2023-06-16 00:13:36.301640 huma_signals-0.4.1/LICENSE
--rw-r--r--   0        0        0     2162 2023-06-16 00:13:36.301640 huma_signals-0.4.1/README.md
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/__init__.py
--rw-r--r--   0        0        0      586 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/__init__.py
--rw-r--r--   0        0        0     3079 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/adapter.py
--rw-r--r--   0        0        0      186 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/settings.py
--rw-r--r--   0        0        0      586 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/README.md
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/__init__.py
--rw-r--r--   0        0        0    23699 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
--rw-r--r--   0        0        0    30632 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
--rw-r--r--   0        0        0    32155 2023-06-16 00:13:36.301640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
--rw-r--r--   0        0        0    30290 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
--rw-r--r--   0        0        0     4523 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/adapter.py
--rw-r--r--   0        0        0     1963 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/registry.py
--rw-r--r--   0        0        0      158 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/lending_pools/settings.py
--rw-r--r--   0        0        0      145 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/models.py
--rw-r--r--   0        0        0      591 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/README.md
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/__init__.py
--rw-r--r--   0        0        0     3191 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/adapter.py
--rw-r--r--   0        0        0      222 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/settings.py
--rw-r--r--   0        0        0      576 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/README.md
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/__init__.py
--rw-r--r--   0        0        0     4156 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/models.py
--rw-r--r--   0        0        0     5481 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/request_invoice_adapter.py
--rw-r--r--   0        0        0     4945 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/request_transaction_adapter.py
--rw-r--r--   0        0        0      283 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/request_network/settings.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/__init__.py
--rw-r--r--   0        0        0      237 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/settings.py
--rw-r--r--   0        0        0     4252 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_adapter.py
--rw-r--r--   0        0        0      491 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_models.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/__init__.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/__init__.py
--rw-r--r--   0        0        0     1427 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/eth_client.py
--rw-r--r--   0        0        0      662 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/eth_client/eth_types.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/__init__.py
--rw-r--r--   0        0        0     1503 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_client.py
--rw-r--r--   0        0        0      674 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_types.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/__init__.py
--rw-r--r--   0        0        0     8282 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/request_client.py
--rw-r--r--   0        0        0      978 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/clients/request_client/request_types.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/commons/__init__.py
--rw-r--r--   0        0        0     1324 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/commons/tokens.py
--rw-r--r--   0        0        0      499 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/dotenv/example.env
--rw-r--r--   0        0        0     1157 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/exceptions.py
--rw-r--r--   0        0        0      322 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/models.py
--rw-r--r--   0        0        0        0 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/py.typed
--rw-r--r--   0        0        0     1562 2023-06-16 00:13:36.305640 huma_signals-0.4.1/huma_signals/settings.py
--rw-r--r--   0        0        0     2814 2023-06-16 00:13:36.305640 huma_signals-0.4.1/pyproject.toml
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 huma_signals-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    34523 2023-06-27 16:58:02.134467 huma_signals-0.5.0/LICENSE
+-rw-r--r--   0        0        0     2162 2023-06-27 16:58:02.134467 huma_signals-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/__init__.py
+-rw-r--r--   0        0        0      586 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/__init__.py
+-rw-r--r--   0        0        0     3079 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/adapter.py
+-rw-r--r--   0        0        0      186 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/settings.py
+-rw-r--r--   0        0        0      586 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/__init__.py
+-rw-r--r--   0        0        0    23699 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json
+-rw-r--r--   0        0        0    30632 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json
+-rw-r--r--   0        0        0    32155 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json
+-rw-r--r--   0        0        0    30290 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json
+-rw-r--r--   0        0        0     4523 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/adapter.py
+-rw-r--r--   0        0        0     2302 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/registry.py
+-rw-r--r--   0        0        0      158 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/lending_pools/settings.py
+-rw-r--r--   0        0        0      145 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/models.py
+-rw-r--r--   0        0        0      591 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/__init__.py
+-rw-r--r--   0        0        0     3191 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/adapter.py
+-rw-r--r--   0        0        0      222 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/settings.py
+-rw-r--r--   0        0        0      576 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/README.md
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/__init__.py
+-rw-r--r--   0        0        0     4156 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/models.py
+-rw-r--r--   0        0        0     5481 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/request_invoice_adapter.py
+-rw-r--r--   0        0        0     4945 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/request_transaction_adapter.py
+-rw-r--r--   0        0        0      283 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/request_network/settings.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/superfluid/__init__.py
+-rw-r--r--   0        0        0      237 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/superfluid/settings.py
+-rw-r--r--   0        0        0     4252 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/superfluid/superfluid_adapter.py
+-rw-r--r--   0        0        0      491 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/adapters/superfluid/superfluid_models.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/eth_client/__init__.py
+-rw-r--r--   0        0        0     1427 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/eth_client/eth_client.py
+-rw-r--r--   0        0        0      662 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/eth_client/eth_types.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/polygon_client/__init__.py
+-rw-r--r--   0        0        0     1503 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/polygon_client/polygon_client.py
+-rw-r--r--   0        0        0      674 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/polygon_client/polygon_types.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/request_client/__init__.py
+-rw-r--r--   0        0        0     8282 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/request_client/request_client.py
+-rw-r--r--   0        0        0      978 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/clients/request_client/request_types.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/commons/__init__.py
+-rw-r--r--   0        0        0     1324 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/commons/tokens.py
+-rw-r--r--   0        0        0      499 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/dotenv/example.env
+-rw-r--r--   0        0        0     1157 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/exceptions.py
+-rw-r--r--   0        0        0      322 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/models.py
+-rw-r--r--   0        0        0        0 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/py.typed
+-rw-r--r--   0        0        0     1562 2023-06-27 16:58:02.134467 huma_signals-0.5.0/huma_signals/settings.py
+-rw-r--r--   0        0        0     2814 2023-06-27 16:58:02.134467 huma_signals-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 huma_signals-0.5.0/PKG-INFO
```

### Comparing `huma_signals-0.4.1/LICENSE` & `huma_signals-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/README.md` & `huma_signals-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/README.md` & `huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/ethereum_wallet/adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/ethereum_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/README.md` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/BaseCreditPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/BasePoolConfig.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/ReceivableFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/abi/SuperfluidFactoringPool.json`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/lending_pools/registry.py` & `huma_signals-0.5.0/huma_signals/adapters/lending_pools/registry.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,14 +32,25 @@
             pathlib.Path(__file__).parent.resolve()
             / "abi"
             / "ReceivableFactoringPool.json"
         ),
     ),
     PoolSetting(
         pool_address=web3.Web3.to_checksum_address(
+            "0x91bd14A985AD18f63E3380ac2510EC6e24eAE687"
+        ),
+        chain=chain_utils.Chain.GOERLI,
+        pool_abi_path=str(
+            pathlib.Path(__file__).parent.resolve()
+            / "abi"
+            / "ReceivableFactoringPool.json"
+        ),
+    ),
+    PoolSetting(
+        pool_address=web3.Web3.to_checksum_address(
             "0xC5BF9750A7BF93479990EF940d7e3984caa22558"
         ),
         chain=chain_utils.Chain.MUMBAI,
         pool_abi_path=str(
             pathlib.Path(__file__).parent.resolve()
             / "abi"
             / "SuperfluidFactoringPool.json"
```

### Comparing `huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/README.md` & `huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/polygon_wallet/adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/polygon_wallet/adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/request_network/README.md` & `huma_signals-0.5.0/huma_signals/adapters/request_network/README.md`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/request_network/models.py` & `huma_signals-0.5.0/huma_signals/adapters/request_network/models.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/request_network/request_invoice_adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/request_network/request_invoice_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/request_network/request_transaction_adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/request_network/request_transaction_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/adapters/superfluid/superfluid_adapter.py` & `huma_signals-0.5.0/huma_signals/adapters/superfluid/superfluid_adapter.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/eth_client/eth_client.py` & `huma_signals-0.5.0/huma_signals/clients/eth_client/eth_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/eth_client/eth_types.py` & `huma_signals-0.5.0/huma_signals/clients/eth_client/eth_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_client.py` & `huma_signals-0.5.0/huma_signals/clients/polygon_client/polygon_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/polygon_client/polygon_types.py` & `huma_signals-0.5.0/huma_signals/clients/polygon_client/polygon_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/request_client/request_client.py` & `huma_signals-0.5.0/huma_signals/clients/request_client/request_client.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/clients/request_client/request_types.py` & `huma_signals-0.5.0/huma_signals/clients/request_client/request_types.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/commons/tokens.py` & `huma_signals-0.5.0/huma_signals/commons/tokens.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/exceptions.py` & `huma_signals-0.5.0/huma_signals/exceptions.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/huma_signals/settings.py` & `huma_signals-0.5.0/huma_signals/settings.py`

 * *Files identical despite different names*

### Comparing `huma_signals-0.4.1/pyproject.toml` & `huma_signals-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "huma-signals"
-version = "0.4.1"
+version = "0.5.0"
 description = "Enables access to high-quality signals about a borrower's income, assets, and liabilities."
 authors = ["Jiatu Liu <jiatu@huma.finance>", "Ji Peng <ji@huma.finance>"]
 license = "AGPL v3"
 readme = "README.md"
 packages = [{include = "huma_signals"}]
 homepage = "https://github.com/00labs/huma-signals/"
 documentation = "https://docs.huma.finance/developer-guidelines/decentralized_signal_portfolio"
```

### Comparing `huma_signals-0.4.1/PKG-INFO` & `huma_signals-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: huma-signals
-Version: 0.4.1
+Version: 0.5.0
 Summary: Enables access to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/
 License: AGPL v3
 Author: Jiatu Liu
 Author-email: jiatu@huma.finance
 Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: huma-signals Version: 0.4.1 Summary: Enables access
+Metadata-Version: 2.1 Name: huma-signals Version: 0.5.0 Summary: Enables access
 to high-quality signals about a borrower's income, assets, and liabilities.
 Home-page: https://github.com/00labs/huma-signals/ License: AGPL v3 Author:
 Jiatu Liu Author-email: jiatu@huma.finance Requires-Python: >=3.10,<3.11
 Classifier: License :: Other/Proprietary License Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: aiofiles (>=22.1.0,<23.0.0) Requires-Dist: httpx
 (>=0.24.0,<0.25.0) Requires-Dist: huma-utils (>=0.2.1,<0.3.0) Requires-Dist:
```

