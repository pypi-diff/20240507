# Comparing `tmp/moonstreamdb-0.4.3.tar.gz` & `tmp/moonstreamdb-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.4.3.tar", last modified: Mon Apr 29 13:44:40 2024, max compression
+gzip compressed data, was "moonstreamdb-0.4.4.tar", last modified: Tue May  7 09:08:32 2024, max compression
```

## Comparing `moonstreamdb-0.4.3.tar` & `moonstreamdb-0.4.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11634 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    65236 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7053 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)     5925 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/subscriptions.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-29 13:44:27.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-29 13:44:39.000000 moonstreamdb-0.4.3/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-29 13:44:40.032055 moonstreamdb-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-04-29 13:44:23.000000 moonstreamdb-0.4.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:08:32.811207 moonstreamdb-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-07 09:08:32.811207 moonstreamdb-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:08:32.807207 moonstreamdb-0.4.4/moonstreamdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12247 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    68839 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6254 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/subscriptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/moonstreamdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-07 09:08:32.811207 moonstreamdb-0.4.4/moonstreamdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-07 09:08:22.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-07 09:08:32.000000 moonstreamdb-0.4.4/moonstreamdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-07 09:08:32.811207 moonstreamdb-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-05-07 09:08:18.000000 moonstreamdb-0.4.4/setup.py
```

### Comparing `moonstreamdb-0.4.3/PKG-INFO` & `moonstreamdb-0.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.3/README.md` & `moonstreamdb-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.3/moonstreamdb/blockchain.py` & `moonstreamdb-0.4.4/moonstreamdb/blockchain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 from enum import Enum
 from typing import Type, Union
 
 from .models import (
     AmoyBlock,
     AmoyLabel,
     AmoyTransaction,
+    ArbitrumOneBlock,
+    ArbitrumOneLabel,
+    ArbitrumOneTransaction,
     ArbitrumNovaBlock,
     ArbitrumNovaLabel,
     ArbitrumNovaTransaction,
     ArbitrumSepoliaBlock,
     ArbitrumSepoliaLabel,
     ArbitrumSepoliaTransaction,
     AvalancheBlock,
@@ -65,14 +68,15 @@
     MUMBAI = "mumbai"
     AMOY = "amoy"
     XDAI = "xdai"
     WYRM = "wyrm"
     ZKSYNC_ERA = "zksync_era"
     ZKSYNC_ERA_TESTNET = "zksync_era_testnet"
     ZKSYNC_ERA_SEPOLIA = "zksync_era_sepolia"
+    ARBITRUM_ONE = "arbitrum_one"
     ARBITRUM_NOVA = "arbitrum_nova"
     ARBITRUM_SEPOLIA = "arbitrum_sepolia"
     XAI = "xai"
     XAI_SEPOLIA = "xai_sepolia"
     AVALANCHE = "avalanche"
     AVALANCHE_FUJI = "avalanche_fuji"
     BLAST = "blast"
@@ -89,14 +93,15 @@
         MumbaiBlock,
         AmoyBlock,
         XDaiBlock,
         WyrmBlock,
         ZkSyncEraTestnetBlock,
         ZkSyncEraBlock,
         ZkSyncEraSepoliaBlock,
+        ArbitrumOneBlock,
         ArbitrumNovaBlock,
         ArbitrumSepoliaBlock,
         XaiBlock,
         XaiSepoliaBlock,
         AvalancheBlock,
         AvalancheFujiBlock,
         BlastBlock,
@@ -114,14 +119,15 @@
             MumbaiBlock,
             AmoyBlock,
             XDaiBlock,
             WyrmBlock,
             ZkSyncEraTestnetBlock,
             ZkSyncEraBlock,
             ZkSyncEraSepoliaBlock,
+            ArbitrumOneBlock,
             ArbitrumNovaBlock,
             ArbitrumSepoliaBlock,
             XaiBlock,
             XaiSepoliaBlock,
             AvalancheBlock,
             AvalancheFujiBlock,
             BlastBlock,
@@ -143,14 +149,16 @@
         block_model = WyrmBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         block_model = ZkSyncEraTestnetBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         block_model = ZkSyncEraBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
         block_model = ZkSyncEraSepoliaBlock
+    elif blockchain_type == AvailableBlockchainType.ARBITRUM_ONE:
+        block_model = ArbitrumOneBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         block_model = ArbitrumNovaBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         block_model = ArbitrumSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.XAI:
         block_model = XaiBlock
     elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
@@ -180,14 +188,15 @@
         MumbaiLabel,
         AmoyLabel,
         XDaiLabel,
         WyrmLabel,
         ZkSyncEraTestnetLabel,
         ZkSyncEraLabel,
         ZkSyncEraSepoliaLabel,
+        ArbitrumOneLabel,
         ArbitrumNovaLabel,
         ArbitrumSepoliaLabel,
         XaiLabel,
         XaiSepoliaLabel,
         AvalancheLabel,
         AvalancheFujiLabel,
         BlastLabel,
@@ -205,14 +214,15 @@
             MumbaiLabel,
             AmoyLabel,
             XDaiLabel,
             WyrmLabel,
             ZkSyncEraTestnetLabel,
             ZkSyncEraLabel,
             ZkSyncEraSepoliaLabel,
+            ArbitrumOneLabel,
             ArbitrumNovaLabel,
             ArbitrumSepoliaLabel,
             XaiLabel,
             XaiSepoliaLabel,
             AvalancheLabel,
             AvalancheFujiLabel,
             BlastLabel,
@@ -234,14 +244,16 @@
         label_model = WyrmLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         label_model = ZkSyncEraTestnetLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         label_model = ZkSyncEraLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
         label_model = ZkSyncEraSepoliaLabel
+    elif blockchain_type == AvailableBlockchainType.ARBITRUM_ONE:
+        label_model = ArbitrumOneLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         label_model = ArbitrumNovaLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         label_model = ArbitrumSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.XAI:
         label_model = XaiLabel
     elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
@@ -271,14 +283,15 @@
         MumbaiTransaction,
         AmoyTransaction,
         XDaiTransaction,
         WyrmTransaction,
         ZkSyncEraTestnetTransaction,
         ZkSyncEraTransaction,
         ZkSyncEraSepoliaTransaction,
+        ArbitrumOneTransaction,
         ArbitrumNovaTransaction,
         ArbitrumSepoliaTransaction,
         XaiTransaction,
         XaiSepoliaTransaction,
         AvalancheTransaction,
         AvalancheFujiTransaction,
         BlastTransaction,
@@ -296,14 +309,15 @@
             MumbaiTransaction,
             AmoyTransaction,
             XDaiTransaction,
             WyrmTransaction,
             ZkSyncEraTestnetTransaction,
             ZkSyncEraTransaction,
             ZkSyncEraSepoliaTransaction,
+            ArbitrumOneTransaction,
             ArbitrumNovaTransaction,
             ArbitrumSepoliaTransaction,
             XaiTransaction,
             XaiSepoliaTransaction,
             AvalancheTransaction,
             AvalancheFujiTransaction,
             BlastTransaction,
@@ -325,14 +339,16 @@
         transaction_model = WyrmTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         transaction_model = ZkSyncEraTestnetTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         transaction_model = ZkSyncEraTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
         transaction_model = ZkSyncEraSepoliaTransaction
+    elif blockchain_type == AvailableBlockchainType.ARBITRUM_ONE:
+        transaction_model = ArbitrumOneTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         transaction_model = ArbitrumNovaTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         transaction_model = ArbitrumSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.XAI:
         transaction_model = XaiTransaction
     elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
```

### Comparing `moonstreamdb-0.4.3/moonstreamdb/cli.py` & `moonstreamdb-0.4.4/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.3/moonstreamdb/db.py` & `moonstreamdb-0.4.4/moonstreamdb/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.4.3/moonstreamdb/models.py` & `moonstreamdb-0.4.4/moonstreamdb/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2052,14 +2052,129 @@
     block_timestamp = Column(BigInteger, index=True)
     log_index = Column(Integer, nullable=True)
     created_at = Column(
         DateTime(timezone=True), server_default=utcnow(), nullable=False
     )
 
 
+class ArbitrumOneBlock(Base):  # type: ignore
+    __tablename__ = "arbitrum_one_blocks"
+
+    block_number = Column(
+        BigInteger, primary_key=True, unique=True, nullable=False, index=True
+    )
+    difficulty = Column(BigInteger)
+    extra_data = Column(VARCHAR(128))
+    gas_limit = Column(BigInteger)
+    gas_used = Column(BigInteger)
+    base_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    hash = Column(VARCHAR(256), index=True)
+    logs_bloom = Column(VARCHAR(1024))
+    miner = Column(VARCHAR(256))
+    nonce = Column(VARCHAR(256))
+    parent_hash = Column(VARCHAR(256))
+    receipt_root = Column(VARCHAR(256))
+    uncles = Column(VARCHAR(256))
+    size = Column(Integer)
+    state_root = Column(VARCHAR(256))
+    timestamp = Column(BigInteger, index=True)
+    total_difficulty = Column(VARCHAR(256))
+    transactions_root = Column(VARCHAR(256))
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+    l1_block_number = Column(BigInteger, nullable=True)
+    send_count = Column(BigInteger, nullable=True)
+    send_root = Column(VARCHAR(256), nullable=True)
+    mix_hash = Column(VARCHAR(256), nullable=True)
+
+
+class ArbitrumOneTransaction(Base):  # type: ignore
+    __tablename__ = "arbitrum_one_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("arbitrum_one_blocks.block_number", ondelete="CASCADE"),
+        nullable=False,
+        index=True,
+    )
+    from_address = Column(VARCHAR(256), index=True)
+    to_address = Column(VARCHAR(256), index=True)
+    gas = Column(Numeric(precision=78, scale=0), index=True)
+    gas_price = Column(Numeric(precision=78, scale=0), index=True)
+    max_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    max_priority_fee_per_gas = Column(Numeric(precision=78, scale=0), nullable=True)
+    input = Column(Text)
+    nonce = Column(VARCHAR(256))
+    transaction_index = Column(BigInteger)
+    transaction_type = Column(Integer, nullable=True)
+    value = Column(Numeric(precision=78, scale=0), index=True)
+
+    indexed_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+    y_parity = Column(BigInteger, nullable=True)
+
+
+class ArbitrumOneLabel(Base):  # type: ignore
+    __tablename__ = "arbitrum_one_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_arbitrum_one_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_arbitrum_one_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
+    id = Column(
+        UUID(as_uuid=True),
+        primary_key=True,
+        default=uuid.uuid4,
+        unique=True,
+        nullable=False,
+    )
+    label = Column(VARCHAR(256), nullable=False, index=True)
+    block_number = Column(
+        BigInteger,
+        nullable=True,
+        index=True,
+    )
+    address = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    transaction_hash = Column(
+        VARCHAR(256),
+        nullable=True,
+        index=True,
+    )
+    label_data = Column(JSONB, nullable=True)
+    block_timestamp = Column(BigInteger, index=True)
+    log_index = Column(Integer, nullable=True)
+    created_at = Column(
+        DateTime(timezone=True), server_default=utcnow(), nullable=False
+    )
+
+
 class ESDFunctionSignature(Base):  # type: ignore
     """
     Function signature from blockchain (Ethereum/Polygon) Signature Database.
     """
 
     __tablename__ = "esd_function_signatures"
```

### Comparing `moonstreamdb-0.4.3/moonstreamdb/networks.py` & `moonstreamdb-0.4.4/moonstreamdb/networks.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,17 @@
 from typing import Dict, Union
 
 from .blockchain import AvailableBlockchainType
 from .models import (
     AmoyBlock,
     AmoyLabel,
     AmoyTransaction,
+    ArbitrumOneBlock,
+    ArbitrumOneLabel,
+    ArbitrumOneTransaction,
     ArbitrumNovaBlock,
     ArbitrumNovaLabel,
     ArbitrumNovaTransaction,
     ArbitrumSepoliaBlock,
     ArbitrumSepoliaLabel,
     ArbitrumSepoliaTransaction,
     AvalancheBlock,
@@ -67,14 +70,15 @@
     mumbai = "mumbai"
     amoy = "amoy"
     xdai = "xdai"
     wyrm = "wyrm"
     zksync_era_testnet = "zksync_era_testnet"
     zksync_era = "zksync_era"
     zksync_era_sepolia = "zksync_era_sepolia"
+    arbitrum_one = "arbitrum_one"
     arbitrum_nova = "arbitrum_nova"
     arbitrum_sepolia = "arbitrum_sepolia"
     xai = "xai"
     xai_sepolia = "xai_sepolia"
     avalanche = "avalanche"
     avalanche_fuji = "avalanche_fuji"
     blast = "blast"
@@ -88,14 +92,15 @@
     AmoyTransaction,
     PolygonTransaction,
     WyrmTransaction,
     XDaiTransaction,
     ZkSyncEraTestnetTransaction,
     ZkSyncEraTransaction,
     ZkSyncEraSepoliaTransaction,
+    ArbitrumOneTransaction,
     ArbitrumNovaTransaction,
     ArbitrumSepoliaTransaction,
     XaiTransaction,
     XaiSepoliaTransaction,
     AvalancheTransaction,
     AvalancheFujiTransaction,
     BlastTransaction,
@@ -145,14 +150,19 @@
         "transactions": ZkSyncEraSepoliaTransaction,
     },
     Network.zksync_era_sepolia: {
         "blocks": ZkSyncEraBlock,
         "labels": ZkSyncEraLabel,
         "transactions": ZkSyncEraTransaction,
     },
+    Network.arbitrum_one: {
+        "blocks": ArbitrumOneBlock,
+        "labels": ArbitrumOneLabel,
+        "transactions": ArbitrumOneTransaction,
+    },
     Network.arbitrum_nova: {
         "blocks": ArbitrumNovaBlock,
         "labels": ArbitrumNovaLabel,
         "transactions": ArbitrumNovaTransaction,
     },
     Network.arbitrum_sepolia: {
         "blocks": ArbitrumSepoliaBlock,
@@ -214,14 +224,16 @@
         return Network.wyrm
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         return Network.zksync_era_testnet
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         return Network.zksync_era
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
         return Network.zksync_era_sepolia
+    elif blockchain_type == AvailableBlockchainType.ARBITRUM_ONE:
+        return Network.arbitrum_one
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         return Network.arbitrum_nova
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         return Network.arbitrum_sepolia
     elif blockchain_type == AvailableBlockchainType.XAI:
         return Network.xai
     elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
```

### Comparing `moonstreamdb-0.4.3/moonstreamdb/subscriptions.py` & `moonstreamdb-0.4.4/moonstreamdb/subscriptions.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     MUMBAI_BLOCKCHAIN = "mumbai_smartcontract"
     AMOY_BLOCKCHAIN = "amoy_smartcontract"
     XDAI_BLOCKCHAIN = "xdai_smartcontract"
     WYRM_BLOCKCHAIN = "wyrm_smartcontract"
     ZKSYNC_ERA_TESTNET_BLOCKCHAIN = "zksync_era_testnet_smartcontract"
     ZKSYNC_ERA_BLOCKCHAIN = "zksync_era_smartcontract"
     ZKSYNC_ERA_SEPOLIA_BLOCKCHAIN = "zksync_era_sepolia_smartcontract"
+    ARBITRUM_ONE_BLOCKCHAIN = "arbitrum_one_smartcontract"
     ARBITRUM_NOVA_BLOCKCHAIN = "arbitrum_nova_smartcontract"
     ARBITRUM_SEPOLIA_BLOCKCHAIN = "arbitrum_sepolia_smartcontract"
     XAI_BLOCKCHAIN = "xai_smartcontract"
     XAI_SEPOLIA_BLOCKCHAIN = "xai_sepolia_smartcontract"
     AVALANCHE_BLOCKCHAIN = "avalanche_smartcontract"
     AVALANCHE_FUJI_BLOCKCHAIN = "avalanche_fuji_smartcontract"
     BLAST_BLOCKCHAIN = "blast_smartcontract"
@@ -41,14 +42,16 @@
         return SubscriptionTypes.WYRM_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         return SubscriptionTypes.ZKSYNC_ERA_TESTNET_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         return SubscriptionTypes.ZKSYNC_ERA_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
         return SubscriptionTypes.ZKSYNC_ERA_SEPOLIA_BLOCKCHAIN
+    elif blockchain_type == AvailableBlockchainType.ARBITRUM_ONE:
+        return SubscriptionTypes.ARBITRUM_ONE_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         return SubscriptionTypes.ARBITRUM_NOVA_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         return SubscriptionTypes.ARBITRUM_SEPOLIA_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.XAI:
         return SubscriptionTypes.XAI_BLOCKCHAIN
     elif blockchain_type == AvailableBlockchainType.XAI_SEPOLIA:
@@ -73,14 +76,15 @@
     "mumbai": "mumbai_smartcontract",
     "amoy": "amoy_smartcontract",
     "xdai": "xdai_smartcontract",
     "wyrm": "wyrm_smartcontract",
     "zksync_era_testnet": "zksync_era_testnet_smartcontract",
     "zksync_era": "zksync_era_smartcontract",
     "zksync_era_sepolia": "zksync_era_sepolia_smartcontract",
+    "arbitrum_one": "arbitrum_one_smartcontract",
     "arbitrum_nova": "arbitrum_nova_smartcontract",
     "arbitrum_sepolia": "arbitrum_sepolia_smartcontract",
     "xai": "xai_smartcontract",
     "xai_sepolia": "xai_sepolia_smartcontract",
     "avalanche": "avalanche_smartcontract",
     "avalanche_fuji": "avalanche_fuji_smartcontract",
     "blast": "blast_smartcontract",
@@ -94,14 +98,15 @@
     "mumbai_blockchain": "mumbai",
     "amoy_blockchain": "amoy",
     "xdai_blockchain": "xdai",
     "wyrm_blockchain": "wyrm",
     "zksync_era_testnet_blockchain": "zksync_era_testnet",
     "zksync_era_blockchain": "zksync_era",
     "zksync_era_sepolia_blockchain": "zksync_era_sepolia",
+    "arbitrum_one_blockchain": "arbitrum_one",
     "arbitrum_nova_blockchain": "arbitrum_nova",
     "arbitrum_sepolia_blockchain": "arbitrum_sepolia",
     "xai_blockchain": "xai",
     "xai_sepolia_blockchain": "xai_sepolia",
     "avalanche_blockchain": "avalanche",
     "avalanche_fuji_blockchain": "avalanche_fuji",
     "blast_blockchain": "blast",
@@ -112,14 +117,15 @@
     "mumbai_smartcontract": "mumbai",
     "amoy_smartcontract": "amoy",
     "xdai_smartcontract": "xdai",
     "wyrm_smartcontract": "wyrm",
     "zksync_era_testnet_smartcontract": "zksync_era_testnet",
     "zksync_era_smartcontract": "zksync_era",
     "zksync_era_sepolia_smartcontract": "zksync_era_sepolia",
+    "arbitrum_one_smartcontract": "arbitrum_one",
     "arbitrum_nova_smartcontract": "arbitrum_nova",
     "arbitrum_sepolia_smartcontract": "arbitrum_sepolia",
     "xai_smartcontract": "xai",
     "xai_sepolia_smartcontract": "xai_sepolia",
     "avalanche_smartcontract": "avalanche",
     "avalanche_fuji_smartcontract": "avalanche_fuji",
     "blast_smartcontract": "blast",
```

### Comparing `moonstreamdb-0.4.3/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.4.4/moonstreamdb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.4.3
+Version: 0.4.4
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.4.3/setup.py` & `moonstreamdb-0.4.4/setup.py`

 * *Files identical despite different names*

