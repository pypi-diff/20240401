# Comparing `tmp/aioetherscan-0.8.8.tar.gz` & `tmp/aioetherscan-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioetherscan-0.8.8.tar", max compression
+gzip compressed data, was "aioetherscan-0.8.9.tar", max compression
```

## Comparing `aioetherscan-0.8.8.tar` & `aioetherscan-0.8.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       39 2023-03-06 21:16:55.496964 aioetherscan-0.8.8/aioetherscan/__init__.py
--rw-r--r--   0        0        0     1781 2023-11-12 22:42:21.990387 aioetherscan-0.8.8/aioetherscan/client.py
--rw-r--r--   0        0        0     1389 2023-11-12 22:42:21.990611 aioetherscan-0.8.8/aioetherscan/common.py
--rw-r--r--   0        0        0      838 2023-03-06 21:16:55.497587 aioetherscan-0.8.8/aioetherscan/exceptions.py
--rw-r--r--   0        0        0     4017 2023-11-12 22:42:21.990909 aioetherscan-0.8.8/aioetherscan/modules/account.py
--rw-r--r--   0        0        0      740 2023-03-06 21:16:55.497945 aioetherscan-0.8.8/aioetherscan/modules/base.py
--rw-r--r--   0        0        0     1023 2023-11-12 22:42:21.991279 aioetherscan-0.8.8/aioetherscan/modules/block.py
--rw-r--r--   0        0        0     2679 2023-11-12 21:52:09.620895 aioetherscan-0.8.8/aioetherscan/modules/contract.py
--rw-r--r--   0        0        0      691 2023-11-08 19:42:11.094546 aioetherscan-0.8.8/aioetherscan/modules/extra/links.py
--rw-r--r--   0        0        0     4236 2023-11-08 19:42:11.094858 aioetherscan-0.8.8/aioetherscan/modules/extra/utils.py
--rw-r--r--   0        0        0     1881 2023-11-12 22:42:21.991501 aioetherscan-0.8.8/aioetherscan/modules/gas_tracker.py
--rw-r--r--   0        0        0     2441 2023-11-12 21:52:09.621125 aioetherscan-0.8.8/aioetherscan/modules/logs.py
--rw-r--r--   0        0        0     4546 2023-11-12 21:52:09.621444 aioetherscan-0.8.8/aioetherscan/modules/proxy.py
--rw-r--r--   0        0        0      504 2023-11-12 21:52:09.621684 aioetherscan-0.8.8/aioetherscan/modules/stats.py
--rw-r--r--   0        0        0     3722 2023-11-12 21:52:09.622031 aioetherscan-0.8.8/aioetherscan/modules/token.py
--rw-r--r--   0        0        0      813 2023-11-12 21:52:09.622254 aioetherscan-0.8.8/aioetherscan/modules/transaction.py
--rw-r--r--   0        0        0     3714 2023-11-08 19:42:11.095105 aioetherscan-0.8.8/aioetherscan/network.py
--rw-r--r--   0        0        0     3067 2023-11-08 19:42:11.095306 aioetherscan-0.8.8/aioetherscan/url_builder.py
--rw-r--r--   0        0        0      645 2023-11-12 22:42:52.096731 aioetherscan-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 aioetherscan-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0       53 2023-11-20 21:25:01.534091 aioetherscan-0.8.9/aioetherscan/__init__.py
+-rw-r--r--   0        0        0     1826 2023-11-20 21:25:01.534321 aioetherscan-0.8.9/aioetherscan/client.py
+-rw-r--r--   0        0        0     2231 2023-11-20 21:43:17.714656 aioetherscan-0.8.9/aioetherscan/common.py
+-rw-r--r--   0        0        0      838 2023-11-20 14:20:07.066225 aioetherscan-0.8.9/aioetherscan/exceptions.py
+-rw-r--r--   0        0        0     4662 2023-11-20 21:43:17.726134 aioetherscan-0.8.9/aioetherscan/modules/account.py
+-rw-r--r--   0        0        0      485 2023-11-20 14:20:07.066998 aioetherscan-0.8.9/aioetherscan/modules/base.py
+-rw-r--r--   0        0        0     2550 2023-11-20 21:43:17.750677 aioetherscan-0.8.9/aioetherscan/modules/block.py
+-rw-r--r--   0        0        0     2908 2023-11-20 21:43:17.711448 aioetherscan-0.8.9/aioetherscan/modules/contract.py
+-rw-r--r--   0        0        0      691 2023-11-20 14:20:07.068047 aioetherscan-0.8.9/aioetherscan/modules/extra/links.py
+-rw-r--r--   0        0        0     4087 2023-11-20 21:43:17.741430 aioetherscan-0.8.9/aioetherscan/modules/extra/utils.py
+-rw-r--r--   0        0        0     1926 2023-11-20 21:43:17.731346 aioetherscan-0.8.9/aioetherscan/modules/gas_tracker.py
+-rw-r--r--   0        0        0     2394 2023-11-20 21:43:17.733492 aioetherscan-0.8.9/aioetherscan/modules/logs.py
+-rw-r--r--   0        0        0     4549 2023-11-20 21:43:17.743568 aioetherscan-0.8.9/aioetherscan/modules/proxy.py
+-rw-r--r--   0        0        0     3756 2023-11-20 21:43:17.745745 aioetherscan-0.8.9/aioetherscan/modules/stats.py
+-rw-r--r--   0        0        0     3640 2023-11-20 21:43:17.737533 aioetherscan-0.8.9/aioetherscan/modules/token.py
+-rw-r--r--   0        0        0      743 2023-11-20 21:43:17.727894 aioetherscan-0.8.9/aioetherscan/modules/transaction.py
+-rw-r--r--   0        0        0     3768 2023-11-20 21:43:17.721173 aioetherscan-0.8.9/aioetherscan/network.py
+-rw-r--r--   0        0        0     3053 2023-11-20 21:43:17.748956 aioetherscan-0.8.9/aioetherscan/url_builder.py
+-rw-r--r--   0        0        0      719 2023-11-20 21:48:33.765964 aioetherscan-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      670 1970-01-01 00:00:00.000000 aioetherscan-0.8.9/PKG-INFO
```

### Comparing `aioetherscan-0.8.8/aioetherscan/client.py` & `aioetherscan-0.8.9/aioetherscan/client.py`

 * *Files 12% similar despite different names*

```diff
@@ -15,17 +15,25 @@
 from aioetherscan.modules.stats import Stats
 from aioetherscan.modules.token import Token
 from aioetherscan.modules.transaction import Transaction
 from aioetherscan.network import Network, UrlBuilder
 
 
 class Client:
-    def __init__(self, api_key: str, api_kind: str = 'eth', network: str = 'main',
-                 loop: AbstractEventLoop = None, timeout: ClientTimeout = None, proxy: str = None,
-                 throttler: AsyncContextManager = None, retry_options: RetryOptionsBase = None) -> None:
+    def __init__(
+        self,
+        api_key: str,
+        api_kind: str = 'eth',
+        network: str = 'main',
+        loop: AbstractEventLoop = None,
+        timeout: ClientTimeout = None,
+        proxy: str = None,
+        throttler: AsyncContextManager = None,
+        retry_options: RetryOptionsBase = None,
+    ) -> None:
         self._url_builder = UrlBuilder(api_key, api_kind, network)
         self._http = Network(self._url_builder, loop, timeout, proxy, throttler, retry_options)
 
         self.account = Account(self)
         self.block = Block(self)
         self.contract = Contract(self)
         self.transaction = Transaction(self)
```

### Comparing `aioetherscan-0.8.8/aioetherscan/exceptions.py` & `aioetherscan-0.8.9/aioetherscan/exceptions.py`

 * *Files identical despite different names*

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/account.py` & `aioetherscan-0.8.9/aioetherscan/modules/account.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,15 @@
 from typing import Iterable, Optional, List, Dict
 
-from aioetherscan.common import check_tag, check_sort_direction, check_blocktype
+from aioetherscan.common import (
+    check_tag,
+    check_sort_direction,
+    check_blocktype,
+    check_token_standard,
+)
 from aioetherscan.modules.base import BaseModule
 
 
 class Account(BaseModule):
     """Accounts
 
     https://docs.etherscan.io/api-endpoints/accounts
@@ -12,112 +17,127 @@
 
     @property
     def _module(self) -> str:
         return 'account'
 
     async def balance(self, address: str, tag: str = 'latest') -> str:
         """Get Ether Balance for a single Address."""
-        return await self._get(
-            action='balance',
-            address=address,
-            tag=check_tag(tag)
-        )
+        return await self._get(action='balance', address=address, tag=check_tag(tag))
 
     async def balances(self, addresses: Iterable[str], tag: str = 'latest') -> List[Dict]:
         """Get Ether Balance for multiple Addresses in a single call."""
         return await self._get(
-            action='balancemulti',
-            address=','.join(addresses),
-            tag=check_tag(tag)
+            action='balancemulti', address=','.join(addresses), tag=check_tag(tag)
         )
 
     async def normal_txs(
-            self,
-            address: str,
-            start_block: Optional[int] = None,
-            end_block: Optional[int] = None,
-            sort: Optional[str] = None,
-            page: Optional[int] = None,
-            offset: Optional[int] = None
+        self,
+        address: str,
+        start_block: Optional[int] = None,
+        end_block: Optional[int] = None,
+        sort: Optional[str] = None,
+        page: Optional[int] = None,
+        offset: Optional[int] = None,
     ) -> List[Dict]:
         """Get a list of 'Normal' Transactions By Address."""
         return await self._get(
             action='txlist',
             address=address,
             startblock=start_block,
             endblock=end_block,
             sort=check_sort_direction(sort),
             page=page,
-            offset=offset
+            offset=offset,
         )
 
     async def internal_txs(
-            self,
-            address: str,
-            start_block: Optional[int] = None,
-            end_block: Optional[int] = None,
-            sort: Optional[str] = None,
-            page: Optional[int] = None,
-            offset: Optional[int] = None,
-            txhash: Optional[str] = None
+        self,
+        address: str,
+        start_block: Optional[int] = None,
+        end_block: Optional[int] = None,
+        sort: Optional[str] = None,
+        page: Optional[int] = None,
+        offset: Optional[int] = None,
+        txhash: Optional[str] = None,
     ) -> List[Dict]:
         """Get a list of 'Internal' Transactions by Address or Transaction Hash."""
         return await self._get(
             action='txlistinternal',
             address=address,
             startblock=start_block,
             endblock=end_block,
             sort=check_sort_direction(sort),
             page=page,
             offset=offset,
-            txhash=txhash
+            txhash=txhash,
         )
 
     async def token_transfers(
-            self,
-            address: Optional[str] = None,
-            contract_address: Optional[str] = None,
-            start_block: Optional[int] = None,
-            end_block: Optional[int] = None,
-            sort: Optional[str] = None,
-            page: Optional[int] = None,
-            offset: Optional[int] = None,
+        self,
+        address: Optional[str] = None,
+        contract_address: Optional[str] = None,
+        start_block: Optional[int] = None,
+        end_block: Optional[int] = None,
+        sort: Optional[str] = None,
+        page: Optional[int] = None,
+        offset: Optional[int] = None,
+        token_standard: str = 'erc20',
     ) -> List[Dict]:
-        """Get a list of "ERC20 - Token Transfer Events" by Address."""
+        """Get a list of "ERC20 - Token Transfer Events" by Address"""
         if not address and not contract_address:
             raise ValueError('At least one of address or contract_address must be specified.')
 
+        token_standard = check_token_standard(token_standard)
+        actions = dict(erc20='tokentx', erc721='tokennfttx', erc1155='token1155tx')
+
         return await self._get(
-            action='tokentx',
+            action=actions.get(token_standard),
             address=address,
             startblock=start_block,
             endblock=end_block,
             sort=check_sort_direction(sort),
             page=page,
             offset=offset,
-            contractaddress=contract_address
+            contractaddress=contract_address,
         )
 
     async def mined_blocks(
-            self,
-            address: str,
-            blocktype: str = 'blocks',
-            page: Optional[int] = None,
-            offset: Optional[int] = None
+        self,
+        address: str,
+        blocktype: str = 'blocks',
+        page: Optional[int] = None,
+        offset: Optional[int] = None,
     ) -> List:
-        """Get list of Blocks Mined by Address."""
+        """Get list of Blocks Validated by Address"""
         return await self._get(
             action='getminedblocks',
             address=address,
             blocktype=check_blocktype(blocktype),
             page=page,
-            offset=offset
+            offset=offset,
         )
 
-    async def token_balance(self, address: str, contract_address: str, tag: str = 'latest') -> str:
-        """Get ERC20-Token Account Balance for TokenContractAddress."""
+    async def beacon_chain_withdrawals(
+        self,
+        address: str,
+        start_block: Optional[int] = None,
+        end_block: Optional[int] = None,
+        sort: Optional[str] = None,
+        page: Optional[int] = None,
+        offset: Optional[int] = None,
+    ) -> List[Dict]:
+        """Get Beacon Chain Withdrawals by Address and Block Range"""
         return await self._get(
-            action='tokenbalance',
+            action='txsBeaconWithdrawal',
             address=address,
-            contractaddress=contract_address,
-            tag=check_tag(tag)
+            startblock=start_block,
+            endblock=end_block,
+            sort=check_sort_direction(sort),
+            page=page,
+            offset=offset,
+        )
+
+    async def account_balance_by_blockno(self, address: str, blockno: int) -> str:
+        """Get Historical Ether Balance for a Single Address By BlockNo"""
+        return await self._get(
+            module='account', action='balancehistory', address=address, blockno=blockno
         )
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/contract.py` & `aioetherscan-0.8.9/aioetherscan/modules/contract.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,78 +10,67 @@
     """
 
     @property
     def _module(self) -> str:
         return 'contract'
 
     async def contract_abi(self, address: str) -> str:
-        """Get Contract ABI for Verified Contract Source Codes
-
-        https://etherscan.io/contractsVerified.
-        """
-        return await self._get(
-            action='getabi',
-            address=address
-        )
+        """Get Contract ABI for Verified Contract Source Codes"""
+        return await self._get(action='getabi', address=address)
 
     async def contract_source_code(self, address: str) -> List[Dict]:
-        """Get Contract Source Code for Verified Contract Source Codes
-
-        https://etherscan.io/contractsVerified.
-        """
-        return await self._get(
-            action='getsourcecode',
-            address=address
-        )
+        """Get Contract Source Code for Verified Contract Source Codes"""
+        return await self._get(action='getsourcecode', address=address)
 
     async def contract_creation(self, addresses: Iterable[str]) -> List[Dict]:
-        """Get Contract deployer address and transaction hash it was created
-
-        https://etherscan.io/contractsVerified.
-        """
-        return await self._get(
-            action='getcontractcreation',
-            contractaddresses=','.join(addresses)
-        )
+        """Get Contract Creator and Creation Tx Hash"""
+        return await self._get(action='getcontractcreation', contractaddresses=','.join(addresses))
 
     async def verify_contract_source_code(
-            self,
-            contract_address: str,
-            source_code: str,
-            contract_name: str,
-            compiler_version: str,
-            optimization_used: bool = False,
-            runs: int = 200,
-            constructor_arguements: str = None,
-            libraries: Dict[str, str] = None
+        self,
+        contract_address: str,
+        source_code: str,
+        contract_name: str,
+        compiler_version: str,
+        optimization_used: bool = False,
+        runs: int = 200,
+        constructor_arguements: str = None,
+        libraries: Dict[str, str] = None,
     ) -> str:
-        """[BETA] Verify Source Code"""
+        """Submits a contract source code to Etherscan for verification."""
         return await self._post(
             module='contract',
             action='verifysourcecode',
             contractaddress=contract_address,
             sourceCode=source_code,
             contractname=contract_name,
             compilerversion=compiler_version,
             optimizationUsed=1 if optimization_used else 0,
             runs=runs,
             constructorArguements=constructor_arguements,
-            **self._parse_libraries(libraries or {})
+            **self._parse_libraries(libraries or {}),
         )
 
     async def check_verification_status(self, guid: str) -> str:
         """Check Source code verification submission status"""
-        return await self._get(
-            action='checkverifystatus',
-            guid=guid
+        return await self._get(action='checkverifystatus', guid=guid)
+
+    async def verify_proxy_contract(self, address: str, expected_implementation: str = None) -> str:
+        """Submits a proxy contract source code to Etherscan for verification."""
+        return await self._post(
+            module='contract',
+            action='verifyproxycontract',
+            address=address,
+            expectedimplementation=expected_implementation,
         )
 
+    async def check_proxy_contract_verification(self, guid: str) -> str:
+        """Checking Proxy Contract Verification Submission Status"""
+        return await self._get(action='checkproxyverification', guid=guid)
+
     @staticmethod
     def _parse_libraries(libraries: Dict[str, str]) -> Dict[str, str]:
         return dict(
             part
             for i, (name, address) in enumerate(libraries.items(), start=1)
-            for part in (
-                (f'libraryname{i}', name),
-                (f'libraryaddress{i}', address)
-            )
+            for part in ((f'libraryname{i}', name), (f'libraryaddress{i}', address))
         )
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/extra/links.py` & `aioetherscan-0.8.9/aioetherscan/modules/extra/links.py`

 * *Files identical despite different names*

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/extra/utils.py` & `aioetherscan-0.8.9/aioetherscan/modules/extra/utils.py`

 * *Files 7% similar despite different names*

```diff
@@ -10,112 +10,111 @@
 class Utils:
     """Helper methods which use the combination of documented APIs."""
 
     def __init__(self, client: 'Client'):
         self._client = client
 
     async def token_transfers_generator(
-            self,
-            address: str = None,
-            contract_address: str = None,
-            block_limit: int = 50,
-            offset: int = 3,
-            start_block: int = 0,
-            end_block: int = None,
+        self,
+        address: str = None,
+        contract_address: str = None,
+        block_limit: int = 50,
+        offset: int = 3,
+        start_block: int = 0,
+        end_block: int = None,
     ) -> AsyncIterator[Dict]:
         if end_block is None:
             end_block = int(await self._client.proxy.block_number(), 16)
 
         for sblock, eblock in self._generate_intervals(start_block, end_block, block_limit):
             async for transfer in self._parse_by_pages(
-                    address=address,
-                    contract_address=contract_address,
-                    start_block=sblock,
-                    end_block=eblock,
-                    offset=offset,
+                address=address,
+                contract_address=contract_address,
+                start_block=sblock,
+                end_block=eblock,
+                offset=offset,
             ):
                 yield transfer
 
     async def token_transfers(
-            self,
-            address: str = None,
-            contract_address: str = None,
-            be_polite: bool = True,
-            block_limit: int = 50,
-            offset: int = 3,
-            start_block: int = 0,
-            end_block: int = None,
+        self,
+        address: str = None,
+        contract_address: str = None,
+        be_polite: bool = True,
+        block_limit: int = 50,
+        offset: int = 3,
+        start_block: int = 0,
+        end_block: int = None,
     ) -> List[Dict]:
         kwargs = {k: v for k, v in locals().items() if k != 'self' and not k.startswith('_')}
         return [t async for t in self.token_transfers_generator(**kwargs)]
 
     async def is_contract(self, address: str) -> bool:
         try:
             response = await self._client.contract.contract_abi(address=address)
         except EtherscanClientApiError as e:
-            if e.message.upper() == 'NOTOK' and e.result.lower() == 'contract source code not verified':
+            if (
+                e.message.upper() == 'NOTOK'
+                and e.result.lower() == 'contract source code not verified'
+            ):
                 return False
             raise
         else:
             return True if response else False
 
     async def get_contract_creator(self, contract_address: str) -> Optional[str]:
         try:
             response = await self._client.account.internal_txs(
-                address=contract_address,
-                start_block=1,
-                page=1,
-                offset=1
+                address=contract_address, start_block=1, page=1, offset=1
             )  # try to find first internal transaction
         except EtherscanClientApiError as e:
             if e.message.lower() != 'no transactions found':
                 raise
             else:
                 response = None
 
         if not response:
             try:
                 response = await self._client.account.normal_txs(
-                    address=contract_address,
-                    start_block=1,
-                    page=1,
-                    offset=1
+                    address=contract_address, start_block=1, page=1, offset=1
                 )  # try to find first normal transaction
             except EtherscanClientApiError as e:
                 if e.message.lower() != 'no transactions found':
                     raise
 
         return next((i['from'].lower() for i in response), None)
 
     async def _parse_by_pages(
-            self,
-            start_block: int,
-            end_block: int,
-            offset: int,
-            address: str = None,
-            contract_address: str = None,
+        self,
+        start_block: int,
+        end_block: int,
+        offset: int,
+        address: str = None,
+        contract_address: str = None,
     ) -> AsyncIterator[Dict]:
         page = 1
 
         while True:
             try:
                 transfers = await self._client.account.token_transfers(
                     address=address,
                     contract_address=contract_address,
                     start_block=start_block,
                     end_block=end_block,
                     page=page,
-                    offset=offset
+                    offset=offset,
                 )
             except EtherscanClientApiError as e:
                 if e.message == 'No transactions found':
                     break
                 raise
             else:
                 for transfer in transfers:
                     yield transfer
                 page += 1
 
     @staticmethod
-    def _generate_intervals(from_number: int, to_number: int, count: int) -> Iterator[Tuple[int, int]]:
+    def _generate_intervals(
+        from_number: int, to_number: int, count: int
+    ) -> Iterator[Tuple[int, int]]:
         for i in range(from_number, to_number + 1, count):
             yield i, min(i + count - 1, to_number)
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/gas_tracker.py` & `aioetherscan-0.8.9/aioetherscan/modules/gas_tracker.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,36 +19,42 @@
         """Get Estimation of Confirmation Time"""
         return await self._get(action='gasestimate', gasprice=gas_price)
 
     async def gas_oracle(self) -> Dict:
         """Get Gas Oracle"""
         return await self._get(action='gasoracle')
 
-    async def daily_average_gas_limit(self, start_date: date, end_date: date, sort: Optional[str] = None) -> List[Dict]:
+    async def daily_average_gas_limit(
+        self, start_date: date, end_date: date, sort: Optional[str] = None
+    ) -> List[Dict]:
         """Get Daily Average Gas Limit"""
         return await self._get(
             module='stats',
             action='dailyavggaslimit',
             startdate=start_date.isoformat(),
             enddate=end_date.isoformat(),
-            sort=check_sort_direction(sort)
+            sort=check_sort_direction(sort),
         )
 
-    async def daily_total_gas_used(self, start_date: date, end_date: date, sort: Optional[str] = None) -> Dict:
+    async def daily_total_gas_used(
+        self, start_date: date, end_date: date, sort: Optional[str] = None
+    ) -> Dict:
         """Get Ethereum Daily Total Gas Used"""
         return await self._get(
             module='stats',
             action='dailygasused',
             startdate=start_date.isoformat(),
             enddate=end_date.isoformat(),
-            sort=check_sort_direction(sort)
+            sort=check_sort_direction(sort),
         )
 
-    async def daily_average_gas_price(self, start_date: date, end_date: date, sort: Optional[str] = None) -> Dict:
+    async def daily_average_gas_price(
+        self, start_date: date, end_date: date, sort: Optional[str] = None
+    ) -> Dict:
         """Get Daily Average Gas Price"""
         return await self._get(
             module='stats',
             action='dailyavggasprice',
             startdate=start_date.isoformat(),
             enddate=end_date.isoformat(),
-            sort=check_sort_direction(sort)
+            sort=check_sort_direction(sort),
         )
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/logs.py` & `aioetherscan-0.8.9/aioetherscan/modules/logs.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,60 +13,58 @@
     _BLOCKS = ('latest',)
 
     @property
     def _module(self) -> str:
         return 'logs'
 
     async def get_logs(
-            self,
-            from_block: Union[int, str],
-            to_block: Union[int, str],
-            address: str,
-            topics: List[str],
-            topic_operators: Optional[List[str]] = None
+        self,
+        from_block: Union[int, str],
+        to_block: Union[int, str],
+        address: str,
+        topics: List[str],
+        topic_operators: Optional[List[str]] = None,
     ) -> List[Dict]:
         """[Beta] The Event Log API was designed to provide an alternative to the native eth_getLogs
 
         https://github.com/ethereum/wiki/wiki/JSON-RPC#eth_getlogs.
         """
         return await self._get(
             action='getLogs',
             fromBlock=self._check_block(from_block),
             toBlock=self._check_block(to_block),
             address=address,
-            **self._fill_topics(topics, topic_operators)
+            **self._fill_topics(topics, topic_operators),
         )
 
     def _check_block(self, block: Union[str, int]) -> Union[str, int]:
         if isinstance(block, int):
             return block
         if block in self._BLOCKS:
             return block
         raise ValueError(f'Invalid value {block!r}, only integers or {self._BLOCKS} are supported.')
 
     def _fill_topics(self, topics: List[str], topic_operators: List[str]):
         if len(topics) > 1:
             self._check_topics(topics, topic_operators)
 
-            topic_params = {
-                f'topic{idx}': value
-                for idx, value in enumerate(topics)
-            }
+            topic_params = {f'topic{idx}': value for idx, value in enumerate(topics)}
             topic_operator_params = {
-                f'topic{idx}_{idx + 1}_opr': value
-                for idx, value in enumerate(topic_operators)
+                f'topic{idx}_{idx + 1}_opr': value for idx, value in enumerate(topic_operators)
             }
 
             return {**topic_params, **topic_operator_params}
         else:
             return {'topic0': topics[0]}
 
     def _check_topics(self, topics: List[str], topic_operators: List[str]) -> None:
         if not topic_operators:
             raise ValueError('Topic operators are required when more than 1 topic passed.')
 
         for op in topic_operators:
             if op not in self._TOPIC_OPERATORS:
-                raise ValueError(f'Invalid topic operator {op!r}, must be one of: {self._TOPIC_OPERATORS}')
+                raise ValueError(
+                    f'Invalid topic operator {op!r}, must be one of: {self._TOPIC_OPERATORS}'
+                )
 
         if len(topics) - len(topic_operators) != 1:
-            raise ValueError(f'Invalid length of topic_operators list, must be len(topics) - 1.')
+            raise ValueError('Invalid length of topic_operators list, must be len(topics) - 1.')
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/proxy.py` & `aioetherscan-0.8.9/aioetherscan/modules/proxy.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
         """Returns information about a block by block number."""
         return await self._get(
             action='eth_getBlockByNumber',
             boolean=full,
             tag=check_tag(tag),
         )
 
-    async def uncle_block_by_number_and_index(self, index: Union[int, str], tag: Union[int, str] = 'latest') -> Dict:
+    async def uncle_block_by_number_and_index(
+        self, index: Union[int, str], tag: Union[int, str] = 'latest'
+    ) -> Dict:
         """Returns information about a uncle by block number."""
         return await self._get(
             action='eth_getUncleByBlockNumberAndIndex',
             index=check_hex(index),
             tag=check_tag(tag),
         )
 
@@ -44,15 +46,17 @@
     async def tx_by_hash(self, txhash: Union[int, str]) -> Dict:
         """Returns the information about a transaction requested by transaction hash."""
         return await self._get(
             action='eth_getTransactionByHash',
             txhash=check_hex(txhash),
         )
 
-    async def tx_by_number_and_index(self, index: Union[int, str], tag: Union[int, str] = 'latest') -> Dict:
+    async def tx_by_number_and_index(
+        self, index: Union[int, str], tag: Union[int, str] = 'latest'
+    ) -> Dict:
         """Returns information about a transaction by block number and transaction index position."""
         return await self._get(
             action='eth_getTransactionByBlockNumberAndIndex',
             index=check_hex(index),
             tag=check_tag(tag),
         )
 
@@ -62,19 +66,15 @@
             action='eth_getTransactionCount',
             address=address,
             tag=check_tag(tag),
         )
 
     async def send_raw_tx(self, raw_hex: str) -> Dict:
         """Creates new message call transaction or a contract creation for signed transactions."""
-        return await self._post(
-            module='proxy',
-            action='eth_sendRawTransaction',
-            hex=raw_hex
-        )
+        return await self._post(module='proxy', action='eth_sendRawTransaction', hex=raw_hex)
 
     async def tx_receipt(self, txhash: str) -> Dict:
         """Returns the receipt of a transaction by transaction hash."""
         return await self._get(
             action='eth_getTransactionReceipt',
             txhash=check_hex(txhash),
         )
@@ -103,15 +103,17 @@
             address=address,
             position=position,
             tag=check_tag(tag),
         )
 
     async def gas_price(self) -> str:
         """Returns the current price per gas in wei."""
-        return await self._get(action='eth_gasPrice', )
+        return await self._get(
+            action='eth_gasPrice',
+        )
 
     async def estimate_gas(self, to: str, value: str, gas_price: str, gas: str) -> str:
         """Makes a call or transaction, which won't be added to the blockchain and returns the used gas.
 
         Can be used for estimating the used gas.
         """
         return await self._get(
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/token.py` & `aioetherscan-0.8.9/aioetherscan/modules/token.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,103 +18,104 @@
         """Get ERC20-Token TotalSupply by ContractAddress"""
         return await self._get(
             module='stats',
             action='tokensupply',
             contractaddress=contract_address,
         )
 
-    async def account_balance(self, address: str, contract_address: str, tag: str = 'latest') -> str:
+    async def account_balance(
+        self, address: str, contract_address: str, tag: str = 'latest'
+    ) -> str:
         """Get ERC20-Token Account Balance for TokenContractAddress"""
         return await self._get(
             module='account',
             action='tokenbalance',
             address=address,
             contractaddress=contract_address,
-            tag=check_tag(tag)
+            tag=check_tag(tag),
         )
 
     async def total_supply_by_blockno(self, contract_address: str, blockno: int) -> str:
         """Get Historical ERC20-Token TotalSupply by ContractAddress & BlockNo"""
         return await self._get(
             module='stats',
             action='tokensupplyhistory',
             contractaddress=contract_address,
-            blockno=blockno
+            blockno=blockno,
         )
 
-    async def account_balance_by_blockno(self, address: str, contract_address: str, blockno: int) -> str:
+    async def account_balance_by_blockno(
+        self, address: str, contract_address: str, blockno: int
+    ) -> str:
         """Get Historical ERC20-Token Account Balance for TokenContractAddress by BlockNo"""
         return await self._get(
             module='account',
             action='tokenbalancehistory',
             address=address,
             contractaddress=contract_address,
-            blockno=blockno
+            blockno=blockno,
         )
 
     async def token_holder_list(
-            self,
-            contract_address: str,
-            page: int = None,
-            offset: int = None,
+        self,
+        contract_address: str,
+        page: int = None,
+        offset: int = None,
     ) -> List[Dict]:
         """Get Token Holder List by Contract Address"""
         return await self._get(
-            action='tokenholderlist',
-            contractaddress=contract_address,
-            page=page,
-            offset=offset
+            action='tokenholderlist', contractaddress=contract_address, page=page, offset=offset
         )
 
     async def token_info(
-            self,
-            contract_address: str = None,
+        self,
+        contract_address: str = None,
     ) -> List[Dict]:
         """Get Token Info by ContractAddress"""
         return await self._get(
             action='tokeninfo',
             contractaddress=contract_address,
         )
 
     async def token_holding_erc20(
-            self,
-            address: str,
-            page: int = None,
-            offset: int = None,
+        self,
+        address: str,
+        page: int = None,
+        offset: int = None,
     ) -> List[Dict]:
         """Get Address ERC20 Token Holding"""
         return await self._get(
             module='account',
             action='addresstokenbalance',
             address=address,
             page=page,
             offset=offset,
         )
 
     async def token_holding_erc721(
-            self,
-            address: str,
-            page: int = None,
-            offset: int = None,
+        self,
+        address: str,
+        page: int = None,
+        offset: int = None,
     ) -> List[Dict]:
-        """Get Address ERC721 Token Holding """
+        """Get Address ERC721 Token Holding"""
         return await self._get(
             module='account',
             action='addresstokennftbalance',
             address=address,
             page=page,
             offset=offset,
         )
 
     async def token_inventory(
-            self,
-            address: str,
-            contract_address: str,
-            page: int = None,
-            offset: int = None,
+        self,
+        address: str,
+        contract_address: str,
+        page: int = None,
+        offset: int = None,
     ) -> List[Dict]:
         """Get Address ERC721 Token Inventory By Contract Address"""
         return await self._get(
             module='account',
             action='addresstokennftinventory',
             address=address,
             contractaddress=contract_address,
```

### Comparing `aioetherscan-0.8.8/aioetherscan/modules/transaction.py` & `aioetherscan-0.8.9/aioetherscan/modules/transaction.py`

 * *Files 24% similar despite different names*

```diff
@@ -10,19 +10,13 @@
     """
 
     @property
     def _module(self) -> str:
         return 'transaction'
 
     async def contract_execution_status(self, txhash: str) -> Dict:
-        """[BETA] Check Contract Execution Status (if there was an error during contract execution) """
-        return await self._get(
-            action='getstatus',
-            txhash=txhash
-        )
+        """[BETA] Check Contract Execution Status (if there was an error during contract execution)"""
+        return await self._get(action='getstatus', txhash=txhash)
 
     async def tx_receipt_status(self, txhash: str) -> Dict:
-        """[BETA] Check Transaction Receipt Status (Only applicable for Post Byzantium fork transactions) """
-        return await self._get(
-            action='gettxreceiptstatus',
-            txhash=txhash
-        )
+        """[BETA] Check Transaction Receipt Status (Only applicable for Post Byzantium fork transactions)"""
+        return await self._get(action='gettxreceiptstatus', txhash=txhash)
```

### Comparing `aioetherscan-0.8.8/aioetherscan/network.py` & `aioetherscan-0.8.9/aioetherscan/network.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,23 +6,33 @@
 import aiohttp
 from aiohttp import ClientTimeout
 from aiohttp.client import ClientSession
 from aiohttp.hdrs import METH_GET, METH_POST
 from aiohttp_retry import RetryOptionsBase, RetryClient
 from asyncio_throttle import Throttler
 
-from aioetherscan.exceptions import EtherscanClientContentTypeError, EtherscanClientError, EtherscanClientApiError, \
-    EtherscanClientProxyError
+from aioetherscan.exceptions import (
+    EtherscanClientContentTypeError,
+    EtherscanClientError,
+    EtherscanClientApiError,
+    EtherscanClientProxyError,
+)
 from aioetherscan.url_builder import UrlBuilder
 
 
 class Network:
-    def __init__(self, url_builder: UrlBuilder,
-                 loop: Optional[AbstractEventLoop], timeout: Optional[ClientTimeout], proxy: Optional[str],
-                 throttler: Optional[AsyncContextManager], retry_options: Optional[RetryOptionsBase]) -> None:
+    def __init__(
+        self,
+        url_builder: UrlBuilder,
+        loop: Optional[AbstractEventLoop],
+        timeout: Optional[ClientTimeout],
+        proxy: Optional[str],
+        throttler: Optional[AsyncContextManager],
+        retry_options: Optional[RetryOptionsBase],
+    ) -> None:
         self._url_builder = url_builder
 
         self._loop = loop or asyncio.get_event_loop()
         self._timeout = timeout
 
         self._proxy = proxy
 
@@ -46,27 +56,29 @@
 
     def _get_retry_client(self) -> RetryClient:
         if self._timeout is not None:
             session = ClientSession(loop=self._loop, timeout=self._timeout)
         else:
             session = ClientSession(loop=self._loop)
 
-        return RetryClient(
-            client_session=session,
-            retry_options=self._retry_options
-        )
+        return RetryClient(client_session=session, retry_options=self._retry_options)
 
-    async def _request(self, method: str, data: Dict = None, params: Dict = None) -> Union[Dict, List, str]:
+    async def _request(
+        self, method: str, data: Dict = None, params: Dict = None
+    ) -> Union[Dict, List, str]:
         if self._retry_client is None:
             self._retry_client = self._get_retry_client()
         session_method = getattr(self._retry_client, method.lower())
         async with self._throttler:
-            async with session_method(self._url_builder.API_URL, params=params, data=data,
-                                      proxy=self._proxy) as response:
-                self._logger.debug('[%s] %r %r %s', method, str(response.url), data, response.status)
+            async with session_method(
+                self._url_builder.API_URL, params=params, data=data, proxy=self._proxy
+            ) as response:
+                self._logger.debug(
+                    '[%s] %r %r %s', method, str(response.url), data, response.status
+                )
                 return await self._handle_response(response)
 
     async def _handle_response(self, response: aiohttp.ClientResponse) -> Union[Dict, list, str]:
         try:
             response_json = await response.json()
         except aiohttp.ContentTypeError:
             raise EtherscanClientContentTypeError(response.status, await response.text())
```

### Comparing `aioetherscan-0.8.8/aioetherscan/url_builder.py` & `aioetherscan-0.8.9/aioetherscan/url_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,17 @@
 
         self.API_URL = self._get_api_url()
         self.BASE_URL = self._get_base_url()
 
     def _set_api_kind(self, api_kind: str) -> None:
         api_kind = api_kind.lower().strip()
         if api_kind not in self._API_KINDS:
-            raise ValueError(f'Incorrect api_kind {api_kind!r}, supported only: {", ".join(self._API_KINDS)}')
+            raise ValueError(
+                f'Incorrect api_kind {api_kind!r}, supported only: {", ".join(self._API_KINDS)}'
+            )
         else:
             self._api_kind = api_kind
 
     @property
     def _is_main(self) -> bool:
         return self._network == 'main'
 
@@ -60,32 +62,28 @@
         }
         default_prefix = 'api' if self._is_main else f'api-{self._network}'
         prefix = prefix_exceptions.get((self._api_kind, self._is_main), default_prefix)
 
         return self._build_url(prefix, 'api')
 
     def _get_base_url(self) -> str:
-        network_exceptions = {
-            ('polygon', 'testnet'): 'mumbai'
-        }
+        network_exceptions = {('polygon', 'testnet'): 'mumbai'}
         network = network_exceptions.get((self._api_kind, self._network), self._network)
 
         prefix_exceptions = {
             ('optimism', True): 'optimistic',
             ('optimism', False): f'{network}-optimism',
         }
         default_prefix = None if self._is_main else network
         prefix = prefix_exceptions.get((self._api_kind, self._is_main), default_prefix)
 
         return self._build_url(prefix)
 
     def filter_and_sign(self, params: Dict):
-        return self._sign(
-            self._filter_params(params or {})
-        )
+        return self._sign(self._filter_params(params or {}))
 
     def _sign(self, params: Dict) -> Dict:
         if not params:
             params = {}
         params['apikey'] = self._API_KEY
         return params
```

### Comparing `aioetherscan-0.8.8/pyproject.toml` & `aioetherscan-0.8.9/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 [tool.poetry]
 name = "aioetherscan"
-version = "0.8.8"
+version = "0.8.9"
 description = "Etherscan API async Python wrapper"
 authors = ["ape364 <ape364@gmail.com>"]
 license = "MIT"
 homepage = "https://github.com/ape364/aioetherscan"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 aiohttp = "^3.4"
 asyncio_throttle = "^1.0.1"
 aiohttp-retry = "^2.8.3"
 
 [tool.poetry.dev-dependencies]
 pytest = "^7.1.2"
-pytest-asyncio = "^0.20.3"
-pre-commit = "^3.1.1"
+pytest-asyncio = "^0.21.1"
+pre-commit = "^3.5.0"
 coveralls = "^3.3.1"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
 
 [tool.pytest.ini_options]
 pythonpath = [
     "."
 ]
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 relative_files = true
+
+[tool.ruff]
+line-length = 100
+
+[tool.ruff.format]
+quote-style = "single"
```

### Comparing `aioetherscan-0.8.8/PKG-INFO` & `aioetherscan-0.8.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioetherscan
-Version: 0.8.8
+Version: 0.8.9
 Summary: Etherscan API async Python wrapper
 Home-page: https://github.com/ape364/aioetherscan
 License: MIT
 Author: ape364
 Author-email: ape364@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

