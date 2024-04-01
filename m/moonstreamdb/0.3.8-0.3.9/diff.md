# Comparing `tmp/moonstreamdb-0.3.8.tar.gz` & `tmp/moonstreamdb-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "moonstreamdb-0.3.8.tar", last modified: Wed Feb 21 15:07:51 2024, max compression
+gzip compressed data, was "moonstreamdb-0.3.9.tar", last modified: Thu Mar 28 12:52:03 2024, max compression
```

## Comparing `moonstreamdb-0.3.8.tar` & `moonstreamdb-0.3.9.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:07:51.377677 moonstreamdb-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-21 15:07:51.377677 moonstreamdb-0.3.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:07:51.373677 moonstreamdb-0.3.8/moonstreamdb/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7195 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/blockchain.py
--rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/db.py
--rw-r--r--   0 runner    (1001) docker     (127)    35754 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/networks.py
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/moonstreamdb/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-21 15:07:51.377677 moonstreamdb-0.3.8/moonstreamdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-02-21 15:07:50.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      434 2024-02-21 15:07:51.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 15:07:50.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       56 2024-02-21 15:07:50.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-21 15:07:40.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-02-21 15:07:50.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-02-21 15:07:50.000000 moonstreamdb-0.3.8/moonstreamdb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-21 15:07:51.377677 moonstreamdb-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-02-21 15:07:30.000000 moonstreamdb-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/moonstreamdb/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9120 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/blockchain.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3157 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3110 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/db.py
+-rw-r--r--   0 runner    (1001) docker     (127)    47298 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3715 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/networks.py
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/moonstreamdb/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/moonstreamdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2344 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      434 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       56 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-28 12:51:54.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-03-28 12:52:03.000000 moonstreamdb-0.3.9/moonstreamdb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-28 12:52:03.559173 moonstreamdb-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1491 2024-03-28 12:51:50.000000 moonstreamdb-0.3.9/setup.py
```

### Comparing `moonstreamdb-0.3.8/PKG-INFO` & `moonstreamdb-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.8
+Version: 0.3.9
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.3.8/README.md` & `moonstreamdb-0.3.9/README.md`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.8/moonstreamdb/blockchain.py` & `moonstreamdb-0.3.9/moonstreamdb/blockchain.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,71 +1,86 @@
 from enum import Enum
 from typing import Type, Union
 
 from .models import (
+    ArbitrumNovaBlock,
+    ArbitrumNovaLabel,
+    ArbitrumNovaTransaction,
+    ArbitrumSepoliaBlock,
+    ArbitrumSepoliaLabel,
+    ArbitrumSepoliaTransaction,
+    AvalancheBlock,
+    AvalancheFujiBlock,
+    AvalancheFujiLabel,
+    AvalancheFujiTransaction,
+    AvalancheLabel,
+    AvalancheTransaction,
     EthereumBlock,
     EthereumLabel,
     EthereumTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
     PolygonBlock,
     PolygonLabel,
     PolygonTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
+    XaiBlock,
+    XaiLabel,
+    XaiTransaction,
     XDaiBlock,
     XDaiLabel,
     XDaiTransaction,
+    ZkSyncEraBlock,
+    ZkSyncEraLabel,
+    ZkSyncEraSepoliaBlock,
+    ZkSyncEraSepoliaLabel,
+    ZkSyncEraSepoliaTransaction,
     ZkSyncEraTestnetBlock,
     ZkSyncEraTestnetLabel,
     ZkSyncEraTestnetTransaction,
-    ZkSyncEraBlock,
-    ZkSyncEraLabel,
     ZkSyncEraTransaction,
-    ArbitrumNovaBlock,
-    ArbitrumNovaTransaction,
-    ArbitrumNovaLabel,
-    ArbitrumSepoliaBlock,
-    ArbitrumSepoliaTransaction,
-    ArbitrumSepoliaLabel,
-    XaiBlock,
-    XaiLabel,
-    XaiTransaction,
 )
 
 
 class AvailableBlockchainType(Enum):
     ETHEREUM = "ethereum"
     POLYGON = "polygon"
     MUMBAI = "mumbai"
     XDAI = "xdai"
     WYRM = "wyrm"
-    ZKSYNC_ERA_TESTNET = "zksync_era_testnet"
     ZKSYNC_ERA = "zksync_era"
+    ZKSYNC_ERA_TESTNET = "zksync_era_testnet"
+    ZKSYNC_ERA_SEPOLIA = "zksync_era_sepolia"
     ARBITRUM_NOVA = "arbitrum_nova"
     ARBITRUM_SEPOLIA = "arbitrum_sepolia"
     XAI = "xai"
+    AVALANCHE = "avalanche"
+    AVALANCHE_FUJI = "avalanche_fuji"
 
 
 def get_block_model(
     blockchain_type: AvailableBlockchainType,
 ) -> Type[
     Union[
         EthereumBlock,
         PolygonBlock,
         MumbaiBlock,
         XDaiBlock,
         WyrmBlock,
         ZkSyncEraTestnetBlock,
         ZkSyncEraBlock,
+        ZkSyncEraSepoliaBlock,
         ArbitrumNovaBlock,
         ArbitrumSepoliaBlock,
         XaiBlock,
+        AvalancheBlock,
+        AvalancheFujiBlock,
     ]
 ]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaBlock, ArbitrumSepoliaBlock, XaiBlock
     set proper blocks model.
     """
     block_model: Type[
@@ -73,17 +88,20 @@
             EthereumBlock,
             PolygonBlock,
             MumbaiBlock,
             XDaiBlock,
             WyrmBlock,
             ZkSyncEraTestnetBlock,
             ZkSyncEraBlock,
+            ZkSyncEraSepoliaBlock,
             ArbitrumNovaBlock,
             ArbitrumSepoliaBlock,
             XaiBlock,
+            AvalancheBlock,
+            AvalancheFujiBlock,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         block_model = EthereumBlock
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         block_model = PolygonBlock
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -92,20 +110,26 @@
         block_model = XDaiBlock
     elif blockchain_type == AvailableBlockchainType.WYRM:
         block_model = WyrmBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         block_model = ZkSyncEraTestnetBlock
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         block_model = ZkSyncEraBlock
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
+        block_model = ZkSyncEraSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         block_model = ArbitrumNovaBlock
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         block_model = ArbitrumSepoliaBlock
     elif blockchain_type == AvailableBlockchainType.XAI:
         block_model = XaiBlock
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE:
+        block_model = AvalancheBlock
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
+        block_model = AvalancheFujiBlock
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return block_model
 
 
 def get_label_model(
@@ -115,17 +139,20 @@
         EthereumLabel,
         PolygonLabel,
         MumbaiLabel,
         XDaiLabel,
         WyrmLabel,
         ZkSyncEraTestnetLabel,
         ZkSyncEraLabel,
+        ZkSyncEraSepoliaLabel,
         ArbitrumNovaLabel,
         ArbitrumSepoliaLabel,
         XaiLabel,
+        AvalancheLabel,
+        AvalancheFujiLabel,
     ]
 ]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaLabel, ArbitrumSepoliaLabel, XaiLabel
     set proper block label model.
     """
     label_model: Type[
@@ -133,17 +160,20 @@
             EthereumLabel,
             PolygonLabel,
             MumbaiLabel,
             XDaiLabel,
             WyrmLabel,
             ZkSyncEraTestnetLabel,
             ZkSyncEraLabel,
+            ZkSyncEraSepoliaLabel,
             ArbitrumNovaLabel,
             ArbitrumSepoliaLabel,
             XaiLabel,
+            AvalancheLabel,
+            AvalancheFujiLabel,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         label_model = EthereumLabel
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         label_model = PolygonLabel
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -152,20 +182,27 @@
         label_model = XDaiLabel
     elif blockchain_type == AvailableBlockchainType.WYRM:
         label_model = WyrmLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         label_model = ZkSyncEraTestnetLabel
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         label_model = ZkSyncEraLabel
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
+        label_model = ZkSyncEraSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         label_model = ArbitrumNovaLabel
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         label_model = ArbitrumSepoliaLabel
     elif blockchain_type == AvailableBlockchainType.XAI:
         label_model = XaiLabel
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE:
+        label_model = AvalancheLabel
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
+        label_model = AvalancheFujiLabel
+
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return label_model
 
 
 def get_transaction_model(
@@ -175,17 +212,20 @@
         EthereumTransaction,
         PolygonTransaction,
         MumbaiTransaction,
         XDaiTransaction,
         WyrmTransaction,
         ZkSyncEraTestnetTransaction,
         ZkSyncEraTransaction,
+        ZkSyncEraSepoliaTransaction,
         ArbitrumNovaTransaction,
         ArbitrumSepoliaTransaction,
         XaiTransaction,
+        AvalancheTransaction,
+        AvalancheFujiTransaction,
     ]
 ]:
     """
     Depends on provided blockchain type: Ethereum, Polygon, Mumbai, XDai, Wyrm, ZkSyncEra, ZkSyncEraTestnet, ArbitrumNovaTransaction, ArbitrumSepoliaTransaction, XaiTransaction
     set proper block transactions model.
     """
     transaction_model: Type[
@@ -193,17 +233,20 @@
             EthereumTransaction,
             PolygonTransaction,
             MumbaiTransaction,
             XDaiTransaction,
             WyrmTransaction,
             ZkSyncEraTestnetTransaction,
             ZkSyncEraTransaction,
+            ZkSyncEraSepoliaTransaction,
             ArbitrumNovaTransaction,
             ArbitrumSepoliaTransaction,
             XaiTransaction,
+            AvalancheTransaction,
+            AvalancheFujiTransaction,
         ]
     ]
     if blockchain_type == AvailableBlockchainType.ETHEREUM:
         transaction_model = EthereumTransaction
     elif blockchain_type == AvailableBlockchainType.POLYGON:
         transaction_model = PolygonTransaction
     elif blockchain_type == AvailableBlockchainType.MUMBAI:
@@ -212,17 +255,23 @@
         transaction_model = XDaiTransaction
     elif blockchain_type == AvailableBlockchainType.WYRM:
         transaction_model = WyrmTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_TESTNET:
         transaction_model = ZkSyncEraTestnetTransaction
     elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA:
         transaction_model = ZkSyncEraTransaction
+    elif blockchain_type == AvailableBlockchainType.ZKSYNC_ERA_SEPOLIA:
+        transaction_model = ZkSyncEraSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_NOVA:
         transaction_model = ArbitrumNovaTransaction
     elif blockchain_type == AvailableBlockchainType.ARBITRUM_SEPOLIA:
         transaction_model = ArbitrumSepoliaTransaction
     elif blockchain_type == AvailableBlockchainType.XAI:
         transaction_model = XaiTransaction
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE:
+        transaction_model = AvalancheTransaction
+    elif blockchain_type == AvailableBlockchainType.AVALANCHE_FUJI:
+        transaction_model = AvalancheFujiTransaction
     else:
         raise Exception("Unsupported blockchain type provided")
 
     return transaction_model
```

### Comparing `moonstreamdb-0.3.8/moonstreamdb/cli.py` & `moonstreamdb-0.3.9/moonstreamdb/cli.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.8/moonstreamdb/db.py` & `moonstreamdb-0.3.9/moonstreamdb/db.py`

 * *Files identical despite different names*

### Comparing `moonstreamdb-0.3.8/moonstreamdb/models.py` & `moonstreamdb-0.3.9/moonstreamdb/models.py`

 * *Files 14% similar despite different names*

```diff
@@ -797,14 +797,130 @@
     block_timestamp = Column(BigInteger, index=True)
     log_index = Column(Integer, nullable=True)
     created_at = Column(
         DateTime(timezone=True), server_default=utcnow(), nullable=False
     )
 
 
+class ZkSyncEraSepoliaBlock(Base):  # type: ignore
+    __tablename__ = "zksync_era_sepolia_blocks"
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
+    mix_hash = Column(VARCHAR(256), nullable=True)
+    sha3_uncles = Column(VARCHAR(256), nullable=True)
+
+    l1_batch_number = Column(BigInteger, nullable=True)
+    l1_batch_timestamp = Column(BigInteger, nullable=True)
+
+
+class ZkSyncEraSepoliaTransaction(Base):  # type: ignore
+    __tablename__ = "zksync_era_sepolia_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("zksync_era_sepolia_blocks.block_number", ondelete="CASCADE"),
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
+    l1_batch_number = Column(BigInteger, nullable=True)
+    l1_batch_tx_index = Column(BigInteger, nullable=True)
+
+
+class ZkSyncEraSepoliaLabel(Base):  # type: ignore
+    __tablename__ = "zksync_era_sepolia_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_zksync_era_sepolia_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_zksync_era_sepolia_labels_address_block_timestamp",
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
 class ArbitrumNovaBlock(Base):  # type: ignore
     __tablename__ = "arbitrum_nova_blocks"
 
     block_number = Column(
         BigInteger, primary_key=True, unique=True, nullable=False, index=True
     )
     difficulty = Column(BigInteger)
@@ -866,14 +982,29 @@
 
     y_parity = Column(BigInteger, nullable=True)
 
 
 class ArbitrumNovaLabel(Base):  # type: ignore
     __tablename__ = "arbitrum_nova_labels"
 
+    __table_args__ = (
+        Index(
+            "ix_arbitrum_nova_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_arbitrum_nova_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
     id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
     )
@@ -966,14 +1097,29 @@
 
     y_parity = Column(BigInteger, nullable=True)
 
 
 class ArbitrumSepoliaLabel(Base):  # type: ignore
     __tablename__ = "arbitrum_sepolia_labels"
 
+    __table_args__ = (
+        Index(
+            "ix_arbitrum_sepolia_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_arbitrum_sepolia_labels_address_block_timestamp",
+            "address",
+            "block_timestamp",
+            unique=False,
+        ),
+    )
+
     id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
     )
@@ -1072,14 +1218,240 @@
 
     id = Column(
         UUID(as_uuid=True),
         primary_key=True,
         default=uuid.uuid4,
         unique=True,
         nullable=False,
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
+class AvalancheBlock(Base):  # type: ignore
+    __tablename__ = "avalanche_blocks"
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
+    mix_hash = Column(VARCHAR(256), nullable=True)
+    block_extra_data = Column(VARCHAR(256), nullable=True)
+    block_gas_cost = Column(VARCHAR(256), nullable=True)
+    ext_data_gas_used = Column(VARCHAR(256), nullable=True)
+    ext_data_hash = Column(VARCHAR(256), nullable=True)
+
+
+class AvalancheTransaction(Base):  # type: ignore
+    __tablename__ = "avalanche_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("avalanche_blocks.block_number", ondelete="CASCADE"),
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
+
+class AvalancheLabel(Base):  # type: ignore
+    __tablename__ = "avalanche_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_avalanche_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_avalanche_labels_address_block_timestamp",
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
+class AvalancheFujiBlock(Base):  # type: ignore
+    __tablename__ = "avalanche_fuji_blocks"
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
+    mix_hash = Column(VARCHAR(256), nullable=True)
+    block_extra_data = Column(VARCHAR(256), nullable=True)
+    block_gas_cost = Column(VARCHAR(256), nullable=True)
+    ext_data_gas_used = Column(VARCHAR(256), nullable=True)
+    ext_data_hash = Column(VARCHAR(256), nullable=True)
+
+
+class AvalancheFujiTransaction(Base):  # type: ignore
+    __tablename__ = "avalanche_fuji_transactions"
+
+    hash = Column(
+        VARCHAR(256), primary_key=True, unique=True, nullable=False, index=True
+    )
+    block_number = Column(
+        BigInteger,
+        ForeignKey("avalanche_fuji_blocks.block_number", ondelete="CASCADE"),
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
+
+class AvalancheFujiLabel(Base):  # type: ignore
+    __tablename__ = "avalanche_fuji_labels"
+
+    __table_args__ = (
+        Index(
+            "ix_avalanche_fuji_labels_address_block_number",
+            "address",
+            "block_number",
+            unique=False,
+        ),
+        Index(
+            "ix_avalanche_fuji_labels_address_block_timestamp",
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
     )
     label = Column(VARCHAR(256), nullable=False, index=True)
     block_number = Column(
         BigInteger,
         nullable=True,
         index=True,
     )
```

### Comparing `moonstreamdb-0.3.8/moonstreamdb/networks.py` & `moonstreamdb-0.3.9/moonstreamdb/networks.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,69 +1,84 @@
 from enum import Enum
 from typing import Dict, Union
 
 from .models import (
+    ArbitrumNovaBlock,
+    ArbitrumNovaLabel,
+    ArbitrumNovaTransaction,
+    ArbitrumSepoliaBlock,
+    ArbitrumSepoliaLabel,
+    ArbitrumSepoliaTransaction,
+    AvalancheBlock,
+    AvalancheFujiBlock,
+    AvalancheFujiLabel,
+    AvalancheFujiTransaction,
+    AvalancheLabel,
+    AvalancheTransaction,
     Base,
     EthereumBlock,
     EthereumLabel,
     EthereumTransaction,
     MumbaiBlock,
     MumbaiLabel,
     MumbaiTransaction,
     PolygonBlock,
     PolygonLabel,
     PolygonTransaction,
     WyrmBlock,
     WyrmLabel,
     WyrmTransaction,
+    XaiBlock,
+    XaiLabel,
+    XaiTransaction,
     XDaiBlock,
     XDaiLabel,
     XDaiTransaction,
+    ZkSyncEraBlock,
+    ZkSyncEraLabel,
+    ZkSyncEraSepoliaBlock,
+    ZkSyncEraSepoliaLabel,
+    ZkSyncEraSepoliaTransaction,
     ZkSyncEraTestnetBlock,
     ZkSyncEraTestnetLabel,
     ZkSyncEraTestnetTransaction,
-    ZkSyncEraBlock,
-    ZkSyncEraLabel,
     ZkSyncEraTransaction,
-    ArbitrumNovaBlock,
-    ArbitrumNovaTransaction,
-    ArbitrumNovaLabel,
-    ArbitrumSepoliaBlock,
-    ArbitrumSepoliaTransaction,
-    ArbitrumSepoliaLabel,
-    XaiBlock,
-    XaiLabel,
-    XaiTransaction,
 )
 
 
 class Network(Enum):
     ethereum = "ethereum"
     polygon = "polygon"
     mumbai = "mumbai"
     xdai = "xdai"
     wyrm = "wyrm"
     zksync_era_testnet = "zksync_era_testnet"
     zksync_era = "zksync_era"
+    zksync_era_sepolia = "zksync_era_sepolia"
     arbitrum_nova = "arbitrum_nova"
     arbitrum_sepolia = "arbitrum_sepolia"
     xai = "xai"
+    avalanche = "avalanche"
+    avalanche_fuji = "avalanche_fuji"
 
 
 tx_raw_types = Union[
     EthereumTransaction,
     MumbaiTransaction,
     PolygonTransaction,
     WyrmTransaction,
     XDaiTransaction,
     ZkSyncEraTestnetTransaction,
     ZkSyncEraTransaction,
+    ZkSyncEraSepoliaTransaction,
     ArbitrumNovaTransaction,
     ArbitrumSepoliaTransaction,
     XaiTransaction,
+    AvalancheTransaction,
+    AvalancheFujiTransaction,
 ]
 
 MODELS: Dict[Network, Dict[str, Base]] = {
     Network.ethereum: {
         "blocks": EthereumBlock,
         "labels": EthereumLabel,
         "transactions": EthereumTransaction,
@@ -90,14 +105,19 @@
     },
     Network.zksync_era_testnet: {
         "blocks": ZkSyncEraTestnetBlock,
         "labels": ZkSyncEraTestnetLabel,
         "transactions": ZkSyncEraTestnetTransaction,
     },
     Network.zksync_era: {
+        "blocks": ZkSyncEraSepoliaBlock,
+        "labels": ZkSyncEraSepoliaLabel,
+        "transactions": ZkSyncEraSepoliaTransaction,
+    },
+    Network.zksync_era_sepolia: {
         "blocks": ZkSyncEraBlock,
         "labels": ZkSyncEraLabel,
         "transactions": ZkSyncEraTransaction,
     },
     Network.arbitrum_nova: {
         "blocks": ArbitrumNovaBlock,
         "labels": ArbitrumNovaLabel,
@@ -109,8 +129,18 @@
         "transactions": ArbitrumSepoliaTransaction,
     },
     Network.xai: {
         "blocks": XaiBlock,
         "labels": XaiLabel,
         "transactions": XaiTransaction,
     },
+    Network.avalanche: {
+        "blocks": AvalancheBlock,
+        "labels": AvalancheLabel,
+        "transactions": AvalancheTransaction,
+    },
+    Network.avalanche_fuji: {
+        "blocks": AvalancheFujiBlock,
+        "labels": AvalancheFujiLabel,
+        "transactions": AvalancheFujiTransaction,
+    },
 }
```

### Comparing `moonstreamdb-0.3.8/moonstreamdb.egg-info/PKG-INFO` & `moonstreamdb-0.3.9/moonstreamdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: moonstreamdb
-Version: 0.3.8
+Version: 0.3.9
 Summary: Moonstream database
 Home-page: https://github.com/bugout-dev/moonstream
 Author: Bugout.dev
 Author-email: engineers@bugout.dev
 License: Apache License 2.0
 Description: # moonstream db
```

### Comparing `moonstreamdb-0.3.8/setup.py` & `moonstreamdb-0.3.9/setup.py`

 * *Files identical despite different names*

