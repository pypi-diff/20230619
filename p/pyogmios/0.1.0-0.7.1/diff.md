# Comparing `tmp/pyogmios-0.1.0.tar.gz` & `tmp/pyogmios-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyogmios-0.1.0.tar", max compression
+gzip compressed data, was "pyogmios-0.7.1.tar", max compression
```

## Comparing `pyogmios-0.1.0.tar` & `pyogmios-0.7.1.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.1.0/README.md
--rw-r--r--   0        0        0       20 2023-06-18 20:35:59.426251 pyogmios-0.1.0/pyogmios_client/__init__.py
--rw-r--r--   0        0        0     5777 2023-06-18 20:30:32.505137 pyogmios-0.1.0/pyogmios_client/connection.py
--rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.1.0/pyogmios_client/enums/__init__.py
--rw-r--r--   0        0        0     2401 2023-06-18 20:30:32.505186 pyogmios-0.1.0/pyogmios_client/exceptions.py
--rw-r--r--   0        0        0    49367 2023-06-18 20:29:46.297072 pyogmios-0.1.0/pyogmios_client/models/__init__.py
--rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.1.0/pyogmios_client/models/base_model.py
--rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.1.0/pyogmios_client/models/base_request_response_model.py
--rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
--rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
--rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
--rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
--rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.1.0/pyogmios_client/models/generated/__init__.py
--rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.1.0/pyogmios_client/models/request_model.py
--rw-r--r--   0        0        0     6680 2023-06-18 20:29:46.297223 pyogmios-0.1.0/pyogmios_client/models/response_model.py
--rw-r--r--   0        0        0     7796 2023-06-18 20:29:46.297268 pyogmios-0.1.0/pyogmios_client/models/result_models.py
--rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.1.0/pyogmios_client/models/server_health_model.py
--rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/__init__.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
--rw-r--r--   0        0        0     4979 2023-06-18 20:30:58.307688 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
--rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
--rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
--rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
--rw-r--r--   0        0        0     1140 2023-06-18 20:20:33.895494 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
--rw-r--r--   0        0        0      892 2023-06-18 20:20:33.921687 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
--rw-r--r--   0        0        0     1480 2023-06-18 20:20:33.954716 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
--rw-r--r--   0        0        0     2159 2023-06-18 20:20:33.931929 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
--rw-r--r--   0        0        0     2054 2023-06-18 20:20:33.946734 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
--rw-r--r--   0        0        0     1091 2023-06-18 20:20:33.932577 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
--rw-r--r--   0        0        0     1183 2023-06-18 20:20:33.945461 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
--rw-r--r--   0        0        0     2014 2023-06-18 20:20:33.977985 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
--rw-r--r--   0        0        0     1796 2023-06-18 20:20:33.964127 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
--rw-r--r--   0        0        0     1997 2023-06-18 20:20:33.991451 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
--rw-r--r--   0        0        0     1675 2023-06-18 20:20:33.964643 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
--rw-r--r--   0        0        0     1888 2023-06-18 20:20:33.975767 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
--rw-r--r--   0        0        0     1657 2023-06-18 20:20:33.975214 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
--rw-r--r--   0        0        0     1644 2023-06-18 20:20:33.977640 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
--rw-r--r--   0        0        0     1687 2023-06-18 20:20:33.987712 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
--rw-r--r--   0        0        0     1722 2023-06-18 20:20:33.996102 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
--rw-r--r--   0        0        0     1660 2023-06-18 20:20:33.996379 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
--rw-r--r--   0        0        0      933 2023-06-18 20:20:34.002175 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
--rw-r--r--   0        0        0     1779 2023-06-18 20:20:34.005188 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
--rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
--rw-r--r--   0        0        0    13463 2023-06-18 20:20:34.288581 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
--rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
--rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
--rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
--rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
--rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
--rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
--rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
--rw-r--r--   0        0        0     4986 2023-06-18 20:20:34.090809 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
--rw-r--r--   0        0        0     4171 2023-06-18 20:20:34.117964 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
--rw-r--r--   0        0        0    22305 2023-06-18 20:20:34.306218 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
--rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
--rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
--rw-r--r--   0        0        0      707 2023-06-18 20:30:32.505453 pyogmios-0.1.0/pyogmios_client/request.py
--rw-r--r--   0        0        0     1130 2023-06-18 20:30:32.505497 pyogmios-0.1.0/pyogmios_client/server_health.py
--rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.1.0/pyogmios_client/utils/__init__.py
--rw-r--r--   0        0        0     2683 2023-06-18 20:20:34.070550 pyogmios-0.1.0/pyogmios_client/utils/event_emitter.py
--rw-r--r--   0        0        0     2538 2023-06-18 20:30:11.984569 pyogmios-0.1.0/pyogmios_client/utils/queue.py
--rw-r--r--   0        0        0      542 2023-06-18 20:30:11.984616 pyogmios-0.1.0/pyogmios_client/utils/socket_utils.py
--rw-r--r--   0        0        0     1532 2023-06-18 20:52:14.037679 pyogmios-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     9719 1970-01-01 00:00:00.000000 pyogmios-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     8987 2023-06-18 20:32:48.588485 pyogmios-0.7.1/README.md
+-rw-r--r--   0        0        0       22 2023-06-19 19:16:42.601321 pyogmios-0.7.1/pyogmios_client/__init__.py
+-rw-r--r--   0        0        0     6150 2023-06-19 19:02:32.153169 pyogmios-0.7.1/pyogmios_client/connection.py
+-rw-r--r--   0        0        0     1767 2023-06-14 02:13:31.891113 pyogmios-0.7.1/pyogmios_client/enums/__init__.py
+-rw-r--r--   0        0        0     2401 2023-06-18 20:30:32.505186 pyogmios-0.7.1/pyogmios_client/exceptions.py
+-rw-r--r--   0        0        0    49367 2023-06-18 20:29:46.297072 pyogmios-0.7.1/pyogmios_client/models/__init__.py
+-rw-r--r--   0        0        0      829 2023-06-02 00:12:52.975582 pyogmios-0.7.1/pyogmios_client/models/base_model.py
+-rw-r--r--   0        0        0      391 2023-06-18 20:29:46.297119 pyogmios-0.7.1/pyogmios_client/models/base_request_response_model.py
+-rw-r--r--   0        0        0      142 2023-05-29 12:12:30.855476 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/__init__.py
+-rw-r--r--   0        0        0      768 2023-06-02 05:09:09.052857 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py
+-rw-r--r--   0        0        0      481 2023-06-02 05:09:09.053018 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/txPayload__.py
+-rw-r--r--   0        0        0      657 2023-06-02 05:09:09.055011 pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block___.py
+-rw-r--r--   0        0        0    96308 2023-06-04 20:21:45.553261 pyogmios-0.7.1/pyogmios_client/models/generated/__init__.py
+-rw-r--r--   0        0        0     2247 2023-06-18 20:29:46.297175 pyogmios-0.7.1/pyogmios_client/models/request_model.py
+-rw-r--r--   0        0        0     6746 2023-06-19 19:01:43.896476 pyogmios-0.7.1/pyogmios_client/models/response_model.py
+-rw-r--r--   0        0        0     7881 2023-06-19 19:01:43.883277 pyogmios-0.7.1/pyogmios_client/models/result_models.py
+-rw-r--r--   0        0        0     1642 2023-06-18 20:29:46.297316 pyogmios-0.7.1/pyogmios_client/models/server_health_model.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:54:40.062980 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:23.680249 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/__init__.py
+-rw-r--r--   0        0        0     4979 2023-06-18 20:30:58.307688 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py
+-rw-r--r--   0        0        0     2039 2023-06-18 20:30:58.307736 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py
+-rw-r--r--   0        0        0      558 2023-06-18 20:30:58.307782 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:35.095043 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/__init__.py
+-rw-r--r--   0        0        0        0 2023-06-02 11:49:09.937446 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/__init__.py
+-rw-r--r--   0        0        0     1124 2023-06-19 13:26:03.805077 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py
+-rw-r--r--   0        0        0     1058 2023-06-19 13:26:03.799723 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py
+-rw-r--r--   0        0        0     1515 2023-06-19 13:26:03.787064 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py
+-rw-r--r--   0        0        0     2442 2023-06-19 19:01:43.872490 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py
+-rw-r--r--   0        0        0     2467 2023-06-19 19:01:43.889843 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py
+-rw-r--r--   0        0        0     1417 2023-06-19 19:01:43.873064 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py
+-rw-r--r--   0        0        0     1513 2023-06-19 12:51:57.285087 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py
+-rw-r--r--   0        0        0     2330 2023-06-19 19:01:43.881035 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py
+-rw-r--r--   0        0        0     2027 2023-06-19 13:26:03.775214 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py
+-rw-r--r--   0        0        0     2374 2023-06-19 13:05:31.395379 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py
+-rw-r--r--   0        0        0     1918 2023-06-19 13:26:03.802451 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py
+-rw-r--r--   0        0        0     2201 2023-06-19 13:26:03.782424 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py
+-rw-r--r--   0        0        0     1905 2023-06-19 13:26:03.776935 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pools_ranking.py
+-rw-r--r--   0        0        0     1720 2023-06-19 13:26:03.779645 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py
+-rw-r--r--   0        0        0     1914 2023-06-19 19:01:44.042282 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py
+-rw-r--r--   0        0        0     1958 2023-06-19 13:29:43.173810 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance_new.py
+-rw-r--r--   0        0        0     1902 2023-06-19 19:01:44.042429 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py
+-rw-r--r--   0        0        0     1093 2023-06-19 13:29:43.176699 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py
+-rw-r--r--   0        0        0     2106 2023-06-19 13:39:50.892528 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/utxo.py
+-rw-r--r--   0        0        0     2297 2023-06-18 20:31:30.892685 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/query.py
+-rw-r--r--   0        0        0    14518 2023-06-19 19:01:52.850535 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:32:49.879933 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/__init__.py
+-rw-r--r--   0        0        0     1534 2023-06-18 12:37:04.955397 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py
+-rw-r--r--   0        0        0     1384 2023-06-18 20:20:34.012346 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py
+-rw-r--r--   0        0        0     1703 2023-06-18 20:20:34.021771 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py
+-rw-r--r--   0        0        0     1359 2023-06-18 20:20:34.030230 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py
+-rw-r--r--   0        0        0     1507 2023-06-18 12:56:13.502657 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py
+-rw-r--r--   0        0        0     3221 2023-06-18 20:20:34.074501 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py
+-rw-r--r--   0        0        0        0 2023-05-26 12:33:01.699483 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/__init__.py
+-rw-r--r--   0        0        0     4986 2023-06-18 20:20:34.090809 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py
+-rw-r--r--   0        0        0     4171 2023-06-18 20:20:34.117964 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py
+-rw-r--r--   0        0        0    22305 2023-06-18 20:20:34.306218 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py
+-rw-r--r--   0        0        0    16290 2023-06-18 20:20:34.294212 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py
+-rw-r--r--   0        0        0     3338 2023-06-18 20:20:34.059117 pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py
+-rw-r--r--   0        0        0      707 2023-06-18 20:30:32.505453 pyogmios-0.7.1/pyogmios_client/request.py
+-rw-r--r--   0        0        0     1130 2023-06-18 20:30:32.505497 pyogmios-0.7.1/pyogmios_client/server_health.py
+-rw-r--r--   0        0        0        0 2023-05-27 19:33:04.693841 pyogmios-0.7.1/pyogmios_client/utils/__init__.py
+-rw-r--r--   0        0        0     2683 2023-06-18 20:20:34.070550 pyogmios-0.7.1/pyogmios_client/utils/event_emitter.py
+-rw-r--r--   0        0        0     2538 2023-06-18 20:30:11.984569 pyogmios-0.7.1/pyogmios_client/utils/queue.py
+-rw-r--r--   0        0        0      337 2023-06-19 19:02:32.153256 pyogmios-0.7.1/pyogmios_client/utils/socket_utils.py
+-rw-r--r--   0        0        0     1532 2023-06-19 19:15:58.350847 pyogmios-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     9719 1970-01-01 00:00:00.000000 pyogmios-0.7.1/PKG-INFO
```

### Comparing `pyogmios-0.1.0/README.md` & `pyogmios-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/connection.py` & `pyogmios-0.7.1/pyogmios_client/connection.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 from pyogmios_client.models.base_model import BaseModel
 from pyogmios_client.server_health import (
     get_server_health,
     ConnectionConfig,
     Connection,
     Options as ServerHealthOptions,
 )
-from pyogmios_client.utils.socket_utils import ensure_socket_is_open
 
 
 class InteractionContext(BaseModel):
     connection: Connection
     socket: WebSocketApp
     after_each: Callable[[WebSocketApp, Callable[[], None]], None]
     log_level: str
@@ -31,21 +30,22 @@
 
 class InteractionContextOptions(BaseModel):
     connection_config: Optional[ConnectionConfig]
     interaction_type: Optional[InteractionType]
     log_level: str = "DEBUG"
 
 
-def default_error_handler(_: WebSocketApp, exception: Exception):
+def default_error_handler(_: WebSocketApp, error: Exception):
     """
     Default error handler.
     :param _: The websocket app
-    :param exception: The exception
+    :param error: The exception
     """
-    raise exception
+    logging.error(error)
+    raise error
 
 
 def default_close_handler(_: WebSocketApp, close_status_code: int, close_msg: str):
     """
     Default close handler.
     :param _: The websocket app
     :param close_status_code: The close status code
@@ -114,14 +114,17 @@
         """
         return interaction_context_options.interaction_type is InteractionType.ONE_TIME
 
     try:
         if health.last_tip_update is None:
             raise ServerNotReady(health)
 
+        # Create an event to signal when the websocket is opened
+        websocket_opened = threading.Event()
+
         def after_each(ws_app: WebSocketApp, callback: Callable[[], None]):
             """
             Callback to run after each.
             :param ws_app: The websocket app
             :param callback: The callback
             """
             if close_on_completion():
@@ -134,46 +137,58 @@
 
         def on_initial_error(ws_app: WebSocketApp, error: Exception):
             """
             On initial error.
             :param ws_app: The websocket app
             :param error: The error
             """
+            logging.error(error)
             ws_app.close()
             raise error
 
-        def on_message(ws_app, message):
+        def on_message_handler(ws_app, message):
             """
             On message.
             :param ws_app: The websocket app
             :param message: The message
             """
             print(f"Message: {message}")
             if message == "error":
                 on_initial_error(ws_app, Exception(message))
             elif message == "close":
                 raise WebSocketClosedError()
 
+        def on_open_handler(_: WebSocketApp):
+            """
+            On open.
+            :param _: The websocket app
+            """
+            websocket_opened.set()
+
         if interaction_context_options.log_level == "INFO":
             enableTrace(True)
+
         websocket_app = WebSocketApp(
             connection.address.webSocket,
-            on_message=on_message,
+            on_message=on_message_handler,
+            on_open=on_open_handler,
             on_close=close_handler or default_close_handler,
             on_error=error_handler or default_error_handler,
         )
 
         websocket_thread = threading.Thread(target=websocket_app.run_forever)
         websocket_thread.daemon = True
         websocket_thread.start()
 
-        await ensure_socket_is_open(websocket_app)
+        if not websocket_opened.is_set():
+            websocket_opened.wait()
+
         return InteractionContext(
             connection=connection,
             socket=websocket_app,
             after_each=after_each,
-            log_level=options.log_level,
+            log_level=interaction_context_options.log_level,
         )
 
     except ServerNotReady as e:
-        print(e)
+        logging.error(e)
         return None
```

### Comparing `pyogmios-0.1.0/pyogmios_client/enums/__init__.py` & `pyogmios-0.7.1/pyogmios_client/enums/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/exceptions.py` & `pyogmios-0.7.1/pyogmios_client/exceptions.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/__init__.py` & `pyogmios-0.7.1/pyogmios_client/models/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/base_model.py` & `pyogmios-0.7.1/pyogmios_client/models/base_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py` & `pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block_Byron_/body/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/generated/Digest_Blake2b___Block___.py` & `pyogmios-0.7.1/pyogmios_client/models/generated/Digest_Blake2b___Block___.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/generated/__init__.py` & `pyogmios-0.7.1/pyogmios_client/models/generated/__init__.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/request_model.py` & `pyogmios-0.7.1/pyogmios_client/models/request_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/models/response_model.py` & `pyogmios-0.7.1/pyogmios_client/models/response_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -44,14 +44,15 @@
     RollForwardResult,
     RollBackwardResult,
     FindIntersectResult,
     AcquireSuccessResult,
     AcquireFailureResult,
     AwaitAcquiredResult,
     ReleaseResponseResult,
+    EraMismatchResult,
 )
 
 
 class Response(BaseRequestResponse):
     fault: Optional[Dict[str, Any]]
     reflection: Optional[Any] = Field(
         None,
@@ -152,33 +153,35 @@
 
 
 class ChainTipResponse(QueryResponse):
     result: Optional[Union[PointOrOrigin, QueryUnavailableInCurrentEra]]
 
 
 class CurrentEpochResponse(QueryResponse):
-    result: Optional[Union[Epoch, EraMismatch, QueryUnavailableInCurrentEra]]
+    result: Optional[Union[Epoch, EraMismatchResult, QueryUnavailableInCurrentEra]]
 
 
 class CurrentProtocolParametersResponse(QueryResponse):
     result: Optional[
         Union[
             ProtocolParametersShelley,
             ProtocolParametersAlonzo,
             ProtocolParametersBabbage,
-            EraMismatch,
+            EraMismatchResult,
             QueryUnavailableInCurrentEra,
         ]
     ]
 
 
 class DelegationsAndRewardsResponse(QueryResponse):
     result: Optional[
         Union[
-            DelegationsAndRewardsByAccounts, EraMismatch, QueryUnavailableInCurrentEra
+            DelegationsAndRewardsByAccounts,
+            EraMismatchResult,
+            QueryUnavailableInCurrentEra,
         ]
     ]
 
 
 class EraStartResponse(QueryResponse):
     result: Optional[Union[Bound, QueryUnavailableInCurrentEra]]
```

### Comparing `pyogmios-0.1.0/pyogmios_client/models/result_models.py` & `pyogmios-0.7.1/pyogmios_client/models/result_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,14 +71,15 @@
     SubmitTxErrorExtraScriptWitnesses,
     SubmitTxErrorMirNegativeTransfer,
     SubmitTxErrorTotalCollateralMismatch,
     SubmitTxErrorMalformedReferenceScripts,
     SubmitTxErrorMalformedScriptWitnesses,
     SubmitTxErrorInvalidWitnesses,
     SubmitTxErrorEraMismatch,
+    EraMismatch,
 )
 from pyogmios_client.models.base_model import BaseModel
 
 
 class AcquireFailure(BaseModel):
     failure: AcquireFailureDetails
 
@@ -138,14 +139,18 @@
     txId: TxId
 
 
 class ReleaseResponseResult(BaseModel):
     Released = "Released"
 
 
+class EraMismatchResult(BaseModel):
+    eraMismatch = EraMismatch
+
+
 class SubmitTxError(BaseModel):
     __root__: List[
         Union[
             SubmitTxErrorEraMismatch,
             SubmitTxErrorInvalidWitnesses,
             SubmitTxErrorMissingVkWitnesses,
             SubmitTxErrorMissingScriptWitnesses,
```

### Comparing `pyogmios-0.1.0/pyogmios_client/models/server_health_model.py` & `pyogmios-0.7.1/pyogmios_client/models/server_health_model.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/chain_sync_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/find_intersect.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/chain_sync/request_next.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/block_height.py`

 * *Files 6% similar despite different names*

```diff
@@ -17,14 +17,14 @@
     """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": "blockHeight"}
     )
 
     try:
         response = await query(request_args, context)
-        print(response.dict())
         query_response = QueryResponseBlockHeight(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("blockHeight")
-        return response.result
+        return result
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/chain_tip.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,17 +6,23 @@
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
 async def chain_tip(context: InteractionContext) -> PointOrOrigin:
+    """
+    Query the current chain tip.
+    :param context: The interaction context to use for the query.
+    :return: The current chain tip.
+    """
     request_args = RequestArgs(method_name=MethodName.QUERY, args={"query": "chainTip"})
 
     try:
         response = await query(request_args, context)
         query_response = ChainTipResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("chainTip")
-        return response.result
+        return result
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_epoch.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,43 @@
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
-from pyogmios_client.models import Epoch, EraMismatch
+from pyogmios_client.models import Epoch
 from pyogmios_client.models.response_model import CurrentEpochResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: CurrentEpochResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 async def current_epoch(context: InteractionContext) -> Epoch:
+    """
+    Query the current epoch.
+    :param context: The interaction context to use for the query.
+    :return: The current epoch.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": "currentEpoch"}
     )
 
     try:
         response = await query(request_args, context)
         query_response = CurrentEpochResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("currentEpoch")
-        elif isinstance(query_response.result, Epoch):
-            return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        elif isinstance(result, Epoch):
+            return result
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/current_protocol_parameters.py`

 * *Files 18% similar despite different names*

```diff
@@ -2,57 +2,63 @@
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
 from pyogmios_client.models import (
-    EraMismatch,
     ProtocolParametersBabbage,
     ProtocolParametersAlonzo,
     ProtocolParametersShelley,
 )
 from pyogmios_client.models.response_model import CurrentProtocolParametersResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: CurrentProtocolParametersResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 def is_protocol_parameters(response: CurrentProtocolParametersResponse) -> bool:
+    """
+    Check if the response is a protocol parameters response.
+    :param response: The response to check.
+    :return: True if the response is a protocol parameters response, False otherwise.
+    """
     result = response.result
     if isinstance(result, ProtocolParametersBabbage):
         return result.coinsPerUtxoByte is not None
     elif isinstance(result, ProtocolParametersAlonzo):
         return result.coinsPerUtxoWord is not None
     elif isinstance(result, ProtocolParametersShelley):
         return result.minUtxoValue is not None
 
 
 async def current_protocol_parameters(
     context: InteractionContext,
 ) -> ProtocolParametersBabbage | ProtocolParametersAlonzo | ProtocolParametersShelley:
+    """
+    Query the current protocol parameters.
+    :param context: The interaction context to use for the query.
+    :return: The current protocol parameters.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": "currentProtocolParameters"}
     )
 
     try:
         response = await query(request_args, context)
         query_response = CurrentProtocolParametersResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("currentProtocolParameters")
         elif is_protocol_parameters(query_response):
             return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/delegations_and_rewards.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,57 +4,64 @@
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
 from pyogmios_client.models import (
-    EraMismatch,
     DigestBlake2BCredential,
     DelegationsAndRewardsByAccounts,
 )
 from pyogmios_client.models.response_model import DelegationsAndRewardsResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: DelegationsAndRewardsResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 def is_delegations_and_rewards_by_accounts(
     response: DelegationsAndRewardsResponse,
 ) -> bool:
+    """
+    Check if the given response is a DelegationsAndRewardsByAccounts.
+    :param response: The response to check.
+    :return: True if the response is a DelegationsAndRewardsByAccounts, False otherwise.
+    """
     result = response.result
     if len(result.__root__) <= 0:
         return True
     sample = list(result.__root__.values())[0]
     return sample.delegate is not None and sample.rewards is not None
 
 
 async def delegations_and_rewards(
     context: InteractionContext, stake_key_hashes: List[DigestBlake2BCredential]
 ) -> DelegationsAndRewardsByAccounts:
+    """
+    Query the delegations and rewards for the given stake key hashes.
+    :param context: The interaction context to use for the query.
+    :param stake_key_hashes: The stake key hashes to query.
+    :return: The delegations and rewards for the given stake key hashes.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY,
         args={"query": {"delegationsAndRewards": stake_key_hashes}},
     )
 
     try:
         response = await query(request_args, context)
         query_response = DelegationsAndRewardsResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("delegationsAndRewards")
         elif is_delegations_and_rewards_by_accounts(query_response):
             return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_start.py`

 * *Files 16% similar despite different names*

```diff
@@ -6,24 +6,34 @@
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
 def is_bound(response: EraStartResponse) -> bool:
+    """
+    Check if the response is a Bound.
+    :param response: The response to check.
+    :return: True if the response is a Bound, False otherwise.
+    """
     bound = response.result
     if isinstance(bound, Bound):
         return (
             bound.time is not None
             and bound.slot is not None
             and bound.epoch is not None
         )
 
 
 async def era_start(context: InteractionContext) -> Bound:
+    """
+    Query the start of the current era.
+    :param context: The interaction context to use for the query.
+    :return: The start of the current era.
+    """
     request_args = RequestArgs(method_name=MethodName.QUERY, args={"query": "eraStart"})
 
     try:
         response = await query(request_args, context)
         query_response = EraStartResponse(**response.dict())
         if is_bound(query_response):
             return query_response.result
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/era_summaries.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,23 +8,33 @@
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
 def is_era_summaries(response: EraSummariesResponse) -> bool:
+    """
+    Check if the response is a list of EraSummary.
+    :param response: The response to check.
+    :return: True if the response is a list of EraSummary, False otherwise.
+    """
     result = response.result
     if isinstance(result, List):
         return all(
             s.start is not None and s.end is not None and s.parameters is not None
             for s in result
         )
 
 
 async def era_summaries(context: InteractionContext) -> List[EraSummary]:
+    """
+    Query the era summaries.
+    :param context: The interaction context to use for the query.
+    :return: The era summaries.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": "eraSummaries"}
     )
 
     try:
         response = await query(request_args, context)
         query_response = EraSummariesResponse(**response.dict())
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/genesis_config.py`

 * *Files 22% similar despite different names*

```diff
@@ -2,59 +2,66 @@
 from pyogmios_client.enums import MethodName, EraWithGenesis
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
 from pyogmios_client.models import (
-    EraMismatch,
     GenesisConfig,
     GenesisByron,
     GenesisShelley,
     GenesisAlonzo,
 )
 from pyogmios_client.models.response_model import GenesisConfigResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: GenesisConfigResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 def is_genesis_config(response: GenesisConfigResponse) -> bool:
+    """
+    Check if the response is a genesis config response.
+    :param response: The response to check.
+    :return: True if the response is a genesis config response, False otherwise.
+    """
     result = response.result
     if isinstance(result, GenesisByron):
         return result.initialCoinOffering is not None
     elif isinstance(result, GenesisShelley):
         return result.initialPools is not None
     elif isinstance(result, GenesisAlonzo):
         return result.costModels is not None
 
 
 async def genesis_config(
     context: InteractionContext, era: EraWithGenesis
 ) -> GenesisConfig:
+    """
+    Query the genesis config.
+    :param context: The interaction context to use for the query.
+    :param era: The era to query the genesis config for.
+    :return: The genesis config.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY,
         args={"query": {"genesisConfig": str(era.value).lower()}},
     )
 
     try:
         response = await query(request_args, context)
         query_response = GenesisConfigResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("genesisConfig")
         elif is_genesis_config(query_response):
             return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,56 @@
+from typing import List
+
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
-from pyogmios_client.models import EraMismatch, Origin, PointOrOrigin, Point
-from pyogmios_client.models.response_model import LedgerTipResponse
+from pyogmios_client.models import PoolId
+from pyogmios_client.models.response_model import PoolIdsResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: LedgerTipResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
-def is_non_origin_point(response: LedgerTipResponse) -> bool:
+def is_pool_ids(response: PoolIdsResponse) -> bool:
+    """
+    Check if the response is a list of pool ids.
+    :param response: The response to check.
+    :return: True if the response is a list of pool ids, False otherwise.
+    """
     result = response.result
-    if isinstance(result, Point):
-        return result.slot is not None and result.hash is not None
+    if isinstance(result, List) and len(result) > 0:
+        if isinstance(result[0], PoolId):
+            return True
     return False
 
 
-async def ledger_tip(context: InteractionContext) -> PointOrOrigin:
-    request_args = RequestArgs(
-        method_name=MethodName.QUERY, args={"query": "ledgerTip"}
-    )
+async def pool_ids(context: InteractionContext) -> List[PoolId]:
+    """
+    Query the pool ids.
+    :param context: The interaction context to use for the query.
+    :return: The pool ids.
+    """
+    request_args = RequestArgs(method_name=MethodName.QUERY, args={"query": "poolIds"})
 
     try:
         response = await query(request_args, context)
-        query_response = LedgerTipResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
-            raise QueryUnavailableInCurrentEraError("ledgerTip")
-        elif isinstance(query_response.result, Origin):
-            return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        query_response = PoolIdsResponse(**response.dict())
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
+            raise QueryUnavailableInCurrentEraError("poolIds")
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
-        elif is_non_origin_point(query_response):
+        elif is_pool_ids(query_response):
             return query_response.result
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/non_myopic_member_rewards.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/proposed_protocol_parameters.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,60 +1,50 @@
-from typing import List
+from typing import Dict
 
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
-    UnknownResultError,
 )
 from pyogmios_client.models import (
-    EraMismatch,
-    Lovelace,
-    DigestBlake2bCredential,
-    NonMyopicMemberRewards,
-    StakeAddress,
+    ProtocolParametersBabbage,
+    ProtocolParametersAlonzo,
+    ProtocolParametersShelley,
 )
-from pyogmios_client.models.response_model import NonMyopicMemberRewardsResponse
+from pyogmios_client.models.response_model import PoolsRankingResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: NonMyopicMemberRewardsResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
-def is_non_myopic_member_rewards(response: NonMyopicMemberRewardsResponse) -> bool:
-    result = response.result
-    if isinstance(result, NonMyopicMemberRewards):
-        return True
-    return False
-
-
-async def non_myopic_member_rewards(
+async def proposed_protocol_parameters(
     context: InteractionContext,
-    input_list: List[Lovelace] | List[DigestBlake2bCredential] | List[StakeAddress],
-) -> NonMyopicMemberRewards:
+) -> Dict[str, ProtocolParametersShelley] | Dict[str, ProtocolParametersAlonzo] | Dict[
+    str, ProtocolParametersBabbage
+] | None:
+    """
+    Query the proposed protocol parameters.
+    :param context: The interaction context to use for the query.
+    :return: The proposed protocol parameters.
+    """
     request_args = RequestArgs(
-        method_name=MethodName.QUERY,
-        args={"query": {"nonMyopicMemberRewards": input_list}},
+        method_name=MethodName.QUERY, args={"query": "proposedProtocolParameters"}
     )
 
     try:
         response = await query(request_args, context)
-        query_response = NonMyopicMemberRewardsResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
-            raise QueryUnavailableInCurrentEraError("nonMyopicMemberRewards")
-        elif is_non_myopic_member_rewards(query_response):
-            return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        query_response = PoolsRankingResponse(**response.dict())
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
+            raise QueryUnavailableInCurrentEraError("proposedProtocolParameters")
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
-            raise UnknownResultError(response)
+            return result
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_ids.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/ledger_tip.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,49 +1,57 @@
-from typing import List
-
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
-from pyogmios_client.models import EraMismatch, PoolId
-from pyogmios_client.models.response_model import PoolIdsResponse
+from pyogmios_client.models import Origin, PointOrOrigin, Point
+from pyogmios_client.models.response_model import LedgerTipResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: PoolIdsResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
-def is_pool_ids(response: PoolIdsResponse) -> bool:
+def is_non_origin_point(response: LedgerTipResponse) -> bool:
+    """
+    Check if the response is a non-origin point.
+    :param response: The response to check.
+    :return: True if the response is a non-origin point, False otherwise.
+    """
     result = response.result
-    if isinstance(result, List) and len(result) > 0:
-        if isinstance(result[0], PoolId):
-            return True
+    if isinstance(result, Point):
+        return result.slot is not None and result.hash is not None
     return False
 
 
-async def pool_ids(context: InteractionContext) -> List[PoolId]:
-    request_args = RequestArgs(method_name=MethodName.QUERY, args={"query": "poolIds"})
+async def ledger_tip(context: InteractionContext) -> PointOrOrigin:
+    """
+    Query the current ledger tip.
+    :param context: The interaction context to use for the query.
+    :return: The current ledger tip.
+    """
+    request_args = RequestArgs(
+        method_name=MethodName.QUERY, args={"query": "ledgerTip"}
+    )
 
     try:
         response = await query(request_args, context)
-        query_response = PoolIdsResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
-            raise QueryUnavailableInCurrentEraError("poolIds")
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        query_response = LedgerTipResponse(**response.dict())
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
+            raise QueryUnavailableInCurrentEraError("ledgerTip")
+        elif isinstance(result, Origin):
+            return result
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
-        elif is_pool_ids(query_response):
+        elif is_non_origin_point(query_response):
             return query_response.result
         else:
             raise UnknownResultError(response)
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/pool_parameters.py`

 * *Files 20% similar despite different names*

```diff
@@ -3,51 +3,59 @@
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
     UnknownResultError,
 )
-from pyogmios_client.models import EraMismatch, PoolId, PoolParameters
+from pyogmios_client.models import PoolId, PoolParameters
 from pyogmios_client.models.response_model import PoolParametersResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: PoolParametersResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 def is_pool_parameters(response: PoolParametersResponse) -> bool:
+    """
+    Check if the response is a list of pool parameters.
+    :param response: The response to check.
+    :return: True if the response is a list of pool parameters, False otherwise.
+    """
     result = response.result
     if isinstance(result, Dict):
         # sample = list(result.values())[0]
         sample = next(iter(result))
         if isinstance(sample, PoolParameters):
             return True
     return False
 
 
 async def pool_parameters(
     context: InteractionContext, pools: List[PoolId]
 ) -> Dict[str, PoolParameters]:
+    """
+    Query the pool parameters.
+    :param context: The interaction context to use for the query.
+    :param pools: The list of pool ids to query.
+    :return: The pool parameters.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": {"poolParameters": pools}}
     )
 
     try:
         response = await query(request_args, context)
         query_response = PoolParametersResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("poolParameters")
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         elif is_pool_parameters(query_response):
             return query_response.result
         else:
             raise UnknownResultError(response)
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/rewards_provenance.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,47 +1,54 @@
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
 from pyogmios_client.exceptions import (
     QueryUnavailableInCurrentEraError,
     EraMismatchError,
 )
-from pyogmios_client.models import EraMismatch, RewardsProvenance
+from pyogmios_client.models import RewardsProvenance
 from pyogmios_client.models.response_model import RewardsProvenanceResponse
+from pyogmios_client.models.result_models import EraMismatchResult
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: RewardsProvenanceResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
 def is_rewards_provenance(response: RewardsProvenanceResponse) -> bool:
+    """
+    Check if the response is a rewards provenance.
+    :param response: The response to check.
+    :return: True if the response is a rewards provenance, False otherwise.
+    """
     result = response.result
     if isinstance(result, RewardsProvenance):
         return True
     return False
 
 
 async def rewards_provenance(context: InteractionContext) -> RewardsProvenance:
+    """
+    Query the rewards provenance.
+    :param context: The interaction context to use for the query.
+    :return: The rewards provenance.
+    """
     request_args = RequestArgs(
         method_name=MethodName.QUERY, args={"query": "rewardsProvenance"}
     )
 
     try:
         response = await query(request_args, context)
         query_response = RewardsProvenanceResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
             raise QueryUnavailableInCurrentEraError("rewardsProvenance")
         elif is_rewards_provenance(query_response):
-            return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
+            return result
+        elif isinstance(result, EraMismatchResult):
+            era_mismatch = result.eraMismatch
             raise EraMismatchError(
                 str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
             )
         else:
-            return query_response.result
+            return result
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/queries/stake_distribution.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/queries/system_start.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,45 +1,31 @@
 from pyogmios_client.connection import InteractionContext
 from pyogmios_client.enums import MethodName
-from pyogmios_client.exceptions import (
-    QueryUnavailableInCurrentEraError,
-    EraMismatchError,
-    UnknownResultError,
-)
-from pyogmios_client.models import EraMismatch, PoolDistribution
-from pyogmios_client.models.response_model import StakeDistributionResponse
+from pyogmios_client.exceptions import QueryUnavailableInCurrentEraError
+from pyogmios_client.models import UtcTime
+from pyogmios_client.models.response_model import SystemStartResponse
 from pyogmios_client.ouroboros_mini_protocols.state_query.query import (
     query,
     RequestArgs,
 )
 
 
-def is_era_mismatch(response: StakeDistributionResponse) -> bool:
-    if isinstance(response, EraMismatch):
-        return response.eraMismatch is not None
-
-
-def is_stake_distribution(response: StakeDistributionResponse) -> bool:
-    return isinstance(response.result, PoolDistribution)
-
-
-async def stake_distribution(context: InteractionContext) -> PoolDistribution:
+async def system_start(context: InteractionContext) -> UtcTime:
+    """
+    Query the system start time.
+    :param context: The interaction context to use for the query.
+    :return: The system start time.
+    """
     request_args = RequestArgs(
-        method_name=MethodName.QUERY, args={"query": "stakeDistribution"}
+        method_name=MethodName.QUERY, args={"query": "systemStart"}
     )
 
     try:
         response = await query(request_args, context)
-        query_response = StakeDistributionResponse(**response.dict())
-        if query_response.result == "QueryUnavailableInCurrentEra":
-            raise QueryUnavailableInCurrentEraError("stakeDistribution")
-        elif is_stake_distribution(query_response):
-            return query_response.result
-        elif is_era_mismatch(query_response):
-            era_mismatch = response.result.eraMismatch
-            raise EraMismatchError(
-                str(era_mismatch.queryEra), str(era_mismatch.ledgerEra)
-            )
+        query_response = SystemStartResponse(**response.dict())
+        result = query_response.result
+        if result == "QueryUnavailableInCurrentEra":
+            raise QueryUnavailableInCurrentEraError("systemStart")
         else:
-            raise UnknownResultError(response)
+            return result
     except Exception as error:
         raise error
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/query.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/query.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/state_query/state_query_client.py`

 * *Files 12% similar despite different names*

```diff
@@ -172,22 +172,24 @@
     :param context: The interaction context
     :param options: The options
     :return: A state query client
     """
     websocket_app = context.socket
 
     async def acquire(point: PointOrOrigin) -> StateQueryClient:
+        """
+        Acquire the a point
+        """
         client = await create_state_query_client(context, Options(point=point))
         return client
 
-    async def run_state_query(state_query: Callable) -> Any:
-        await ensure_socket_is_open(websocket_app)
-        return await state_query(context)
-
     async def release() -> ReleaseResponse | None:
+        """
+        Release the state query client
+        """
         await ensure_socket_is_open(websocket_app)
         request_id = generate(size=5)
         try:
             request = RequestRelease.from_base(mirror={"requestId": str(request_id)})
             websocket_app.send(request.json())
             result = websocket_app.sock.recv()
             release_response = ReleaseResponse(**json.loads(result))
@@ -208,96 +210,153 @@
             websocket_app.close()
         except Exception as err:
             print(err)
         else:
             print("Shutting down State Query Client...")
 
     async def query_block_height() -> BlockNoOrOrigin:
+        """
+        Query the block height
+        """
         await ensure_socket_is_open(websocket_app)
         return await block_height(context)
 
     async def query_chain_tip() -> PointOrOrigin:
+        """
+        Query the chain tip
+        """
         await ensure_socket_is_open(websocket_app)
         return await chain_tip(context)
 
     async def query_current_epoch() -> Epoch:
+        """
+        Query the current epoch
+        """
         await ensure_socket_is_open(websocket_app)
         return await current_epoch(context)
 
     async def query_current_protocol_parameters() -> ProtocolParametersBabbage | ProtocolParametersAlonzo | ProtocolParametersShelley:
+        """
+        Query the current protocol parameters
+        """
         await ensure_socket_is_open(websocket_app)
         return await current_protocol_parameters(context)
 
     async def query_delegations_and_rewards(
         stake_key_hashes: List[DigestBlake2BCredential],
     ) -> DelegationsAndRewardsByAccounts:
+        """
+        Query delegations and rewards
+        """
         await ensure_socket_is_open(websocket_app)
         return await delegations_and_rewards(context, stake_key_hashes)
 
     async def query_era_start() -> Bound:
+        """
+        Query the era start
+        """
         await ensure_socket_is_open(websocket_app)
         return await era_start(context)
 
     async def query_era_summaries() -> List[EraSummary]:
+        """
+        Query the era summaries
+        """
         await ensure_socket_is_open(websocket_app)
         return await era_summaries(context)
 
     async def query_genesis_config(era: EraWithGenesis) -> List[EraSummary]:
+        """
+        Query the genesis config
+        """
         await ensure_socket_is_open(websocket_app)
         return await genesis_config(context, era)
 
     async def query_ledger_tip() -> PointOrOrigin:
+        """
+        Query the ledger tip
+        """
         await ensure_socket_is_open(websocket_app)
         return await ledger_tip(context)
 
     async def query_non_myopic_member_rewards(
         input_list: List[Lovelace] | List[DigestBlake2bCredential],
     ) -> NonMyopicMemberRewards:
+        """
+        Query non myopic member rewards
+        """
         await ensure_socket_is_open(websocket_app)
         return await non_myopic_member_rewards(context, input_list)
 
     async def query_pool_ids() -> List[PoolId]:
+        """
+        Query pool ids
+        """
         await ensure_socket_is_open(websocket_app)
         return await pool_ids(context)
 
     async def query_pool_parameters(pools: List[PoolId]) -> Dict[str, PoolParameters]:
+        """
+        Query pool parameters
+        """
         await ensure_socket_is_open(websocket_app)
         return await pool_parameters(context, pools)
 
     async def query_pools_ranking() -> PoolsRanking:
+        """
+        Query pools ranking
+        """
         await ensure_socket_is_open(websocket_app)
         return await pools_ranking(context)
 
     async def query_proposed_protocol_parameters() -> Dict[
         str, ProtocolParametersShelley
     ] | Dict[str, ProtocolParametersAlonzo] | Dict[
         str, ProtocolParametersBabbage
     ] | None:
+        """
+        Query proposed protocol parameters
+        """
         await ensure_socket_is_open(websocket_app)
         return await proposed_protocol_parameters(context)
 
     async def query_rewards_provenance() -> RewardsProvenance:
+        """
+        Query rewards provenance
+        """
         await ensure_socket_is_open(websocket_app)
         return await rewards_provenance(context)
 
     async def query_rewards_provenance_new() -> RewardsProvenanceNew:
+        """
+        Query rewards provenance new
+        """
         await ensure_socket_is_open(websocket_app)
         return await rewards_provenance_new(context)
 
     async def query_stake_distribution() -> PoolDistribution:
+        """
+        Query stake distribution
+        """
         await ensure_socket_is_open(websocket_app)
         return await stake_distribution(context)
 
     async def query_system_start() -> UtcTime:
+        """
+        Query system start
+        """
         await ensure_socket_is_open(websocket_app)
         return await system_start(context)
 
     try:
 
         def create_client() -> StateQueryClient:
+            """
+            Create a state query client
+            """
             return StateQueryClient(
                 context=context,
                 acquire=acquire,
                 release=release,
                 shutdown=shutdown,
                 block_height=query_block_height,
                 chain_tip=query_chain_tip,
```

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/await_acquire.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/has_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/next_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/release.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/size_and_capacity.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_monitor/tx_monitor_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluate_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/evaluation_errors.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submission_errors.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/submit_tx.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py` & `pyogmios-0.7.1/pyogmios_client/ouroboros_mini_protocols/tx_submission/tx_submission_client.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/request.py` & `pyogmios-0.7.1/pyogmios_client/request.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/server_health.py` & `pyogmios-0.7.1/pyogmios_client/server_health.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/utils/event_emitter.py` & `pyogmios-0.7.1/pyogmios_client/utils/event_emitter.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyogmios_client/utils/queue.py` & `pyogmios-0.7.1/pyogmios_client/utils/queue.py`

 * *Files identical despite different names*

### Comparing `pyogmios-0.1.0/pyproject.toml` & `pyogmios-0.7.1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyogmios"
-version = "0.1.0"
+version = "0.7.1"
 description = "Python client for Ogmios"
 authors = ["Hareem Adderley <hadderley@kingpinapps.com>"]
 readme = "README.md"
 packages = [{include = "pyogmios_client"}]
 
 
 [tool.poetry.dependencies]
@@ -40,15 +40,15 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = "-p no:cacheprovider"
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "0.7.0"
+version = "0.7.1"
 version_files = [
     "pyogmios_client/__init__.py:__version__",
     "pyproject.toml:version"
 ]
 update_changelog_on_bump = true
 style = [
     ["qmark", "fg:#ff9d00 bold"],
```

### Comparing `pyogmios-0.1.0/PKG-INFO` & `pyogmios-0.7.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyogmios
-Version: 0.1.0
+Version: 0.7.1
 Summary: Python client for Ogmios
 Author: Hareem Adderley
 Author-email: hadderley@kingpinapps.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

