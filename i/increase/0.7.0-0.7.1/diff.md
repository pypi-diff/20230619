# Comparing `tmp/increase-0.7.0.tar.gz` & `tmp/increase-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "increase-0.7.0.tar", max compression
+gzip compressed data, was "increase-0.7.1.tar", max compression
```

## Comparing `increase-0.7.0.tar` & `increase-0.7.1.tar`

### file list

```diff
@@ -1,210 +1,210 @@
--rw-r--r--   0        0        0    11338 2023-06-13 15:45:28.392204 increase-0.7.0/LICENSE
--rw-r--r--   0        0        0     8425 2023-06-13 15:45:28.392204 increase-0.7.0/README.md
--rw-r--r--   0        0        0     1883 2023-06-13 15:45:28.396205 increase-0.7.0/pyproject.toml
--rw-r--r--   0        0        0     2587 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/__init__.py
--rw-r--r--   0        0        0    45082 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_base_client.py
--rw-r--r--   0        0        0     3889 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_base_exceptions.py
--rw-r--r--   0        0        0    26762 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_client.py
--rw-r--r--   0        0        0    10875 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_exceptions.py
--rw-r--r--   0        0        0     7343 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_models.py
--rw-r--r--   0        0        0     4846 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_qs.py
--rw-r--r--   0        0        0      890 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_resource.py
--rw-r--r--   0        0        0     5884 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_streaming.py
--rw-r--r--   0        0        0     4229 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_types.py
--rw-r--r--   0        0        0     1277 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_utils/__init__.py
--rw-r--r--   0        0        0     6710 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_utils/_transform.py
--rw-r--r--   0        0        0     9411 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_utils/_utils.py
--rw-r--r--   0        0        0      127 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/_version.py
--rw-r--r--   0        0        0     1109 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/pagination.py
--rw-r--r--   0        0        0        0 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/py.typed
--rw-r--r--   0        0        0     4478 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/__init__.py
--rw-r--r--   0        0        0    15065 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/account_numbers.py
--rw-r--r--   0        0        0     7400 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/account_statements.py
--rw-r--r--   0        0        0    18102 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/account_transfers.py
--rw-r--r--   0        0        0    18476 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/accounts.py
--rw-r--r--   0        0        0    15600 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/ach_prenotifications.py
--rw-r--r--   0        0        0    26071 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/ach_transfers.py
--rw-r--r--   0        0        0     4285 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/balance_lookups.py
--rw-r--r--   0        0        0     8651 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/bookkeeping_accounts.py
--rw-r--r--   0        0        0     4122 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/bookkeeping_entries.py
--rw-r--r--   0        0        0     4842 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/bookkeeping_entry_sets.py
--rw-r--r--   0        0        0    10707 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/card_disputes.py
--rw-r--r--   0        0        0    10597 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/card_profiles.py
--rw-r--r--   0        0        0    19120 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/cards.py
--rw-r--r--   0        0        0    11757 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/check_deposits.py
--rw-r--r--   0        0        0    23188 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/check_transfers.py
--rw-r--r--   0        0        0     7771 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/declined_transactions.py
--rw-r--r--   0        0        0     7353 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/digital_wallet_tokens.py
--rw-r--r--   0        0        0     7177 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/documents.py
--rw-r--r--   0        0        0      282 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/entities/__init__.py
--rw-r--r--   0        0        0    14010 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/entities/entities.py
--rw-r--r--   0        0        0     8071 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/entities/supplemental_documents.py
--rw-r--r--   0        0        0    18799 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/event_subscriptions.py
--rw-r--r--   0        0        0     7154 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/events.py
--rw-r--r--   0        0        0    10548 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/exports.py
--rw-r--r--   0        0        0    15315 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/external_accounts.py
--rw-r--r--   0        0        0    12781 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/files.py
--rw-r--r--   0        0        0     2040 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/groups.py
--rw-r--r--   0        0        0    12035 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/inbound_ach_transfer_returns.py
--rw-r--r--   0        0        0     7075 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0    14231 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/limits.py
--rw-r--r--   0        0        0     6593 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/oauth_connections.py
--rw-r--r--   0        0        0     8344 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/pending_transactions.py
--rw-r--r--   0        0        0     6300 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/programs.py
--rw-r--r--   0        0        0     8536 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/real_time_decisions.py
--rw-r--r--   0        0        0    14968 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4951 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/routing_numbers.py
--rw-r--r--   0        0        0     1989 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/__init__.py
--rw-r--r--   0        0        0     4026 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/account_statements.py
--rw-r--r--   0        0        0     4024 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/account_transfers.py
--rw-r--r--   0        0        0    21913 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/ach_transfers.py
--rw-r--r--   0        0        0     5051 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/card_disputes.py
--rw-r--r--   0        0        0     3967 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/card_refunds.py
--rw-r--r--   0        0        0    11463 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/cards.py
--rw-r--r--   0        0        0    10125 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/check_deposits.py
--rw-r--r--   0        0        0    11013 2023-06-13 15:45:28.396205 increase-0.7.0/src/increase/resources/simulations/check_transfers.py
--rw-r--r--   0        0        0     4085 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/digital_wallet_token_requests.py
--rw-r--r--   0        0        0     3639 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/documents.py
--rw-r--r--   0        0        0    13466 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
--rw-r--r--   0        0        0     4411 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/interest_payments.py
--rw-r--r--   0        0        0     3919 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/programs.py
--rw-r--r--   0        0        0    11257 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/real_time_payments_transfers.py
--rw-r--r--   0        0        0     4588 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/simulations.py
--rw-r--r--   0        0        0    12351 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/simulations/wire_transfers.py
--rw-r--r--   0        0        0     7800 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/transactions.py
--rw-r--r--   0        0        0    13338 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/wire_drawdown_requests.py
--rw-r--r--   0        0        0    27583 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/resources/wire_transfers.py
--rw-r--r--   0        0        0     8739 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/__init__.py
--rw-r--r--   0        0        0     1666 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account.py
--rw-r--r--   0        0        0      747 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_create_params.py
--rw-r--r--   0        0        0     1693 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_list_params.py
--rw-r--r--   0        0        0     1026 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_number.py
--rw-r--r--   0        0        0      408 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_number_create_params.py
--rw-r--r--   0        0        0     1598 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_number_list_params.py
--rw-r--r--   0        0        0      435 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_number_update_params.py
--rw-r--r--   0        0        0     1347 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_statement.py
--rw-r--r--   0        0        0     1534 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_statement_list_params.py
--rw-r--r--   0        0        0     2648 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_transfer.py
--rw-r--r--   0        0        0      814 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_transfer_create_params.py
--rw-r--r--   0        0        0     1494 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_transfer_list_params.py
--rw-r--r--   0        0        0      271 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/account_update_params.py
--rw-r--r--   0        0        0     2152 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_prenotification.py
--rw-r--r--   0        0        0     1847 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_prenotification_create_params.py
--rw-r--r--   0        0        0     1391 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_prenotification_list_params.py
--rw-r--r--   0        0        0     8899 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_transfer.py
--rw-r--r--   0        0        0     3388 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_transfer_create_params.py
--rw-r--r--   0        0        0     1592 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/ach_transfer_list_params.py
--rw-r--r--   0        0        0      585 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/balance_lookup_lookup_params.py
--rw-r--r--   0        0        0      780 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/balance_lookup_lookup_response.py
--rw-r--r--   0        0        0      823 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_account.py
--rw-r--r--   0        0        0      626 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_account_create_params.py
--rw-r--r--   0        0        0      428 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_account_list_params.py
--rw-r--r--   0        0        0      698 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_entry.py
--rw-r--r--   0        0        0      424 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_entry_list_params.py
--rw-r--r--   0        0        0      895 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_entry_set.py
--rw-r--r--   0        0        0     1133 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/bookkeeping_entry_set_create_params.py
--rw-r--r--   0        0        0     2342 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card.py
--rw-r--r--   0        0        0     1767 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_create_params.py
--rw-r--r--   0        0        0      907 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_details.py
--rw-r--r--   0        0        0     2011 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_dispute.py
--rw-r--r--   0        0        0      483 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_dispute_create_params.py
--rw-r--r--   0        0        0     1661 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_dispute_list_params.py
--rw-r--r--   0        0        0     1451 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_list_params.py
--rw-r--r--   0        0        0     2186 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_profile.py
--rw-r--r--   0        0        0     1820 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_profile_create_params.py
--rw-r--r--   0        0        0      716 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_profile_list_params.py
--rw-r--r--   0        0        0     1619 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/card_update_params.py
--rw-r--r--   0        0        0     4861 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_deposit.py
--rw-r--r--   0        0        0      748 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_deposit_create_params.py
--rw-r--r--   0        0        0     1477 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_deposit_list_params.py
--rw-r--r--   0        0        0     6608 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_transfer.py
--rw-r--r--   0        0        0     1939 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_transfer_create_params.py
--rw-r--r--   0        0        0     1488 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/check_transfer_list_params.py
--rw-r--r--   0        0        0    13934 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/declined_transaction.py
--rw-r--r--   0        0        0     1598 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/declined_transaction_list_params.py
--rw-r--r--   0        0        0      950 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/digital_wallet_token.py
--rw-r--r--   0        0        0     1489 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/digital_wallet_token_list_params.py
--rw-r--r--   0        0        0     2581 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/document.py
--rw-r--r--   0        0        0     3900 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/document_list_params.py
--rw-r--r--   0        0        0      418 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entities/__init__.py
--rw-r--r--   0        0        0      634 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entities/supplemental_document.py
--rw-r--r--   0        0        0      343 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entities/supplemental_document_create_params.py
--rw-r--r--   0        0        0      547 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entities/supplemental_document_list_params.py
--rw-r--r--   0        0        0    11893 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entity.py
--rw-r--r--   0        0        0    25685 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entity_create_params.py
--rw-r--r--   0        0        0     1367 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/entity_list_params.py
--rw-r--r--   0        0        0     2724 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event.py
--rw-r--r--   0        0        0     4044 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event_list_params.py
--rw-r--r--   0        0        0     3124 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event_subscription.py
--rw-r--r--   0        0        0     2526 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event_subscription_create_params.py
--rw-r--r--   0        0        0      426 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event_subscription_list_params.py
--rw-r--r--   0        0        0      360 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/event_subscription_update_params.py
--rw-r--r--   0        0        0     1147 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/export.py
--rw-r--r--   0        0        0     2946 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/export_create_params.py
--rw-r--r--   0        0        0      404 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/export_list_params.py
--rw-r--r--   0        0        0     1205 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/external_account.py
--rw-r--r--   0        0        0      706 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/external_account_create_params.py
--rw-r--r--   0        0        0      701 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/external_account_list_params.py
--rw-r--r--   0        0        0      420 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/external_account_update_params.py
--rw-r--r--   0        0        0     1546 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/file.py
--rw-r--r--   0        0        0     1041 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/file_create_params.py
--rw-r--r--   0        0        0     2120 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/file_list_params.py
--rw-r--r--   0        0        0      738 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/group.py
--rw-r--r--   0        0        0     1693 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/inbound_ach_transfer_return.py
--rw-r--r--   0        0        0     1109 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/inbound_ach_transfer_return_create_params.py
--rw-r--r--   0        0        0      440 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/inbound_ach_transfer_return_list_params.py
--rw-r--r--   0        0        0     2916 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/inbound_wire_drawdown_request.py
--rw-r--r--   0        0        0      444 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/inbound_wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     1041 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/limit.py
--rw-r--r--   0        0        0      696 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/limit_create_params.py
--rw-r--r--   0        0        0      527 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/limit_list_params.py
--rw-r--r--   0        0        0      332 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/limit_update_params.py
--rw-r--r--   0        0        0      779 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/oauth_connection.py
--rw-r--r--   0        0        0      422 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/oauth_connection_list_params.py
--rw-r--r--   0        0        0    13613 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/pending_transaction.py
--rw-r--r--   0        0        0     1956 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/pending_transaction_list_params.py
--rw-r--r--   0        0        0      735 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/program.py
--rw-r--r--   0        0        0      406 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/program_list_params.py
--rw-r--r--   0        0        0     6113 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/real_time_decision.py
--rw-r--r--   0        0        0     2451 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/real_time_decision_action_params.py
--rw-r--r--   0        0        0     5096 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/real_time_payments_transfer.py
--rw-r--r--   0        0        0     1283 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/real_time_payments_transfer_create_params.py
--rw-r--r--   0        0        0     1664 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/real_time_payments_transfer_list_params.py
--rw-r--r--   0        0        0      895 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/routing_number.py
--rw-r--r--   0        0        0      522 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/routing_number_list_params.py
--rw-r--r--   0        0        0      155 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/shared/__init__.py
--rw-r--r--   0        0        0      489 2023-06-13 15:45:28.400205 increase-0.7.0/src/increase/types/shared/point_of_service_entry_mode.py
--rw-r--r--   0        0        0      155 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/shared_params/__init__.py
--rw-r--r--   0        0        0      525 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/shared_params/point_of_service_entry_mode.py
--rw-r--r--   0        0        0     2608 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/__init__.py
--rw-r--r--   0        0        0      338 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/account_statement_create_params.py
--rw-r--r--   0        0        0     1027 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     3320 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/ach_transfer_return_params.py
--rw-r--r--   0        0        0    56855 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/ach_transfer_simulation.py
--rw-r--r--   0        0        0    29451 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/card_authorization_simulation.py
--rw-r--r--   0        0        0      823 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/card_authorize_params.py
--rw-r--r--   0        0        0      443 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/card_dispute_action_params.py
--rw-r--r--   0        0        0      400 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/card_refund_create_params.py
--rw-r--r--   0        0        0      610 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/card_settlement_params.py
--rw-r--r--   0        0        0      425 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/check_transfer_return_params.py
--rw-r--r--   0        0        0      346 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/digital_wallet_token_request_create_params.py
--rw-r--r--   0        0        0      953 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py
--rw-r--r--   0        0        0      325 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/document_create_params.py
--rw-r--r--   0        0        0    57026 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
--rw-r--r--   0        0        0     2648 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      435 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/interest_payment_create_params.py
--rw-r--r--   0        0        0    42198 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/interest_payment_simulation_result.py
--rw-r--r--   0        0        0      299 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/program_create_params.py
--rw-r--r--   0        0        0     1362 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
--rw-r--r--   0        0        0     1020 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
--rw-r--r--   0        0        0     2591 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py
--rw-r--r--   0        0        0    42242 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/simulations/wire_transfer_simulation.py
--rw-r--r--   0        0        0    40458 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/transaction.py
--rw-r--r--   0        0        0     3652 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/transaction_list_params.py
--rw-r--r--   0        0        0     2239 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_drawdown_request.py
--rw-r--r--   0        0        0     1148 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_drawdown_request_create_params.py
--rw-r--r--   0        0        0      430 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_drawdown_request_list_params.py
--rw-r--r--   0        0        0     5343 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_transfer.py
--rw-r--r--   0        0        0     1367 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_transfer_create_params.py
--rw-r--r--   0        0        0     1588 2023-06-13 15:45:28.404205 increase-0.7.0/src/increase/types/wire_transfer_list_params.py
--rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-06-19 20:19:01.358159 increase-0.7.1/LICENSE
+-rw-r--r--   0        0        0     8425 2023-06-19 20:19:01.358159 increase-0.7.1/README.md
+-rw-r--r--   0        0        0     1883 2023-06-19 20:19:01.358159 increase-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0     2587 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/__init__.py
+-rw-r--r--   0        0        0    46808 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_base_client.py
+-rw-r--r--   0        0        0     3889 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_base_exceptions.py
+-rw-r--r--   0        0        0    26762 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_client.py
+-rw-r--r--   0        0        0    10875 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_exceptions.py
+-rw-r--r--   0        0        0     7343 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_models.py
+-rw-r--r--   0        0        0     4846 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_qs.py
+-rw-r--r--   0        0        0      890 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_resource.py
+-rw-r--r--   0        0        0     5884 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_streaming.py
+-rw-r--r--   0        0        0     4229 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_types.py
+-rw-r--r--   0        0        0     1277 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/__init__.py
+-rw-r--r--   0        0        0     6710 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/_transform.py
+-rw-r--r--   0        0        0     9411 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_utils/_utils.py
+-rw-r--r--   0        0        0      127 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/_version.py
+-rw-r--r--   0        0        0     1109 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/pagination.py
+-rw-r--r--   0        0        0        0 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/py.typed
+-rw-r--r--   0        0        0     4478 2023-06-19 20:19:01.358159 increase-0.7.1/src/increase/resources/__init__.py
+-rw-r--r--   0        0        0    15065 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_numbers.py
+-rw-r--r--   0        0        0     7400 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_statements.py
+-rw-r--r--   0        0        0    18102 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/account_transfers.py
+-rw-r--r--   0        0        0    18476 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/accounts.py
+-rw-r--r--   0        0        0    15600 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/ach_prenotifications.py
+-rw-r--r--   0        0        0    26071 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/ach_transfers.py
+-rw-r--r--   0        0        0     4285 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/balance_lookups.py
+-rw-r--r--   0        0        0     8651 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_accounts.py
+-rw-r--r--   0        0        0     4122 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_entries.py
+-rw-r--r--   0        0        0     4842 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/bookkeeping_entry_sets.py
+-rw-r--r--   0        0        0    10707 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/card_disputes.py
+-rw-r--r--   0        0        0    10597 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/card_profiles.py
+-rw-r--r--   0        0        0    19120 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/cards.py
+-rw-r--r--   0        0        0    11757 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/check_deposits.py
+-rw-r--r--   0        0        0    23188 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/check_transfers.py
+-rw-r--r--   0        0        0     7771 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/declined_transactions.py
+-rw-r--r--   0        0        0     7353 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/digital_wallet_tokens.py
+-rw-r--r--   0        0        0     7177 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/documents.py
+-rw-r--r--   0        0        0      282 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/__init__.py
+-rw-r--r--   0        0        0    14010 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/entities.py
+-rw-r--r--   0        0        0     8071 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/entities/supplemental_documents.py
+-rw-r--r--   0        0        0    18799 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/event_subscriptions.py
+-rw-r--r--   0        0        0     7154 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/events.py
+-rw-r--r--   0        0        0    10548 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/exports.py
+-rw-r--r--   0        0        0    15315 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/external_accounts.py
+-rw-r--r--   0        0        0    12781 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/files.py
+-rw-r--r--   0        0        0     2040 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/groups.py
+-rw-r--r--   0        0        0    12035 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/inbound_ach_transfer_returns.py
+-rw-r--r--   0        0        0     7075 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0    14231 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/limits.py
+-rw-r--r--   0        0        0     6593 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/oauth_connections.py
+-rw-r--r--   0        0        0     8344 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/pending_transactions.py
+-rw-r--r--   0        0        0     6300 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/programs.py
+-rw-r--r--   0        0        0     8536 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/real_time_decisions.py
+-rw-r--r--   0        0        0    14968 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4951 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/routing_numbers.py
+-rw-r--r--   0        0        0     1989 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/__init__.py
+-rw-r--r--   0        0        0     4026 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/account_statements.py
+-rw-r--r--   0        0        0     4024 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/account_transfers.py
+-rw-r--r--   0        0        0    21913 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/ach_transfers.py
+-rw-r--r--   0        0        0     5051 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/card_disputes.py
+-rw-r--r--   0        0        0     3967 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/card_refunds.py
+-rw-r--r--   0        0        0    11463 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/cards.py
+-rw-r--r--   0        0        0    10125 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/check_deposits.py
+-rw-r--r--   0        0        0    11013 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/check_transfers.py
+-rw-r--r--   0        0        0     4085 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/digital_wallet_token_requests.py
+-rw-r--r--   0        0        0     3639 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/documents.py
+-rw-r--r--   0        0        0    13466 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py
+-rw-r--r--   0        0        0     4411 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/interest_payments.py
+-rw-r--r--   0        0        0     3919 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/programs.py
+-rw-r--r--   0        0        0    11257 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/real_time_payments_transfers.py
+-rw-r--r--   0        0        0     4588 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/simulations.py
+-rw-r--r--   0        0        0    12351 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/simulations/wire_transfers.py
+-rw-r--r--   0        0        0     7800 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/transactions.py
+-rw-r--r--   0        0        0    13338 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/wire_drawdown_requests.py
+-rw-r--r--   0        0        0    27583 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/resources/wire_transfers.py
+-rw-r--r--   0        0        0     8739 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/__init__.py
+-rw-r--r--   0        0        0     1666 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account.py
+-rw-r--r--   0        0        0      747 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_create_params.py
+-rw-r--r--   0        0        0     1693 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_list_params.py
+-rw-r--r--   0        0        0     1026 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number.py
+-rw-r--r--   0        0        0      408 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_create_params.py
+-rw-r--r--   0        0        0     1598 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_list_params.py
+-rw-r--r--   0        0        0      435 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_number_update_params.py
+-rw-r--r--   0        0        0     1347 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_statement.py
+-rw-r--r--   0        0        0     1534 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_statement_list_params.py
+-rw-r--r--   0        0        0     2648 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer.py
+-rw-r--r--   0        0        0      814 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer_create_params.py
+-rw-r--r--   0        0        0     1494 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_transfer_list_params.py
+-rw-r--r--   0        0        0      271 2023-06-19 20:19:01.362159 increase-0.7.1/src/increase/types/account_update_params.py
+-rw-r--r--   0        0        0     2152 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification.py
+-rw-r--r--   0        0        0     1847 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification_create_params.py
+-rw-r--r--   0        0        0     1391 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_prenotification_list_params.py
+-rw-r--r--   0        0        0     8899 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer.py
+-rw-r--r--   0        0        0     3388 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer_create_params.py
+-rw-r--r--   0        0        0     1592 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/ach_transfer_list_params.py
+-rw-r--r--   0        0        0      585 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/balance_lookup_lookup_params.py
+-rw-r--r--   0        0        0      780 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/balance_lookup_lookup_response.py
+-rw-r--r--   0        0        0      823 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account.py
+-rw-r--r--   0        0        0      626 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account_create_params.py
+-rw-r--r--   0        0        0      428 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_account_list_params.py
+-rw-r--r--   0        0        0      698 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry.py
+-rw-r--r--   0        0        0      424 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_set.py
+-rw-r--r--   0        0        0     1133 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/bookkeeping_entry_set_create_params.py
+-rw-r--r--   0        0        0     2342 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card.py
+-rw-r--r--   0        0        0     1767 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_create_params.py
+-rw-r--r--   0        0        0      907 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_details.py
+-rw-r--r--   0        0        0     2011 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute.py
+-rw-r--r--   0        0        0      483 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute_create_params.py
+-rw-r--r--   0        0        0     1661 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_dispute_list_params.py
+-rw-r--r--   0        0        0     1451 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_list_params.py
+-rw-r--r--   0        0        0     2186 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile.py
+-rw-r--r--   0        0        0     1820 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile_create_params.py
+-rw-r--r--   0        0        0      716 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_profile_list_params.py
+-rw-r--r--   0        0        0     1619 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/card_update_params.py
+-rw-r--r--   0        0        0     4894 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit.py
+-rw-r--r--   0        0        0      748 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit_create_params.py
+-rw-r--r--   0        0        0     1477 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_deposit_list_params.py
+-rw-r--r--   0        0        0     6647 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer.py
+-rw-r--r--   0        0        0     1939 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer_create_params.py
+-rw-r--r--   0        0        0     1488 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/check_transfer_list_params.py
+-rw-r--r--   0        0        0    13068 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/declined_transaction.py
+-rw-r--r--   0        0        0     1598 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/declined_transaction_list_params.py
+-rw-r--r--   0        0        0      950 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/digital_wallet_token.py
+-rw-r--r--   0        0        0     1489 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/digital_wallet_token_list_params.py
+-rw-r--r--   0        0        0     2581 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/document.py
+-rw-r--r--   0        0        0     3900 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/document_list_params.py
+-rw-r--r--   0        0        0      418 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/__init__.py
+-rw-r--r--   0        0        0      634 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document.py
+-rw-r--r--   0        0        0      343 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document_create_params.py
+-rw-r--r--   0        0        0      547 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entities/supplemental_document_list_params.py
+-rw-r--r--   0        0        0    11893 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity.py
+-rw-r--r--   0        0        0    25685 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity_create_params.py
+-rw-r--r--   0        0        0     1367 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/entity_list_params.py
+-rw-r--r--   0        0        0     2724 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event.py
+-rw-r--r--   0        0        0     4044 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_list_params.py
+-rw-r--r--   0        0        0     3124 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription.py
+-rw-r--r--   0        0        0     2526 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_create_params.py
+-rw-r--r--   0        0        0      426 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_list_params.py
+-rw-r--r--   0        0        0      360 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/event_subscription_update_params.py
+-rw-r--r--   0        0        0     1147 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export.py
+-rw-r--r--   0        0        0     2946 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export_create_params.py
+-rw-r--r--   0        0        0      404 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/export_list_params.py
+-rw-r--r--   0        0        0     1205 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account.py
+-rw-r--r--   0        0        0      706 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_create_params.py
+-rw-r--r--   0        0        0      701 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_list_params.py
+-rw-r--r--   0        0        0      420 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/external_account_update_params.py
+-rw-r--r--   0        0        0     1546 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file.py
+-rw-r--r--   0        0        0     1041 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file_create_params.py
+-rw-r--r--   0        0        0     2120 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/file_list_params.py
+-rw-r--r--   0        0        0      738 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/group.py
+-rw-r--r--   0        0        0     1693 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return.py
+-rw-r--r--   0        0        0     1109 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return_create_params.py
+-rw-r--r--   0        0        0      440 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_ach_transfer_return_list_params.py
+-rw-r--r--   0        0        0     2916 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_wire_drawdown_request.py
+-rw-r--r--   0        0        0      444 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/inbound_wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     1041 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit.py
+-rw-r--r--   0        0        0      696 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_create_params.py
+-rw-r--r--   0        0        0      527 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_list_params.py
+-rw-r--r--   0        0        0      332 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/limit_update_params.py
+-rw-r--r--   0        0        0      779 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/oauth_connection.py
+-rw-r--r--   0        0        0      422 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/oauth_connection_list_params.py
+-rw-r--r--   0        0        0    12078 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/pending_transaction.py
+-rw-r--r--   0        0        0     1956 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/pending_transaction_list_params.py
+-rw-r--r--   0        0        0      735 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/program.py
+-rw-r--r--   0        0        0      406 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/program_list_params.py
+-rw-r--r--   0        0        0     6113 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_decision.py
+-rw-r--r--   0        0        0     2451 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_decision_action_params.py
+-rw-r--r--   0        0        0     5096 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer.py
+-rw-r--r--   0        0        0     1283 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer_create_params.py
+-rw-r--r--   0        0        0     1664 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/real_time_payments_transfer_list_params.py
+-rw-r--r--   0        0        0      895 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/routing_number.py
+-rw-r--r--   0        0        0      522 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/routing_number_list_params.py
+-rw-r--r--   0        0        0      155 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared/__init__.py
+-rw-r--r--   0        0        0      489 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0      155 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared_params/__init__.py
+-rw-r--r--   0        0        0      525 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/shared_params/point_of_service_entry_mode.py
+-rw-r--r--   0        0        0     2608 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/__init__.py
+-rw-r--r--   0        0        0      338 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/account_statement_create_params.py
+-rw-r--r--   0        0        0     1027 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     3320 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_return_params.py
+-rw-r--r--   0        0        0    50512 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/ach_transfer_simulation.py
+-rw-r--r--   0        0        0    26885 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_authorization_simulation.py
+-rw-r--r--   0        0        0      823 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_authorize_params.py
+-rw-r--r--   0        0        0      443 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_dispute_action_params.py
+-rw-r--r--   0        0        0      400 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_refund_create_params.py
+-rw-r--r--   0        0        0      610 2023-06-19 20:19:01.366159 increase-0.7.1/src/increase/types/simulations/card_settlement_params.py
+-rw-r--r--   0        0        0      425 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/check_transfer_return_params.py
+-rw-r--r--   0        0        0      346 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_params.py
+-rw-r--r--   0        0        0      953 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py
+-rw-r--r--   0        0        0      325 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/document_create_params.py
+-rw-r--r--   0        0        0    50683 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py
+-rw-r--r--   0        0        0     2648 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      435 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/interest_payment_create_params.py
+-rw-r--r--   0        0        0    36778 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/interest_payment_simulation_result.py
+-rw-r--r--   0        0        0      299 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/program_create_params.py
+-rw-r--r--   0        0        0     1362 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py
+-rw-r--r--   0        0        0     1020 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0     2591 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py
+-rw-r--r--   0        0        0    36822 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/simulations/wire_transfer_simulation.py
+-rw-r--r--   0        0        0    35302 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/transaction.py
+-rw-r--r--   0        0        0     3251 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/transaction_list_params.py
+-rw-r--r--   0        0        0     2239 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request.py
+-rw-r--r--   0        0        0     1148 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request_create_params.py
+-rw-r--r--   0        0        0      430 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_drawdown_request_list_params.py
+-rw-r--r--   0        0        0     5343 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer.py
+-rw-r--r--   0        0        0     1367 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer_create_params.py
+-rw-r--r--   0        0        0     1588 2023-06-19 20:19:01.370159 increase-0.7.1/src/increase/types/wire_transfer_list_params.py
+-rw-r--r--   0        0        0     9328 1970-01-01 00:00:00.000000 increase-0.7.1/PKG-INFO
```

### Comparing `increase-0.7.0/LICENSE` & `increase-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/README.md` & `increase-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/pyproject.toml` & `increase-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "increase"
-version = "0.7.0"
+version = "0.7.1"
 description = "Client library for the increase API"
 readme = "README.md"
 authors = ["Increase <dev-feedback@increase.com>"]
 license = "Apache-2.0"
 repository = "https://github.com/increase/increase-python"
 packages = [
   { include = "increase", from = "src" }
```

### Comparing `increase-0.7.0/src/increase/__init__.py` & `increase-0.7.1/src/increase/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_base_client.py` & `increase-0.7.1/src/increase/_base_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -816,25 +816,62 @@
         resp._set_private_attributes(  # pyright: ignore[reportPrivateUsage]
             client=self,
             model=model,
             options=options,
         )
         return resp
 
+    @overload
     def get(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         options: RequestOptions = {},
+        stream: Literal[False] = False,
     ) -> ResponseT:
+        ...
+
+    @overload
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: Literal[True],
+        stream_cls: type[_StreamT],
+    ) -> _StreamT:
+        ...
+
+    @overload
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool,
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
+        ...
+
+    def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool = False,
+        stream_cls: type[_StreamT] | None = None,
+    ) -> ResponseT | _StreamT:
         opts = FinalRequestOptions.construct(method="get", url=path, **options)
         # cast is required because mypy complains about returning Any even though
         # it understands the type variables
-        return cast(ResponseT, self.request(cast_to, opts, stream=False))
+        return cast(ResponseT, self.request(cast_to, opts, stream=stream, stream_cls=stream_cls))
 
     @overload
     def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
@@ -1113,23 +1150,60 @@
         self,
         model: Type[ModelT],
         page: Type[AsyncPageT],
         options: FinalRequestOptions,
     ) -> AsyncPaginator[ModelT, AsyncPageT]:
         return AsyncPaginator(client=self, options=options, page_cls=page, model=model)
 
+    @overload
     async def get(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
         options: RequestOptions = {},
+        stream: Literal[False] = False,
     ) -> ResponseT:
+        ...
+
+    @overload
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: Literal[True],
+        stream_cls: type[_AsyncStreamT],
+    ) -> _AsyncStreamT:
+        ...
+
+    @overload
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool,
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
+        ...
+
+    async def get(
+        self,
+        path: str,
+        *,
+        cast_to: Type[ResponseT],
+        options: RequestOptions = {},
+        stream: bool = False,
+        stream_cls: type[_AsyncStreamT] | None = None,
+    ) -> ResponseT | _AsyncStreamT:
         opts = FinalRequestOptions.construct(method="get", url=path, **options)
-        return await self.request(cast_to, opts)
+        return await self.request(cast_to, opts, stream=stream, stream_cls=stream_cls)
 
     @overload
     async def post(
         self,
         path: str,
         *,
         cast_to: Type[ResponseT],
```

### Comparing `increase-0.7.0/src/increase/_base_exceptions.py` & `increase-0.7.1/src/increase/_base_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_client.py` & `increase-0.7.1/src/increase/_client.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_exceptions.py` & `increase-0.7.1/src/increase/_exceptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_models.py` & `increase-0.7.1/src/increase/_models.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_qs.py` & `increase-0.7.1/src/increase/_qs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_resource.py` & `increase-0.7.1/src/increase/_resource.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_streaming.py` & `increase-0.7.1/src/increase/_streaming.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_types.py` & `increase-0.7.1/src/increase/_types.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_utils/__init__.py` & `increase-0.7.1/src/increase/_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_utils/_transform.py` & `increase-0.7.1/src/increase/_utils/_transform.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/_utils/_utils.py` & `increase-0.7.1/src/increase/_utils/_utils.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/pagination.py` & `increase-0.7.1/src/increase/pagination.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/__init__.py` & `increase-0.7.1/src/increase/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/account_numbers.py` & `increase-0.7.1/src/increase/resources/account_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/account_statements.py` & `increase-0.7.1/src/increase/resources/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/account_transfers.py` & `increase-0.7.1/src/increase/resources/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/accounts.py` & `increase-0.7.1/src/increase/resources/accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/ach_prenotifications.py` & `increase-0.7.1/src/increase/resources/ach_prenotifications.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/ach_transfers.py` & `increase-0.7.1/src/increase/resources/ach_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/balance_lookups.py` & `increase-0.7.1/src/increase/resources/balance_lookups.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/bookkeeping_accounts.py` & `increase-0.7.1/src/increase/resources/bookkeeping_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/bookkeeping_entries.py` & `increase-0.7.1/src/increase/resources/bookkeeping_entries.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/bookkeeping_entry_sets.py` & `increase-0.7.1/src/increase/resources/bookkeeping_entry_sets.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/card_disputes.py` & `increase-0.7.1/src/increase/resources/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/card_profiles.py` & `increase-0.7.1/src/increase/resources/card_profiles.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/cards.py` & `increase-0.7.1/src/increase/resources/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/check_deposits.py` & `increase-0.7.1/src/increase/resources/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/check_transfers.py` & `increase-0.7.1/src/increase/resources/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/declined_transactions.py` & `increase-0.7.1/src/increase/resources/declined_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/digital_wallet_tokens.py` & `increase-0.7.1/src/increase/resources/digital_wallet_tokens.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/documents.py` & `increase-0.7.1/src/increase/resources/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/entities/entities.py` & `increase-0.7.1/src/increase/resources/entities/entities.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/entities/supplemental_documents.py` & `increase-0.7.1/src/increase/resources/entities/supplemental_documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/event_subscriptions.py` & `increase-0.7.1/src/increase/resources/event_subscriptions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/events.py` & `increase-0.7.1/src/increase/resources/events.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/exports.py` & `increase-0.7.1/src/increase/resources/exports.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/external_accounts.py` & `increase-0.7.1/src/increase/resources/external_accounts.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/files.py` & `increase-0.7.1/src/increase/resources/files.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/groups.py` & `increase-0.7.1/src/increase/resources/groups.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/inbound_ach_transfer_returns.py` & `increase-0.7.1/src/increase/resources/inbound_ach_transfer_returns.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/inbound_wire_drawdown_requests.py` & `increase-0.7.1/src/increase/resources/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/limits.py` & `increase-0.7.1/src/increase/resources/limits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/oauth_connections.py` & `increase-0.7.1/src/increase/resources/oauth_connections.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/pending_transactions.py` & `increase-0.7.1/src/increase/resources/pending_transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/programs.py` & `increase-0.7.1/src/increase/resources/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/real_time_decisions.py` & `increase-0.7.1/src/increase/resources/real_time_decisions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/real_time_payments_transfers.py` & `increase-0.7.1/src/increase/resources/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/routing_numbers.py` & `increase-0.7.1/src/increase/resources/routing_numbers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/__init__.py` & `increase-0.7.1/src/increase/resources/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/account_statements.py` & `increase-0.7.1/src/increase/resources/simulations/account_statements.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/account_transfers.py` & `increase-0.7.1/src/increase/resources/simulations/account_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/ach_transfers.py` & `increase-0.7.1/src/increase/resources/simulations/ach_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/card_disputes.py` & `increase-0.7.1/src/increase/resources/simulations/card_disputes.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/card_refunds.py` & `increase-0.7.1/src/increase/resources/simulations/card_refunds.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/cards.py` & `increase-0.7.1/src/increase/resources/simulations/cards.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/check_deposits.py` & `increase-0.7.1/src/increase/resources/simulations/check_deposits.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/check_transfers.py` & `increase-0.7.1/src/increase/resources/simulations/check_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/digital_wallet_token_requests.py` & `increase-0.7.1/src/increase/resources/simulations/digital_wallet_token_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/documents.py` & `increase-0.7.1/src/increase/resources/simulations/documents.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/inbound_wire_drawdown_requests.py` & `increase-0.7.1/src/increase/resources/simulations/inbound_wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/interest_payments.py` & `increase-0.7.1/src/increase/resources/simulations/interest_payments.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/programs.py` & `increase-0.7.1/src/increase/resources/simulations/programs.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/real_time_payments_transfers.py` & `increase-0.7.1/src/increase/resources/simulations/real_time_payments_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/simulations.py` & `increase-0.7.1/src/increase/resources/simulations/simulations.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/simulations/wire_transfers.py` & `increase-0.7.1/src/increase/resources/simulations/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/transactions.py` & `increase-0.7.1/src/increase/resources/transactions.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/wire_drawdown_requests.py` & `increase-0.7.1/src/increase/resources/wire_drawdown_requests.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/resources/wire_transfers.py` & `increase-0.7.1/src/increase/resources/wire_transfers.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/__init__.py` & `increase-0.7.1/src/increase/types/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account.py` & `increase-0.7.1/src/increase/types/account.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_create_params.py` & `increase-0.7.1/src/increase/types/account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_list_params.py` & `increase-0.7.1/src/increase/types/account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_number.py` & `increase-0.7.1/src/increase/types/account_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_number_list_params.py` & `increase-0.7.1/src/increase/types/account_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_statement.py` & `increase-0.7.1/src/increase/types/account_statement.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_statement_list_params.py` & `increase-0.7.1/src/increase/types/account_statement_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_transfer.py` & `increase-0.7.1/src/increase/types/account_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_transfer_create_params.py` & `increase-0.7.1/src/increase/types/account_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/account_transfer_list_params.py` & `increase-0.7.1/src/increase/types/account_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_prenotification.py` & `increase-0.7.1/src/increase/types/ach_prenotification.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_prenotification_create_params.py` & `increase-0.7.1/src/increase/types/ach_prenotification_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_prenotification_list_params.py` & `increase-0.7.1/src/increase/types/ach_prenotification_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_transfer.py` & `increase-0.7.1/src/increase/types/ach_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_transfer_create_params.py` & `increase-0.7.1/src/increase/types/ach_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/ach_transfer_list_params.py` & `increase-0.7.1/src/increase/types/ach_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/balance_lookup_lookup_params.py` & `increase-0.7.1/src/increase/types/balance_lookup_lookup_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/balance_lookup_lookup_response.py` & `increase-0.7.1/src/increase/types/balance_lookup_lookup_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/bookkeeping_account.py` & `increase-0.7.1/src/increase/types/bookkeeping_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/bookkeeping_account_create_params.py` & `increase-0.7.1/src/increase/types/bookkeeping_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/bookkeeping_entry.py` & `increase-0.7.1/src/increase/types/bookkeeping_entry.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/bookkeeping_entry_set.py` & `increase-0.7.1/src/increase/types/bookkeeping_entry_set.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/bookkeeping_entry_set_create_params.py` & `increase-0.7.1/src/increase/types/bookkeeping_entry_set_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card.py` & `increase-0.7.1/src/increase/types/card.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_create_params.py` & `increase-0.7.1/src/increase/types/card_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_details.py` & `increase-0.7.1/src/increase/types/card_details.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_dispute.py` & `increase-0.7.1/src/increase/types/card_dispute.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_dispute_list_params.py` & `increase-0.7.1/src/increase/types/card_dispute_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_list_params.py` & `increase-0.7.1/src/increase/types/card_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_profile.py` & `increase-0.7.1/src/increase/types/card_profile.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_profile_create_params.py` & `increase-0.7.1/src/increase/types/card_profile_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_profile_list_params.py` & `increase-0.7.1/src/increase/types/card_profile_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/card_update_params.py` & `increase-0.7.1/src/increase/types/card_update_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/check_deposit.py` & `increase-0.7.1/src/increase/types/check_deposit.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
```

### Comparing `increase-0.7.0/src/increase/types/check_deposit_create_params.py` & `increase-0.7.1/src/increase/types/check_deposit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/check_deposit_list_params.py` & `increase-0.7.1/src/increase/types/check_deposit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/check_transfer.py` & `increase-0.7.1/src/increase/types/check_transfer.py`

 * *Files 1% similar despite different names*

```diff
@@ -209,14 +209,15 @@
     """
 
     status: Literal[
         "pending_approval",
         "pending_submission",
         "submitted",
         "pending_mailing",
+        "stopped_and_pending_mailing",
         "mailed",
         "canceled",
         "deposited",
         "stopped",
         "returned",
         "rejected",
         "requires_attention",
```

### Comparing `increase-0.7.0/src/increase/types/check_transfer_create_params.py` & `increase-0.7.1/src/increase/types/check_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/check_transfer_list_params.py` & `increase-0.7.1/src/increase/types/check_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/declined_transaction.py` & `increase-0.7.1/src/increase/types/declined_transaction.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,14 @@
     "SourceACHDecline",
     "SourceCardDecline",
     "SourceCardDeclineNetworkDetails",
     "SourceCardDeclineNetworkDetailsVisa",
     "SourceCheckDecline",
     "SourceInboundRealTimePaymentsTransferDecline",
     "SourceInternationalACHDecline",
-    "SourceCardRouteDecline",
     "SourceWireDecline",
 ]
 
 
 class SourceACHDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
@@ -310,40 +309,14 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class SourceCardRouteDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class SourceWireDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -399,28 +372,20 @@
     card_decline: Optional[SourceCardDecline]
     """A Card Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_decline`.
     """
 
-    card_route_decline: Optional[SourceCardRouteDecline]
-    """A Deprecated Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_decline`.
-    """
-
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
-        "card_route_decline",
         "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
```

### Comparing `increase-0.7.0/src/increase/types/declined_transaction_list_params.py` & `increase-0.7.1/src/increase/types/declined_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/digital_wallet_token.py` & `increase-0.7.1/src/increase/types/digital_wallet_token.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/digital_wallet_token_list_params.py` & `increase-0.7.1/src/increase/types/digital_wallet_token_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/document.py` & `increase-0.7.1/src/increase/types/document.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/document_list_params.py` & `increase-0.7.1/src/increase/types/document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/entities/supplemental_document.py` & `increase-0.7.1/src/increase/types/entities/supplemental_document.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/entities/supplemental_document_list_params.py` & `increase-0.7.1/src/increase/types/entities/supplemental_document_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/entity.py` & `increase-0.7.1/src/increase/types/entity.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/entity_create_params.py` & `increase-0.7.1/src/increase/types/entity_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/entity_list_params.py` & `increase-0.7.1/src/increase/types/entity_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/event.py` & `increase-0.7.1/src/increase/types/event.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/event_list_params.py` & `increase-0.7.1/src/increase/types/event_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/event_subscription.py` & `increase-0.7.1/src/increase/types/event_subscription.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/event_subscription_create_params.py` & `increase-0.7.1/src/increase/types/event_subscription_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/export.py` & `increase-0.7.1/src/increase/types/export.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/export_create_params.py` & `increase-0.7.1/src/increase/types/export_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/external_account.py` & `increase-0.7.1/src/increase/types/external_account.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/external_account_create_params.py` & `increase-0.7.1/src/increase/types/external_account_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/external_account_list_params.py` & `increase-0.7.1/src/increase/types/external_account_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/file.py` & `increase-0.7.1/src/increase/types/file.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/file_create_params.py` & `increase-0.7.1/src/increase/types/file_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/file_list_params.py` & `increase-0.7.1/src/increase/types/file_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/group.py` & `increase-0.7.1/src/increase/types/group.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/inbound_ach_transfer_return.py` & `increase-0.7.1/src/increase/types/inbound_ach_transfer_return.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/inbound_ach_transfer_return_create_params.py` & `increase-0.7.1/src/increase/types/inbound_ach_transfer_return_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/inbound_wire_drawdown_request.py` & `increase-0.7.1/src/increase/types/inbound_wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/limit.py` & `increase-0.7.1/src/increase/types/limit.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/limit_create_params.py` & `increase-0.7.1/src/increase/types/limit_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/limit_list_params.py` & `increase-0.7.1/src/increase/types/limit_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/oauth_connection.py` & `increase-0.7.1/src/increase/types/oauth_connection.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/pending_transaction.py` & `increase-0.7.1/src/increase/types/pending_transaction.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,17 +14,15 @@
     "SourceACHTransferInstruction",
     "SourceCardAuthorization",
     "SourceCardAuthorizationNetworkDetails",
     "SourceCardAuthorizationNetworkDetailsVisa",
     "SourceCheckDepositInstruction",
     "SourceCheckTransferInstruction",
     "SourceInboundFundsHold",
-    "SourceCardRouteAuthorization",
     "SourceRealTimePaymentsTransferInstruction",
-    "SourceWireDrawdownPaymentInstruction",
     "SourceWireTransferInstruction",
 ]
 
 
 class SourceAccountTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
@@ -235,68 +233,28 @@
     released_at: Optional[datetime]
     """When the hold was released (if it has been released)."""
 
     status: Literal["held", "complete"]
     """The status of the hold."""
 
 
-class SourceCardRouteAuthorization(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: str
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class SourceRealTimePaymentsTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     transfer_id: str
     """
     The identifier of the Real Time Payments Transfer that led to this Pending
     Transaction.
     """
 
 
-class SourceWireDrawdownPaymentInstruction(BaseModel):
-    account_number: str
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    message_to_recipient: str
-
-    routing_number: str
-
-
 class SourceWireTransferInstruction(BaseModel):
     account_number: str
 
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -327,31 +285,22 @@
     card_authorization: Optional[SourceCardAuthorization]
     """A Card Authorization object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_authorization`.
     """
 
-    card_route_authorization: Optional[SourceCardRouteAuthorization]
-    """A Deprecated Card Authorization object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_authorization`.
-    """
-
     category: Literal[
         "account_transfer_instruction",
         "ach_transfer_instruction",
         "card_authorization",
         "check_deposit_instruction",
         "check_transfer_instruction",
         "inbound_funds_hold",
-        "card_route_authorization",
         "real_time_payments_transfer_instruction",
-        "wire_drawdown_payment_instruction",
         "wire_transfer_instruction",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
@@ -381,21 +330,14 @@
     real_time_payments_transfer_instruction: Optional[SourceRealTimePaymentsTransferInstruction]
     """A Real Time Payments Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `real_time_payments_transfer_instruction`.
     """
 
-    wire_drawdown_payment_instruction: Optional[SourceWireDrawdownPaymentInstruction]
-    """A Wire Drawdown Payment Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_instruction`.
-    """
-
     wire_transfer_instruction: Optional[SourceWireTransferInstruction]
     """A Wire Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_instruction`.
     """
```

### Comparing `increase-0.7.0/src/increase/types/pending_transaction_list_params.py` & `increase-0.7.1/src/increase/types/pending_transaction_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/program.py` & `increase-0.7.1/src/increase/types/program.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/real_time_decision.py` & `increase-0.7.1/src/increase/types/real_time_decision.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/real_time_decision_action_params.py` & `increase-0.7.1/src/increase/types/real_time_decision_action_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/real_time_payments_transfer.py` & `increase-0.7.1/src/increase/types/real_time_payments_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/real_time_payments_transfer_create_params.py` & `increase-0.7.1/src/increase/types/real_time_payments_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/real_time_payments_transfer_list_params.py` & `increase-0.7.1/src/increase/types/real_time_payments_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/routing_number.py` & `increase-0.7.1/src/increase/types/routing_number.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/routing_number_list_params.py` & `increase-0.7.1/src/increase/types/routing_number_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/shared_params/point_of_service_entry_mode.py` & `increase-0.7.1/src/increase/types/shared_params/point_of_service_entry_mode.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/__init__.py` & `increase-0.7.1/src/increase/types/simulations/__init__.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/ach_transfer_create_inbound_params.py` & `increase-0.7.1/src/increase/types/simulations/ach_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/ach_transfer_return_params.py` & `increase-0.7.1/src/increase/types/simulations/ach_transfer_return_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/ach_transfer_simulation.py` & `increase-0.7.1/src/increase/types/simulations/ach_transfer_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -8,60 +8,51 @@
 from ..._models import BaseModel
 
 __all__ = [
     "ACHTransferSimulation",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
-    "TransactionSourceACHCheckConversionReturn",
-    "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
-    "TransactionSourceDisputeResolution",
-    "TransactionSourceEmpyrealCashDeposit",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
-    "TransactionSourceCardRouteRefund",
-    "TransactionSourceCardRouteSettlement",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
-    "TransactionSourceWireDrawdownPaymentIntention",
-    "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
     "DeclinedTransactionSourceACHDecline",
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceCardRouteDecline",
     "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
@@ -84,36 +75,14 @@
     source_account_id: str
     """The identifier of the Account from where the Account Transfer was sent."""
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class TransactionSourceACHCheckConversionReturn(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    return_reason_code: str
-    """Why the transfer was returned."""
-
-
-class TransactionSourceACHCheckConversion(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    file_id: str
-    """The identifier of the File containing an image of the returned check."""
-
-
 class TransactionSourceACHTransferIntention(BaseModel):
     account_number: str
 
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -430,14 +399,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
@@ -522,43 +492,14 @@
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
-class TransactionSourceDisputeResolution(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    disputed_transaction_id: str
-    """The identifier of the Transaction that was disputed."""
-
-
-class TransactionSourceEmpyrealCashDeposit(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    bag_id: str
-
-    deposit_date: datetime
-
-
 class TransactionSourceFeePayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -928,66 +869,14 @@
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
-class TransactionSourceCardRouteRefund(BaseModel):
-    amount: int
-    """The refunded amount in the minor unit of the refunded currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the refund
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
-class TransactionSourceCardRouteSettlement(BaseModel):
-    amount: int
-    """The settled amount in the minor unit of the settlement currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the settlement
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: Optional[str]
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
     """The destination account number."""
 
@@ -1002,31 +891,14 @@
 
 
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
-class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class TransactionSourceWireDrawdownPaymentRejection(BaseModel):
-    transfer_id: str
-
-
 class TransactionSourceWireTransferIntention(BaseModel):
     account_number: str
     """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
@@ -1047,28 +919,14 @@
     account_transfer_intention: Optional[TransactionSourceAccountTransferIntention]
     """A Account Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `account_transfer_intention`.
     """
 
-    ach_check_conversion: Optional[TransactionSourceACHCheckConversion]
-    """A ACH Check Conversion object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion`.
-    """
-
-    ach_check_conversion_return: Optional[TransactionSourceACHCheckConversionReturn]
-    """A ACH Check Conversion Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion_return`.
-    """
-
     ach_transfer_intention: Optional[TransactionSourceACHTransferIntention]
     """A ACH Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_transfer_intention`.
     """
 
@@ -1103,73 +961,50 @@
     card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
     """A Card Revenue Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_revenue_payment`.
     """
 
-    card_route_refund: Optional[TransactionSourceCardRouteRefund]
-    """A Deprecated Card Refund object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_refund`.
-    """
-
-    card_route_settlement: Optional[TransactionSourceCardRouteSettlement]
-    """A Deprecated Card Settlement object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_settlement`.
-    """
-
     card_settlement: Optional[TransactionSourceCardSettlement]
     """A Card Settlement object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_settlement`.
     """
 
     category: Literal[
         "account_transfer_intention",
-        "ach_check_conversion_return",
-        "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
         "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
-        "dispute_resolution",
-        "empyreal_cash_deposit",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
-        "internal_general_ledger_transaction",
         "internal_source",
-        "card_route_refund",
-        "card_route_settlement",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
-        "wire_drawdown_payment_intention",
-        "wire_drawdown_payment_rejection",
         "wire_transfer_intention",
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
@@ -1214,28 +1049,14 @@
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
-    dispute_resolution: Optional[TransactionSourceDisputeResolution]
-    """A Dispute Resolution object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `dispute_resolution`.
-    """
-
-    empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
-    """A Empyreal Cash Deposit object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `empyreal_cash_deposit`.
-    """
-
     fee_payment: Optional[TransactionSourceFeePayment]
     """A Fee Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `fee_payment`.
     """
 
@@ -1321,28 +1142,14 @@
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
-    wire_drawdown_payment_intention: Optional[TransactionSourceWireDrawdownPaymentIntention]
-    """A Wire Drawdown Payment Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_intention`.
-    """
-
-    wire_drawdown_payment_rejection: Optional[TransactionSourceWireDrawdownPaymentRejection]
-    """A Wire Drawdown Payment Rejection object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_rejection`.
-    """
-
     wire_transfer_intention: Optional[TransactionSourceWireTransferIntention]
     """A Wire Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_intention`.
     """
 
@@ -1699,40 +1506,14 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class DeclinedTransactionSourceCardRouteDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class DeclinedTransactionSourceWireDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -1788,28 +1569,20 @@
     card_decline: Optional[DeclinedTransactionSourceCardDecline]
     """A Card Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_decline`.
     """
 
-    card_route_decline: Optional[DeclinedTransactionSourceCardRouteDecline]
-    """A Deprecated Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_decline`.
-    """
-
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
-        "card_route_decline",
         "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
```

### Comparing `increase-0.7.0/src/increase/types/simulations/card_authorization_simulation.py` & `increase-0.7.1/src/increase/types/simulations/card_authorization_simulation.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,28 +15,25 @@
     "PendingTransactionSourceACHTransferInstruction",
     "PendingTransactionSourceCardAuthorization",
     "PendingTransactionSourceCardAuthorizationNetworkDetails",
     "PendingTransactionSourceCardAuthorizationNetworkDetailsVisa",
     "PendingTransactionSourceCheckDepositInstruction",
     "PendingTransactionSourceCheckTransferInstruction",
     "PendingTransactionSourceInboundFundsHold",
-    "PendingTransactionSourceCardRouteAuthorization",
     "PendingTransactionSourceRealTimePaymentsTransferInstruction",
-    "PendingTransactionSourceWireDrawdownPaymentInstruction",
     "PendingTransactionSourceWireTransferInstruction",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
     "DeclinedTransactionSourceACHDecline",
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceCardRouteDecline",
     "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class PendingTransactionSourceAccountTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
@@ -247,68 +244,28 @@
     released_at: Optional[datetime]
     """When the hold was released (if it has been released)."""
 
     status: Literal["held", "complete"]
     """The status of the hold."""
 
 
-class PendingTransactionSourceCardRouteAuthorization(BaseModel):
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: str
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class PendingTransactionSourceRealTimePaymentsTransferInstruction(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
     transfer_id: str
     """
     The identifier of the Real Time Payments Transfer that led to this Pending
     Transaction.
     """
 
 
-class PendingTransactionSourceWireDrawdownPaymentInstruction(BaseModel):
-    account_number: str
-
-    amount: int
-    """The pending amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    message_to_recipient: str
-
-    routing_number: str
-
-
 class PendingTransactionSourceWireTransferInstruction(BaseModel):
     account_number: str
 
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -339,31 +296,22 @@
     card_authorization: Optional[PendingTransactionSourceCardAuthorization]
     """A Card Authorization object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_authorization`.
     """
 
-    card_route_authorization: Optional[PendingTransactionSourceCardRouteAuthorization]
-    """A Deprecated Card Authorization object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_authorization`.
-    """
-
     category: Literal[
         "account_transfer_instruction",
         "ach_transfer_instruction",
         "card_authorization",
         "check_deposit_instruction",
         "check_transfer_instruction",
         "inbound_funds_hold",
-        "card_route_authorization",
         "real_time_payments_transfer_instruction",
-        "wire_drawdown_payment_instruction",
         "wire_transfer_instruction",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
@@ -393,21 +341,14 @@
     real_time_payments_transfer_instruction: Optional[PendingTransactionSourceRealTimePaymentsTransferInstruction]
     """A Real Time Payments Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `real_time_payments_transfer_instruction`.
     """
 
-    wire_drawdown_payment_instruction: Optional[PendingTransactionSourceWireDrawdownPaymentInstruction]
-    """A Wire Drawdown Payment Instruction object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_instruction`.
-    """
-
     wire_transfer_instruction: Optional[PendingTransactionSourceWireTransferInstruction]
     """A Wire Transfer Instruction object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_instruction`.
     """
 
@@ -768,40 +709,14 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class DeclinedTransactionSourceCardRouteDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class DeclinedTransactionSourceWireDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -857,28 +772,20 @@
     card_decline: Optional[DeclinedTransactionSourceCardDecline]
     """A Card Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_decline`.
     """
 
-    card_route_decline: Optional[DeclinedTransactionSourceCardRouteDecline]
-    """A Deprecated Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_decline`.
-    """
-
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
-        "card_route_decline",
         "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
```

### Comparing `increase-0.7.0/src/increase/types/simulations/card_authorize_params.py` & `increase-0.7.1/src/increase/types/simulations/card_authorize_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/card_settlement_params.py` & `increase-0.7.1/src/increase/types/simulations/card_settlement_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/digital_wallet_token_request_create_response.py` & `increase-0.7.1/src/increase/types/simulations/digital_wallet_token_request_create_response.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py` & `increase-0.7.1/src/increase/types/simulations/inbound_real_time_payments_transfer_simulation_result.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,60 +8,51 @@
 from ..._models import BaseModel
 
 __all__ = [
     "InboundRealTimePaymentsTransferSimulationResult",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
-    "TransactionSourceACHCheckConversionReturn",
-    "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
-    "TransactionSourceDisputeResolution",
-    "TransactionSourceEmpyrealCashDeposit",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
-    "TransactionSourceCardRouteRefund",
-    "TransactionSourceCardRouteSettlement",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
-    "TransactionSourceWireDrawdownPaymentIntention",
-    "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
     "DeclinedTransaction",
     "DeclinedTransactionSource",
     "DeclinedTransactionSourceACHDecline",
     "DeclinedTransactionSourceCardDecline",
     "DeclinedTransactionSourceCardDeclineNetworkDetails",
     "DeclinedTransactionSourceCardDeclineNetworkDetailsVisa",
     "DeclinedTransactionSourceCheckDecline",
     "DeclinedTransactionSourceInboundRealTimePaymentsTransferDecline",
     "DeclinedTransactionSourceInternationalACHDecline",
-    "DeclinedTransactionSourceCardRouteDecline",
     "DeclinedTransactionSourceWireDecline",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
     """The pending amount in the minor unit of the transaction's currency.
@@ -84,36 +75,14 @@
     source_account_id: str
     """The identifier of the Account from where the Account Transfer was sent."""
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class TransactionSourceACHCheckConversionReturn(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    return_reason_code: str
-    """Why the transfer was returned."""
-
-
-class TransactionSourceACHCheckConversion(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    file_id: str
-    """The identifier of the File containing an image of the returned check."""
-
-
 class TransactionSourceACHTransferIntention(BaseModel):
     account_number: str
 
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -430,14 +399,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
@@ -522,43 +492,14 @@
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
-class TransactionSourceDisputeResolution(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    disputed_transaction_id: str
-    """The identifier of the Transaction that was disputed."""
-
-
-class TransactionSourceEmpyrealCashDeposit(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    bag_id: str
-
-    deposit_date: datetime
-
-
 class TransactionSourceFeePayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -928,66 +869,14 @@
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
-class TransactionSourceCardRouteRefund(BaseModel):
-    amount: int
-    """The refunded amount in the minor unit of the refunded currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the refund
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
-class TransactionSourceCardRouteSettlement(BaseModel):
-    amount: int
-    """The settled amount in the minor unit of the settlement currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the settlement
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: Optional[str]
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
     """The destination account number."""
 
@@ -1002,31 +891,14 @@
 
 
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
-class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class TransactionSourceWireDrawdownPaymentRejection(BaseModel):
-    transfer_id: str
-
-
 class TransactionSourceWireTransferIntention(BaseModel):
     account_number: str
     """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
@@ -1047,28 +919,14 @@
     account_transfer_intention: Optional[TransactionSourceAccountTransferIntention]
     """A Account Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `account_transfer_intention`.
     """
 
-    ach_check_conversion: Optional[TransactionSourceACHCheckConversion]
-    """A ACH Check Conversion object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion`.
-    """
-
-    ach_check_conversion_return: Optional[TransactionSourceACHCheckConversionReturn]
-    """A ACH Check Conversion Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion_return`.
-    """
-
     ach_transfer_intention: Optional[TransactionSourceACHTransferIntention]
     """A ACH Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_transfer_intention`.
     """
 
@@ -1103,73 +961,50 @@
     card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
     """A Card Revenue Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_revenue_payment`.
     """
 
-    card_route_refund: Optional[TransactionSourceCardRouteRefund]
-    """A Deprecated Card Refund object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_refund`.
-    """
-
-    card_route_settlement: Optional[TransactionSourceCardRouteSettlement]
-    """A Deprecated Card Settlement object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_settlement`.
-    """
-
     card_settlement: Optional[TransactionSourceCardSettlement]
     """A Card Settlement object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_settlement`.
     """
 
     category: Literal[
         "account_transfer_intention",
-        "ach_check_conversion_return",
-        "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
         "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
-        "dispute_resolution",
-        "empyreal_cash_deposit",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
-        "internal_general_ledger_transaction",
         "internal_source",
-        "card_route_refund",
-        "card_route_settlement",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
-        "wire_drawdown_payment_intention",
-        "wire_drawdown_payment_rejection",
         "wire_transfer_intention",
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
@@ -1214,28 +1049,14 @@
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
-    dispute_resolution: Optional[TransactionSourceDisputeResolution]
-    """A Dispute Resolution object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `dispute_resolution`.
-    """
-
-    empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
-    """A Empyreal Cash Deposit object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `empyreal_cash_deposit`.
-    """
-
     fee_payment: Optional[TransactionSourceFeePayment]
     """A Fee Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `fee_payment`.
     """
 
@@ -1321,28 +1142,14 @@
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
-    wire_drawdown_payment_intention: Optional[TransactionSourceWireDrawdownPaymentIntention]
-    """A Wire Drawdown Payment Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_intention`.
-    """
-
-    wire_drawdown_payment_rejection: Optional[TransactionSourceWireDrawdownPaymentRejection]
-    """A Wire Drawdown Payment Rejection object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_rejection`.
-    """
-
     wire_transfer_intention: Optional[TransactionSourceWireTransferIntention]
     """A Wire Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_intention`.
     """
 
@@ -1699,40 +1506,14 @@
     receiving_depository_financial_institution_id_qualifier: str
 
     receiving_depository_financial_institution_name: str
 
     trace_number: str
 
 
-class DeclinedTransactionSourceCardRouteDecline(BaseModel):
-    amount: int
-    """The declined amount in the minor unit of the destination account currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the destination
-    account currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class DeclinedTransactionSourceWireDecline(BaseModel):
     amount: int
     """The declined amount in the minor unit of the destination account currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -1788,28 +1569,20 @@
     card_decline: Optional[DeclinedTransactionSourceCardDecline]
     """A Card Decline object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_decline`.
     """
 
-    card_route_decline: Optional[DeclinedTransactionSourceCardRouteDecline]
-    """A Deprecated Card Decline object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_decline`.
-    """
-
     category: Literal[
         "ach_decline",
         "card_decline",
         "check_decline",
         "inbound_real_time_payments_transfer_decline",
         "international_ach_decline",
-        "card_route_decline",
         "wire_decline",
         "other",
     ]
     """The type of decline that took place.
 
     We may add additional possible values for this enum over time; your application
     should be able to handle such additions gracefully.
```

### Comparing `increase-0.7.0/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py` & `increase-0.7.1/src/increase/types/simulations/inbound_wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/interest_payment_simulation_result.py` & `increase-0.7.1/src/increase/types/simulations/interest_payment_simulation_result.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,48 +7,40 @@
 from ..._models import BaseModel
 
 __all__ = [
     "InterestPaymentSimulationResult",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
-    "TransactionSourceACHCheckConversionReturn",
-    "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
-    "TransactionSourceDisputeResolution",
-    "TransactionSourceEmpyrealCashDeposit",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
-    "TransactionSourceCardRouteRefund",
-    "TransactionSourceCardRouteSettlement",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
-    "TransactionSourceWireDrawdownPaymentIntention",
-    "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
@@ -72,36 +64,14 @@
     source_account_id: str
     """The identifier of the Account from where the Account Transfer was sent."""
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class TransactionSourceACHCheckConversionReturn(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    return_reason_code: str
-    """Why the transfer was returned."""
-
-
-class TransactionSourceACHCheckConversion(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    file_id: str
-    """The identifier of the File containing an image of the returned check."""
-
-
 class TransactionSourceACHTransferIntention(BaseModel):
     account_number: str
 
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -418,14 +388,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
@@ -510,43 +481,14 @@
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
-class TransactionSourceDisputeResolution(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    disputed_transaction_id: str
-    """The identifier of the Transaction that was disputed."""
-
-
-class TransactionSourceEmpyrealCashDeposit(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    bag_id: str
-
-    deposit_date: datetime
-
-
 class TransactionSourceFeePayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -916,66 +858,14 @@
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
-class TransactionSourceCardRouteRefund(BaseModel):
-    amount: int
-    """The refunded amount in the minor unit of the refunded currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the refund
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
-class TransactionSourceCardRouteSettlement(BaseModel):
-    amount: int
-    """The settled amount in the minor unit of the settlement currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the settlement
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: Optional[str]
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
     """The destination account number."""
 
@@ -990,31 +880,14 @@
 
 
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
-class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class TransactionSourceWireDrawdownPaymentRejection(BaseModel):
-    transfer_id: str
-
-
 class TransactionSourceWireTransferIntention(BaseModel):
     account_number: str
     """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
@@ -1035,28 +908,14 @@
     account_transfer_intention: Optional[TransactionSourceAccountTransferIntention]
     """A Account Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `account_transfer_intention`.
     """
 
-    ach_check_conversion: Optional[TransactionSourceACHCheckConversion]
-    """A ACH Check Conversion object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion`.
-    """
-
-    ach_check_conversion_return: Optional[TransactionSourceACHCheckConversionReturn]
-    """A ACH Check Conversion Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion_return`.
-    """
-
     ach_transfer_intention: Optional[TransactionSourceACHTransferIntention]
     """A ACH Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_transfer_intention`.
     """
 
@@ -1091,73 +950,50 @@
     card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
     """A Card Revenue Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_revenue_payment`.
     """
 
-    card_route_refund: Optional[TransactionSourceCardRouteRefund]
-    """A Deprecated Card Refund object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_refund`.
-    """
-
-    card_route_settlement: Optional[TransactionSourceCardRouteSettlement]
-    """A Deprecated Card Settlement object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_settlement`.
-    """
-
     card_settlement: Optional[TransactionSourceCardSettlement]
     """A Card Settlement object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_settlement`.
     """
 
     category: Literal[
         "account_transfer_intention",
-        "ach_check_conversion_return",
-        "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
         "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
-        "dispute_resolution",
-        "empyreal_cash_deposit",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
-        "internal_general_ledger_transaction",
         "internal_source",
-        "card_route_refund",
-        "card_route_settlement",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
-        "wire_drawdown_payment_intention",
-        "wire_drawdown_payment_rejection",
         "wire_transfer_intention",
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
@@ -1202,28 +1038,14 @@
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
-    dispute_resolution: Optional[TransactionSourceDisputeResolution]
-    """A Dispute Resolution object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `dispute_resolution`.
-    """
-
-    empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
-    """A Empyreal Cash Deposit object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `empyreal_cash_deposit`.
-    """
-
     fee_payment: Optional[TransactionSourceFeePayment]
     """A Fee Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `fee_payment`.
     """
 
@@ -1309,28 +1131,14 @@
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
-    wire_drawdown_payment_intention: Optional[TransactionSourceWireDrawdownPaymentIntention]
-    """A Wire Drawdown Payment Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_intention`.
-    """
-
-    wire_drawdown_payment_rejection: Optional[TransactionSourceWireDrawdownPaymentRejection]
-    """A Wire Drawdown Payment Rejection object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_rejection`.
-    """
-
     wire_transfer_intention: Optional[TransactionSourceWireTransferIntention]
     """A Wire Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_intention`.
     """
```

### Comparing `increase-0.7.0/src/increase/types/simulations/real_time_payments_transfer_complete_params.py` & `increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_complete_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py` & `increase-0.7.1/src/increase/types/simulations/real_time_payments_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/wire_transfer_create_inbound_params.py` & `increase-0.7.1/src/increase/types/simulations/wire_transfer_create_inbound_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/simulations/wire_transfer_simulation.py` & `increase-0.7.1/src/increase/types/simulations/wire_transfer_simulation.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,48 +7,40 @@
 from ..._models import BaseModel
 
 __all__ = [
     "WireTransferSimulation",
     "Transaction",
     "TransactionSource",
     "TransactionSourceAccountTransferIntention",
-    "TransactionSourceACHCheckConversionReturn",
-    "TransactionSourceACHCheckConversion",
     "TransactionSourceACHTransferIntention",
     "TransactionSourceACHTransferRejection",
     "TransactionSourceACHTransferReturn",
     "TransactionSourceCardDisputeAcceptance",
     "TransactionSourceCardRefund",
     "TransactionSourceCardSettlement",
     "TransactionSourceCardRevenuePayment",
     "TransactionSourceCheckDepositAcceptance",
     "TransactionSourceCheckDepositReturn",
     "TransactionSourceCheckTransferIntention",
     "TransactionSourceCheckTransferReturn",
     "TransactionSourceCheckTransferRejection",
     "TransactionSourceCheckTransferStopPaymentRequest",
-    "TransactionSourceDisputeResolution",
-    "TransactionSourceEmpyrealCashDeposit",
     "TransactionSourceFeePayment",
     "TransactionSourceInboundACHTransfer",
     "TransactionSourceInboundCheck",
     "TransactionSourceInboundInternationalACHTransfer",
     "TransactionSourceInboundRealTimePaymentsTransferConfirmation",
     "TransactionSourceInboundWireDrawdownPaymentReversal",
     "TransactionSourceInboundWireDrawdownPayment",
     "TransactionSourceInboundWireReversal",
     "TransactionSourceInboundWireTransfer",
     "TransactionSourceInterestPayment",
     "TransactionSourceInternalSource",
-    "TransactionSourceCardRouteRefund",
-    "TransactionSourceCardRouteSettlement",
     "TransactionSourceRealTimePaymentsTransferAcknowledgement",
     "TransactionSourceSampleFunds",
-    "TransactionSourceWireDrawdownPaymentIntention",
-    "TransactionSourceWireDrawdownPaymentRejection",
     "TransactionSourceWireTransferIntention",
     "TransactionSourceWireTransferRejection",
 ]
 
 
 class TransactionSourceAccountTransferIntention(BaseModel):
     amount: int
@@ -72,36 +64,14 @@
     source_account_id: str
     """The identifier of the Account from where the Account Transfer was sent."""
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class TransactionSourceACHCheckConversionReturn(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    return_reason_code: str
-    """Why the transfer was returned."""
-
-
-class TransactionSourceACHCheckConversion(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    file_id: str
-    """The identifier of the File containing an image of the returned check."""
-
-
 class TransactionSourceACHTransferIntention(BaseModel):
     account_number: str
 
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -418,14 +388,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
@@ -510,43 +481,14 @@
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
-class TransactionSourceDisputeResolution(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    disputed_transaction_id: str
-    """The identifier of the Transaction that was disputed."""
-
-
-class TransactionSourceEmpyrealCashDeposit(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    bag_id: str
-
-    deposit_date: datetime
-
-
 class TransactionSourceFeePayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -916,66 +858,14 @@
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
-class TransactionSourceCardRouteRefund(BaseModel):
-    amount: int
-    """The refunded amount in the minor unit of the refunded currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the refund
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
-class TransactionSourceCardRouteSettlement(BaseModel):
-    amount: int
-    """The settled amount in the minor unit of the settlement currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the settlement
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: Optional[str]
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class TransactionSourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
     """The destination account number."""
 
@@ -990,31 +880,14 @@
 
 
 class TransactionSourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
-class TransactionSourceWireDrawdownPaymentIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class TransactionSourceWireDrawdownPaymentRejection(BaseModel):
-    transfer_id: str
-
-
 class TransactionSourceWireTransferIntention(BaseModel):
     account_number: str
     """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
@@ -1035,28 +908,14 @@
     account_transfer_intention: Optional[TransactionSourceAccountTransferIntention]
     """A Account Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `account_transfer_intention`.
     """
 
-    ach_check_conversion: Optional[TransactionSourceACHCheckConversion]
-    """A ACH Check Conversion object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion`.
-    """
-
-    ach_check_conversion_return: Optional[TransactionSourceACHCheckConversionReturn]
-    """A ACH Check Conversion Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion_return`.
-    """
-
     ach_transfer_intention: Optional[TransactionSourceACHTransferIntention]
     """A ACH Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_transfer_intention`.
     """
 
@@ -1091,73 +950,50 @@
     card_revenue_payment: Optional[TransactionSourceCardRevenuePayment]
     """A Card Revenue Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_revenue_payment`.
     """
 
-    card_route_refund: Optional[TransactionSourceCardRouteRefund]
-    """A Deprecated Card Refund object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_refund`.
-    """
-
-    card_route_settlement: Optional[TransactionSourceCardRouteSettlement]
-    """A Deprecated Card Settlement object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_settlement`.
-    """
-
     card_settlement: Optional[TransactionSourceCardSettlement]
     """A Card Settlement object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_settlement`.
     """
 
     category: Literal[
         "account_transfer_intention",
-        "ach_check_conversion_return",
-        "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
         "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
-        "dispute_resolution",
-        "empyreal_cash_deposit",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
-        "internal_general_ledger_transaction",
         "internal_source",
-        "card_route_refund",
-        "card_route_settlement",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
-        "wire_drawdown_payment_intention",
-        "wire_drawdown_payment_rejection",
         "wire_transfer_intention",
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
@@ -1202,28 +1038,14 @@
     check_transfer_stop_payment_request: Optional[TransactionSourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
-    dispute_resolution: Optional[TransactionSourceDisputeResolution]
-    """A Dispute Resolution object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `dispute_resolution`.
-    """
-
-    empyreal_cash_deposit: Optional[TransactionSourceEmpyrealCashDeposit]
-    """A Empyreal Cash Deposit object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `empyreal_cash_deposit`.
-    """
-
     fee_payment: Optional[TransactionSourceFeePayment]
     """A Fee Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `fee_payment`.
     """
 
@@ -1309,28 +1131,14 @@
     sample_funds: Optional[TransactionSourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
-    wire_drawdown_payment_intention: Optional[TransactionSourceWireDrawdownPaymentIntention]
-    """A Wire Drawdown Payment Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_intention`.
-    """
-
-    wire_drawdown_payment_rejection: Optional[TransactionSourceWireDrawdownPaymentRejection]
-    """A Wire Drawdown Payment Rejection object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_rejection`.
-    """
-
     wire_transfer_intention: Optional[TransactionSourceWireTransferIntention]
     """A Wire Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_intention`.
     """
```

### Comparing `increase-0.7.0/src/increase/types/transaction.py` & `increase-0.7.1/src/increase/types/transaction.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,48 +6,40 @@
 
 from .._models import BaseModel
 
 __all__ = [
     "Transaction",
     "Source",
     "SourceAccountTransferIntention",
-    "SourceACHCheckConversionReturn",
-    "SourceACHCheckConversion",
     "SourceACHTransferIntention",
     "SourceACHTransferRejection",
     "SourceACHTransferReturn",
     "SourceCardDisputeAcceptance",
     "SourceCardRefund",
     "SourceCardSettlement",
     "SourceCardRevenuePayment",
     "SourceCheckDepositAcceptance",
     "SourceCheckDepositReturn",
     "SourceCheckTransferIntention",
     "SourceCheckTransferReturn",
     "SourceCheckTransferRejection",
     "SourceCheckTransferStopPaymentRequest",
-    "SourceDisputeResolution",
-    "SourceEmpyrealCashDeposit",
     "SourceFeePayment",
     "SourceInboundACHTransfer",
     "SourceInboundCheck",
     "SourceInboundInternationalACHTransfer",
     "SourceInboundRealTimePaymentsTransferConfirmation",
     "SourceInboundWireDrawdownPaymentReversal",
     "SourceInboundWireDrawdownPayment",
     "SourceInboundWireReversal",
     "SourceInboundWireTransfer",
     "SourceInterestPayment",
     "SourceInternalSource",
-    "SourceCardRouteRefund",
-    "SourceCardRouteSettlement",
     "SourceRealTimePaymentsTransferAcknowledgement",
     "SourceSampleFunds",
-    "SourceWireDrawdownPaymentIntention",
-    "SourceWireDrawdownPaymentRejection",
     "SourceWireTransferIntention",
     "SourceWireTransferRejection",
 ]
 
 
 class SourceAccountTransferIntention(BaseModel):
     amount: int
@@ -71,36 +63,14 @@
     source_account_id: str
     """The identifier of the Account from where the Account Transfer was sent."""
 
     transfer_id: str
     """The identifier of the Account Transfer that led to this Pending Transaction."""
 
 
-class SourceACHCheckConversionReturn(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    return_reason_code: str
-    """Why the transfer was returned."""
-
-
-class SourceACHCheckConversion(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    file_id: str
-    """The identifier of the File containing an image of the returned check."""
-
-
 class SourceACHTransferIntention(BaseModel):
     account_number: str
 
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
@@ -417,14 +387,15 @@
         "no_account",
         "not_authorized",
         "stale_dated",
         "stop_payment",
         "unknown_reason",
         "unmatched_details",
         "unreadable_image",
+        "endorsement_irregular",
     ]
 
     returned_at: datetime
     """
     The [ISO 8601](https://en.wikipedia.org/wiki/ISO_8601) date and time at which
     the check deposit was returned.
     """
@@ -509,43 +480,14 @@
     type: Literal["check_transfer_stop_payment_request"]
     """A constant representing the object's type.
 
     For this resource it will always be `check_transfer_stop_payment_request`.
     """
 
 
-class SourceDisputeResolution(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the
-    transaction's currency.
-    """
-
-    disputed_transaction_id: str
-    """The identifier of the Transaction that was disputed."""
-
-
-class SourceEmpyrealCashDeposit(BaseModel):
-    amount: int
-    """The amount in the minor unit of the transaction's currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    bag_id: str
-
-    deposit_date: datetime
-
-
 class SourceFeePayment(BaseModel):
     amount: int
     """The amount in the minor unit of the transaction's currency.
 
     For dollars, for example, this is cents.
     """
 
@@ -915,66 +857,14 @@
         "interest",
         "negative_balance_forgiveness",
         "sample_funds",
         "sample_funds_return",
     ]
 
 
-class SourceCardRouteRefund(BaseModel):
-    amount: int
-    """The refunded amount in the minor unit of the refunded currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the refund
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: str
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
-class SourceCardRouteSettlement(BaseModel):
-    amount: int
-    """The settled amount in the minor unit of the settlement currency.
-
-    For dollars, for example, this is cents.
-    """
-
-    currency: Literal["CAD", "CHF", "EUR", "GBP", "JPY", "USD"]
-    """
-    The [ISO 4217](https://en.wikipedia.org/wiki/ISO_4217) code for the settlement
-    currency.
-    """
-
-    merchant_acceptor_id: str
-
-    merchant_category_code: Optional[str]
-
-    merchant_city: Optional[str]
-
-    merchant_country: Optional[str]
-
-    merchant_descriptor: str
-
-    merchant_state: Optional[str]
-
-
 class SourceRealTimePaymentsTransferAcknowledgement(BaseModel):
     amount: int
     """The transfer amount in USD cents."""
 
     destination_account_number: str
     """The destination account number."""
 
@@ -989,31 +879,14 @@
 
 
 class SourceSampleFunds(BaseModel):
     originator: str
     """Where the sample funds came from."""
 
 
-class SourceWireDrawdownPaymentIntention(BaseModel):
-    account_number: str
-
-    amount: int
-    """The transfer amount in USD cents."""
-
-    message_to_recipient: str
-
-    routing_number: str
-
-    transfer_id: str
-
-
-class SourceWireDrawdownPaymentRejection(BaseModel):
-    transfer_id: str
-
-
 class SourceWireTransferIntention(BaseModel):
     account_number: str
     """The destination account number."""
 
     amount: int
     """The transfer amount in USD cents."""
 
@@ -1034,28 +907,14 @@
     account_transfer_intention: Optional[SourceAccountTransferIntention]
     """A Account Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `account_transfer_intention`.
     """
 
-    ach_check_conversion: Optional[SourceACHCheckConversion]
-    """A ACH Check Conversion object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion`.
-    """
-
-    ach_check_conversion_return: Optional[SourceACHCheckConversionReturn]
-    """A ACH Check Conversion Return object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `ach_check_conversion_return`.
-    """
-
     ach_transfer_intention: Optional[SourceACHTransferIntention]
     """A ACH Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `ach_transfer_intention`.
     """
 
@@ -1090,73 +949,50 @@
     card_revenue_payment: Optional[SourceCardRevenuePayment]
     """A Card Revenue Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_revenue_payment`.
     """
 
-    card_route_refund: Optional[SourceCardRouteRefund]
-    """A Deprecated Card Refund object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_refund`.
-    """
-
-    card_route_settlement: Optional[SourceCardRouteSettlement]
-    """A Deprecated Card Settlement object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `card_route_settlement`.
-    """
-
     card_settlement: Optional[SourceCardSettlement]
     """A Card Settlement object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `card_settlement`.
     """
 
     category: Literal[
         "account_transfer_intention",
-        "ach_check_conversion_return",
-        "ach_check_conversion",
         "ach_transfer_intention",
         "ach_transfer_rejection",
         "ach_transfer_return",
         "card_dispute_acceptance",
         "card_refund",
         "card_settlement",
         "card_revenue_payment",
         "check_deposit_acceptance",
         "check_deposit_return",
         "check_transfer_intention",
         "check_transfer_return",
         "check_transfer_rejection",
         "check_transfer_stop_payment_request",
-        "dispute_resolution",
-        "empyreal_cash_deposit",
         "fee_payment",
         "inbound_ach_transfer",
         "inbound_ach_transfer_return_intention",
         "inbound_check",
         "inbound_international_ach_transfer",
         "inbound_real_time_payments_transfer_confirmation",
         "inbound_wire_drawdown_payment_reversal",
         "inbound_wire_drawdown_payment",
         "inbound_wire_reversal",
         "inbound_wire_transfer",
         "interest_payment",
-        "internal_general_ledger_transaction",
         "internal_source",
-        "card_route_refund",
-        "card_route_settlement",
         "real_time_payments_transfer_acknowledgement",
         "sample_funds",
-        "wire_drawdown_payment_intention",
-        "wire_drawdown_payment_rejection",
         "wire_transfer_intention",
         "wire_transfer_rejection",
         "other",
     ]
     """The type of transaction that took place.
 
     We may add additional possible values for this enum over time; your application
@@ -1201,28 +1037,14 @@
     check_transfer_stop_payment_request: Optional[SourceCheckTransferStopPaymentRequest]
     """A Check Transfer Stop Payment Request object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `check_transfer_stop_payment_request`.
     """
 
-    dispute_resolution: Optional[SourceDisputeResolution]
-    """A Dispute Resolution object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `dispute_resolution`.
-    """
-
-    empyreal_cash_deposit: Optional[SourceEmpyrealCashDeposit]
-    """A Empyreal Cash Deposit object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `empyreal_cash_deposit`.
-    """
-
     fee_payment: Optional[SourceFeePayment]
     """A Fee Payment object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `fee_payment`.
     """
 
@@ -1306,28 +1128,14 @@
     sample_funds: Optional[SourceSampleFunds]
     """A Sample Funds object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `sample_funds`.
     """
 
-    wire_drawdown_payment_intention: Optional[SourceWireDrawdownPaymentIntention]
-    """A Wire Drawdown Payment Intention object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_intention`.
-    """
-
-    wire_drawdown_payment_rejection: Optional[SourceWireDrawdownPaymentRejection]
-    """A Wire Drawdown Payment Rejection object.
-
-    This field will be present in the JSON response if and only if `category` is
-    equal to `wire_drawdown_payment_rejection`.
-    """
-
     wire_transfer_intention: Optional[SourceWireTransferIntention]
     """A Wire Transfer Intention object.
 
     This field will be present in the JSON response if and only if `category` is
     equal to `wire_transfer_intention`.
     """
```

### Comparing `increase-0.7.0/src/increase/types/transaction_list_params.py` & `increase-0.7.1/src/increase/types/transaction_list_params.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,50 +37,41 @@
 
 _CategoryReservedKeywords = TypedDict(
     "_CategoryReservedKeywords",
     {
         "in": List[
             Literal[
                 "account_transfer_intention",
-                "ach_check_conversion_return",
-                "ach_check_conversion",
                 "ach_transfer_intention",
                 "ach_transfer_rejection",
                 "ach_transfer_return",
                 "card_dispute_acceptance",
                 "card_refund",
                 "card_settlement",
                 "card_revenue_payment",
                 "check_deposit_acceptance",
                 "check_deposit_return",
                 "check_transfer_intention",
                 "check_transfer_return",
                 "check_transfer_rejection",
                 "check_transfer_stop_payment_request",
-                "dispute_resolution",
-                "empyreal_cash_deposit",
                 "fee_payment",
                 "inbound_ach_transfer",
                 "inbound_ach_transfer_return_intention",
                 "inbound_check",
                 "inbound_international_ach_transfer",
                 "inbound_real_time_payments_transfer_confirmation",
                 "inbound_wire_drawdown_payment_reversal",
                 "inbound_wire_drawdown_payment",
                 "inbound_wire_reversal",
                 "inbound_wire_transfer",
                 "interest_payment",
-                "internal_general_ledger_transaction",
                 "internal_source",
-                "card_route_refund",
-                "card_route_settlement",
                 "real_time_payments_transfer_acknowledgement",
                 "sample_funds",
-                "wire_drawdown_payment_intention",
-                "wire_drawdown_payment_rejection",
                 "wire_transfer_intention",
                 "wire_transfer_rejection",
                 "other",
             ]
         ],
     },
     total=False,
```

### Comparing `increase-0.7.0/src/increase/types/wire_drawdown_request.py` & `increase-0.7.1/src/increase/types/wire_drawdown_request.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/wire_drawdown_request_create_params.py` & `increase-0.7.1/src/increase/types/wire_drawdown_request_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/wire_transfer.py` & `increase-0.7.1/src/increase/types/wire_transfer.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/wire_transfer_create_params.py` & `increase-0.7.1/src/increase/types/wire_transfer_create_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/src/increase/types/wire_transfer_list_params.py` & `increase-0.7.1/src/increase/types/wire_transfer_list_params.py`

 * *Files identical despite different names*

### Comparing `increase-0.7.0/PKG-INFO` & `increase-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: increase
-Version: 0.7.0
+Version: 0.7.1
 Summary: Client library for the increase API
 Home-page: https://github.com/increase/increase-python
 License: Apache-2.0
 Author: Increase
 Author-email: dev-feedback@increase.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

