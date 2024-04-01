# Comparing `tmp/xchainpy2-thornode-1.125.0.tar.gz` & `tmp/xchainpy2-thornode-1.130.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xchainpy2-thornode-1.125.0.tar", last modified: Sun Dec 24 07:21:51 2023, max compression
+gzip compressed data, was "xchainpy2-thornode-1.130.1.tar", last modified: Mon Apr  1 10:29:36 2024, max compression
```

## Comparing `xchainpy2-thornode-1.125.0.tar` & `xchainpy2-thornode-1.130.1.tar`

### file list

```diff
@@ -1,263 +1,279 @@
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.938332 xchainpy2-thornode-1.125.0/
--rw-r--r--   0 tirinox    (501) staff       (20)     2124 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/LICENSE
--rw-r--r--   0 tirinox    (501) staff       (20)    13027 2023-12-24 07:21:51.937860 xchainpy2-thornode-1.125.0/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)    12671 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/README.md
--rw-r--r--   0 tirinox    (501) staff       (20)       38 2023-12-24 07:21:51.938381 xchainpy2-thornode-1.125.0/setup.cfg
--rw-r--r--   0 tirinox    (501) staff       (20)     1270 2023-12-24 07:01:23.000000 xchainpy2-thornode-1.125.0/setup.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.903427 xchainpy2-thornode-1.125.0/test/
--rw-r--r--   0 tirinox    (501) staff       (20)       15 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_base_quote_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      730 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_block_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_response_header.py
--rw-r--r--   0 tirinox    (501) staff       (20)      995 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_response_header_version.py
--rw-r--r--   0 tirinox    (501) staff       (20)      905 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_response_id.py
--rw-r--r--   0 tirinox    (501) staff       (20)      947 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_response_id_parts.py
--rw-r--r--   0 tirinox    (501) staff       (20)      839 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      889 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_block_tx_result.py
--rw-r--r--   0 tirinox    (501) staff       (20)      845 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_borrower.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_borrower_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      848 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_borrowers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_borrowers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)      746 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_clout_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_derived_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_derived_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_derived_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      733 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_invariant_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      857 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_invariants_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      927 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_invariants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      985 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      977 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)      934 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      993 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1296 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      929 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      931 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_mimir_v2_ids_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)      839 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_msg_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1398 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)      847 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      937 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)      891 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      812 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)      716 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      813 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      982 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1030 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1158 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)      963 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_loan_close_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      955 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_loan_open_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      987 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      995 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      919 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_streaming_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)      881 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_streaming_swap_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      953 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_streaming_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      961 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_streaming_swaps_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_swap_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_swapper_clout_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      845 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_thorname.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_thorname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)      911 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_thorname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      756 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_thornames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1139 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1016 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)      797 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_details_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      857 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)      863 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      921 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1127 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_confirmation_counted.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1045 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1037 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_observed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1021 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_outbound_delay.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1029 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_outbound_signed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1021 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)      997 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1071 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_status_streaming.py
--rw-r--r--   0 tirinox    (501) staff       (20)      913 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_status_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1023 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_tx_status_response_planned_out_txs.py
--rw-r--r--   0 tirinox    (501) staff       (20)      821 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)      879 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)      855 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)      945 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      887 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      871 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/test/test_vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     1013 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)      895 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)      903 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/test/test_version_response.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.904658 xchainpy2-thornode-1.125.0/xchainpy2_thornode/
--rw-r--r--   0 tirinox    (501) staff       (20)     9020 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/__init__.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.911379 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/
--rw-r--r--   0 tirinox    (501) staff       (20)     1199 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4010 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/block_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8841 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/borrowers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4618 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/clout_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3591 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/health_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7957 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/invariants_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9207 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/liquidity_providers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25039 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/mimir_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    28645 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/network_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7800 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/nodes_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4014 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/pol_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14824 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/pools_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14025 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/queue_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    24945 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/quote_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8757 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/savers_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7898 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/streaming_swap_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4563 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/thornames_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    19756 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/transactions_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16119 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/tss_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14407 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/vaults_api.py
--rw-r--r--   0 tirinox    (501) staff       (20)    25046 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/api_client.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7927 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/configuration.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.937082 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/
--rw-r--r--   0 tirinox    (501) staff       (20)     7748 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/__init__.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4499 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/ban_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16196 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/base_quote_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6451 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14461 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_header.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3874 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_header_version.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3814 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_id.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3823 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_id_parts.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4358 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7409 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_tx_result.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10805 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrower.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrower_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrowers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3757 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/chain_height.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4298 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/coin.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4796 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/constants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7204 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2416 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2420 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14332 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/inbound_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2436 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/inbound_addresses_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4957 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/invariant_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3149 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/invariants_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3950 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keygen_metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4071 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3820 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_metrics.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3760 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5575 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/last_block.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/last_block_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    16304 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2440 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    11875 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider_summary.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2444 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_providers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3763 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/metrics_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3087 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2628 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5619 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_v2_ids_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4109 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_vote.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14536 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/msg_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20441 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/network_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    21507 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3748 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_bond_provider.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4111 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_bond_providers.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3732 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_jail.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3728 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_keygen_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4804 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_preflight_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3712 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_pub_key_set.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/nodes_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    12377 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/observed_tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/outbound_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2899 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/ping.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6975 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pol_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    19097 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pool.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2388 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pool_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pools_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7066 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8184 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_fees.py
--rw-r--r--   0 tirinox    (501) staff       (20)    26967 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_loan_close_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    26986 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_loan_open_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20465 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_saver_deposit_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    20804 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_saver_withdraw_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    24690 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8754 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/saver.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/saver_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/savers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/scheduled_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    14192 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swap.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2424 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swap_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2428 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swaps_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2408 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/swap_queue_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7826 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/swapper_clout_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     7228 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3632 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname_alias.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2404 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3937 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tss_keysign_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3644 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tss_metric.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6573 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10350 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_details_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9115 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_out_item.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6805 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10350 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_signers_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     8982 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     9909 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3538 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     6606 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5854 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5938 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3604 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4149 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_status.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5297 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5286 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_status_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5721 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py
--rw-r--r--   0 tirinox    (501) staff       (20)    12716 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3620 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_address.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3838 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_info.py
--rw-r--r--   0 tirinox    (501) staff       (20)     4833 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_pubkeys_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2392 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     3588 2023-12-24 06:57:02.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_router.py
--rw-r--r--   0 tirinox    (501) staff       (20)     2396 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vaults_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)     5861 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/version_response.py
--rw-r--r--   0 tirinox    (501) staff       (20)    10622 2023-12-24 06:57:03.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode/rest.py
-drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2023-12-24 07:21:51.937474 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/
--rw-r--r--   0 tirinox    (501) staff       (20)    13027 2023-12-24 07:21:51.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/PKG-INFO
--rw-r--r--   0 tirinox    (501) staff       (20)     9673 2023-12-24 07:21:51.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/SOURCES.txt
--rw-r--r--   0 tirinox    (501) staff       (20)        1 2023-12-24 07:21:51.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/dependency_links.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       56 2023-12-24 07:21:51.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/requires.txt
--rw-r--r--   0 tirinox    (501) staff       (20)       24 2023-12-24 07:21:51.000000 xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/top_level.txt
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.057469 xchainpy2-thornode-1.130.1/
+-rw-r--r--   0 tirinox    (501) staff       (20)     2124 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/LICENSE
+-rw-r--r--   0 tirinox    (501) staff       (20)    13717 2024-04-01 10:29:36.056913 xchainpy2-thornode-1.130.1/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)    13361 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/README.md
+-rw-r--r--   0 tirinox    (501) staff       (20)       38 2024-04-01 10:29:36.057510 xchainpy2-thornode-1.130.1/setup.cfg
+-rw-r--r--   0 tirinox    (501) staff       (20)     1270 2024-04-01 10:24:14.000000 xchainpy2-thornode-1.130.1/setup.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.035430 xchainpy2-thornode-1.130.1/test/
+-rw-r--r--   0 tirinox    (501) staff       (20)       15 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      730 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_block_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      905 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      947 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      889 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrower.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrower_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      848 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_borrowers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_borrowers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      746 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_clout_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_derived_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      733 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_invariant_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_invariants_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      927 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_invariants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      985 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      977 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      934 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      993 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1296 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      931 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_v2_ids_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      839 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_msg_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1398 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      847 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      891 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      812 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      716 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      813 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      982 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1030 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1158 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      963 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_loan_close_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      955 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_loan_open_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      987 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      995 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      919 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      881 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      961 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_streaming_swaps_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_swap_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_swapper_clout_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      845 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      911 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_thorname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      756 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_thornames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      782 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_account_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_account_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      789 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_accounts_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      953 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_accounts_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      761 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_unit_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_unit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      768 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_trade_units_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      929 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_trade_units_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1139 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1016 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      797 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_details_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      857 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      863 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      921 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1127 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_confirmation_counted.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1045 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_finalised.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1037 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_observed.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1021 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_delay.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1029 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_signed.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1021 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_finalised.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      997 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1071 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status_streaming.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      913 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_status_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1023 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_tx_status_response_planned_out_txs.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      821 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      879 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      855 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      945 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      887 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      871 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     1013 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/test/test_vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      895 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)      903 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/test/test_version_response.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.036931 xchainpy2-thornode-1.130.1/xchainpy2_thornode/
+-rw-r--r--   0 tirinox    (501) staff       (20)     9608 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/__init__.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.041879 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/
+-rw-r--r--   0 tirinox    (501) staff       (20)     1467 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4010 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/block_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8841 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/borrowers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4618 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/clout_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3591 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/health_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7957 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/invariants_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9207 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/liquidity_providers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25039 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/mimir_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    28645 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/network_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7800 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/nodes_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4014 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pol_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14824 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pools_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14025 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/queue_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25292 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/quote_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8757 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/savers_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7898 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/streaming_swap_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4563 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/thornames_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4646 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_account_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4628 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_accounts_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4575 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_unit_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4139 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/trade_units_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    19756 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/transactions_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16119 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/tss_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14407 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/vaults_api.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    25046 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/api_client.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8023 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/configuration.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.056402 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/
+-rw-r--r--   0 tirinox    (501) staff       (20)     8068 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/__init__.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4499 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ban_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16196 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/base_quote_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6451 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14461 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3874 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header_version.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3814 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3823 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id_parts.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4358 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7409 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx_result.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10805 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrowers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3757 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/chain_height.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4298 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/coin.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4796 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/constants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7204 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2416 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2420 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14332 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2436 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_addresses_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4957 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariant_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3149 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariants_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3950 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4071 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3820 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_metrics.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3760 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5575 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    16304 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2440 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    11875 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_summary.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2444 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_providers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3763 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/metrics_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3087 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2628 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5619 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_v2_ids_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4109 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_vote.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14536 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/msg_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20441 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/network_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    21507 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3748 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_provider.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4111 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_providers.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3732 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_jail.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3728 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_keygen_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4804 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_preflight_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3712 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_pub_key_set.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/nodes_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    12377 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/observed_tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/outbound_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2899 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ping.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6975 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pol_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20318 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2388 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pools_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7066 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8184 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_fees.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    26967 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_close_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    26986 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_open_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20465 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_deposit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    20804 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_withdraw_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    24690 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8754 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/savers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/scheduled_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    14192 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2428 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swaps_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2408 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swap_queue_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7826 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swapper_clout_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7228 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3632 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_alias.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2404 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     7043 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_account_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2424 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_accounts_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4831 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_unit_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2412 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/trade_units_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3937 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_keysign_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3644 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_metric.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6573 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_details_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9938 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_out_item.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6805 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10350 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_signers_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     8982 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     9909 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3538 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     6606 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5854 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5938 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3604 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4149 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5297 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5286 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5721 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    12716 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3620 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_address.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3838 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_info.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     4833 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_pubkeys_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2392 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     3588 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_router.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     2396 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vaults_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)     5861 2024-03-31 19:25:01.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/version_response.py
+-rw-r--r--   0 tirinox    (501) staff       (20)    10622 2024-03-31 19:25:02.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode/rest.py
+drwxr-xr-x   0 tirinox    (501) staff       (20)        0 2024-04-01 10:29:36.056629 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/
+-rw-r--r--   0 tirinox    (501) staff       (20)    13717 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/PKG-INFO
+-rw-r--r--   0 tirinox    (501) staff       (20)    10309 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/SOURCES.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)        1 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/dependency_links.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       56 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/requires.txt
+-rw-r--r--   0 tirinox    (501) staff       (20)       24 2024-04-01 10:29:36.000000 xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/top_level.txt
```

### Comparing `xchainpy2-thornode-1.125.0/LICENSE` & `xchainpy2-thornode-1.130.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xchainpy2-thornode-1.125.0/PKG-INFO` & `xchainpy2-thornode-1.130.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xchainpy2-thornode
-Version: 1.125.0
+Version: 1.130.1
 Summary: Thornode API
 Home-page: 
 Author-email: devs@thorchain.org
 Keywords: Swagger,Thornode API
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: urllib3>=1.15
@@ -14,16 +14,16 @@
 Requires-Dist: aiohttp
 
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.125.0
-- Package version: 1.125.0
+- API version: 1.130.1
+- Package version: 1.130.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -128,14 +128,18 @@
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
+*TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
+*TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
+*TradeUnitApi* | [**trade_unit**](docs/TradeUnitApi.md#trade_unit) | **GET** /thorchain/trade/unit/{asset} | 
+*TradeUnitsApi* | [**trade_units**](docs/TradeUnitsApi.md#trade_units) | **GET** /thorchain/trade/units | 
 *TransactionsApi* | [**tx**](docs/TransactionsApi.md#tx) | **GET** /thorchain/tx/{hash} | 
 *TransactionsApi* | [**tx_signers**](docs/TransactionsApi.md#tx_signers) | **GET** /thorchain/tx/details/{hash} | 
 *TransactionsApi* | [**tx_signers_old**](docs/TransactionsApi.md#tx_signers_old) | **GET** /thorchain/tx/{hash}/signers | 
 *TransactionsApi* | [**tx_stages**](docs/TransactionsApi.md#tx_stages) | **GET** /thorchain/tx/stages/{hash} | 
 *TransactionsApi* | [**tx_status**](docs/TransactionsApi.md#tx_status) | **GET** /thorchain/tx/status/{hash} | 
 *VaultsApi* | [**asgard**](docs/VaultsApi.md#asgard) | **GET** /thorchain/vaults/asgard | 
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /thorchain/vault/{pubkey} | 
@@ -215,14 +219,18 @@
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
+ - [TradeAccountResponse](docs/TradeAccountResponse.md)
+ - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
+ - [TradeUnitResponse](docs/TradeUnitResponse.md)
+ - [TradeUnitsResponse](docs/TradeUnitsResponse.md)
  - [TssKeysignMetric](docs/TssKeysignMetric.md)
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
```

### Comparing `xchainpy2-thornode-1.125.0/README.md` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,29 @@
+Metadata-Version: 2.1
+Name: xchainpy2-thornode
+Version: 1.130.1
+Summary: Thornode API
+Home-page: 
+Author-email: devs@thorchain.org
+Keywords: Swagger,Thornode API
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: urllib3>=1.15
+Requires-Dist: six>=1.10
+Requires-Dist: certifi
+Requires-Dist: python-dateutil
+Requires-Dist: aiohttp
+
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.125.0
-- Package version: 1.125.0
+- API version: 1.130.1
+- Package version: 1.130.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -113,14 +128,18 @@
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
+*TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
+*TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
+*TradeUnitApi* | [**trade_unit**](docs/TradeUnitApi.md#trade_unit) | **GET** /thorchain/trade/unit/{asset} | 
+*TradeUnitsApi* | [**trade_units**](docs/TradeUnitsApi.md#trade_units) | **GET** /thorchain/trade/units | 
 *TransactionsApi* | [**tx**](docs/TransactionsApi.md#tx) | **GET** /thorchain/tx/{hash} | 
 *TransactionsApi* | [**tx_signers**](docs/TransactionsApi.md#tx_signers) | **GET** /thorchain/tx/details/{hash} | 
 *TransactionsApi* | [**tx_signers_old**](docs/TransactionsApi.md#tx_signers_old) | **GET** /thorchain/tx/{hash}/signers | 
 *TransactionsApi* | [**tx_stages**](docs/TransactionsApi.md#tx_stages) | **GET** /thorchain/tx/stages/{hash} | 
 *TransactionsApi* | [**tx_status**](docs/TransactionsApi.md#tx_status) | **GET** /thorchain/tx/status/{hash} | 
 *VaultsApi* | [**asgard**](docs/VaultsApi.md#asgard) | **GET** /thorchain/vaults/asgard | 
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /thorchain/vault/{pubkey} | 
@@ -200,14 +219,18 @@
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
+ - [TradeAccountResponse](docs/TradeAccountResponse.md)
+ - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
+ - [TradeUnitResponse](docs/TradeUnitResponse.md)
+ - [TradeUnitsResponse](docs/TradeUnitsResponse.md)
  - [TssKeysignMetric](docs/TssKeysignMetric.md)
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
```

### Comparing `xchainpy2-thornode-1.125.0/setup.py` & `xchainpy2-thornode-1.130.1/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from setuptools import setup, find_packages  # noqa: H301
 
 NAME = "xchainpy2-thornode"
-VERSION = "1.125.0"
+VERSION = "1.130.1"
 # To install the library, run the following
 #
 # python setup.py install
 #
 # prerequisite: setuptools
 # http://pypi.python.org/pypi/setuptools
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_ban_response.py` & `xchainpy2-thornode-1.130.1/test/test_ban_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_base_quote_response.py` & `xchainpy2-thornode-1.130.1/test/test_base_quote_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_api.py` & `xchainpy2-thornode-1.130.1/test/test_trade_units_api.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.block_api import BlockApi  # noqa: E501
+from xchainpy2_thornode.api.trade_units_api import TradeUnitsApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestBlockApi(unittest.TestCase):
-    """BlockApi unit test stubs"""
+class TestTradeUnitsApi(unittest.TestCase):
+    """TradeUnitsApi unit test stubs"""
 
     def setUp(self):
-        self.api = BlockApi()  # noqa: E501
+        self.api = TradeUnitsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_block(self):
-        """Test case for block
+    def test_trade_units(self):
+        """Test case for trade_units
 
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_response.py` & `xchainpy2-thornode-1.130.1/test/test_saver_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.block_response import BlockResponse  # noqa: E501
+from xchainpy2_thornode.models.saver_response import SaverResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestBlockResponse(unittest.TestCase):
-    """BlockResponse unit test stubs"""
+class TestSaverResponse(unittest.TestCase):
+    """SaverResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBlockResponse(self):
-        """Test BlockResponse"""
+    def testSaverResponse(self):
+        """Test SaverResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.block_response.BlockResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.saver_response.SaverResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_response_header.py` & `xchainpy2-thornode-1.130.1/test/test_block_response_header.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_response_header_version.py` & `xchainpy2-thornode-1.130.1/test/test_block_response_header_version.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_response_id.py` & `xchainpy2-thornode-1.130.1/test/test_block_response_id.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_response_id_parts.py` & `xchainpy2-thornode-1.130.1/test/test_block_response_id_parts.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_tx.py` & `xchainpy2-thornode-1.130.1/test/test_block_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_block_tx_result.py` & `xchainpy2-thornode-1.130.1/test/test_block_tx_result.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_borrower.py` & `xchainpy2-thornode-1.130.1/test/test_borrower.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_borrower_response.py` & `xchainpy2-thornode-1.130.1/test/test_borrower_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_borrowers_api.py` & `xchainpy2-thornode-1.130.1/test/test_borrowers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_borrowers_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.borrowers_response import BorrowersResponse  # noqa: E501
+from xchainpy2_thornode.models.tx import Tx  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestBorrowersResponse(unittest.TestCase):
-    """BorrowersResponse unit test stubs"""
+class TestTx(unittest.TestCase):
+    """Tx unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testBorrowersResponse(self):
-        """Test BorrowersResponse"""
+    def testTx(self):
+        """Test Tx"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.borrowers_response.BorrowersResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx.Tx()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_chain_height.py` & `xchainpy2-thornode-1.130.1/test/test_chain_height.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_clout_api.py` & `xchainpy2-thornode-1.130.1/test/test_clout_api.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_coin.py` & `xchainpy2-thornode-1.130.1/test/test_coin.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_constants_response.py` & `xchainpy2-thornode-1.130.1/test/test_constants_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_derived_pool.py` & `xchainpy2-thornode-1.130.1/test/test_derived_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_derived_pool_response.py` & `xchainpy2-thornode-1.130.1/test/test_derived_pools_response.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.derived_pool_response import DerivedPoolResponse  # noqa: E501
+from xchainpy2_thornode.models.derived_pools_response import DerivedPoolsResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestDerivedPoolResponse(unittest.TestCase):
-    """DerivedPoolResponse unit test stubs"""
+class TestDerivedPoolsResponse(unittest.TestCase):
+    """DerivedPoolsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDerivedPoolResponse(self):
-        """Test DerivedPoolResponse"""
+    def testDerivedPoolsResponse(self):
+        """Test DerivedPoolsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.derived_pool_response.DerivedPoolResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.derived_pools_response.DerivedPoolsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_derived_pools_response.py` & `xchainpy2-thornode-1.130.1/test/test_pools_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.derived_pools_response import DerivedPoolsResponse  # noqa: E501
+from xchainpy2_thornode.models.pools_response import PoolsResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestDerivedPoolsResponse(unittest.TestCase):
-    """DerivedPoolsResponse unit test stubs"""
+class TestPoolsResponse(unittest.TestCase):
+    """PoolsResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testDerivedPoolsResponse(self):
-        """Test DerivedPoolsResponse"""
+    def testPoolsResponse(self):
+        """Test PoolsResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.derived_pools_response.DerivedPoolsResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.pools_response.PoolsResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_health_api.py` & `xchainpy2-thornode-1.130.1/test/test_health_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_inbound_address.py` & `xchainpy2-thornode-1.130.1/test/test_inbound_address.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_inbound_addresses_response.py` & `xchainpy2-thornode-1.130.1/test/test_inbound_addresses_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_invariant_response.py` & `xchainpy2-thornode-1.130.1/test/test_invariant_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_invariants_api.py` & `xchainpy2-thornode-1.130.1/test/test_invariants_api.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_invariants_response.py` & `xchainpy2-thornode-1.130.1/test/test_invariants_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_keygen_metric.py` & `xchainpy2-thornode-1.130.1/test/test_keygen_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_keygen_metrics_response.py` & `xchainpy2-thornode-1.130.1/test/test_keygen_metrics_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_keysign_info.py` & `xchainpy2-thornode-1.130.1/test/test_keysign_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_keysign_metrics.py` & `xchainpy2-thornode-1.130.1/test/test_keysign_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_keysign_response.py` & `xchainpy2-thornode-1.130.1/test/test_keysign_response.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_last_block.py` & `xchainpy2-thornode-1.130.1/test/test_last_block.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_last_block_response.py` & `xchainpy2-thornode-1.130.1/test/test_last_block_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_liquidity_provider.py` & `xchainpy2-thornode-1.130.1/test/test_liquidity_provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_liquidity_provider_response.py` & `xchainpy2-thornode-1.130.1/test/test_liquidity_provider_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_liquidity_provider_summary.py` & `xchainpy2-thornode-1.130.1/test/test_liquidity_provider_summary.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_liquidity_providers_api.py` & `xchainpy2-thornode-1.130.1/test/test_liquidity_providers_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_liquidity_providers_response.py` & `xchainpy2-thornode-1.130.1/test/test_liquidity_providers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_metrics_response.py` & `xchainpy2-thornode-1.130.1/test/test_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_mimir_api.py` & `xchainpy2-thornode-1.130.1/test/test_network_api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,75 +1,81 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.mimir_api import MimirApi  # noqa: E501
+from xchainpy2_thornode.api.network_api import NetworkApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestMimirApi(unittest.TestCase):
-    """MimirApi unit test stubs"""
+class TestNetworkApi(unittest.TestCase):
+    """NetworkApi unit test stubs"""
 
     def setUp(self):
-        self.api = MimirApi()  # noqa: E501
+        self.api = NetworkApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_mimir(self):
-        """Test case for mimir
+    def test_ban(self):
+        """Test case for ban
 
         """
         pass
 
-    def test_mimir_admin(self):
-        """Test case for mimir_admin
+    def test_constants(self):
+        """Test case for constants
 
         """
         pass
 
-    def test_mimir_key(self):
-        """Test case for mimir_key
+    def test_inbound_addresses(self):
+        """Test case for inbound_addresses
 
         """
         pass
 
-    def test_mimir_node(self):
-        """Test case for mimir_node
+    def test_lastblock(self):
+        """Test case for lastblock
 
         """
         pass
 
-    def test_mimir_nodes(self):
-        """Test case for mimir_nodes
+    def test_lastblock_chain(self):
+        """Test case for lastblock_chain
 
         """
         pass
 
-    def test_mimir_v2(self):
-        """Test case for mimir_v2
+    def test_network(self):
+        """Test case for network
 
         """
         pass
 
-    def test_mimir_v2_ids(self):
-        """Test case for mimir_v2_ids
+    def test_ragnarok(self):
+        """Test case for ragnarok
+
+        """
+        pass
+
+    def test_version(self):
+        """Test case for version
 
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_mimir_nodes_response.py` & `xchainpy2-thornode-1.130.1/test/test_mimir_nodes_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_mimir_response.py` & `xchainpy2-thornode-1.130.1/test/test_mimir_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_mimir_v2_ids_response.py` & `xchainpy2-thornode-1.130.1/test/test_mimir_v2_ids_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_mimir_vote.py` & `xchainpy2-thornode-1.130.1/test/test_mimir_vote.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_msg_swap.py` & `xchainpy2-thornode-1.130.1/test/test_msg_swap.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_network_api.py` & `xchainpy2-thornode-1.130.1/test/test_streaming_swap_api.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,81 +1,45 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.network_api import NetworkApi  # noqa: E501
+from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestNetworkApi(unittest.TestCase):
-    """NetworkApi unit test stubs"""
+class TestStreamingSwapApi(unittest.TestCase):
+    """StreamingSwapApi unit test stubs"""
 
     def setUp(self):
-        self.api = NetworkApi()  # noqa: E501
+        self.api = StreamingSwapApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_ban(self):
-        """Test case for ban
+    def test_stream_swap(self):
+        """Test case for stream_swap
 
         """
         pass
 
-    def test_constants(self):
-        """Test case for constants
-
-        """
-        pass
-
-    def test_inbound_addresses(self):
-        """Test case for inbound_addresses
-
-        """
-        pass
-
-    def test_lastblock(self):
-        """Test case for lastblock
-
-        """
-        pass
-
-    def test_lastblock_chain(self):
-        """Test case for lastblock_chain
-
-        """
-        pass
-
-    def test_network(self):
-        """Test case for network
-
-        """
-        pass
-
-    def test_ragnarok(self):
-        """Test case for ragnarok
-
-        """
-        pass
-
-    def test_version(self):
-        """Test case for version
+    def test_stream_swaps(self):
+        """Test case for stream_swaps
 
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_network_response.py` & `xchainpy2-thornode-1.130.1/test/test_network_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node.py` & `xchainpy2-thornode-1.130.1/test/test_node.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_bond_provider.py` & `xchainpy2-thornode-1.130.1/test/test_node_bond_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_bond_providers.py` & `xchainpy2-thornode-1.130.1/test/test_node_bond_providers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_jail.py` & `xchainpy2-thornode-1.130.1/test/test_node_jail.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_keygen_metric.py` & `xchainpy2-thornode-1.130.1/test/test_node_keygen_metric.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_preflight_status.py` & `xchainpy2-thornode-1.130.1/test/test_node_preflight_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_pub_key_set.py` & `xchainpy2-thornode-1.130.1/test/test_node_pub_key_set.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_node_response.py` & `xchainpy2-thornode-1.130.1/test/test_node_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_nodes_api.py` & `xchainpy2-thornode-1.130.1/test/test_nodes_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_nodes_response.py` & `xchainpy2-thornode-1.130.1/test/test_nodes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_observed_tx.py` & `xchainpy2-thornode-1.130.1/test/test_observed_tx.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_outbound_response.py` & `xchainpy2-thornode-1.130.1/test/test_outbound_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_ping.py` & `xchainpy2-thornode-1.130.1/test/test_ping.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pol_api.py` & `xchainpy2-thornode-1.130.1/test/test_pol_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pol_response.py` & `xchainpy2-thornode-1.130.1/test/test_pol_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pool.py` & `xchainpy2-thornode-1.130.1/test/test_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pool_response.py` & `xchainpy2-thornode-1.130.1/test/test_pool_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pools_api.py` & `xchainpy2-thornode-1.130.1/test/test_pools_api.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_pools_response.py` & `xchainpy2-thornode-1.130.1/test/test_version_response.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.pools_response import PoolsResponse  # noqa: E501
+from xchainpy2_thornode.models.version_response import VersionResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestPoolsResponse(unittest.TestCase):
-    """PoolsResponse unit test stubs"""
+class TestVersionResponse(unittest.TestCase):
+    """VersionResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testPoolsResponse(self):
-        """Test PoolsResponse"""
+    def testVersionResponse(self):
+        """Test VersionResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.pools_response.PoolsResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.version_response.VersionResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_queue_api.py` & `xchainpy2-thornode-1.130.1/test/test_queue_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_queue_response.py` & `xchainpy2-thornode-1.130.1/test/test_queue_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_api.py` & `xchainpy2-thornode-1.130.1/test/test_quote_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_fees.py` & `xchainpy2-thornode-1.130.1/test/test_quote_fees.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_loan_close_response.py` & `xchainpy2-thornode-1.130.1/test/test_quote_loan_close_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_loan_open_response.py` & `xchainpy2-thornode-1.130.1/test/test_quote_loan_open_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_saver_deposit_response.py` & `xchainpy2-thornode-1.130.1/test/test_quote_saver_deposit_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_saver_withdraw_response.py` & `xchainpy2-thornode-1.130.1/test/test_quote_saver_withdraw_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_quote_swap_response.py` & `xchainpy2-thornode-1.130.1/test/test_quote_swap_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_saver.py` & `xchainpy2-thornode-1.130.1/test/test_saver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_saver_response.py` & `xchainpy2-thornode-1.130.1/test/test_block_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.saver_response import SaverResponse  # noqa: E501
+from xchainpy2_thornode.models.block_response import BlockResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestSaverResponse(unittest.TestCase):
-    """SaverResponse unit test stubs"""
+class TestBlockResponse(unittest.TestCase):
+    """BlockResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSaverResponse(self):
-        """Test SaverResponse"""
+    def testBlockResponse(self):
+        """Test BlockResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.saver_response.SaverResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.block_response.BlockResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_savers_api.py` & `xchainpy2-thornode-1.130.1/test/test_savers_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_savers_response.py` & `xchainpy2-thornode-1.130.1/test/test_savers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_scheduled_response.py` & `xchainpy2-thornode-1.130.1/test/test_scheduled_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_streaming_swap.py` & `xchainpy2-thornode-1.130.1/test/test_streaming_swap.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_streaming_swap_api.py` & `xchainpy2-thornode-1.130.1/test/test_vaults_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,45 +1,57 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi  # noqa: E501
+from xchainpy2_thornode.api.vaults_api import VaultsApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestStreamingSwapApi(unittest.TestCase):
-    """StreamingSwapApi unit test stubs"""
+class TestVaultsApi(unittest.TestCase):
+    """VaultsApi unit test stubs"""
 
     def setUp(self):
-        self.api = StreamingSwapApi()  # noqa: E501
+        self.api = VaultsApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def test_stream_swap(self):
-        """Test case for stream_swap
+    def test_asgard(self):
+        """Test case for asgard
 
         """
         pass
 
-    def test_stream_swaps(self):
-        """Test case for stream_swaps
+    def test_vault(self):
+        """Test case for vault
+
+        """
+        pass
+
+    def test_vault_pubkeys(self):
+        """Test case for vault_pubkeys
+
+        """
+        pass
+
+    def test_yggdrasil(self):
+        """Test case for yggdrasil
 
         """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_streaming_swap_response.py` & `xchainpy2-thornode-1.130.1/test/test_streaming_swap_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_streaming_swaps_response.py` & `xchainpy2-thornode-1.130.1/test/test_streaming_swaps_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_swap_queue_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx_response.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse  # noqa: E501
+from xchainpy2_thornode.models.tx_response import TxResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestSwapQueueResponse(unittest.TestCase):
-    """SwapQueueResponse unit test stubs"""
+class TestTxResponse(unittest.TestCase):
+    """TxResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testSwapQueueResponse(self):
-        """Test SwapQueueResponse"""
+    def testTxResponse(self):
+        """Test TxResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.swap_queue_response.SwapQueueResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_response.TxResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_swapper_clout_response.py` & `xchainpy2-thornode-1.130.1/test/test_swapper_clout_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_thorname.py` & `xchainpy2-thornode-1.130.1/test/test_thorname.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_thorname_alias.py` & `xchainpy2-thornode-1.130.1/test/test_thorname_alias.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_thorname_response.py` & `xchainpy2-thornode-1.130.1/test/test_thorname_response.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_thornames_api.py` & `xchainpy2-thornode-1.130.1/test/test_thornames_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_transactions_api.py` & `xchainpy2-thornode-1.130.1/test/test_transactions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tss_api.py` & `xchainpy2-thornode-1.130.1/test/test_tss_api.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tss_keysign_metric.py` & `xchainpy2-thornode-1.130.1/test/test_tss_keysign_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tss_metric.py` & `xchainpy2-thornode-1.130.1/test/test_tss_metric.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx.py` & `xchainpy2-thornode-1.130.1/test/test_tx_out_item.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx import Tx  # noqa: E501
+from xchainpy2_thornode.models.tx_out_item import TxOutItem  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTx(unittest.TestCase):
-    """Tx unit test stubs"""
+class TestTxOutItem(unittest.TestCase):
+    """TxOutItem unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTx(self):
-        """Test Tx"""
+    def testTxOutItem(self):
+        """Test TxOutItem"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx.Tx()  # noqa: E501
+        # model = xchainpy2_thornode.models.tx_out_item.TxOutItem()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_details_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_out_item.py` & `xchainpy2-thornode-1.130.1/test/test_vault_router.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_out_item import TxOutItem  # noqa: E501
+from xchainpy2_thornode.models.vault_router import VaultRouter  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxOutItem(unittest.TestCase):
-    """TxOutItem unit test stubs"""
+class TestVaultRouter(unittest.TestCase):
+    """VaultRouter unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxOutItem(self):
-        """Test TxOutItem"""
+    def testVaultRouter(self):
+        """Test VaultRouter"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_out_item.TxOutItem()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault_router.VaultRouter()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_response.py` & `xchainpy2-thornode-1.130.1/test/test_trade_unit_response.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.tx_response import TxResponse  # noqa: E501
+from xchainpy2_thornode.models.trade_unit_response import TradeUnitResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestTxResponse(unittest.TestCase):
-    """TxResponse unit test stubs"""
+class TestTradeUnitResponse(unittest.TestCase):
+    """TradeUnitResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testTxResponse(self):
-        """Test TxResponse"""
+    def testTradeUnitResponse(self):
+        """Test TradeUnitResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.tx_response.TxResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.trade_unit_response.TradeUnitResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_signers_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx_signers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_confirmation_counted.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_confirmation_counted.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_finalised.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_finalised.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_inbound_observed.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_inbound_observed.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_outbound_delay.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_delay.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_outbound_signed.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_outbound_signed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_finalised.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_finalised.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_status.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_stages_response_swap_status_streaming.py` & `xchainpy2-thornode-1.130.1/test/test_tx_stages_response_swap_status_streaming.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_status_response.py` & `xchainpy2-thornode-1.130.1/test/test_tx_status_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_tx_status_response_planned_out_txs.py` & `xchainpy2-thornode-1.130.1/test/test_tx_status_response_planned_out_txs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault.py` & `xchainpy2-thornode-1.130.1/test/test_vault_info.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault import Vault  # noqa: E501
+from xchainpy2_thornode.models.vault_info import VaultInfo  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVault(unittest.TestCase):
-    """Vault unit test stubs"""
+class TestVaultInfo(unittest.TestCase):
+    """VaultInfo unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVault(self):
-        """Test Vault"""
+    def testVaultInfo(self):
+        """Test VaultInfo"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault.Vault()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault_info.VaultInfo()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault_address.py` & `xchainpy2-thornode-1.130.1/test/test_vault_address.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault_info.py` & `xchainpy2-thornode-1.130.1/test/test_vault_response.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault_info import VaultInfo  # noqa: E501
+from xchainpy2_thornode.models.vault_response import VaultResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultInfo(unittest.TestCase):
-    """VaultInfo unit test stubs"""
+class TestVaultResponse(unittest.TestCase):
+    """VaultResponse unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultInfo(self):
-        """Test VaultInfo"""
+    def testVaultResponse(self):
+        """Test VaultResponse"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault_info.VaultInfo()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault_response.VaultResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault_pubkeys_response.py` & `xchainpy2-thornode-1.130.1/test/test_vault_pubkeys_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault_response.py` & `xchainpy2-thornode-1.130.1/test/test_vault.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault_response import VaultResponse  # noqa: E501
+from xchainpy2_thornode.models.vault import Vault  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultResponse(unittest.TestCase):
-    """VaultResponse unit test stubs"""
+class TestVault(unittest.TestCase):
+    """Vault unit test stubs"""
 
     def setUp(self):
         pass
 
     def tearDown(self):
         pass
 
-    def testVaultResponse(self):
-        """Test VaultResponse"""
+    def testVault(self):
+        """Test Vault"""
         # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault_response.VaultResponse()  # noqa: E501
+        # model = xchainpy2_thornode.models.vault.Vault()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vault_router.py` & `xchainpy2-thornode-1.130.1/test/test_block_api.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.vault_router import VaultRouter  # noqa: E501
+from xchainpy2_thornode.api.block_api import BlockApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultRouter(unittest.TestCase):
-    """VaultRouter unit test stubs"""
+class TestBlockApi(unittest.TestCase):
+    """BlockApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = BlockApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testVaultRouter(self):
-        """Test VaultRouter"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.vault_router.VaultRouter()  # noqa: E501
+    def test_block(self):
+        """Test case for block
+
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vaults_api.py` & `xchainpy2-thornode-1.130.1/test/test_swap_queue_response.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,57 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.api.vaults_api import VaultsApi  # noqa: E501
+from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVaultsApi(unittest.TestCase):
-    """VaultsApi unit test stubs"""
+class TestSwapQueueResponse(unittest.TestCase):
+    """SwapQueueResponse unit test stubs"""
 
     def setUp(self):
-        self.api = VaultsApi()  # noqa: E501
-
-    def tearDown(self):
-        pass
-
-    def test_asgard(self):
-        """Test case for asgard
-
-        """
         pass
 
-    def test_vault(self):
-        """Test case for vault
-
-        """
-        pass
-
-    def test_vault_pubkeys(self):
-        """Test case for vault_pubkeys
-
-        """
+    def tearDown(self):
         pass
 
-    def test_yggdrasil(self):
-        """Test case for yggdrasil
-
-        """
+    def testSwapQueueResponse(self):
+        """Test SwapQueueResponse"""
+        # FIXME: construct object with mandatory attributes with example values
+        # model = xchainpy2_thornode.models.swap_queue_response.SwapQueueResponse()  # noqa: E501
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_vaults_response.py` & `xchainpy2-thornode-1.130.1/test/test_vaults_response.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
```

### Comparing `xchainpy2-thornode-1.125.0/test/test_version_response.py` & `xchainpy2-thornode-1.130.1/test/test_trade_unit_api.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,39 +1,39 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import unittest
 
 import xchainpy2_thornode
-from xchainpy2_thornode.models.version_response import VersionResponse  # noqa: E501
+from xchainpy2_thornode.api.trade_unit_api import TradeUnitApi  # noqa: E501
 from xchainpy2_thornode.rest import ApiException
 
 
-class TestVersionResponse(unittest.TestCase):
-    """VersionResponse unit test stubs"""
+class TestTradeUnitApi(unittest.TestCase):
+    """TradeUnitApi unit test stubs"""
 
     def setUp(self):
-        pass
+        self.api = TradeUnitApi()  # noqa: E501
 
     def tearDown(self):
         pass
 
-    def testVersionResponse(self):
-        """Test VersionResponse"""
-        # FIXME: construct object with mandatory attributes with example values
-        # model = xchainpy2_thornode.models.version_response.VersionResponse()  # noqa: E501
+    def test_trade_unit(self):
+        """Test case for trade_unit
+
+        """
         pass
 
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/__init__.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import apis into sdk package
@@ -28,14 +28,18 @@
 from xchainpy2_thornode.api.pools_api import PoolsApi
 from xchainpy2_thornode.api.queue_api import QueueApi
 from xchainpy2_thornode.api.quote_api import QuoteApi
 from xchainpy2_thornode.api.savers_api import SaversApi
 from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi
 from xchainpy2_thornode.api.tss_api import TSSApi
 from xchainpy2_thornode.api.thornames_api import ThornamesApi
+from xchainpy2_thornode.api.trade_account_api import TradeAccountApi
+from xchainpy2_thornode.api.trade_accounts_api import TradeAccountsApi
+from xchainpy2_thornode.api.trade_unit_api import TradeUnitApi
+from xchainpy2_thornode.api.trade_units_api import TradeUnitsApi
 from xchainpy2_thornode.api.transactions_api import TransactionsApi
 from xchainpy2_thornode.api.vaults_api import VaultsApi
 # import ApiClient
 from xchainpy2_thornode.api_client import ApiClient
 from xchainpy2_thornode.configuration import Configuration
 # import models into sdk package
 from xchainpy2_thornode.models.ban_response import BanResponse
@@ -109,14 +113,18 @@
 from xchainpy2_thornode.models.streaming_swap_response import StreamingSwapResponse
 from xchainpy2_thornode.models.streaming_swaps_response import StreamingSwapsResponse
 from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse
 from xchainpy2_thornode.models.swapper_clout_response import SwapperCloutResponse
 from xchainpy2_thornode.models.thorname import Thorname
 from xchainpy2_thornode.models.thorname_alias import ThornameAlias
 from xchainpy2_thornode.models.thorname_response import ThornameResponse
+from xchainpy2_thornode.models.trade_account_response import TradeAccountResponse
+from xchainpy2_thornode.models.trade_accounts_response import TradeAccountsResponse
+from xchainpy2_thornode.models.trade_unit_response import TradeUnitResponse
+from xchainpy2_thornode.models.trade_units_response import TradeUnitsResponse
 from xchainpy2_thornode.models.tss_keysign_metric import TssKeysignMetric
 from xchainpy2_thornode.models.tss_metric import TssMetric
 from xchainpy2_thornode.models.tx import Tx
 from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse
 from xchainpy2_thornode.models.tx_out_item import TxOutItem
 from xchainpy2_thornode.models.tx_response import TxResponse
 from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/__init__.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -16,9 +16,13 @@
 from xchainpy2_thornode.api.pools_api import PoolsApi
 from xchainpy2_thornode.api.queue_api import QueueApi
 from xchainpy2_thornode.api.quote_api import QuoteApi
 from xchainpy2_thornode.api.savers_api import SaversApi
 from xchainpy2_thornode.api.streaming_swap_api import StreamingSwapApi
 from xchainpy2_thornode.api.tss_api import TSSApi
 from xchainpy2_thornode.api.thornames_api import ThornamesApi
+from xchainpy2_thornode.api.trade_account_api import TradeAccountApi
+from xchainpy2_thornode.api.trade_accounts_api import TradeAccountsApi
+from xchainpy2_thornode.api.trade_unit_api import TradeUnitApi
+from xchainpy2_thornode.api.trade_units_api import TradeUnitsApi
 from xchainpy2_thornode.api.transactions_api import TransactionsApi
 from xchainpy2_thornode.api.vaults_api import VaultsApi
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/block_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/block_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/borrowers_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/borrowers_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/clout_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/clout_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/health_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/health_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/invariants_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/invariants_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/liquidity_providers_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/liquidity_providers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/mimir_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/mimir_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/network_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/network_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/nodes_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/nodes_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/pol_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pol_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/pools_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/pools_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/queue_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/queue_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/quote_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/quote_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
@@ -475,14 +475,15 @@
 
         :param async_req bool
         :param int height: optional block height, defaults to current tip
         :param str from_asset: the source asset
         :param str to_asset: the target asset
         :param int amount: the source asset amount in 1e8 decimals
         :param str destination: the destination address, required to generate memo
+        :param str refund_address: the refund address, refunds will be sent here if the swap fails
         :param int streaming_interval: the interval in which streaming swaps are swapped
         :param int streaming_quantity: the quantity of swaps within a streaming swap
         :param int tolerance_bps: the maximum basis points from the current feeless swap price to set the limit in the generated memo
         :param int affiliate_bps: the affiliate fee in basis points
         :param str affiliate: the affiliate (address or thorname)
         :return: QuoteSwapResponse
                  If the method is called asynchronously,
@@ -506,25 +507,26 @@
 
         :param async_req bool
         :param int height: optional block height, defaults to current tip
         :param str from_asset: the source asset
         :param str to_asset: the target asset
         :param int amount: the source asset amount in 1e8 decimals
         :param str destination: the destination address, required to generate memo
+        :param str refund_address: the refund address, refunds will be sent here if the swap fails
         :param int streaming_interval: the interval in which streaming swaps are swapped
         :param int streaming_quantity: the quantity of swaps within a streaming swap
         :param int tolerance_bps: the maximum basis points from the current feeless swap price to set the limit in the generated memo
         :param int affiliate_bps: the affiliate fee in basis points
         :param str affiliate: the affiliate (address or thorname)
         :return: QuoteSwapResponse
                  If the method is called asynchronously,
                  returns the request thread.
         """
 
-        all_params = ['height', 'from_asset', 'to_asset', 'amount', 'destination', 'streaming_interval', 'streaming_quantity', 'tolerance_bps', 'affiliate_bps', 'affiliate']  # noqa: E501
+        all_params = ['height', 'from_asset', 'to_asset', 'amount', 'destination', 'refund_address', 'streaming_interval', 'streaming_quantity', 'tolerance_bps', 'affiliate_bps', 'affiliate']  # noqa: E501
         all_params.append('async_req')
         all_params.append('_return_http_data_only')
         all_params.append('_preload_content')
         all_params.append('_request_timeout')
 
         params = locals()
         for key, val in six.iteritems(params['kwargs']):
@@ -547,14 +549,16 @@
             query_params.append(('from_asset', params['from_asset']))  # noqa: E501
         if 'to_asset' in params:
             query_params.append(('to_asset', params['to_asset']))  # noqa: E501
         if 'amount' in params:
             query_params.append(('amount', params['amount']))  # noqa: E501
         if 'destination' in params:
             query_params.append(('destination', params['destination']))  # noqa: E501
+        if 'refund_address' in params:
+            query_params.append(('refund_address', params['refund_address']))  # noqa: E501
         if 'streaming_interval' in params:
             query_params.append(('streaming_interval', params['streaming_interval']))  # noqa: E501
         if 'streaming_quantity' in params:
             query_params.append(('streaming_quantity', params['streaming_quantity']))  # noqa: E501
         if 'tolerance_bps' in params:
             query_params.append(('tolerance_bps', params['tolerance_bps']))  # noqa: E501
         if 'affiliate_bps' in params:
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/savers_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/savers_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/streaming_swap_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/streaming_swap_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/thornames_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/thornames_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/transactions_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/transactions_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/tss_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/tss_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api/vaults_api.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api/vaults_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/api_client.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # coding: utf-8
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
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
-        self.user_agent = 'Swagger-Codegen/1.125.0/python'
+        self.user_agent = 'Swagger-Codegen/1.130.1/python'
 
     def __del__(self):
         self.pool.close()
         self.pool.join()
 
     @property
     def user_agent(self):
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/configuration.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/configuration.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
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
-               "Version of the API: 1.125.0\n"\
-               "SDK Package Version: 1.125.0".\
+               "Version of the API: 1.130.1\n"\
+               "SDK Package Version: 1.130.1".\
                format(env=sys.platform, pyversion=sys.version)
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/__init__.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 from __future__ import absolute_import
 
 # import models into model package
@@ -85,14 +85,18 @@
 from xchainpy2_thornode.models.streaming_swap_response import StreamingSwapResponse
 from xchainpy2_thornode.models.streaming_swaps_response import StreamingSwapsResponse
 from xchainpy2_thornode.models.swap_queue_response import SwapQueueResponse
 from xchainpy2_thornode.models.swapper_clout_response import SwapperCloutResponse
 from xchainpy2_thornode.models.thorname import Thorname
 from xchainpy2_thornode.models.thorname_alias import ThornameAlias
 from xchainpy2_thornode.models.thorname_response import ThornameResponse
+from xchainpy2_thornode.models.trade_account_response import TradeAccountResponse
+from xchainpy2_thornode.models.trade_accounts_response import TradeAccountsResponse
+from xchainpy2_thornode.models.trade_unit_response import TradeUnitResponse
+from xchainpy2_thornode.models.trade_units_response import TradeUnitsResponse
 from xchainpy2_thornode.models.tss_keysign_metric import TssKeysignMetric
 from xchainpy2_thornode.models.tss_metric import TssMetric
 from xchainpy2_thornode.models.tx import Tx
 from xchainpy2_thornode.models.tx_details_response import TxDetailsResponse
 from xchainpy2_thornode.models.tx_out_item import TxOutItem
 from xchainpy2_thornode.models.tx_response import TxResponse
 from xchainpy2_thornode.models.tx_signers_response import TxSignersResponse
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/ban_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ban_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/base_quote_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/base_quote_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_header.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_header_version.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_header_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_id.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_response_id_parts.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_response_id_parts.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_tx.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/block_tx_result.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/block_tx_result.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrower.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrower_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrower_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/borrowers_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/borrowers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/chain_height.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/chain_height.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/coin.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/coin.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/constants_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/constants_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pool.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pool_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pool_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/derived_pools_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/derived_pools_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/inbound_address.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_address.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/inbound_addresses_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/inbound_addresses_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/invariant_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariant_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/invariants_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/invariants_response.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keygen_metric.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metric.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keygen_metrics_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keygen_metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_info.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_metrics.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_metrics.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/keysign_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/keysign_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/last_block.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/last_block_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/last_block_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_provider_summary.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_provider_summary.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/liquidity_providers_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/liquidity_providers_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/metrics_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/metrics_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_nodes_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_nodes_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_response.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_v2_ids_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_v2_ids_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/mimir_vote.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/mimir_vote.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/msg_swap.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/msg_swap.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/network_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/network_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_bond_provider.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_provider.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_bond_providers.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_bond_providers.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_jail.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_jail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_keygen_metric.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_keygen_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_preflight_status.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_preflight_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_pub_key_set.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_pub_key_set.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/node_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/node_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/nodes_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/nodes_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/observed_tx.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/observed_tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/outbound_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/outbound_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/ping.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/ping.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pol_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pol_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pool.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -41,14 +41,15 @@
         'synth_units': 'str',
         'synth_supply': 'str',
         'savers_depth': 'str',
         'savers_units': 'str',
         'synth_mint_paused': 'bool',
         'synth_supply_remaining': 'str',
         'loan_collateral': 'str',
+        'loan_collateral_remaining': 'str',
         'loan_cr': 'str',
         'derived_depth_bps': 'str'
     }
 
     attribute_map = {
         'asset': 'asset',
         'short_code': 'short_code',
@@ -63,19 +64,20 @@
         'synth_units': 'synth_units',
         'synth_supply': 'synth_supply',
         'savers_depth': 'savers_depth',
         'savers_units': 'savers_units',
         'synth_mint_paused': 'synth_mint_paused',
         'synth_supply_remaining': 'synth_supply_remaining',
         'loan_collateral': 'loan_collateral',
+        'loan_collateral_remaining': 'loan_collateral_remaining',
         'loan_cr': 'loan_cr',
         'derived_depth_bps': 'derived_depth_bps'
     }
 
-    def __init__(self, asset=None, short_code=None, status=None, decimals=None, pending_inbound_asset=None, pending_inbound_rune=None, balance_asset=None, balance_rune=None, pool_units=None, lp_units=None, synth_units=None, synth_supply=None, savers_depth=None, savers_units=None, synth_mint_paused=None, synth_supply_remaining=None, loan_collateral=None, loan_cr=None, derived_depth_bps=None):  # noqa: E501
+    def __init__(self, asset=None, short_code=None, status=None, decimals=None, pending_inbound_asset=None, pending_inbound_rune=None, balance_asset=None, balance_rune=None, pool_units=None, lp_units=None, synth_units=None, synth_supply=None, savers_depth=None, savers_units=None, synth_mint_paused=None, synth_supply_remaining=None, loan_collateral=None, loan_collateral_remaining=None, loan_cr=None, derived_depth_bps=None):  # noqa: E501
         """Pool - a model defined in Swagger"""  # noqa: E501
         self._asset = None
         self._short_code = None
         self._status = None
         self._decimals = None
         self._pending_inbound_asset = None
         self._pending_inbound_rune = None
@@ -86,14 +88,15 @@
         self._synth_units = None
         self._synth_supply = None
         self._savers_depth = None
         self._savers_units = None
         self._synth_mint_paused = None
         self._synth_supply_remaining = None
         self._loan_collateral = None
+        self._loan_collateral_remaining = None
         self._loan_cr = None
         self._derived_depth_bps = None
         self.discriminator = None
         self.asset = asset
         if short_code is not None:
             self.short_code = short_code
         self.status = status
@@ -108,14 +111,15 @@
         self.synth_units = synth_units
         self.synth_supply = synth_supply
         self.savers_depth = savers_depth
         self.savers_units = savers_units
         self.synth_mint_paused = synth_mint_paused
         self.synth_supply_remaining = synth_supply_remaining
         self.loan_collateral = loan_collateral
+        self.loan_collateral_remaining = loan_collateral_remaining
         self.loan_cr = loan_cr
         self.derived_depth_bps = derived_depth_bps
 
     @property
     def asset(self):
         """Gets the asset of this Pool.  # noqa: E501
 
@@ -517,14 +521,39 @@
         """
         if loan_collateral is None:
             raise ValueError("Invalid value for `loan_collateral`, must not be `None`")  # noqa: E501
 
         self._loan_collateral = loan_collateral
 
     @property
+    def loan_collateral_remaining(self):
+        """Gets the loan_collateral_remaining of this Pool.  # noqa: E501
+
+        the amount of remaining collateral collects for loans  # noqa: E501
+
+        :return: The loan_collateral_remaining of this Pool.  # noqa: E501
+        :rtype: str
+        """
+        return self._loan_collateral_remaining
+
+    @loan_collateral_remaining.setter
+    def loan_collateral_remaining(self, loan_collateral_remaining):
+        """Sets the loan_collateral_remaining of this Pool.
+
+        the amount of remaining collateral collects for loans  # noqa: E501
+
+        :param loan_collateral_remaining: The loan_collateral_remaining of this Pool.  # noqa: E501
+        :type: str
+        """
+        if loan_collateral_remaining is None:
+            raise ValueError("Invalid value for `loan_collateral_remaining`, must not be `None`")  # noqa: E501
+
+        self._loan_collateral_remaining = loan_collateral_remaining
+
+    @property
     def loan_cr(self):
         """Gets the loan_cr of this Pool.  # noqa: E501
 
         the current loan collateralization ratio  # noqa: E501
 
         :return: The loan_cr of this Pool.  # noqa: E501
         :rtype: str
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pool_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pool_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/pools_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/pools_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/queue_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/queue_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_fees.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_fees.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_loan_close_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_close_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_loan_open_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_loan_open_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_saver_deposit_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_deposit_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_saver_withdraw_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_saver_withdraw_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/quote_swap_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/quote_swap_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/saver.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/saver_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/savers_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SaverResponse(object):
+class SaversResponse(object):
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
-        """SaverResponse - a model defined in Swagger"""  # noqa: E501
+        """SaversResponse - a model defined in Swagger"""  # noqa: E501
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
-        if issubclass(SaverResponse, dict):
+        if issubclass(SaversResponse, dict):
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
-        if not isinstance(other, SaverResponse):
+        if not isinstance(other, SaversResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/savers_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/saver_response.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
 import six
 
-class SaversResponse(object):
+class SaverResponse(object):
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
-        """SaversResponse - a model defined in Swagger"""  # noqa: E501
+        """SaverResponse - a model defined in Swagger"""  # noqa: E501
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
-        if issubclass(SaversResponse, dict):
+        if issubclass(SaverResponse, dict):
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
-        if not isinstance(other, SaversResponse):
+        if not isinstance(other, SaverResponse):
             return False
 
         return self.__dict__ == other.__dict__
 
     def __ne__(self, other):
         """Returns true if both objects are not equal"""
         return not self == other
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/scheduled_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/scheduled_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swap.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swap_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swap_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/streaming_swaps_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/streaming_swaps_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/swap_queue_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swap_queue_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/swapper_clout_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/swapper_clout_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname_alias.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_alias.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/thorname_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/thorname_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tss_keysign_metric.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_keysign_metric.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tss_metric.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tss_metric.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_details_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_details_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_out_item.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_out_item.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
 
@@ -33,42 +33,45 @@
         'vault_pub_key': 'str',
         'coin': 'Coin',
         'memo': 'str',
         'max_gas': 'list[Coin]',
         'gas_rate': 'int',
         'in_hash': 'str',
         'out_hash': 'str',
-        'height': 'int'
+        'height': 'int',
+        'clout_spent': 'str'
     }
 
     attribute_map = {
         'chain': 'chain',
         'to_address': 'to_address',
         'vault_pub_key': 'vault_pub_key',
         'coin': 'coin',
         'memo': 'memo',
         'max_gas': 'max_gas',
         'gas_rate': 'gas_rate',
         'in_hash': 'in_hash',
         'out_hash': 'out_hash',
-        'height': 'height'
+        'height': 'height',
+        'clout_spent': 'clout_spent'
     }
 
-    def __init__(self, chain=None, to_address=None, vault_pub_key=None, coin=None, memo=None, max_gas=None, gas_rate=None, in_hash=None, out_hash=None, height=None):  # noqa: E501
+    def __init__(self, chain=None, to_address=None, vault_pub_key=None, coin=None, memo=None, max_gas=None, gas_rate=None, in_hash=None, out_hash=None, height=None, clout_spent=None):  # noqa: E501
         """TxOutItem - a model defined in Swagger"""  # noqa: E501
         self._chain = None
         self._to_address = None
         self._vault_pub_key = None
         self._coin = None
         self._memo = None
         self._max_gas = None
         self._gas_rate = None
         self._in_hash = None
         self._out_hash = None
         self._height = None
+        self._clout_spent = None
         self.discriminator = None
         self.chain = chain
         self.to_address = to_address
         if vault_pub_key is not None:
             self.vault_pub_key = vault_pub_key
         self.coin = coin
         if memo is not None:
@@ -77,14 +80,16 @@
         if gas_rate is not None:
             self.gas_rate = gas_rate
         if in_hash is not None:
             self.in_hash = in_hash
         if out_hash is not None:
             self.out_hash = out_hash
         self.height = height
+        if clout_spent is not None:
+            self.clout_spent = clout_spent
 
     @property
     def chain(self):
         """Gets the chain of this TxOutItem.  # noqa: E501
 
 
         :return: The chain of this TxOutItem.  # noqa: E501
@@ -298,14 +303,37 @@
         :type: int
         """
         if height is None:
             raise ValueError("Invalid value for `height`, must not be `None`")  # noqa: E501
 
         self._height = height
 
+    @property
+    def clout_spent(self):
+        """Gets the clout_spent of this TxOutItem.  # noqa: E501
+
+        clout spent in RUNE for the outbound  # noqa: E501
+
+        :return: The clout_spent of this TxOutItem.  # noqa: E501
+        :rtype: str
+        """
+        return self._clout_spent
+
+    @clout_spent.setter
+    def clout_spent(self, clout_spent):
+        """Sets the clout_spent of this TxOutItem.
+
+        clout spent in RUNE for the outbound  # noqa: E501
+
+        :param clout_spent: The clout_spent of this TxOutItem.  # noqa: E501
+        :type: str
+        """
+
+        self._clout_spent = clout_spent
+
     def to_dict(self):
         """Returns the model properties as a dict"""
         result = {}
 
         for attr, _ in six.iteritems(self.swagger_types):
             value = getattr(self, attr)
             if isinstance(value, list):
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_signers_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_signers_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_confirmation_counted.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_finalised.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_inbound_observed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_delay.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_outbound_signed.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_finalised.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_status.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_stages_response_swap_status_streaming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_status_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/tx_status_response_planned_out_txs.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_address.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_address.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_info.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_pubkeys_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_pubkeys_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vault_router.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vault_router.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/vaults_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/vaults_response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/models/version_response.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/models/version_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import pprint
 import re  # noqa: F401
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode/rest.py` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode/rest.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     Thornode API
 
     Thornode REST API.  # noqa: E501
 
-    OpenAPI spec version: 1.125.0
+    OpenAPI spec version: 1.130.1
     Contact: devs@thorchain.org
     Generated by: https://github.com/swagger-api/swagger-codegen.git
 """
 
 import io
 import json
 import logging
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/PKG-INFO` & `xchainpy2-thornode-1.130.1/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,29 +1,14 @@
-Metadata-Version: 2.1
-Name: xchainpy2-thornode
-Version: 1.125.0
-Summary: Thornode API
-Home-page: 
-Author-email: devs@thorchain.org
-Keywords: Swagger,Thornode API
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: urllib3>=1.15
-Requires-Dist: six>=1.10
-Requires-Dist: certifi
-Requires-Dist: python-dateutil
-Requires-Dist: aiohttp
-
 # xchainpy2-thornode
 Thornode REST API.
 
 This Python package is automatically generated by the [Swagger Codegen](https://github.com/swagger-api/swagger-codegen) project:
 
-- API version: 1.125.0
-- Package version: 1.125.0
+- API version: 1.130.1
+- Package version: 1.130.1
 - Build package: io.swagger.codegen.v3.generators.python.PythonClientCodegen
 
 ## Requirements.
 
 Python 2.7 and 3.4+
 
 ## Installation & Usage
@@ -128,14 +113,18 @@
 *StreamingSwapApi* | [**stream_swap**](docs/StreamingSwapApi.md#stream_swap) | **GET** /thorchain/swap/streaming/{hash} | 
 *StreamingSwapApi* | [**stream_swaps**](docs/StreamingSwapApi.md#stream_swaps) | **GET** /thorchain/swaps/streaming | 
 *TSSApi* | [**keysign**](docs/TSSApi.md#keysign) | **GET** /thorchain/keysign/{height} | 
 *TSSApi* | [**keysign_pubkey**](docs/TSSApi.md#keysign_pubkey) | **GET** /thorchain/keysign/{height}/{pubkey} | 
 *TSSApi* | [**metrics**](docs/TSSApi.md#metrics) | **GET** /thorchain/metrics | 
 *TSSApi* | [**metrics_keygen**](docs/TSSApi.md#metrics_keygen) | **GET** /thorchain/metric/keygen/{pubkey} | 
 *ThornamesApi* | [**thorname**](docs/ThornamesApi.md#thorname) | **GET** /thorchain/thorname/{name} | 
+*TradeAccountApi* | [**trade_account**](docs/TradeAccountApi.md#trade_account) | **GET** /thorchain/trade/account/{address} | 
+*TradeAccountsApi* | [**trade_accounts**](docs/TradeAccountsApi.md#trade_accounts) | **GET** /thorchain/trade/accounts/{asset} | 
+*TradeUnitApi* | [**trade_unit**](docs/TradeUnitApi.md#trade_unit) | **GET** /thorchain/trade/unit/{asset} | 
+*TradeUnitsApi* | [**trade_units**](docs/TradeUnitsApi.md#trade_units) | **GET** /thorchain/trade/units | 
 *TransactionsApi* | [**tx**](docs/TransactionsApi.md#tx) | **GET** /thorchain/tx/{hash} | 
 *TransactionsApi* | [**tx_signers**](docs/TransactionsApi.md#tx_signers) | **GET** /thorchain/tx/details/{hash} | 
 *TransactionsApi* | [**tx_signers_old**](docs/TransactionsApi.md#tx_signers_old) | **GET** /thorchain/tx/{hash}/signers | 
 *TransactionsApi* | [**tx_stages**](docs/TransactionsApi.md#tx_stages) | **GET** /thorchain/tx/stages/{hash} | 
 *TransactionsApi* | [**tx_status**](docs/TransactionsApi.md#tx_status) | **GET** /thorchain/tx/status/{hash} | 
 *VaultsApi* | [**asgard**](docs/VaultsApi.md#asgard) | **GET** /thorchain/vaults/asgard | 
 *VaultsApi* | [**vault**](docs/VaultsApi.md#vault) | **GET** /thorchain/vault/{pubkey} | 
@@ -215,14 +204,18 @@
  - [StreamingSwapResponse](docs/StreamingSwapResponse.md)
  - [StreamingSwapsResponse](docs/StreamingSwapsResponse.md)
  - [SwapQueueResponse](docs/SwapQueueResponse.md)
  - [SwapperCloutResponse](docs/SwapperCloutResponse.md)
  - [Thorname](docs/Thorname.md)
  - [ThornameAlias](docs/ThornameAlias.md)
  - [ThornameResponse](docs/ThornameResponse.md)
+ - [TradeAccountResponse](docs/TradeAccountResponse.md)
+ - [TradeAccountsResponse](docs/TradeAccountsResponse.md)
+ - [TradeUnitResponse](docs/TradeUnitResponse.md)
+ - [TradeUnitsResponse](docs/TradeUnitsResponse.md)
  - [TssKeysignMetric](docs/TssKeysignMetric.md)
  - [TssMetric](docs/TssMetric.md)
  - [Tx](docs/Tx.md)
  - [TxDetailsResponse](docs/TxDetailsResponse.md)
  - [TxOutItem](docs/TxOutItem.md)
  - [TxResponse](docs/TxResponse.md)
  - [TxSignersResponse](docs/TxSignersResponse.md)
```

### Comparing `xchainpy2-thornode-1.125.0/xchainpy2_thornode.egg-info/SOURCES.txt` & `xchainpy2-thornode-1.130.1/xchainpy2_thornode.egg-info/SOURCES.txt`

 * *Files 7% similar despite different names*

```diff
@@ -89,14 +89,22 @@
 test/test_streaming_swaps_response.py
 test/test_swap_queue_response.py
 test/test_swapper_clout_response.py
 test/test_thorname.py
 test/test_thorname_alias.py
 test/test_thorname_response.py
 test/test_thornames_api.py
+test/test_trade_account_api.py
+test/test_trade_account_response.py
+test/test_trade_accounts_api.py
+test/test_trade_accounts_response.py
+test/test_trade_unit_api.py
+test/test_trade_unit_response.py
+test/test_trade_units_api.py
+test/test_trade_units_response.py
 test/test_transactions_api.py
 test/test_tss_api.py
 test/test_tss_keysign_metric.py
 test/test_tss_metric.py
 test/test_tx.py
 test/test_tx_details_response.py
 test/test_tx_out_item.py
@@ -144,14 +152,18 @@
 xchainpy2_thornode/api/pol_api.py
 xchainpy2_thornode/api/pools_api.py
 xchainpy2_thornode/api/queue_api.py
 xchainpy2_thornode/api/quote_api.py
 xchainpy2_thornode/api/savers_api.py
 xchainpy2_thornode/api/streaming_swap_api.py
 xchainpy2_thornode/api/thornames_api.py
+xchainpy2_thornode/api/trade_account_api.py
+xchainpy2_thornode/api/trade_accounts_api.py
+xchainpy2_thornode/api/trade_unit_api.py
+xchainpy2_thornode/api/trade_units_api.py
 xchainpy2_thornode/api/transactions_api.py
 xchainpy2_thornode/api/tss_api.py
 xchainpy2_thornode/api/vaults_api.py
 xchainpy2_thornode/models/__init__.py
 xchainpy2_thornode/models/ban_response.py
 xchainpy2_thornode/models/base_quote_response.py
 xchainpy2_thornode/models/block_response.py
@@ -223,14 +235,18 @@
 xchainpy2_thornode/models/streaming_swap_response.py
 xchainpy2_thornode/models/streaming_swaps_response.py
 xchainpy2_thornode/models/swap_queue_response.py
 xchainpy2_thornode/models/swapper_clout_response.py
 xchainpy2_thornode/models/thorname.py
 xchainpy2_thornode/models/thorname_alias.py
 xchainpy2_thornode/models/thorname_response.py
+xchainpy2_thornode/models/trade_account_response.py
+xchainpy2_thornode/models/trade_accounts_response.py
+xchainpy2_thornode/models/trade_unit_response.py
+xchainpy2_thornode/models/trade_units_response.py
 xchainpy2_thornode/models/tss_keysign_metric.py
 xchainpy2_thornode/models/tss_metric.py
 xchainpy2_thornode/models/tx.py
 xchainpy2_thornode/models/tx_details_response.py
 xchainpy2_thornode/models/tx_out_item.py
 xchainpy2_thornode/models/tx_response.py
 xchainpy2_thornode/models/tx_signers_response.py
```

