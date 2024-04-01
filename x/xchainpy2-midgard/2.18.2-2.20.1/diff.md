# Comparing `tmp/xchainpy2-midgard-2.18.2.tar.gz` & `tmp/xchainpy2-midgard-2.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2-midgard-2.18.2.tar", last modified: Sun Dec 24 07:19:27 2023, max compression
+gzip compressed data, was "xchainpy2-midgard-2.20.1.tar", last modified: Mon Apr  1 11:01:21 2024, max compression
```

## Comparing `xchainpy2-midgard-2.18.2.tar` & `xchainpy2-midgard-2.20.1.tar`

### file list

```diff
@@ -1,151 +1,151 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.363809 xchainpy2-midgard-2.18.2/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)     8841 2023-12-24 07:19:27.363388 xchainpy2-midgard-2.18.2/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     8475 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2023-12-24 07:19:27.363850 xchainpy2-midgard-2.18.2/setup.cfg
--rw-r--r--   0 tirinox    (501) staff       (20)     1682 2023-12-24 07:16:50.000000 xchainpy2-midgard-2.18.2/setup.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.339242 xchainpy2-midgard-2.18.2/test/
--rw-r--r--   0 tirinox    (501) staff       (20)       15 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1227 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_action.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_action_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1343 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_add_liquidity_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1235 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_balance.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_block_rewards.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1269 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_bond_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1301 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_borrower_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_borrower_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1251 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_borrowers.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1253 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_churn_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1227 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_churns.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1211 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1219 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_coins.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4711 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_default_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_depth_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1351 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_depth_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1311 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_depth_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1345 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_depth_history_item_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1311 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_depth_history_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1301 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_earnings_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1375 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_earnings_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1335 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_earnings_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1369 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_earnings_history_item_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_genesis_inf.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1227 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_health.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1245 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_height_ts.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1317 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_inline_response200.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_known_pools.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1309 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_liquidity_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1383 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_liquidity_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1343 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_liquidity_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1285 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_member_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_member_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1235 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_members.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1243 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1235 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_network.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1269 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_network_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1211 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1219 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_nodes.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_pool_detail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1269 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_pool_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1303 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_pool_stats_detail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1293 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_refund_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1311 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_reverse_thor_names.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_saver_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1253 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_saver_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1285 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_savers_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1359 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_savers_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1319 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_savers_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1319 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_savers_history_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1342 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_specification_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1253 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_stats_data.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1319 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_streaming_swap_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1269 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_swap_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1343 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_swap_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1303 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_swap_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_swap_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1303 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_thor_name_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1287 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_thor_name_entry.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1267 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_transaction.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1261 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_tvl_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1335 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_tvl_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1295 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_tvl_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1309 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/test/test_withdraw_metadata.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.344249 xchainpy2-midgard-2.18.2/xchainpy2_midgard/
--rw-r--r--   0 tirinox    (501) staff       (20)     5098 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.346178 xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/
--rw-r--r--   0 tirinox    (501) staff       (20)      213 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)   117276 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/default_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6966 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/specification_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25443 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/api_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8326 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/configuration.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.362715 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/
--rw-r--r--   0 tirinox    (501) staff       (20)     4814 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9753 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/action.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5116 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/action_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3970 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/add_liquidity_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5207 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/balance.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5227 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/block_rewards.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14666 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/bond_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3710 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrower_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11784 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrower_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2778 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrowers.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4480 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/churn_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2766 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/churns.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4271 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2762 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/coins.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4306 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2826 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14644 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4852 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_item_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)    18100 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4360 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2838 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)    13294 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10464 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_item_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4294 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/genesis_inf.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9610 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/health.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4397 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/height_ts.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5398 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/inline_response200.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3018 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/known_pools.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4378 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2842 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)    18064 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3716 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/member_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)    17170 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/member_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2770 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/members.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5465 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16994 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/network.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2786 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/network_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5233 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2762 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/nodes.py
--rw-r--r--   0 tirinox    (501) staff       (20)    22054 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_detail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2786 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)    40215 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_stats_detail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7321 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/refund_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2806 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/reverse_thor_names.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3679 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/saver_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11766 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/saver_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4324 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2830 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7751 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11414 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)    22584 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/stats_data.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11131 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/streaming_swap_meta.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4288 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2822 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)    28593 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11368 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5412 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/thor_name_details.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4358 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/thor_name_entry.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6001 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/transaction.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4270 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2818 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history_intervals.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10277 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9038 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/withdraw_metadata.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11024 2023-12-24 07:16:04.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard/rest.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:19:27.363033 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)     8841 2023-12-24 07:19:27.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     5003 2023-12-24 07:19:27.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2023-12-24 07:19:27.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       56 2023-12-24 07:19:27.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       23 2023-12-24 07:19:27.000000 xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.620902 xchainpy2-midgard-2.20.1/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)     8841 2024-04-01 11:01:21.620659 xchainpy2-midgard-2.20.1/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     8475 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-04-01 11:01:21.620935 xchainpy2-midgard-2.20.1/setup.cfg
+-rw-r--r--   0 tirinox    (501) staff       (20)     1682 2024-04-01 11:00:36.000000 xchainpy2-midgard-2.20.1/setup.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.599922 xchainpy2-midgard-2.20.1/test/
+-rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1227 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_action.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_action_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1343 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_add_liquidity_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1235 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_balance.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_block_rewards.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1269 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_bond_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1301 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_borrower_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_borrower_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1251 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_borrowers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1253 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_churn_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1227 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_churns.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1211 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1219 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_coins.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4711 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_default_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_depth_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1351 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_depth_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1311 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_depth_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1345 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_depth_history_item_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1311 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_depth_history_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1301 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_earnings_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1375 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_earnings_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1335 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_earnings_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1369 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_earnings_history_item_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_genesis_inf.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1227 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_health.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1245 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_height_ts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1317 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_inline_response200.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_known_pools.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1309 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_liquidity_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1383 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_liquidity_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1343 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_liquidity_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1285 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_member_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_member_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1235 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_members.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1243 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1235 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_network.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1269 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_network_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1211 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1219 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_nodes.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_pool_detail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1269 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_pool_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1303 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_pool_stats_detail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1293 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_refund_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1311 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_reverse_thor_names.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_saver_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1253 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_saver_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1285 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_savers_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1359 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_savers_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1319 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_savers_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1319 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_savers_history_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1342 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_specification_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1253 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_stats_data.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1319 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_streaming_swap_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1269 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_swap_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1343 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_swap_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1303 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_swap_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_swap_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1303 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_thor_name_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1287 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_thor_name_entry.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1267 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_transaction.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1261 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_tvl_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1335 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_tvl_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1295 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_tvl_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1309 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/test/test_withdraw_metadata.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.600693 xchainpy2-midgard-2.20.1/xchainpy2_midgard/
+-rw-r--r--   0 tirinox    (501) staff       (20)     5098 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.602712 xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/
+-rw-r--r--   0 tirinox    (501) staff       (20)      213 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)   117276 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/default_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6966 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/specification_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25443 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/api_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8422 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/configuration.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.620021 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/
+-rw-r--r--   0 tirinox    (501) staff       (20)     4814 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9753 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/action.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5116 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/action_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3970 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/add_liquidity_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5207 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/balance.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5227 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/block_rewards.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14666 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/bond_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3710 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrower_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11784 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrower_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2778 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrowers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4480 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/churn_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2766 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/churns.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4271 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2762 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/coins.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4306 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2826 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14644 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4852 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_item_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    18100 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4360 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2838 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    13294 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10464 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_item_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4294 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/genesis_inf.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9610 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/health.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4397 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/height_ts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5398 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/inline_response200.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3018 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/known_pools.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4378 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2842 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16545 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3716 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/member_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    17170 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/member_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2770 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/members.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5465 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16994 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/network.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2786 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/network_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5233 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2762 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/nodes.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    26184 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_detail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2786 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    42575 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_stats_detail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7321 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/refund_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2806 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/reverse_thor_names.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3679 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/saver_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11766 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/saver_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4324 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2830 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7751 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11414 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    21207 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/stats_data.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11131 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/streaming_swap_meta.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4288 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2822 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    34806 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11368 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5412 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/thor_name_details.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4358 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/thor_name_entry.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6001 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/transaction.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4270 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2818 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history_intervals.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10277 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9038 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/withdraw_metadata.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11024 2024-04-01 10:50:15.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard/rest.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 11:01:21.620361 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)     8841 2024-04-01 11:01:21.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)     5003 2024-04-01 11:01:21.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-04-01 11:01:21.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-04-01 11:01:21.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       23 2024-04-01 11:01:21.000000 xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/top_level.txt
```

### Comparing `xchainpy2-midgard-2.18.2/LICENSE` & `xchainpy2-midgard-2.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2-midgard-2.18.2/PKG-INFO` & `xchainpy2-midgard-2.20.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-midgard
-Version: 2.18.2
+Version: 2.20.1
 Summary: Midgard Public API
 Home-page: 
 Author-email: devs@thorchain.org
 Keywords: Swagger,Midgard Public API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-midgard
 The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 2.18.2
-- Package version: 2.18.2
+- API version: 2.20.1
+- Package version: 2.20.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `xchainpy2-midgard-2.18.2/README.md` & `xchainpy2-midgard-2.20.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # xchainpy2-midgard
 The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 2.18.2
-- Package version: 2.18.2
+- API version: 2.20.1
+- Package version: 2.20.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `xchainpy2-midgard-2.18.2/setup.py` & `xchainpy2-midgard-2.20.1/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "xchainpy2-midgard"
-VERSION = "2.18.2"
+VERSION = "2.20.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_action.py` & `xchainpy2-midgard-2.20.1/test/test_action.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_action_meta.py` & `xchainpy2-midgard-2.20.1/test/test_action_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_add_liquidity_metadata.py` & `xchainpy2-midgard-2.20.1/test/test_add_liquidity_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_balance.py` & `xchainpy2-midgard-2.20.1/test/test_balance.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_block_rewards.py` & `xchainpy2-midgard-2.20.1/test/test_block_rewards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_bond_metrics.py` & `xchainpy2-midgard-2.20.1/test/test_bond_metrics.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_borrower_details.py` & `xchainpy2-midgard-2.20.1/test/test_borrower_details.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_borrower_pool.py` & `xchainpy2-midgard-2.20.1/test/test_borrower_pool.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_borrowers.py` & `xchainpy2-midgard-2.20.1/test/test_borrowers.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_churn_item.py` & `xchainpy2-midgard-2.20.1/test/test_churn_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_churns.py` & `xchainpy2-midgard-2.20.1/test/test_churns.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_coin.py` & `xchainpy2-midgard-2.20.1/test/test_nodes.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.coin import Coin  # noqa: E501
+from xchainpy2_midgard.models.nodes import Nodes  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestCoin(unittest.TestCase):
-    """Coin unit test stubs"""
+class TestNodes(unittest.TestCase):
+    """Nodes unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testCoin(self):
-        """Test Coin"""
+    def testNodes(self):
+        """Test Nodes"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.coin.Coin()  # noqa: E501
+        # model = xchainpy2_midgard.models.nodes.Nodes()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_coins.py` & `xchainpy2-midgard-2.20.1/test/test_coins.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_default_api.py` & `xchainpy2-midgard-2.20.1/test/test_default_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_depth_history.py` & `xchainpy2-midgard-2.20.1/test/test_depth_history.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_depth_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_depth_history_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_depth_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_depth_history_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_depth_history_item_pool.py` & `xchainpy2-midgard-2.20.1/test/test_depth_history_item_pool.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_depth_history_meta.py` & `xchainpy2-midgard-2.20.1/test/test_depth_history_meta.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_earnings_history.py` & `xchainpy2-midgard-2.20.1/test/test_earnings_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_earnings_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_earnings_history_intervals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_earnings_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_earnings_history_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_earnings_history_item_pool.py` & `xchainpy2-midgard-2.20.1/test/test_earnings_history_item_pool.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_genesis_inf.py` & `xchainpy2-midgard-2.20.1/test/test_genesis_inf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_health.py` & `xchainpy2-midgard-2.20.1/test/test_health.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_height_ts.py` & `xchainpy2-midgard-2.20.1/test/test_height_ts.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_inline_response200.py` & `xchainpy2-midgard-2.20.1/test/test_inline_response200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_known_pools.py` & `xchainpy2-midgard-2.20.1/test/test_known_pools.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_liquidity_history.py` & `xchainpy2-midgard-2.20.1/test/test_liquidity_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_liquidity_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_liquidity_history_intervals.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_liquidity_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_liquidity_history_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_member_details.py` & `xchainpy2-midgard-2.20.1/test/test_member_details.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_member_pool.py` & `xchainpy2-midgard-2.20.1/test/test_member_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_members.py` & `xchainpy2-midgard-2.20.1/test/test_members.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_metadata.py` & `xchainpy2-midgard-2.20.1/test/test_swap_metadata.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.metadata import Metadata  # noqa: E501
+from xchainpy2_midgard.models.swap_metadata import SwapMetadata  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestMetadata(unittest.TestCase):
-    """Metadata unit test stubs"""
+class TestSwapMetadata(unittest.TestCase):
+    """SwapMetadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testMetadata(self):
-        """Test Metadata"""
+    def testSwapMetadata(self):
+        """Test SwapMetadata"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.metadata.Metadata()  # noqa: E501
+        # model = xchainpy2_midgard.models.swap_metadata.SwapMetadata()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_network.py` & `xchainpy2-midgard-2.20.1/test/test_network_fees.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.network import Network  # noqa: E501
+from xchainpy2_midgard.models.network_fees import NetworkFees  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestNetwork(unittest.TestCase):
-    """Network unit test stubs"""
+class TestNetworkFees(unittest.TestCase):
+    """NetworkFees unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNetwork(self):
-        """Test Network"""
+    def testNetworkFees(self):
+        """Test NetworkFees"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.network.Network()  # noqa: E501
+        # model = xchainpy2_midgard.models.network_fees.NetworkFees()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_network_fees.py` & `xchainpy2-midgard-2.20.1/test/test_refund_metadata.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.network_fees import NetworkFees  # noqa: E501
+from xchainpy2_midgard.models.refund_metadata import RefundMetadata  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestNetworkFees(unittest.TestCase):
-    """NetworkFees unit test stubs"""
+class TestRefundMetadata(unittest.TestCase):
+    """RefundMetadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNetworkFees(self):
-        """Test NetworkFees"""
+    def testRefundMetadata(self):
+        """Test RefundMetadata"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.network_fees.NetworkFees()  # noqa: E501
+        # model = xchainpy2_midgard.models.refund_metadata.RefundMetadata()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_node.py` & `xchainpy2-midgard-2.20.1/test/test_node.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_nodes.py` & `xchainpy2-midgard-2.20.1/test/test_transaction.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.nodes import Nodes  # noqa: E501
+from xchainpy2_midgard.models.transaction import Transaction  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestNodes(unittest.TestCase):
-    """Nodes unit test stubs"""
+class TestTransaction(unittest.TestCase):
+    """Transaction unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testNodes(self):
-        """Test Nodes"""
+    def testTransaction(self):
+        """Test Transaction"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.nodes.Nodes()  # noqa: E501
+        # model = xchainpy2_midgard.models.transaction.Transaction()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_pool_detail.py` & `xchainpy2-midgard-2.20.1/test/test_pool_detail.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_pool_details.py` & `xchainpy2-midgard-2.20.1/test/test_pool_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_pool_stats_detail.py` & `xchainpy2-midgard-2.20.1/test/test_pool_stats_detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_refund_metadata.py` & `xchainpy2-midgard-2.20.1/test/test_savers_history_meta.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.refund_metadata import RefundMetadata  # noqa: E501
+from xchainpy2_midgard.models.savers_history_meta import SaversHistoryMeta  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestRefundMetadata(unittest.TestCase):
-    """RefundMetadata unit test stubs"""
+class TestSaversHistoryMeta(unittest.TestCase):
+    """SaversHistoryMeta unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testRefundMetadata(self):
-        """Test RefundMetadata"""
+    def testSaversHistoryMeta(self):
+        """Test SaversHistoryMeta"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.refund_metadata.RefundMetadata()  # noqa: E501
+        # model = xchainpy2_midgard.models.savers_history_meta.SaversHistoryMeta()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_reverse_thor_names.py` & `xchainpy2-midgard-2.20.1/test/test_reverse_thor_names.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_saver_details.py` & `xchainpy2-midgard-2.20.1/test/test_saver_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_saver_pool.py` & `xchainpy2-midgard-2.20.1/test/test_saver_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_savers_history.py` & `xchainpy2-midgard-2.20.1/test/test_savers_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_savers_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_savers_history_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_savers_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_savers_history_item.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_savers_history_meta.py` & `xchainpy2-midgard-2.20.1/test/test_tvl_history.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.savers_history_meta import SaversHistoryMeta  # noqa: E501
+from xchainpy2_midgard.models.tvl_history import TVLHistory  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestSaversHistoryMeta(unittest.TestCase):
-    """SaversHistoryMeta unit test stubs"""
+class TestTVLHistory(unittest.TestCase):
+    """TVLHistory unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaversHistoryMeta(self):
-        """Test SaversHistoryMeta"""
+    def testTVLHistory(self):
+        """Test TVLHistory"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.savers_history_meta.SaversHistoryMeta()  # noqa: E501
+        # model = xchainpy2_midgard.models.tvl_history.TVLHistory()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_specification_api.py` & `xchainpy2-midgard-2.20.1/test/test_specification_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_stats_data.py` & `xchainpy2-midgard-2.20.1/test/test_stats_data.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_streaming_swap_meta.py` & `xchainpy2-midgard-2.20.1/test/test_streaming_swap_meta.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_swap_history.py` & `xchainpy2-midgard-2.20.1/test/test_swap_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_swap_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_swap_history_intervals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_swap_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_swap_history_item.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_swap_metadata.py` & `xchainpy2-midgard-2.20.1/test/test_metadata.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.swap_metadata import SwapMetadata  # noqa: E501
+from xchainpy2_midgard.models.metadata import Metadata  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestSwapMetadata(unittest.TestCase):
-    """SwapMetadata unit test stubs"""
+class TestMetadata(unittest.TestCase):
+    """Metadata unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSwapMetadata(self):
-        """Test SwapMetadata"""
+    def testMetadata(self):
+        """Test Metadata"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.swap_metadata.SwapMetadata()  # noqa: E501
+        # model = xchainpy2_midgard.models.metadata.Metadata()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_thor_name_details.py` & `xchainpy2-midgard-2.20.1/test/test_thor_name_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_thor_name_entry.py` & `xchainpy2-midgard-2.20.1/test/test_thor_name_entry.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_transaction.py` & `xchainpy2-midgard-2.20.1/test/test_coin.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.transaction import Transaction  # noqa: E501
+from xchainpy2_midgard.models.coin import Coin  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestTransaction(unittest.TestCase):
-    """Transaction unit test stubs"""
+class TestCoin(unittest.TestCase):
+    """Coin unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTransaction(self):
-        """Test Transaction"""
+    def testCoin(self):
+        """Test Coin"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.transaction.Transaction()  # noqa: E501
+        # model = xchainpy2_midgard.models.coin.Coin()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_tvl_history.py` & `xchainpy2-midgard-2.20.1/test/test_tvl_history_intervals.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.tvl_history import TVLHistory  # noqa: E501
+from xchainpy2_midgard.models.tvl_history_intervals import TVLHistoryIntervals  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestTVLHistory(unittest.TestCase):
-    """TVLHistory unit test stubs"""
+class TestTVLHistoryIntervals(unittest.TestCase):
+    """TVLHistoryIntervals unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTVLHistory(self):
-        """Test TVLHistory"""
+    def testTVLHistoryIntervals(self):
+        """Test TVLHistoryIntervals"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.tvl_history.TVLHistory()  # noqa: E501
+        # model = xchainpy2_midgard.models.tvl_history_intervals.TVLHistoryIntervals()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_tvl_history_intervals.py` & `xchainpy2-midgard-2.20.1/test/test_network.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_midgard
-from xchainpy2_midgard.models.tvl_history_intervals import TVLHistoryIntervals  # noqa: E501
+from xchainpy2_midgard.models.network import Network  # noqa: E501
 from xchainpy2_midgard.rest import ApiException
 
 
-class TestTVLHistoryIntervals(unittest.TestCase):
-    """TVLHistoryIntervals unit test stubs"""
+class TestNetwork(unittest.TestCase):
+    """Network unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTVLHistoryIntervals(self):
-        """Test TVLHistoryIntervals"""
+    def testNetwork(self):
+        """Test Network"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_midgard.models.tvl_history_intervals.TVLHistoryIntervals()  # noqa: E501
+        # model = xchainpy2_midgard.models.network.Network()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_tvl_history_item.py` & `xchainpy2-midgard-2.20.1/test/test_tvl_history_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/test/test_withdraw_metadata.py` & `xchainpy2-midgard-2.20.1/test/test_withdraw_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/__init__.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/default_api.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/default_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -1413,15 +1413,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_pool(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: pool name (required)
-        :param str period: Specifies the base interval from which APY is extrapolated. Default is 30d. 
+        :param str period: Specifies the base interval from which APY is extrapolated. Default is 14d. 
         :return: PoolDetail
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_pool_with_http_info(asset, **kwargs)  # noqa: E501
@@ -1436,15 +1436,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_pool_with_http_info(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: pool name (required)
-        :param str period: Specifies the base interval from which APY is extrapolated. Default is 30d. 
+        :param str period: Specifies the base interval from which APY is extrapolated. Default is 14d. 
         :return: PoolDetail
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['asset', 'period']  # noqa: E501
         all_params.append('async_req')
@@ -1512,15 +1512,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_pool_stats(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: pool name (required)
-        :param str period: Restricts aggregation type fields to the last period only. Default is 30d. 
+        :param str period: Restricts aggregation type fields to the last period only. Default is 14d. 
         :return: PoolStatsDetail
                  If the method is called asynchronously,
                  returns the request thread.
         """
         kwargs['_return_http_data_only'] = True
         if kwargs.get('async_req'):
             return self.get_pool_stats_with_http_info(asset, **kwargs)  # noqa: E501
@@ -1535,15 +1535,15 @@
         This method makes a synchronous HTTP request by default. To make an
         asynchronous HTTP request, please pass async_req=True
         >>> thread = api.get_pool_stats_with_http_info(asset, async_req=True)
         >>> result = thread.get()
 
         :param async_req bool
         :param str asset: pool name (required)
-        :param str period: Restricts aggregation type fields to the last period only. Default is 30d. 
+        :param str period: Restricts aggregation type fields to the last period only. Default is 14d. 
         :return: PoolStatsDetail
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
         all_params = ['asset', 'period']  # noqa: E501
         all_params.append('async_req')
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/api/specification_api.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/api/specification_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/api_client.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 from __future__ import absolute_import
 
 import datetime
 import json
@@ -68,15 +68,15 @@
         self.pool = ThreadPool()
         self.rest_client = rest.RESTClientObject(configuration)
         self.default_headers = {}
         if header_name is not None:
             self.default_headers[header_name] = header_value
         self.cookie = cookie
         # Set default User-Agent.
-        self.user_agent = 'Swagger-Codegen/2.18.2/python'
+        self.user_agent = 'Swagger-Codegen/2.20.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/configuration.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/configuration.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import copy
@@ -215,17 +215,20 @@
                 return key
 
     def get_basic_auth_token(self):
         """Gets HTTP basic authentication header (string).
 
         :return: The token for basic HTTP authentication.
         """
-        return urllib3.util.make_headers(
-            basic_auth=self.username + ':' + self.password
-        ).get('authorization')
+        token = ""
+        if self.username or self.password:
+            token = urllib3.util.make_headers(
+                basic_auth=self.username + ':' + self.password
+            ).get('authorization')
+        return token
 
     def auth_settings(self):
         """Gets Auth Settings dict for api client.
 
         :return: The Auth Settings information dict.
         """
         return {
@@ -235,10 +238,10 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 2.18.2\n"\
-               "SDK Package Version: 2.18.2".\
+               "Version of the API: 2.20.1\n"\
+               "SDK Package Version: 2.20.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/__init__.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/action.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/action.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/action_meta.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/action_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/add_liquidity_metadata.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/add_liquidity_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/balance.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/balance.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/block_rewards.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/block_rewards.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/bond_metrics.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/bond_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrower_details.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrower_details.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrower_pool.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrower_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/borrowers.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/borrowers.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/churn_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/churn_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/churns.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/network_fees.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Churns(object):
+class NetworkFees(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """Churns - a model defined in Swagger"""  # noqa: E501
+        """NetworkFees - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Churns, dict):
+        if issubclass(NetworkFees, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Churns):
+        if not isinstance(other, NetworkFees):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/coin.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/coin.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/coins.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/churns.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Coins(object):
+class Churns(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """Coins - a model defined in Swagger"""  # noqa: E501
+        """Churns - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Coins, dict):
+        if issubclass(Churns, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Coins):
+        if not isinstance(other, Churns):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_intervals.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_item_pool.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_item_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/depth_history_meta.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/depth_history_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_intervals.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/earnings_history_item_pool.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/earnings_history_item_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/genesis_inf.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/genesis_inf.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/health.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/health.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/height_ts.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/height_ts.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/inline_response200.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/inline_response200.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/known_pools.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/known_pools.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/liquidity_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/liquidity_history_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -29,15 +29,14 @@
     """
     swagger_types = {
         'add_asset_liquidity_volume': 'str',
         'add_liquidity_count': 'str',
         'add_liquidity_volume': 'str',
         'add_rune_liquidity_volume': 'str',
         'end_time': 'str',
-        'impermanent_loss_protection_paid': 'str',
         'net': 'str',
         'rune_price_usd': 'str',
         'start_time': 'str',
         'withdraw_asset_volume': 'str',
         'withdraw_count': 'str',
         'withdraw_rune_volume': 'str',
         'withdraw_volume': 'str'
@@ -45,46 +44,43 @@
 
     attribute_map = {
         'add_asset_liquidity_volume': 'addAssetLiquidityVolume',
         'add_liquidity_count': 'addLiquidityCount',
         'add_liquidity_volume': 'addLiquidityVolume',
         'add_rune_liquidity_volume': 'addRuneLiquidityVolume',
         'end_time': 'endTime',
-        'impermanent_loss_protection_paid': 'impermanentLossProtectionPaid',
         'net': 'net',
         'rune_price_usd': 'runePriceUSD',
         'start_time': 'startTime',
         'withdraw_asset_volume': 'withdrawAssetVolume',
         'withdraw_count': 'withdrawCount',
         'withdraw_rune_volume': 'withdrawRuneVolume',
         'withdraw_volume': 'withdrawVolume'
     }
 
-    def __init__(self, add_asset_liquidity_volume=None, add_liquidity_count=None, add_liquidity_volume=None, add_rune_liquidity_volume=None, end_time=None, impermanent_loss_protection_paid=None, net=None, rune_price_usd=None, start_time=None, withdraw_asset_volume=None, withdraw_count=None, withdraw_rune_volume=None, withdraw_volume=None):  # noqa: E501
+    def __init__(self, add_asset_liquidity_volume=None, add_liquidity_count=None, add_liquidity_volume=None, add_rune_liquidity_volume=None, end_time=None, net=None, rune_price_usd=None, start_time=None, withdraw_asset_volume=None, withdraw_count=None, withdraw_rune_volume=None, withdraw_volume=None):  # noqa: E501
         """LiquidityHistoryItem - a model defined in Swagger"""  # noqa: E501
         self._add_asset_liquidity_volume = None
         self._add_liquidity_count = None
         self._add_liquidity_volume = None
         self._add_rune_liquidity_volume = None
         self._end_time = None
-        self._impermanent_loss_protection_paid = None
         self._net = None
         self._rune_price_usd = None
         self._start_time = None
         self._withdraw_asset_volume = None
         self._withdraw_count = None
         self._withdraw_rune_volume = None
         self._withdraw_volume = None
         self.discriminator = None
         self.add_asset_liquidity_volume = add_asset_liquidity_volume
         self.add_liquidity_count = add_liquidity_count
         self.add_liquidity_volume = add_liquidity_volume
         self.add_rune_liquidity_volume = add_rune_liquidity_volume
         self.end_time = end_time
-        self.impermanent_loss_protection_paid = impermanent_loss_protection_paid
         self.net = net
         self.rune_price_usd = rune_price_usd
         self.start_time = start_time
         self.withdraw_asset_volume = withdraw_asset_volume
         self.withdraw_count = withdraw_count
         self.withdraw_rune_volume = withdraw_rune_volume
         self.withdraw_volume = withdraw_volume
@@ -211,39 +207,14 @@
         """
         if end_time is None:
             raise ValueError("Invalid value for `end_time`, must not be `None`")  # noqa: E501
 
         self._end_time = end_time
 
     @property
-    def impermanent_loss_protection_paid(self):
-        """Gets the impermanent_loss_protection_paid of this LiquidityHistoryItem.  # noqa: E501
-
-        Int64(e8), part of the withdrawRuneVolume which was payed because of impermanent loss protection.   # noqa: E501
-
-        :return: The impermanent_loss_protection_paid of this LiquidityHistoryItem.  # noqa: E501
-        :rtype: str
-        """
-        return self._impermanent_loss_protection_paid
-
-    @impermanent_loss_protection_paid.setter
-    def impermanent_loss_protection_paid(self, impermanent_loss_protection_paid):
-        """Sets the impermanent_loss_protection_paid of this LiquidityHistoryItem.
-
-        Int64(e8), part of the withdrawRuneVolume which was payed because of impermanent loss protection.   # noqa: E501
-
-        :param impermanent_loss_protection_paid: The impermanent_loss_protection_paid of this LiquidityHistoryItem.  # noqa: E501
-        :type: str
-        """
-        if impermanent_loss_protection_paid is None:
-            raise ValueError("Invalid value for `impermanent_loss_protection_paid`, must not be `None`")  # noqa: E501
-
-        self._impermanent_loss_protection_paid = impermanent_loss_protection_paid
-
-    @property
     def net(self):
         """Gets the net of this LiquidityHistoryItem.  # noqa: E501
 
         Int64(e8), net liquidity changes (withdrawals - deposits) during the time interval   # noqa: E501
 
         :return: The net of this LiquidityHistoryItem.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/member_details.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/member_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/member_pool.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/member_pool.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/members.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/members.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/metadata.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/network.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/network.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/network_fees.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history_intervals.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class NetworkFees(object):
+class TVLHistoryIntervals(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """NetworkFees - a model defined in Swagger"""  # noqa: E501
+        """TVLHistoryIntervals - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(NetworkFees, dict):
+        if issubclass(TVLHistoryIntervals, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, NetworkFees):
+        if not isinstance(other, TVLHistoryIntervals):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/node.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/nodes.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_details.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class Nodes(object):
+class PoolDetails(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """Nodes - a model defined in Swagger"""  # noqa: E501
+        """PoolDetails - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(Nodes, dict):
+        if issubclass(PoolDetails, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, Nodes):
+        if not isinstance(other, PoolDetails):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_detail.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_detail.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -29,15 +29,18 @@
     """
     swagger_types = {
         'annual_percentage_rate': 'str',
         'asset': 'str',
         'asset_depth': 'str',
         'asset_price': 'str',
         'asset_price_usd': 'str',
+        'earnings': 'str',
+        'earnings_annual_as_percent_of_depth': 'str',
         'liquidity_units': 'str',
+        'lp_luvi': 'str',
         'native_decimal': 'str',
         'pool_apy': 'str',
         'rune_depth': 'str',
         'savers_apr': 'str',
         'savers_depth': 'str',
         'savers_units': 'str',
         'status': 'str',
@@ -51,15 +54,18 @@
 
     attribute_map = {
         'annual_percentage_rate': 'annualPercentageRate',
         'asset': 'asset',
         'asset_depth': 'assetDepth',
         'asset_price': 'assetPrice',
         'asset_price_usd': 'assetPriceUSD',
+        'earnings': 'earnings',
+        'earnings_annual_as_percent_of_depth': 'earningsAnnualAsPercentOfDepth',
         'liquidity_units': 'liquidityUnits',
+        'lp_luvi': 'lpLuvi',
         'native_decimal': 'nativeDecimal',
         'pool_apy': 'poolAPY',
         'rune_depth': 'runeDepth',
         'savers_apr': 'saversAPR',
         'savers_depth': 'saversDepth',
         'savers_units': 'saversUnits',
         'status': 'status',
@@ -67,22 +73,25 @@
         'synth_units': 'synthUnits',
         'total_collateral': 'totalCollateral',
         'total_debt_tor': 'totalDebtTor',
         'units': 'units',
         'volume24h': 'volume24h'
     }
 
-    def __init__(self, annual_percentage_rate=None, asset=None, asset_depth=None, asset_price=None, asset_price_usd=None, liquidity_units=None, native_decimal=None, pool_apy=None, rune_depth=None, savers_apr=None, savers_depth=None, savers_units=None, status=None, synth_supply=None, synth_units=None, total_collateral=None, total_debt_tor=None, units=None, volume24h=None):  # noqa: E501
+    def __init__(self, annual_percentage_rate=None, asset=None, asset_depth=None, asset_price=None, asset_price_usd=None, earnings=None, earnings_annual_as_percent_of_depth=None, liquidity_units=None, lp_luvi=None, native_decimal=None, pool_apy=None, rune_depth=None, savers_apr=None, savers_depth=None, savers_units=None, status=None, synth_supply=None, synth_units=None, total_collateral=None, total_debt_tor=None, units=None, volume24h=None):  # noqa: E501
         """PoolDetail - a model defined in Swagger"""  # noqa: E501
         self._annual_percentage_rate = None
         self._asset = None
         self._asset_depth = None
         self._asset_price = None
         self._asset_price_usd = None
+        self._earnings = None
+        self._earnings_annual_as_percent_of_depth = None
         self._liquidity_units = None
+        self._lp_luvi = None
         self._native_decimal = None
         self._pool_apy = None
         self._rune_depth = None
         self._savers_apr = None
         self._savers_depth = None
         self._savers_units = None
         self._status = None
@@ -94,15 +103,18 @@
         self._volume24h = None
         self.discriminator = None
         self.annual_percentage_rate = annual_percentage_rate
         self.asset = asset
         self.asset_depth = asset_depth
         self.asset_price = asset_price
         self.asset_price_usd = asset_price_usd
+        self.earnings = earnings
+        self.earnings_annual_as_percent_of_depth = earnings_annual_as_percent_of_depth
         self.liquidity_units = liquidity_units
+        self.lp_luvi = lp_luvi
         self.native_decimal = native_decimal
         self.pool_apy = pool_apy
         self.rune_depth = rune_depth
         self.savers_apr = savers_apr
         self.savers_depth = savers_depth
         self.savers_units = savers_units
         self.status = status
@@ -113,26 +125,26 @@
         self.units = units
         self.volume24h = volume24h
 
     @property
     def annual_percentage_rate(self):
         """Gets the annual_percentage_rate of this PoolDetail.  # noqa: E501
 
-        Float, Also called APR. Annual return estimated linearly (not compounded) from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. Due to Impermanent Loss and Synths this might be negative, but given Impermanent Loss Protection for 100+ day members, frontends might show MAX(APR, 0).   # noqa: E501
+        Float, Annual Percentage Yield of earning to depth (earning/depth) estimated from a period (configurable by the period parameter, default is 14) E.g. 0.1 means 10% yearly return.   # noqa: E501
 
         :return: The annual_percentage_rate of this PoolDetail.  # noqa: E501
         :rtype: str
         """
         return self._annual_percentage_rate
 
     @annual_percentage_rate.setter
     def annual_percentage_rate(self, annual_percentage_rate):
         """Sets the annual_percentage_rate of this PoolDetail.
 
-        Float, Also called APR. Annual return estimated linearly (not compounded) from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. Due to Impermanent Loss and Synths this might be negative, but given Impermanent Loss Protection for 100+ day members, frontends might show MAX(APR, 0).   # noqa: E501
+        Float, Annual Percentage Yield of earning to depth (earning/depth) estimated from a period (configurable by the period parameter, default is 14) E.g. 0.1 means 10% yearly return.   # noqa: E501
 
         :param annual_percentage_rate: The annual_percentage_rate of this PoolDetail.  # noqa: E501
         :type: str
         """
         if annual_percentage_rate is None:
             raise ValueError("Invalid value for `annual_percentage_rate`, must not be `None`")  # noqa: E501
 
@@ -233,14 +245,64 @@
         """
         if asset_price_usd is None:
             raise ValueError("Invalid value for `asset_price_usd`, must not be `None`")  # noqa: E501
 
         self._asset_price_usd = asset_price_usd
 
     @property
+    def earnings(self):
+        """Gets the earnings of this PoolDetail.  # noqa: E501
+
+        Int64(e8), The earning that has been recorded from the pool asset's Liquidity Fees and Rewards in RUNE. The earnings shown are from the period parameter default being 14 days  (configurable by the period parameter).   # noqa: E501
+
+        :return: The earnings of this PoolDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._earnings
+
+    @earnings.setter
+    def earnings(self, earnings):
+        """Sets the earnings of this PoolDetail.
+
+        Int64(e8), The earning that has been recorded from the pool asset's Liquidity Fees and Rewards in RUNE. The earnings shown are from the period parameter default being 14 days  (configurable by the period parameter).   # noqa: E501
+
+        :param earnings: The earnings of this PoolDetail.  # noqa: E501
+        :type: str
+        """
+        if earnings is None:
+            raise ValueError("Invalid value for `earnings`, must not be `None`")  # noqa: E501
+
+        self._earnings = earnings
+
+    @property
+    def earnings_annual_as_percent_of_depth(self):
+        """Gets the earnings_annual_as_percent_of_depth of this PoolDetail.  # noqa: E501
+
+        Float, The estimation of earnings during the time interval expanded through a year  compared to the current pool depth. E.g. 0.1 means the pool based on this interval earnings can earn 10% of its pool during a year.   # noqa: E501
+
+        :return: The earnings_annual_as_percent_of_depth of this PoolDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._earnings_annual_as_percent_of_depth
+
+    @earnings_annual_as_percent_of_depth.setter
+    def earnings_annual_as_percent_of_depth(self, earnings_annual_as_percent_of_depth):
+        """Sets the earnings_annual_as_percent_of_depth of this PoolDetail.
+
+        Float, The estimation of earnings during the time interval expanded through a year  compared to the current pool depth. E.g. 0.1 means the pool based on this interval earnings can earn 10% of its pool during a year.   # noqa: E501
+
+        :param earnings_annual_as_percent_of_depth: The earnings_annual_as_percent_of_depth of this PoolDetail.  # noqa: E501
+        :type: str
+        """
+        if earnings_annual_as_percent_of_depth is None:
+            raise ValueError("Invalid value for `earnings_annual_as_percent_of_depth`, must not be `None`")  # noqa: E501
+
+        self._earnings_annual_as_percent_of_depth = earnings_annual_as_percent_of_depth
+
+    @property
     def liquidity_units(self):
         """Gets the liquidity_units of this PoolDetail.  # noqa: E501
 
         Int64, Liquidity Units in the pool.  # noqa: E501
 
         :return: The liquidity_units of this PoolDetail.  # noqa: E501
         :rtype: str
@@ -258,14 +320,39 @@
         """
         if liquidity_units is None:
             raise ValueError("Invalid value for `liquidity_units`, must not be `None`")  # noqa: E501
 
         self._liquidity_units = liquidity_units
 
     @property
+    def lp_luvi(self):
+        """Gets the lp_luvi of this PoolDetail.  # noqa: E501
+
+        Float, Annual yield estimated (compounding) from a period (default being 14d) configurable by the period parameter. Calculated from Liquidity Unit Value Index (LUVI). Due to Impermanent Loss and Synths Leverage this might be negative.   # noqa: E501
+
+        :return: The lp_luvi of this PoolDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._lp_luvi
+
+    @lp_luvi.setter
+    def lp_luvi(self, lp_luvi):
+        """Sets the lp_luvi of this PoolDetail.
+
+        Float, Annual yield estimated (compounding) from a period (default being 14d) configurable by the period parameter. Calculated from Liquidity Unit Value Index (LUVI). Due to Impermanent Loss and Synths Leverage this might be negative.   # noqa: E501
+
+        :param lp_luvi: The lp_luvi of this PoolDetail.  # noqa: E501
+        :type: str
+        """
+        if lp_luvi is None:
+            raise ValueError("Invalid value for `lp_luvi`, must not be `None`")  # noqa: E501
+
+        self._lp_luvi = lp_luvi
+
+    @property
     def native_decimal(self):
         """Gets the native_decimal of this PoolDetail.  # noqa: E501
 
         Int64, The native decimal number of the pool asset. (If the value is \"-1\", it means midgard doesn't know the pool native decimal)  # noqa: E501
 
         :return: The native_decimal of this PoolDetail.  # noqa: E501
         :rtype: str
@@ -286,26 +373,26 @@
 
         self._native_decimal = native_decimal
 
     @property
     def pool_apy(self):
         """Gets the pool_apy of this PoolDetail.  # noqa: E501
 
-        Float, MAX(AnnualPercentageRate, 0)   # noqa: E501
+        Float, Annual Percentage Yield of earning to depth (earning/depth) estimated from a period (configurable by the period parameter, default is 14) E.g. 0.1 means 10% yearly return.   # noqa: E501
 
         :return: The pool_apy of this PoolDetail.  # noqa: E501
         :rtype: str
         """
         return self._pool_apy
 
     @pool_apy.setter
     def pool_apy(self, pool_apy):
         """Sets the pool_apy of this PoolDetail.
 
-        Float, MAX(AnnualPercentageRate, 0)   # noqa: E501
+        Float, Annual Percentage Yield of earning to depth (earning/depth) estimated from a period (configurable by the period parameter, default is 14) E.g. 0.1 means 10% yearly return.   # noqa: E501
 
         :param pool_apy: The pool_apy of this PoolDetail.  # noqa: E501
         :type: str
         """
         if pool_apy is None:
             raise ValueError("Invalid value for `pool_apy`, must not be `None`")  # noqa: E501
 
@@ -336,26 +423,26 @@
 
         self._rune_depth = rune_depth
 
     @property
     def savers_apr(self):
         """Gets the savers_apr of this PoolDetail.  # noqa: E501
 
-        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
+        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 14). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
 
         :return: The savers_apr of this PoolDetail.  # noqa: E501
         :rtype: str
         """
         return self._savers_apr
 
     @savers_apr.setter
     def savers_apr(self, savers_apr):
         """Sets the savers_apr of this PoolDetail.
 
-        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
+        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 14). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
 
         :param savers_apr: The savers_apr of this PoolDetail.  # noqa: E501
         :type: str
         """
         if savers_apr is None:
             raise ValueError("Invalid value for `savers_apr`, must not be `None`")  # noqa: E501
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_details.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/coins.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class PoolDetails(object):
+class Coins(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """PoolDetails - a model defined in Swagger"""  # noqa: E501
+        """Coins - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(PoolDetails, dict):
+        if issubclass(Coins, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, PoolDetails):
+        if not isinstance(other, Coins):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/pool_stats_detail.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/pool_stats_detail.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -34,18 +34,20 @@
         'add_rune_liquidity_volume': 'str',
         'annual_percentage_rate': 'str',
         'asset': 'str',
         'asset_depth': 'str',
         'asset_price': 'str',
         'asset_price_usd': 'str',
         'average_slip': 'str',
-        'impermanent_loss_protection_paid': 'str',
+        'earnings': 'str',
+        'earnings_annual_as_percent_of_depth': 'str',
         'liquidity_units': 'str',
         'pool_apy': 'str',
         'rune_depth': 'str',
+        'savers_apr': 'str',
         'status': 'str',
         'swap_count': 'str',
         'swap_volume': 'str',
         'synth_supply': 'str',
         'synth_units': 'str',
         'to_asset_average_slip': 'str',
         'to_asset_count': 'str',
@@ -72,18 +74,20 @@
         'add_rune_liquidity_volume': 'addRuneLiquidityVolume',
         'annual_percentage_rate': 'annualPercentageRate',
         'asset': 'asset',
         'asset_depth': 'assetDepth',
         'asset_price': 'assetPrice',
         'asset_price_usd': 'assetPriceUSD',
         'average_slip': 'averageSlip',
-        'impermanent_loss_protection_paid': 'impermanentLossProtectionPaid',
+        'earnings': 'earnings',
+        'earnings_annual_as_percent_of_depth': 'earningsAnnualAsPercentOfDepth',
         'liquidity_units': 'liquidityUnits',
         'pool_apy': 'poolAPY',
         'rune_depth': 'runeDepth',
+        'savers_apr': 'saversAPR',
         'status': 'status',
         'swap_count': 'swapCount',
         'swap_volume': 'swapVolume',
         'synth_supply': 'synthSupply',
         'synth_units': 'synthUnits',
         'to_asset_average_slip': 'toAssetAverageSlip',
         'to_asset_count': 'toAssetCount',
@@ -99,30 +103,32 @@
         'units': 'units',
         'withdraw_asset_volume': 'withdrawAssetVolume',
         'withdraw_count': 'withdrawCount',
         'withdraw_rune_volume': 'withdrawRuneVolume',
         'withdraw_volume': 'withdrawVolume'
     }
 
-    def __init__(self, add_asset_liquidity_volume=None, add_liquidity_count=None, add_liquidity_volume=None, add_rune_liquidity_volume=None, annual_percentage_rate=None, asset=None, asset_depth=None, asset_price=None, asset_price_usd=None, average_slip=None, impermanent_loss_protection_paid=None, liquidity_units=None, pool_apy=None, rune_depth=None, status=None, swap_count=None, swap_volume=None, synth_supply=None, synth_units=None, to_asset_average_slip=None, to_asset_count=None, to_asset_fees=None, to_asset_volume=None, to_rune_average_slip=None, to_rune_count=None, to_rune_fees=None, to_rune_volume=None, total_fees=None, unique_member_count=None, unique_swapper_count=None, units=None, withdraw_asset_volume=None, withdraw_count=None, withdraw_rune_volume=None, withdraw_volume=None):  # noqa: E501
+    def __init__(self, add_asset_liquidity_volume=None, add_liquidity_count=None, add_liquidity_volume=None, add_rune_liquidity_volume=None, annual_percentage_rate=None, asset=None, asset_depth=None, asset_price=None, asset_price_usd=None, average_slip=None, earnings=None, earnings_annual_as_percent_of_depth=None, liquidity_units=None, pool_apy=None, rune_depth=None, savers_apr=None, status=None, swap_count=None, swap_volume=None, synth_supply=None, synth_units=None, to_asset_average_slip=None, to_asset_count=None, to_asset_fees=None, to_asset_volume=None, to_rune_average_slip=None, to_rune_count=None, to_rune_fees=None, to_rune_volume=None, total_fees=None, unique_member_count=None, unique_swapper_count=None, units=None, withdraw_asset_volume=None, withdraw_count=None, withdraw_rune_volume=None, withdraw_volume=None):  # noqa: E501
         """PoolStatsDetail - a model defined in Swagger"""  # noqa: E501
         self._add_asset_liquidity_volume = None
         self._add_liquidity_count = None
         self._add_liquidity_volume = None
         self._add_rune_liquidity_volume = None
         self._annual_percentage_rate = None
         self._asset = None
         self._asset_depth = None
         self._asset_price = None
         self._asset_price_usd = None
         self._average_slip = None
-        self._impermanent_loss_protection_paid = None
+        self._earnings = None
+        self._earnings_annual_as_percent_of_depth = None
         self._liquidity_units = None
         self._pool_apy = None
         self._rune_depth = None
+        self._savers_apr = None
         self._status = None
         self._swap_count = None
         self._swap_volume = None
         self._synth_supply = None
         self._synth_units = None
         self._to_asset_average_slip = None
         self._to_asset_count = None
@@ -147,18 +153,20 @@
         self.add_rune_liquidity_volume = add_rune_liquidity_volume
         self.annual_percentage_rate = annual_percentage_rate
         self.asset = asset
         self.asset_depth = asset_depth
         self.asset_price = asset_price
         self.asset_price_usd = asset_price_usd
         self.average_slip = average_slip
-        self.impermanent_loss_protection_paid = impermanent_loss_protection_paid
+        self.earnings = earnings
+        self.earnings_annual_as_percent_of_depth = earnings_annual_as_percent_of_depth
         self.liquidity_units = liquidity_units
         self.pool_apy = pool_apy
         self.rune_depth = rune_depth
+        self.savers_apr = savers_apr
         self.status = status
         self.swap_count = swap_count
         self.swap_volume = swap_volume
         self.synth_supply = synth_supply
         self.synth_units = synth_units
         self.to_asset_average_slip = to_asset_average_slip
         self.to_asset_count = to_asset_count
@@ -277,26 +285,26 @@
 
         self._add_rune_liquidity_volume = add_rune_liquidity_volume
 
     @property
     def annual_percentage_rate(self):
         """Gets the annual_percentage_rate of this PoolStatsDetail.  # noqa: E501
 
-        Float, Also called APR. Annual return estimated linearly (not compounded) from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. Due to Impermanent Loss and Synths this might be negative, but given Impermanent Loss Protection for 100+ day members, frontends might show MAX(APR, 0).   # noqa: E501
+        deprecated now it's only showing zero util being deleted.  # noqa: E501
 
         :return: The annual_percentage_rate of this PoolStatsDetail.  # noqa: E501
         :rtype: str
         """
         return self._annual_percentage_rate
 
     @annual_percentage_rate.setter
     def annual_percentage_rate(self, annual_percentage_rate):
         """Sets the annual_percentage_rate of this PoolStatsDetail.
 
-        Float, Also called APR. Annual return estimated linearly (not compounded) from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 30). E.g. 0.1 means 10% yearly return. Due to Impermanent Loss and Synths this might be negative, but given Impermanent Loss Protection for 100+ day members, frontends might show MAX(APR, 0).   # noqa: E501
+        deprecated now it's only showing zero util being deleted.  # noqa: E501
 
         :param annual_percentage_rate: The annual_percentage_rate of this PoolStatsDetail.  # noqa: E501
         :type: str
         """
         if annual_percentage_rate is None:
             raise ValueError("Invalid value for `annual_percentage_rate`, must not be `None`")  # noqa: E501
 
@@ -422,37 +430,62 @@
         """
         if average_slip is None:
             raise ValueError("Invalid value for `average_slip`, must not be `None`")  # noqa: E501
 
         self._average_slip = average_slip
 
     @property
-    def impermanent_loss_protection_paid(self):
-        """Gets the impermanent_loss_protection_paid of this PoolStatsDetail.  # noqa: E501
+    def earnings(self):
+        """Gets the earnings of this PoolStatsDetail.  # noqa: E501
 
-        Int64(e8), part of the withdrawRuneVolume which was payed because of impermanent loss protection.   # noqa: E501
+        Int64(e8), The earning that has been recorded from the pool asset's Liquidity Fees and Rewards in RUNE. The earnings shown are from the period parameter default being 14 days  (configurable by the period parameter).   # noqa: E501
 
-        :return: The impermanent_loss_protection_paid of this PoolStatsDetail.  # noqa: E501
+        :return: The earnings of this PoolStatsDetail.  # noqa: E501
         :rtype: str
         """
-        return self._impermanent_loss_protection_paid
+        return self._earnings
 
-    @impermanent_loss_protection_paid.setter
-    def impermanent_loss_protection_paid(self, impermanent_loss_protection_paid):
-        """Sets the impermanent_loss_protection_paid of this PoolStatsDetail.
+    @earnings.setter
+    def earnings(self, earnings):
+        """Sets the earnings of this PoolStatsDetail.
 
-        Int64(e8), part of the withdrawRuneVolume which was payed because of impermanent loss protection.   # noqa: E501
+        Int64(e8), The earning that has been recorded from the pool asset's Liquidity Fees and Rewards in RUNE. The earnings shown are from the period parameter default being 14 days  (configurable by the period parameter).   # noqa: E501
 
-        :param impermanent_loss_protection_paid: The impermanent_loss_protection_paid of this PoolStatsDetail.  # noqa: E501
+        :param earnings: The earnings of this PoolStatsDetail.  # noqa: E501
         :type: str
         """
-        if impermanent_loss_protection_paid is None:
-            raise ValueError("Invalid value for `impermanent_loss_protection_paid`, must not be `None`")  # noqa: E501
+        if earnings is None:
+            raise ValueError("Invalid value for `earnings`, must not be `None`")  # noqa: E501
 
-        self._impermanent_loss_protection_paid = impermanent_loss_protection_paid
+        self._earnings = earnings
+
+    @property
+    def earnings_annual_as_percent_of_depth(self):
+        """Gets the earnings_annual_as_percent_of_depth of this PoolStatsDetail.  # noqa: E501
+
+        Float, The estimation of earnings during the time interval expanded through a year  compared to the current pool depth. E.g. 0.1 means the pool based on this interval earnings can earn 10% of its pool during a year.   # noqa: E501
+
+        :return: The earnings_annual_as_percent_of_depth of this PoolStatsDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._earnings_annual_as_percent_of_depth
+
+    @earnings_annual_as_percent_of_depth.setter
+    def earnings_annual_as_percent_of_depth(self, earnings_annual_as_percent_of_depth):
+        """Sets the earnings_annual_as_percent_of_depth of this PoolStatsDetail.
+
+        Float, The estimation of earnings during the time interval expanded through a year  compared to the current pool depth. E.g. 0.1 means the pool based on this interval earnings can earn 10% of its pool during a year.   # noqa: E501
+
+        :param earnings_annual_as_percent_of_depth: The earnings_annual_as_percent_of_depth of this PoolStatsDetail.  # noqa: E501
+        :type: str
+        """
+        if earnings_annual_as_percent_of_depth is None:
+            raise ValueError("Invalid value for `earnings_annual_as_percent_of_depth`, must not be `None`")  # noqa: E501
+
+        self._earnings_annual_as_percent_of_depth = earnings_annual_as_percent_of_depth
 
     @property
     def liquidity_units(self):
         """Gets the liquidity_units of this PoolStatsDetail.  # noqa: E501
 
         Int64, Liquidity Units in the pool  # noqa: E501
 
@@ -475,26 +508,26 @@
 
         self._liquidity_units = liquidity_units
 
     @property
     def pool_apy(self):
         """Gets the pool_apy of this PoolStatsDetail.  # noqa: E501
 
-        Float, MAX(AnnualPercentageRate, 0)   # noqa: E501
+        deprecated now it's only showing zero util being deleted.  # noqa: E501
 
         :return: The pool_apy of this PoolStatsDetail.  # noqa: E501
         :rtype: str
         """
         return self._pool_apy
 
     @pool_apy.setter
     def pool_apy(self, pool_apy):
         """Sets the pool_apy of this PoolStatsDetail.
 
-        Float, MAX(AnnualPercentageRate, 0)   # noqa: E501
+        deprecated now it's only showing zero util being deleted.  # noqa: E501
 
         :param pool_apy: The pool_apy of this PoolStatsDetail.  # noqa: E501
         :type: str
         """
         if pool_apy is None:
             raise ValueError("Invalid value for `pool_apy`, must not be `None`")  # noqa: E501
 
@@ -522,14 +555,39 @@
         """
         if rune_depth is None:
             raise ValueError("Invalid value for `rune_depth`, must not be `None`")  # noqa: E501
 
         self._rune_depth = rune_depth
 
     @property
+    def savers_apr(self):
+        """Gets the savers_apr of this PoolStatsDetail.  # noqa: E501
+
+        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 14). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
+
+        :return: The savers_apr of this PoolStatsDetail.  # noqa: E501
+        :rtype: str
+        """
+        return self._savers_apr
+
+    @savers_apr.setter
+    def savers_apr(self, savers_apr):
+        """Sets the savers_apr of this PoolStatsDetail.
+
+        Float, Annual Return estimated linearly (not compounded) for savers from a period of typically the last 30 or 100 days (configurable by the period parameter, default is 14). E.g. 0.1 means 10% yearly return. If the savers period has not yet been reached, It will show zero instead.   # noqa: E501
+
+        :param savers_apr: The savers_apr of this PoolStatsDetail.  # noqa: E501
+        :type: str
+        """
+        if savers_apr is None:
+            raise ValueError("Invalid value for `savers_apr`, must not be `None`")  # noqa: E501
+
+        self._savers_apr = savers_apr
+
+    @property
     def status(self):
         """Gets the status of this PoolStatsDetail.  # noqa: E501
 
         The state of the pool, e.g. Available, Staged  # noqa: E501
 
         :return: The status of this PoolStatsDetail.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/refund_metadata.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/refund_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/reverse_thor_names.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/reverse_thor_names.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/saver_details.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/saver_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/saver_pool.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/saver_pool.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_item.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/savers_history_meta.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/savers_history_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/stats_data.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/stats_data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -27,15 +27,14 @@
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     swagger_types = {
         'add_liquidity_count': 'str',
         'add_liquidity_volume': 'str',
         'daily_active_users': 'str',
-        'impermanent_loss_protection_paid': 'str',
         'monthly_active_users': 'str',
         'rune_depth': 'str',
         'rune_price_usd': 'str',
         'swap_count': 'str',
         'swap_count24h': 'str',
         'swap_count30d': 'str',
         'swap_volume': 'str',
@@ -49,15 +48,14 @@
         'withdraw_volume': 'str'
     }
 
     attribute_map = {
         'add_liquidity_count': 'addLiquidityCount',
         'add_liquidity_volume': 'addLiquidityVolume',
         'daily_active_users': 'dailyActiveUsers',
-        'impermanent_loss_protection_paid': 'impermanentLossProtectionPaid',
         'monthly_active_users': 'monthlyActiveUsers',
         'rune_depth': 'runeDepth',
         'rune_price_usd': 'runePriceUSD',
         'swap_count': 'swapCount',
         'swap_count24h': 'swapCount24h',
         'swap_count30d': 'swapCount30d',
         'swap_volume': 'swapVolume',
@@ -67,20 +65,19 @@
         'to_asset_count': 'toAssetCount',
         'to_rune_count': 'toRuneCount',
         'unique_swapper_count': 'uniqueSwapperCount',
         'withdraw_count': 'withdrawCount',
         'withdraw_volume': 'withdrawVolume'
     }
 
-    def __init__(self, add_liquidity_count=None, add_liquidity_volume=None, daily_active_users=None, impermanent_loss_protection_paid=None, monthly_active_users=None, rune_depth=None, rune_price_usd=None, swap_count=None, swap_count24h=None, swap_count30d=None, swap_volume=None, switched_rune=None, synth_burn_count=None, synth_mint_count=None, to_asset_count=None, to_rune_count=None, unique_swapper_count=None, withdraw_count=None, withdraw_volume=None):  # noqa: E501
+    def __init__(self, add_liquidity_count=None, add_liquidity_volume=None, daily_active_users=None, monthly_active_users=None, rune_depth=None, rune_price_usd=None, swap_count=None, swap_count24h=None, swap_count30d=None, swap_volume=None, switched_rune=None, synth_burn_count=None, synth_mint_count=None, to_asset_count=None, to_rune_count=None, unique_swapper_count=None, withdraw_count=None, withdraw_volume=None):  # noqa: E501
         """StatsData - a model defined in Swagger"""  # noqa: E501
         self._add_liquidity_count = None
         self._add_liquidity_volume = None
         self._daily_active_users = None
-        self._impermanent_loss_protection_paid = None
         self._monthly_active_users = None
         self._rune_depth = None
         self._rune_price_usd = None
         self._swap_count = None
         self._swap_count24h = None
         self._swap_count30d = None
         self._swap_volume = None
@@ -92,15 +89,14 @@
         self._unique_swapper_count = None
         self._withdraw_count = None
         self._withdraw_volume = None
         self.discriminator = None
         self.add_liquidity_count = add_liquidity_count
         self.add_liquidity_volume = add_liquidity_volume
         self.daily_active_users = daily_active_users
-        self.impermanent_loss_protection_paid = impermanent_loss_protection_paid
         self.monthly_active_users = monthly_active_users
         self.rune_depth = rune_depth
         self.rune_price_usd = rune_price_usd
         self.swap_count = swap_count
         self.swap_count24h = swap_count24h
         self.swap_count30d = swap_count30d
         self.swap_volume = swap_volume
@@ -185,39 +181,14 @@
         """
         if daily_active_users is None:
             raise ValueError("Invalid value for `daily_active_users`, must not be `None`")  # noqa: E501
 
         self._daily_active_users = daily_active_users
 
     @property
-    def impermanent_loss_protection_paid(self):
-        """Gets the impermanent_loss_protection_paid of this StatsData.  # noqa: E501
-
-        Int64(e8), impermanent loss protection paid out.   # noqa: E501
-
-        :return: The impermanent_loss_protection_paid of this StatsData.  # noqa: E501
-        :rtype: str
-        """
-        return self._impermanent_loss_protection_paid
-
-    @impermanent_loss_protection_paid.setter
-    def impermanent_loss_protection_paid(self, impermanent_loss_protection_paid):
-        """Sets the impermanent_loss_protection_paid of this StatsData.
-
-        Int64(e8), impermanent loss protection paid out.   # noqa: E501
-
-        :param impermanent_loss_protection_paid: The impermanent_loss_protection_paid of this StatsData.  # noqa: E501
-        :type: str
-        """
-        if impermanent_loss_protection_paid is None:
-            raise ValueError("Invalid value for `impermanent_loss_protection_paid`, must not be `None`")  # noqa: E501
-
-        self._impermanent_loss_protection_paid = impermanent_loss_protection_paid
-
-    @property
     def monthly_active_users(self):
         """Gets the monthly_active_users of this StatsData.  # noqa: E501
 
         Deprecated, it's always 0.  # noqa: E501
 
         :return: The monthly_active_users of this StatsData.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/streaming_swap_meta.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/streaming_swap_meta.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history_intervals.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_history_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -32,106 +32,126 @@
         'end_time': 'str',
         'rune_price_usd': 'str',
         'start_time': 'str',
         'synth_mint_average_slip': 'str',
         'synth_mint_count': 'str',
         'synth_mint_fees': 'str',
         'synth_mint_volume': 'str',
+        'synth_mint_volume_usd': 'str',
         'synth_redeem_average_slip': 'str',
         'synth_redeem_count': 'str',
         'synth_redeem_fees': 'str',
         'synth_redeem_volume': 'str',
+        'synth_redeem_volume_usd': 'str',
         'to_asset_average_slip': 'str',
         'to_asset_count': 'str',
         'to_asset_fees': 'str',
         'to_asset_volume': 'str',
+        'to_asset_volume_usd': 'str',
         'to_rune_average_slip': 'str',
         'to_rune_count': 'str',
         'to_rune_fees': 'str',
         'to_rune_volume': 'str',
+        'to_rune_volume_usd': 'str',
         'total_count': 'str',
         'total_fees': 'str',
-        'total_volume': 'str'
+        'total_volume': 'str',
+        'total_volume_usd': 'str'
     }
 
     attribute_map = {
         'average_slip': 'averageSlip',
         'end_time': 'endTime',
         'rune_price_usd': 'runePriceUSD',
         'start_time': 'startTime',
         'synth_mint_average_slip': 'synthMintAverageSlip',
         'synth_mint_count': 'synthMintCount',
         'synth_mint_fees': 'synthMintFees',
         'synth_mint_volume': 'synthMintVolume',
+        'synth_mint_volume_usd': 'synthMintVolumeUSD',
         'synth_redeem_average_slip': 'synthRedeemAverageSlip',
         'synth_redeem_count': 'synthRedeemCount',
         'synth_redeem_fees': 'synthRedeemFees',
         'synth_redeem_volume': 'synthRedeemVolume',
+        'synth_redeem_volume_usd': 'synthRedeemVolumeUSD',
         'to_asset_average_slip': 'toAssetAverageSlip',
         'to_asset_count': 'toAssetCount',
         'to_asset_fees': 'toAssetFees',
         'to_asset_volume': 'toAssetVolume',
+        'to_asset_volume_usd': 'toAssetVolumeUSD',
         'to_rune_average_slip': 'toRuneAverageSlip',
         'to_rune_count': 'toRuneCount',
         'to_rune_fees': 'toRuneFees',
         'to_rune_volume': 'toRuneVolume',
+        'to_rune_volume_usd': 'toRuneVolumeUSD',
         'total_count': 'totalCount',
         'total_fees': 'totalFees',
-        'total_volume': 'totalVolume'
+        'total_volume': 'totalVolume',
+        'total_volume_usd': 'totalVolumeUSD'
     }
 
-    def __init__(self, average_slip=None, end_time=None, rune_price_usd=None, start_time=None, synth_mint_average_slip=None, synth_mint_count=None, synth_mint_fees=None, synth_mint_volume=None, synth_redeem_average_slip=None, synth_redeem_count=None, synth_redeem_fees=None, synth_redeem_volume=None, to_asset_average_slip=None, to_asset_count=None, to_asset_fees=None, to_asset_volume=None, to_rune_average_slip=None, to_rune_count=None, to_rune_fees=None, to_rune_volume=None, total_count=None, total_fees=None, total_volume=None):  # noqa: E501
+    def __init__(self, average_slip=None, end_time=None, rune_price_usd=None, start_time=None, synth_mint_average_slip=None, synth_mint_count=None, synth_mint_fees=None, synth_mint_volume=None, synth_mint_volume_usd=None, synth_redeem_average_slip=None, synth_redeem_count=None, synth_redeem_fees=None, synth_redeem_volume=None, synth_redeem_volume_usd=None, to_asset_average_slip=None, to_asset_count=None, to_asset_fees=None, to_asset_volume=None, to_asset_volume_usd=None, to_rune_average_slip=None, to_rune_count=None, to_rune_fees=None, to_rune_volume=None, to_rune_volume_usd=None, total_count=None, total_fees=None, total_volume=None, total_volume_usd=None):  # noqa: E501
         """SwapHistoryItem - a model defined in Swagger"""  # noqa: E501
         self._average_slip = None
         self._end_time = None
         self._rune_price_usd = None
         self._start_time = None
         self._synth_mint_average_slip = None
         self._synth_mint_count = None
         self._synth_mint_fees = None
         self._synth_mint_volume = None
+        self._synth_mint_volume_usd = None
         self._synth_redeem_average_slip = None
         self._synth_redeem_count = None
         self._synth_redeem_fees = None
         self._synth_redeem_volume = None
+        self._synth_redeem_volume_usd = None
         self._to_asset_average_slip = None
         self._to_asset_count = None
         self._to_asset_fees = None
         self._to_asset_volume = None
+        self._to_asset_volume_usd = None
         self._to_rune_average_slip = None
         self._to_rune_count = None
         self._to_rune_fees = None
         self._to_rune_volume = None
+        self._to_rune_volume_usd = None
         self._total_count = None
         self._total_fees = None
         self._total_volume = None
+        self._total_volume_usd = None
         self.discriminator = None
         self.average_slip = average_slip
         self.end_time = end_time
         self.rune_price_usd = rune_price_usd
         self.start_time = start_time
         self.synth_mint_average_slip = synth_mint_average_slip
         self.synth_mint_count = synth_mint_count
         self.synth_mint_fees = synth_mint_fees
         self.synth_mint_volume = synth_mint_volume
+        self.synth_mint_volume_usd = synth_mint_volume_usd
         self.synth_redeem_average_slip = synth_redeem_average_slip
         self.synth_redeem_count = synth_redeem_count
         self.synth_redeem_fees = synth_redeem_fees
         self.synth_redeem_volume = synth_redeem_volume
+        self.synth_redeem_volume_usd = synth_redeem_volume_usd
         self.to_asset_average_slip = to_asset_average_slip
         self.to_asset_count = to_asset_count
         self.to_asset_fees = to_asset_fees
         self.to_asset_volume = to_asset_volume
+        self.to_asset_volume_usd = to_asset_volume_usd
         self.to_rune_average_slip = to_rune_average_slip
         self.to_rune_count = to_rune_count
         self.to_rune_fees = to_rune_fees
         self.to_rune_volume = to_rune_volume
+        self.to_rune_volume_usd = to_rune_volume_usd
         self.total_count = total_count
         self.total_fees = total_fees
         self.total_volume = total_volume
+        self.total_volume_usd = total_volume_usd
 
     @property
     def average_slip(self):
         """Gets the average_slip of this SwapHistoryItem.  # noqa: E501
 
         Float64 (Basis points, 0-10000, where 10000=100%), the weighted average (by count) of toAssetAverageSlip, toRuneAverageSlip, synthMintAverageSlip, synthRedeemAverageSlip. Big swaps have the same weight as small swaps.   # noqa: E501
 
@@ -326,14 +346,39 @@
         """
         if synth_mint_volume is None:
             raise ValueError("Invalid value for `synth_mint_volume`, must not be `None`")  # noqa: E501
 
         self._synth_mint_volume = synth_mint_volume
 
     @property
+    def synth_mint_volume_usd(self):
+        """Gets the synth_mint_volume_usd of this SwapHistoryItem.  # noqa: E501
+
+        Int64(e2), volume of swaps from rune to synthetic asset denoted in USD price of the rune in each swap  # noqa: E501
+
+        :return: The synth_mint_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._synth_mint_volume_usd
+
+    @synth_mint_volume_usd.setter
+    def synth_mint_volume_usd(self, synth_mint_volume_usd):
+        """Sets the synth_mint_volume_usd of this SwapHistoryItem.
+
+        Int64(e2), volume of swaps from rune to synthetic asset denoted in USD price of the rune in each swap  # noqa: E501
+
+        :param synth_mint_volume_usd: The synth_mint_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :type: str
+        """
+        if synth_mint_volume_usd is None:
+            raise ValueError("Invalid value for `synth_mint_volume_usd`, must not be `None`")  # noqa: E501
+
+        self._synth_mint_volume_usd = synth_mint_volume_usd
+
+    @property
     def synth_redeem_average_slip(self):
         """Gets the synth_redeem_average_slip of this SwapHistoryItem.  # noqa: E501
 
         Float64 (Basis points, 0-10000, where 10000=100%), the average slip for swaps from synthetic asset to rune. Big swaps have the same weight as small swaps   # noqa: E501
 
         :return: The synth_redeem_average_slip of this SwapHistoryItem.  # noqa: E501
         :rtype: str
@@ -426,14 +471,39 @@
         """
         if synth_redeem_volume is None:
             raise ValueError("Invalid value for `synth_redeem_volume`, must not be `None`")  # noqa: E501
 
         self._synth_redeem_volume = synth_redeem_volume
 
     @property
+    def synth_redeem_volume_usd(self):
+        """Gets the synth_redeem_volume_usd of this SwapHistoryItem.  # noqa: E501
+
+        Int64(e2), volume of swaps from synthetic asset to rune denoted in USD price of the rune in each swap  # noqa: E501
+
+        :return: The synth_redeem_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._synth_redeem_volume_usd
+
+    @synth_redeem_volume_usd.setter
+    def synth_redeem_volume_usd(self, synth_redeem_volume_usd):
+        """Sets the synth_redeem_volume_usd of this SwapHistoryItem.
+
+        Int64(e2), volume of swaps from synthetic asset to rune denoted in USD price of the rune in each swap  # noqa: E501
+
+        :param synth_redeem_volume_usd: The synth_redeem_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :type: str
+        """
+        if synth_redeem_volume_usd is None:
+            raise ValueError("Invalid value for `synth_redeem_volume_usd`, must not be `None`")  # noqa: E501
+
+        self._synth_redeem_volume_usd = synth_redeem_volume_usd
+
+    @property
     def to_asset_average_slip(self):
         """Gets the to_asset_average_slip of this SwapHistoryItem.  # noqa: E501
 
         Float64 (Basis points, 0-10000, where 10000=100%), the average slip for swaps from rune to asset. Big swaps have the same weight as small swaps   # noqa: E501
 
         :return: The to_asset_average_slip of this SwapHistoryItem.  # noqa: E501
         :rtype: str
@@ -526,14 +596,39 @@
         """
         if to_asset_volume is None:
             raise ValueError("Invalid value for `to_asset_volume`, must not be `None`")  # noqa: E501
 
         self._to_asset_volume = to_asset_volume
 
     @property
+    def to_asset_volume_usd(self):
+        """Gets the to_asset_volume_usd of this SwapHistoryItem.  # noqa: E501
+
+        Int64(e2), volume of swaps from rune to asset denoted in USD price of the rune in each swap  # noqa: E501
+
+        :return: The to_asset_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._to_asset_volume_usd
+
+    @to_asset_volume_usd.setter
+    def to_asset_volume_usd(self, to_asset_volume_usd):
+        """Sets the to_asset_volume_usd of this SwapHistoryItem.
+
+        Int64(e2), volume of swaps from rune to asset denoted in USD price of the rune in each swap  # noqa: E501
+
+        :param to_asset_volume_usd: The to_asset_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :type: str
+        """
+        if to_asset_volume_usd is None:
+            raise ValueError("Invalid value for `to_asset_volume_usd`, must not be `None`")  # noqa: E501
+
+        self._to_asset_volume_usd = to_asset_volume_usd
+
+    @property
     def to_rune_average_slip(self):
         """Gets the to_rune_average_slip of this SwapHistoryItem.  # noqa: E501
 
         Float64 (Basis points, 0-10000, where 10000=100%), the average slip for swaps from asset to rune. Big swaps have the same weight as small swaps   # noqa: E501
 
         :return: The to_rune_average_slip of this SwapHistoryItem.  # noqa: E501
         :rtype: str
@@ -626,14 +721,39 @@
         """
         if to_rune_volume is None:
             raise ValueError("Invalid value for `to_rune_volume`, must not be `None`")  # noqa: E501
 
         self._to_rune_volume = to_rune_volume
 
     @property
+    def to_rune_volume_usd(self):
+        """Gets the to_rune_volume_usd of this SwapHistoryItem.  # noqa: E501
+
+        Int64(e2), volume of swaps from asset to rune denoted in USD price of the rune in each swap  # noqa: E501
+
+        :return: The to_rune_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._to_rune_volume_usd
+
+    @to_rune_volume_usd.setter
+    def to_rune_volume_usd(self, to_rune_volume_usd):
+        """Sets the to_rune_volume_usd of this SwapHistoryItem.
+
+        Int64(e2), volume of swaps from asset to rune denoted in USD price of the rune in each swap  # noqa: E501
+
+        :param to_rune_volume_usd: The to_rune_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :type: str
+        """
+        if to_rune_volume_usd is None:
+            raise ValueError("Invalid value for `to_rune_volume_usd`, must not be `None`")  # noqa: E501
+
+        self._to_rune_volume_usd = to_rune_volume_usd
+
+    @property
     def total_count(self):
         """Gets the total_count of this SwapHistoryItem.  # noqa: E501
 
         Int64, toAssetCount + toRuneCount + synthMintCount + synthRedeemCount  # noqa: E501
 
         :return: The total_count of this SwapHistoryItem.  # noqa: E501
         :rtype: str
@@ -700,14 +820,39 @@
         :type: str
         """
         if total_volume is None:
             raise ValueError("Invalid value for `total_volume`, must not be `None`")  # noqa: E501
 
         self._total_volume = total_volume
 
+    @property
+    def total_volume_usd(self):
+        """Gets the total_volume_usd of this SwapHistoryItem.  # noqa: E501
+
+        Int64(e2), toAssetVolume + toRuneVolume + synthMintVolume + synthRedeemVolume (denoted in USD price of the rune in each swap)   # noqa: E501
+
+        :return: The total_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._total_volume_usd
+
+    @total_volume_usd.setter
+    def total_volume_usd(self, total_volume_usd):
+        """Sets the total_volume_usd of this SwapHistoryItem.
+
+        Int64(e2), toAssetVolume + toRuneVolume + synthMintVolume + synthRedeemVolume (denoted in USD price of the rune in each swap)   # noqa: E501
+
+        :param total_volume_usd: The total_volume_usd of this SwapHistoryItem.  # noqa: E501
+        :type: str
+        """
+        if total_volume_usd is None:
+            raise ValueError("Invalid value for `total_volume_usd`, must not be `None`")  # noqa: E501
+
+        self._total_volume_usd = total_volume_usd
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/swap_metadata.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/swap_metadata.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/thor_name_details.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/thor_name_details.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/thor_name_entry.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/thor_name_entry.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/transaction.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/transaction.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history_intervals.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/nodes.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class TVLHistoryIntervals(object):
+class Nodes(object):
     """NOTE: This class is auto generated by the swagger code generator program.
 
     Do not edit the class manually.
     """
     """
     Attributes:
       swagger_types (dict): The key is attribute name
@@ -30,15 +30,15 @@
     swagger_types = {
     }
 
     attribute_map = {
     }
 
     def __init__(self):  # noqa: E501
-        """TVLHistoryIntervals - a model defined in Swagger"""  # noqa: E501
+        """Nodes - a model defined in Swagger"""  # noqa: E501
         self.discriminator = None
 
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
@@ -54,15 +54,15 @@
                 result[attr] = dict(map(
                     lambda item: (item[0], item[1].to_dict())
                     if hasattr(item[1], "to_dict") else item,
                     value.items()
                 ))
             else:
                 result[attr] = value
-        if issubclass(TVLHistoryIntervals, dict):
+        if issubclass(Nodes, dict):
             for key, value in self.items():
                 result[key] = value
 
         return result
 
     def to_str(self):
         """Returns the string representation of the model"""
@@ -70,15 +70,15 @@
 
     def __repr__(self):
         """For `print` and `pprint`"""
         return self.to_str()
 
     def __eq__(self, other):
         """Returns true if both objects are equal"""
-        if not isinstance(other, TVLHistoryIntervals):
+        if not isinstance(other, Nodes):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/tvl_history_item.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/tvl_history_item.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/models/withdraw_metadata.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/models/withdraw_metadata.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard/rest.py` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Midgard Public API
 
     The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.  # noqa: E501
 
-    OpenAPI spec version: 2.18.2
+    OpenAPI spec version: 2.20.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import io
 import json
 import logging
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/PKG-INFO` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-midgard
-Version: 2.18.2
+Version: 2.20.1
 Summary: Midgard Public API
 Home-page: 
 Author-email: devs@thorchain.org
 Keywords: Swagger,Midgard Public API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-midgard
 The Midgard Public API queries THORChain and any chains linked via the Bifröst and prepares information about the network to be readily available for public users. The API parses transaction event data from THORChain and stores them in a time-series database to make time-dependent queries easy. Midgard does not hold critical information. To interact with THORChain protocol, users should query THORNode directly.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 2.18.2
-- Package version: 2.18.2
+- API version: 2.20.1
+- Package version: 2.20.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
```

### Comparing `xchainpy2-midgard-2.18.2/xchainpy2_midgard.egg-info/SOURCES.txt` & `xchainpy2-midgard-2.20.1/xchainpy2_midgard.egg-info/SOURCES.txt`

 * *Files identical despite different names*

