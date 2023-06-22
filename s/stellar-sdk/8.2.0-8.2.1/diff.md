# Comparing `tmp/stellar_sdk-8.2.0.tar.gz` & `tmp/stellar_sdk-8.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stellar_sdk-8.2.0.tar", max compression
+gzip compressed data, was "stellar_sdk-8.2.1.tar", max compression
```

## Comparing `stellar_sdk-8.2.0.tar` & `stellar_sdk-8.2.1.tar`

### file list

```diff
@@ -1,434 +1,435 @@
--rw-r--r--   0        0        0    11357 2021-10-20 03:21:42.904252 stellar_sdk-8.2.0/LICENSE
--rw-r--r--   0        0        0     6068 2023-03-15 02:03:24.285034 stellar_sdk-8.2.0/README.rst
--rw-r--r--   0        0        0     2870 2023-03-15 04:01:25.723715 stellar_sdk-8.2.0/pyproject.toml
--rw-r--r--   0        0        0      962 2023-02-28 03:15:42.992748 stellar_sdk-8.2.0/stellar_sdk/__init__.py
--rw-r--r--   0        0        0      853 2023-03-15 04:01:25.227903 stellar_sdk-8.2.0/stellar_sdk/__version__.py
--rw-r--r--   0        0        0     4604 2023-03-15 02:03:24.289594 stellar_sdk-8.2.0/stellar_sdk/account.py
--rw-r--r--   0        0        0     9246 2023-03-15 02:03:24.289875 stellar_sdk-8.2.0/stellar_sdk/asset.py
--rw-r--r--   0        0        0    13673 2023-03-15 02:03:24.290382 stellar_sdk-8.2.0/stellar_sdk/base_server.py
--rw-r--r--   0        0        0     5544 2023-03-15 02:03:24.290705 stellar_sdk-8.2.0/stellar_sdk/base_transaction_envelope.py
--rw-r--r--   0        0        0        0 2021-11-23 14:13:01.306920 stellar_sdk-8.2.0/stellar_sdk/call_builder/__init__.py
--rw-r--r--   0        0        0      824 2021-11-23 14:13:01.307012 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/__init__.py
--rw-r--r--   0        0        0     3404 2023-03-15 02:03:24.290867 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py
--rw-r--r--   0        0        0     1507 2023-03-15 02:03:24.290974 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_assets_call_builder.py
--rw-r--r--   0        0        0     4794 2023-03-15 02:03:24.291118 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_call_builder.py
--rw-r--r--   0        0        0     2777 2023-03-15 02:03:24.291248 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py
--rw-r--r--   0        0        0      793 2023-03-15 02:03:24.291373 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_data_call_builder.py
--rw-r--r--   0        0        0     3274 2023-03-15 02:03:24.291493 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_effects_call_builder.py
--rw-r--r--   0        0        0      592 2023-03-15 02:03:24.291601 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py
--rw-r--r--   0        0        0     1014 2023-03-15 02:03:24.291711 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py
--rw-r--r--   0        0        0     2146 2023-03-15 02:03:24.292268 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py
--rw-r--r--   0        0        0     4237 2023-03-15 02:03:24.292783 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_offers_call_builder.py
--rw-r--r--   0        0        0     4618 2023-03-15 02:03:24.293096 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_operations_call_builder.py
--rw-r--r--   0        0        0     1143 2023-03-15 02:03:24.293384 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py
--rw-r--r--   0        0        0     2866 2023-03-15 02:03:24.293506 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_payments_call_builder.py
--rw-r--r--   0        0        0      433 2023-03-15 02:03:24.293635 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_root_call_builder.py
--rw-r--r--   0        0        0     2821 2023-03-15 02:03:24.294042 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2572 2023-03-15 02:03:24.294328 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     3235 2023-03-15 02:03:24.294434 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py
--rw-r--r--   0        0        0     3273 2023-03-15 02:03:24.294539 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_trades_call_builder.py
--rw-r--r--   0        0        0     3729 2023-03-15 02:03:24.294663 stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py
--rw-r--r--   0        0        0      734 2021-11-23 14:13:01.308924 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/__init__.py
--rw-r--r--   0        0        0      925 2023-03-15 02:03:24.294784 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py
--rw-r--r--   0        0        0      887 2023-03-15 02:03:24.294892 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py
--rw-r--r--   0        0        0     4165 2023-03-15 02:03:24.295217 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py
--rw-r--r--   0        0        0      967 2023-03-15 02:03:24.295396 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py
--rw-r--r--   0        0        0     1213 2023-03-15 02:03:24.295515 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py
--rw-r--r--   0        0        0      895 2023-03-15 02:03:24.295628 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py
--rw-r--r--   0        0        0      895 2023-03-15 02:03:24.295731 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py
--rw-r--r--   0        0        0      895 2023-03-15 02:03:24.295826 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py
--rw-r--r--   0        0        0      929 2023-03-15 02:03:24.295974 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py
--rw-r--r--   0        0        0      887 2023-03-15 02:03:24.296082 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py
--rw-r--r--   0        0        0      914 2023-03-15 02:03:24.296187 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py
--rw-r--r--   0        0        0     1136 2023-03-15 02:03:24.296287 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py
--rw-r--r--   0        0        0      914 2023-03-15 02:03:24.296394 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py
--rw-r--r--   0        0        0      764 2023-03-15 02:03:24.296756 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py
--rw-r--r--   0        0        0     2608 2023-03-15 02:03:24.297313 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2377 2023-03-15 02:03:24.297558 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     2182 2023-03-15 02:03:24.297688 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py
--rw-r--r--   0        0        0      887 2023-03-15 02:03:24.297804 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py
--rw-r--r--   0        0        0      935 2023-03-15 02:03:24.297910 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py
--rw-r--r--   0        0        0      734 2021-11-23 14:13:01.310680 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/__init__.py
--rw-r--r--   0        0        0      916 2023-03-15 02:03:24.298382 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py
--rw-r--r--   0        0        0      878 2023-03-15 02:03:24.298510 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py
--rw-r--r--   0        0        0     3967 2023-03-15 02:03:24.298667 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py
--rw-r--r--   0        0        0      958 2023-03-15 02:03:24.298792 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py
--rw-r--r--   0        0        0     1230 2023-03-15 02:03:24.298905 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py
--rw-r--r--   0        0        0      886 2023-03-15 02:03:24.299009 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py
--rw-r--r--   0        0        0      886 2023-03-15 02:03:24.299111 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py
--rw-r--r--   0        0        0      886 2023-03-15 02:03:24.299203 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py
--rw-r--r--   0        0        0      920 2023-03-15 02:03:24.299310 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py
--rw-r--r--   0        0        0      878 2023-03-15 02:03:24.299410 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py
--rw-r--r--   0        0        0      905 2023-03-15 02:03:24.299521 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py
--rw-r--r--   0        0        0     1127 2023-03-15 02:03:24.299623 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py
--rw-r--r--   0        0        0      905 2023-03-15 02:03:24.299732 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py
--rw-r--r--   0        0        0      755 2023-03-15 02:03:24.299840 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py
--rw-r--r--   0        0        0     2625 2023-03-15 02:03:24.300148 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py
--rw-r--r--   0        0        0     2394 2023-03-15 02:03:24.300431 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py
--rw-r--r--   0        0        0     2199 2023-03-15 02:03:24.300548 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py
--rw-r--r--   0        0        0      878 2023-03-15 02:03:24.300666 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py
--rw-r--r--   0        0        0      926 2023-03-15 02:03:24.300767 stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py
--rw-r--r--   0        0        0        0 2021-10-20 03:21:42.917965 stellar_sdk-8.2.0/stellar_sdk/client/__init__.py
--rw-r--r--   0        0        0     9190 2023-03-15 02:03:24.301088 stellar_sdk-8.2.0/stellar_sdk/client/aiohttp_client.py
--rw-r--r--   0        0        0     1872 2023-03-15 02:03:24.301305 stellar_sdk-8.2.0/stellar_sdk/client/base_async_client.py
--rw-r--r--   0        0        0     1754 2023-03-15 02:03:24.301560 stellar_sdk-8.2.0/stellar_sdk/client/base_sync_client.py
--rw-r--r--   0        0        0      445 2021-10-20 03:21:42.918543 stellar_sdk-8.2.0/stellar_sdk/client/defines.py
--rw-r--r--   0        0        0     8438 2023-03-15 02:03:24.301840 stellar_sdk-8.2.0/stellar_sdk/client/requests_client.py
--rw-r--r--   0        0        0     1301 2023-03-15 02:03:24.301938 stellar_sdk-8.2.0/stellar_sdk/client/response.py
--rw-r--r--   0        0        0     2684 2023-03-15 02:03:24.302184 stellar_sdk-8.2.0/stellar_sdk/client/simple_requests_client.py
--rw-r--r--   0        0        0     1888 2023-03-15 02:03:24.302289 stellar_sdk-8.2.0/stellar_sdk/decorated_signature.py
--rw-r--r--   0        0        0     4753 2023-03-15 02:03:24.302398 stellar_sdk-8.2.0/stellar_sdk/exceptions.py
--rw-r--r--   0        0        0     5278 2023-03-15 02:03:24.302517 stellar_sdk-8.2.0/stellar_sdk/fee_bump_transaction.py
--rw-r--r--   0        0        0     5614 2023-03-15 02:03:24.302785 stellar_sdk-8.2.0/stellar_sdk/fee_bump_transaction_envelope.py
--rw-r--r--   0        0        0     2050 2023-03-15 02:03:24.302891 stellar_sdk-8.2.0/stellar_sdk/helpers.py
--rw-r--r--   0        0        0    12132 2023-03-15 02:03:24.303203 stellar_sdk-8.2.0/stellar_sdk/keypair.py
--rw-r--r--   0        0        0     2350 2023-03-15 02:03:24.303630 stellar_sdk-8.2.0/stellar_sdk/ledger_bounds.py
--rw-r--r--   0        0        0     6049 2023-03-15 03:38:59.856105 stellar_sdk-8.2.0/stellar_sdk/liquidity_pool_asset.py
--rw-r--r--   0        0        0     2247 2023-03-15 02:03:24.303897 stellar_sdk-8.2.0/stellar_sdk/liquidity_pool_id.py
--rw-r--r--   0        0        0     9063 2023-03-15 02:03:24.304282 stellar_sdk-8.2.0/stellar_sdk/memo.py
--rw-r--r--   0        0        0     6162 2023-03-15 02:03:24.304553 stellar_sdk-8.2.0/stellar_sdk/muxed_account.py
--rw-r--r--   0        0        0     1794 2023-03-15 02:03:24.304666 stellar_sdk-8.2.0/stellar_sdk/network.py
--rw-r--r--   0        0        0      845 2023-03-15 02:03:24.304787 stellar_sdk-8.2.0/stellar_sdk/operation/__init__.py
--rw-r--r--   0        0        0     2141 2023-03-15 02:03:24.304900 stellar_sdk-8.2.0/stellar_sdk/operation/account_merge.py
--rw-r--r--   0        0        0     6313 2023-03-15 02:03:24.305162 stellar_sdk-8.2.0/stellar_sdk/operation/allow_trust.py
--rw-r--r--   0        0        0     2944 2023-03-15 02:03:24.305283 stellar_sdk-8.2.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py
--rw-r--r--   0        0        0     2217 2023-03-15 02:03:24.305383 stellar_sdk-8.2.0/stellar_sdk/operation/bump_sequence.py
--rw-r--r--   0        0        0     3211 2023-03-15 02:03:24.305644 stellar_sdk-8.2.0/stellar_sdk/operation/change_trust.py
--rw-r--r--   0        0        0     2583 2023-03-15 02:03:24.305742 stellar_sdk-8.2.0/stellar_sdk/operation/claim_claimable_balance.py
--rw-r--r--   0        0        0     2733 2023-03-15 02:03:24.305837 stellar_sdk-8.2.0/stellar_sdk/operation/clawback.py
--rw-r--r--   0        0        0     2564 2023-03-15 02:03:24.305927 stellar_sdk-8.2.0/stellar_sdk/operation/clawback_claimable_balance.py
--rw-r--r--   0        0        0     3325 2023-03-15 02:03:24.306033 stellar_sdk-8.2.0/stellar_sdk/operation/create_account.py
--rw-r--r--   0        0        0    16790 2023-03-15 02:03:24.306340 stellar_sdk-8.2.0/stellar_sdk/operation/create_claimable_balance.py
--rw-r--r--   0        0        0     4411 2023-03-15 02:03:24.306491 stellar_sdk-8.2.0/stellar_sdk/operation/create_passive_sell_offer.py
--rw-r--r--   0        0        0     1791 2023-03-15 02:03:24.306597 stellar_sdk-8.2.0/stellar_sdk/operation/end_sponsoring_future_reserves.py
--rw-r--r--   0        0        0     1266 2023-03-15 02:03:24.306695 stellar_sdk-8.2.0/stellar_sdk/operation/inflation.py
--rw-r--r--   0        0        0     4795 2023-03-15 02:03:24.306803 stellar_sdk-8.2.0/stellar_sdk/operation/liquidity_pool_deposit.py
--rw-r--r--   0        0        0     4201 2023-03-15 02:03:24.306928 stellar_sdk-8.2.0/stellar_sdk/operation/liquidity_pool_withdraw.py
--rw-r--r--   0        0        0     3935 2023-03-15 02:03:24.307040 stellar_sdk-8.2.0/stellar_sdk/operation/manage_buy_offer.py
--rw-r--r--   0        0        0     3445 2023-03-15 02:03:24.307144 stellar_sdk-8.2.0/stellar_sdk/operation/manage_data.py
--rw-r--r--   0        0        0     3946 2023-03-15 02:03:24.307255 stellar_sdk-8.2.0/stellar_sdk/operation/manage_sell_offer.py
--rw-r--r--   0        0        0     4963 2023-03-15 02:03:24.307526 stellar_sdk-8.2.0/stellar_sdk/operation/operation.py
--rw-r--r--   0        0        0     5055 2023-03-15 02:03:24.307793 stellar_sdk-8.2.0/stellar_sdk/operation/path_payment_strict_receive.py
--rw-r--r--   0        0        0     4989 2023-03-15 02:03:24.307983 stellar_sdk-8.2.0/stellar_sdk/operation/path_payment_strict_send.py
--rw-r--r--   0        0        0     2837 2023-03-15 02:03:24.308136 stellar_sdk-8.2.0/stellar_sdk/operation/payment.py
--rw-r--r--   0        0        0    23802 2023-03-15 02:03:24.308433 stellar_sdk-8.2.0/stellar_sdk/operation/revoke_sponsorship.py
--rw-r--r--   0        0        0    10531 2023-03-15 02:03:24.308581 stellar_sdk-8.2.0/stellar_sdk/operation/set_options.py
--rw-r--r--   0        0        0     4687 2023-03-15 02:03:24.308698 stellar_sdk-8.2.0/stellar_sdk/operation/set_trust_line_flags.py
--rw-r--r--   0        0        0     8384 2023-03-15 02:03:24.308973 stellar_sdk-8.2.0/stellar_sdk/preconditions.py
--rw-r--r--   0        0        0     2091 2023-03-15 02:03:24.309082 stellar_sdk-8.2.0/stellar_sdk/price.py
--rw-r--r--   0        0        0        0 2021-11-23 14:13:01.323130 stellar_sdk-8.2.0/stellar_sdk/py.typed
--rw-r--r--   0        0        0        0 2021-10-20 03:21:42.923400 stellar_sdk-8.2.0/stellar_sdk/sep/__init__.py
--rw-r--r--   0        0        0      817 2023-03-15 02:03:24.309193 stellar_sdk-8.2.0/stellar_sdk/sep/ed25519_public_key_signer.py
--rw-r--r--   0        0        0     1550 2021-10-20 03:21:42.923854 stellar_sdk-8.2.0/stellar_sdk/sep/exceptions.py
--rw-r--r--   0        0        0     9288 2023-03-15 02:03:24.309308 stellar_sdk-8.2.0/stellar_sdk/sep/federation.py
--rw-r--r--   0        0        0     3209 2023-03-15 02:03:24.309554 stellar_sdk-8.2.0/stellar_sdk/sep/mnemonic.py
--rw-r--r--   0        0        0     3143 2023-03-15 02:03:24.309653 stellar_sdk-8.2.0/stellar_sdk/sep/stellar_toml.py
--rw-r--r--   0        0        0    19500 2023-03-15 02:03:24.309959 stellar_sdk-8.2.0/stellar_sdk/sep/stellar_uri.py
--rw-r--r--   0        0        0    27755 2023-03-15 02:03:24.310296 stellar_sdk-8.2.0/stellar_sdk/sep/stellar_web_authentication.py
--rw-r--r--   0        0        0     5025 2023-03-15 04:00:52.587223 stellar_sdk-8.2.0/stellar_sdk/sep/toid.py
--rw-r--r--   0        0        0    71993 2023-03-15 02:03:24.310759 stellar_sdk-8.2.0/stellar_sdk/sep/txrep.py
--rw-r--r--   0        0        0    15450 2023-03-15 02:03:24.311263 stellar_sdk-8.2.0/stellar_sdk/server.py
--rw-r--r--   0        0        0    15574 2023-02-27 07:09:33.481238 stellar_sdk-8.2.0/stellar_sdk/server_async.py
--rw-r--r--   0        0        0     4124 2023-03-15 02:03:24.311510 stellar_sdk-8.2.0/stellar_sdk/signer.py
--rw-r--r--   0        0        0    11249 2023-03-15 02:03:24.311783 stellar_sdk-8.2.0/stellar_sdk/signer_key.py
--rw-r--r--   0        0        0    12279 2023-03-15 02:03:24.312080 stellar_sdk-8.2.0/stellar_sdk/strkey.py
--rw-r--r--   0        0        0     2568 2023-03-15 02:03:24.312629 stellar_sdk-8.2.0/stellar_sdk/time_bounds.py
--rw-r--r--   0        0        0    10522 2023-03-15 03:38:59.857067 stellar_sdk-8.2.0/stellar_sdk/transaction.py
--rw-r--r--   0        0        0    55433 2023-03-15 02:03:24.313562 stellar_sdk-8.2.0/stellar_sdk/transaction_builder.py
--rw-r--r--   0        0        0     7188 2023-03-15 02:03:24.314379 stellar_sdk-8.2.0/stellar_sdk/transaction_envelope.py
--rw-r--r--   0        0        0      682 2023-03-15 02:03:24.315192 stellar_sdk-8.2.0/stellar_sdk/type_checked.py
--rw-r--r--   0        0        0     6028 2023-03-15 02:03:24.315982 stellar_sdk-8.2.0/stellar_sdk/utils.py
--rw-r--r--   0        0        0    15456 2023-03-15 02:03:24.316698 stellar_sdk-8.2.0/stellar_sdk/xdr/__init__.py
--rw-r--r--   0        0        0     5998 2023-02-27 07:09:33.738108 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry.py
--rw-r--r--   0        0        0     2173 2023-02-27 07:09:33.705187 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_ext.py
--rw-r--r--   0        0        0     2199 2023-02-27 07:09:33.700481 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v1.py
--rw-r--r--   0        0        0     2239 2023-02-27 07:09:33.732735 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     3775 2023-02-27 07:09:33.760779 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v2.py
--rw-r--r--   0        0        0     2239 2023-02-27 07:09:33.757598 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py
--rw-r--r--   0        0        0     2600 2023-02-27 07:09:33.772865 stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v3.py
--rw-r--r--   0        0        0     1975 2023-02-27 06:10:44.169437 stellar_sdk-8.2.0/stellar_sdk/xdr/account_flags.py
--rw-r--r--   0        0        0     1435 2023-02-27 06:10:44.169539 stellar_sdk-8.2.0/stellar_sdk/xdr/account_id.py
--rw-r--r--   0        0        0     2643 2023-03-15 02:03:24.317016 stellar_sdk-8.2.0/stellar_sdk/xdr/account_merge_result.py
--rw-r--r--   0        0        0     2246 2023-02-27 06:10:44.169824 stellar_sdk-8.2.0/stellar_sdk/xdr/account_merge_result_code.py
--rw-r--r--   0        0        0     2307 2023-02-27 07:09:33.790612 stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_op.py
--rw-r--r--   0        0        0     1865 2023-03-15 02:03:24.319462 stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_result.py
--rw-r--r--   0        0        0     2154 2023-03-15 02:03:24.320061 stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_result_code.py
--rw-r--r--   0        0        0     1903 2023-02-27 07:09:33.802169 stellar_sdk-8.2.0/stellar_sdk/xdr/alpha_num12.py
--rw-r--r--   0        0        0     1891 2023-02-27 07:09:33.817168 stellar_sdk-8.2.0/stellar_sdk/xdr/alpha_num4.py
--rw-r--r--   0        0        0     3284 2023-03-15 02:03:24.320323 stellar_sdk-8.2.0/stellar_sdk/xdr/asset.py
--rw-r--r--   0        0        0     3133 2023-03-15 02:03:24.320564 stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code.py
--rw-r--r--   0        0        0     1482 2023-02-27 06:10:44.172276 stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code12.py
--rw-r--r--   0        0        0     1462 2023-02-27 06:10:44.172372 stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code4.py
--rw-r--r--   0        0        0     1368 2023-02-27 06:10:44.172498 stellar_sdk-8.2.0/stellar_sdk/xdr/asset_type.py
--rw-r--r--   0        0        0     1586 2023-03-15 02:03:24.320794 stellar_sdk-8.2.0/stellar_sdk/xdr/auth.py
--rw-r--r--   0        0        0     2203 2023-02-27 07:09:33.878596 stellar_sdk-8.2.0/stellar_sdk/xdr/auth_cert.py
--rw-r--r--   0        0        0     2188 2023-02-27 07:09:33.878606 stellar_sdk-8.2.0/stellar_sdk/xdr/authenticated_message.py
--rw-r--r--   0        0        0     2297 2023-02-27 07:09:33.921023 stellar_sdk-8.2.0/stellar_sdk/xdr/authenticated_message_v0.py
--rw-r--r--   0        0        0     6074 2023-02-27 07:09:34.015349 stellar_sdk-8.2.0/stellar_sdk/xdr/base.py
--rw-r--r--   0        0        0     1771 2023-02-27 07:09:33.878586 stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
--rw-r--r--   0        0        0     2290 2023-03-15 02:03:24.320963 stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
--rw-r--r--   0        0        0     1843 2023-02-27 06:10:44.173901 stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
--rw-r--r--   0        0        0     4114 2023-03-15 02:03:24.321236 stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_entry.py
--rw-r--r--   0        0        0     1529 2023-02-27 06:10:44.174249 stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_entry_type.py
--rw-r--r--   0        0        0     2165 2023-02-27 07:09:33.921412 stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_metadata.py
--rw-r--r--   0        0        0     1620 2023-02-27 07:09:33.959035 stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_metadata_ext.py
--rw-r--r--   0        0        0     1617 2023-02-27 07:09:33.965898 stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_op.py
--rw-r--r--   0        0        0     1899 2023-03-15 02:03:24.321464 stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_result.py
--rw-r--r--   0        0        0     1451 2023-02-27 06:10:44.175637 stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_result_code.py
--rw-r--r--   0        0        0     4223 2023-03-15 02:03:24.321757 stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_asset.py
--rw-r--r--   0        0        0     1907 2023-02-27 07:09:33.986185 stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_op.py
--rw-r--r--   0        0        0     1882 2023-03-15 02:03:24.321912 stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_result.py
--rw-r--r--   0        0        0     2395 2023-03-15 02:03:24.322216 stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_result_code.py
--rw-r--r--   0        0        0     3812 2023-03-15 02:03:24.322745 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_atom.py
--rw-r--r--   0        0        0     1327 2023-02-27 06:10:44.176551 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_atom_type.py
--rw-r--r--   0        0        0     1737 2023-02-27 07:09:34.022431 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_op.py
--rw-r--r--   0        0        0     2056 2023-03-15 02:03:24.322908 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_result.py
--rw-r--r--   0        0        0     1795 2023-03-15 02:03:24.323016 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py
--rw-r--r--   0        0        0     3197 2023-02-27 07:09:34.077304 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_liquidity_atom.py
--rw-r--r--   0        0        0     3449 2023-02-27 07:09:34.070124 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_offer_atom.py
--rw-r--r--   0        0        0     3512 2023-02-27 07:09:34.117163 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_offer_atom_v0.py
--rw-r--r--   0        0        0     7156 2023-03-15 02:03:24.323351 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_predicate.py
--rw-r--r--   0        0        0     1604 2023-02-27 06:10:44.177988 stellar_sdk-8.2.0/stellar_sdk/xdr/claim_predicate_type.py
--rw-r--r--   0        0        0     3858 2023-02-27 07:09:34.135151 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry.py
--rw-r--r--   0        0        0     2273 2023-02-27 07:09:34.119732 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_ext.py
--rw-r--r--   0        0        0     2176 2023-02-27 07:09:34.128175 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
--rw-r--r--   0        0        0     1728 2023-02-27 07:09:34.123324 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     1388 2023-02-27 06:10:44.179394 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_flags.py
--rw-r--r--   0        0        0     2220 2023-03-15 02:03:24.323527 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_id.py
--rw-r--r--   0        0        0     1235 2023-02-27 06:10:44.179656 stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_id_type.py
--rw-r--r--   0        0        0     2258 2023-03-15 02:03:24.323687 stellar_sdk-8.2.0/stellar_sdk/xdr/claimant.py
--rw-r--r--   0        0        0     1151 2023-02-27 06:10:44.179897 stellar_sdk-8.2.0/stellar_sdk/xdr/claimant_type.py
--rw-r--r--   0        0        0     2075 2023-02-27 07:09:34.169450 stellar_sdk-8.2.0/stellar_sdk/xdr/claimant_v0.py
--rw-r--r--   0        0        0     1758 2023-02-27 07:09:34.159365 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_op.py
--rw-r--r--   0        0        0     2192 2023-03-15 02:03:24.323838 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_result.py
--rw-r--r--   0        0        0     1783 2023-02-27 06:10:44.181019 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
--rw-r--r--   0        0        0     2136 2023-02-27 07:09:34.221095 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_op.py
--rw-r--r--   0        0        0     1827 2023-03-15 02:03:24.324111 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_result.py
--rw-r--r--   0        0        0     1598 2023-02-27 06:10:44.181782 stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_result_code.py
--rw-r--r--   0        0        0      847 2023-03-15 02:03:24.324363 stellar_sdk-8.2.0/stellar_sdk/xdr/constants.py
--rw-r--r--   0        0        0     2123 2023-02-27 07:09:34.308579 stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_op.py
--rw-r--r--   0        0        0     1916 2023-03-15 02:03:24.324525 stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_result.py
--rw-r--r--   0        0        0     1857 2023-02-27 06:10:44.182867 stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_result_code.py
--rw-r--r--   0        0        0     2745 2023-02-27 07:09:34.300758 stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_op.py
--rw-r--r--   0        0        0     2670 2023-03-15 02:03:24.324683 stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_result.py
--rw-r--r--   0        0        0     1804 2023-02-27 06:10:44.183444 stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_result_code.py
--rw-r--r--   0        0        0     2543 2023-02-27 07:09:34.328710 stellar_sdk-8.2.0/stellar_sdk/xdr/create_passive_sell_offer_op.py
--rw-r--r--   0        0        0     1578 2023-02-27 06:10:44.183900 stellar_sdk-8.2.0/stellar_sdk/xdr/crypto_key_type.py
--rw-r--r--   0        0        0     1572 2023-02-27 07:09:34.335604 stellar_sdk-8.2.0/stellar_sdk/xdr/curve25519_public.py
--rw-r--r--   0        0        0     1572 2023-02-27 07:09:34.339620 stellar_sdk-8.2.0/stellar_sdk/xdr/curve25519_secret.py
--rw-r--r--   0        0        0     2750 2023-02-27 07:09:34.363572 stellar_sdk-8.2.0/stellar_sdk/xdr/data_entry.py
--rw-r--r--   0        0        0     1590 2023-02-27 07:09:34.381913 stellar_sdk-8.2.0/stellar_sdk/xdr/data_entry_ext.py
--rw-r--r--   0        0        0     1450 2023-02-27 06:10:44.185280 stellar_sdk-8.2.0/stellar_sdk/xdr/data_value.py
--rw-r--r--   0        0        0     2004 2023-02-27 07:09:34.358434 stellar_sdk-8.2.0/stellar_sdk/xdr/decorated_signature.py
--rw-r--r--   0        0        0     1830 2023-02-27 07:09:34.387644 stellar_sdk-8.2.0/stellar_sdk/xdr/dont_have.py
--rw-r--r--   0        0        0     1392 2023-02-27 06:10:44.185943 stellar_sdk-8.2.0/stellar_sdk/xdr/duration.py
--rw-r--r--   0        0        0     1527 2023-02-27 06:10:44.186064 stellar_sdk-8.2.0/stellar_sdk/xdr/encrypted_body.py
--rw-r--r--   0        0        0     2256 2023-03-15 02:03:24.324981 stellar_sdk-8.2.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
--rw-r--r--   0        0        0     1589 2023-02-27 06:10:44.186430 stellar_sdk-8.2.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
--rw-r--r--   0        0        0     1642 2023-03-15 02:03:24.325222 stellar_sdk-8.2.0/stellar_sdk/xdr/envelope_type.py
--rw-r--r--   0        0        0     1750 2023-02-27 07:09:34.381309 stellar_sdk-8.2.0/stellar_sdk/xdr/error.py
--rw-r--r--   0        0        0     1401 2023-02-27 06:10:44.187032 stellar_sdk-8.2.0/stellar_sdk/xdr/error_code.py
--rw-r--r--   0        0        0     1595 2023-03-15 02:03:24.325574 stellar_sdk-8.2.0/stellar_sdk/xdr/extension_point.py
--rw-r--r--   0        0        0     2890 2023-02-27 07:09:34.406594 stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction.py
--rw-r--r--   0        0        0     2668 2023-02-27 07:09:34.401292 stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py
--rw-r--r--   0        0        0     1644 2023-02-27 07:09:34.467807 stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_ext.py
--rw-r--r--   0        0        0     2237 2023-03-15 02:03:24.325884 stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
--rw-r--r--   0        0        0     1353 2023-02-27 06:10:44.188014 stellar_sdk-8.2.0/stellar_sdk/xdr/hash.py
--rw-r--r--   0        0        0     3538 2023-03-15 02:03:24.326124 stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage.py
--rw-r--r--   0        0        0     2399 2023-02-27 07:09:34.496261 stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py
--rw-r--r--   0        0        0     3081 2023-02-27 07:09:34.521114 stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
--rw-r--r--   0        0        0     4324 2023-02-27 09:45:12.987593 stellar_sdk-8.2.0/stellar_sdk/xdr/hello.py
--rw-r--r--   0        0        0     1551 2023-02-27 07:09:34.531278 stellar_sdk-8.2.0/stellar_sdk/xdr/hmac_sha256_key.py
--rw-r--r--   0        0        0     1551 2023-02-27 07:09:34.541055 stellar_sdk-8.2.0/stellar_sdk/xdr/hmac_sha256_mac.py
--rw-r--r--   0        0        0     1964 2023-02-27 07:09:34.538921 stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_payout.py
--rw-r--r--   0        0        0     2804 2023-03-15 02:03:24.326460 stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_result.py
--rw-r--r--   0        0        0     1386 2023-02-27 06:10:44.190042 stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_result_code.py
--rw-r--r--   0        0        0     3356 2023-03-15 02:03:24.326800 stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result.py
--rw-r--r--   0        0        0     1668 2023-02-27 07:09:34.587333 stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_ext.py
--rw-r--r--   0        0        0     2231 2023-02-27 07:09:34.575501 stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_pair.py
--rw-r--r--   0        0        0     6296 2023-03-15 02:03:24.327063 stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_result.py
--rw-r--r--   0        0        0     1344 2023-02-27 06:10:44.190757 stellar_sdk-8.2.0/stellar_sdk/xdr/int32.py
--rw-r--r--   0        0        0     1340 2023-02-27 06:10:44.190852 stellar_sdk-8.2.0/stellar_sdk/xdr/int64.py
--rw-r--r--   0        0        0     1150 2023-02-27 06:10:44.190945 stellar_sdk-8.2.0/stellar_sdk/xdr/ip_addr_type.py
--rw-r--r--   0        0        0     1948 2023-02-27 07:09:34.619723 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_bounds.py
--rw-r--r--   0        0        0     2012 2023-03-15 02:03:24.327240 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_meta.py
--rw-r--r--   0        0        0     5280 2023-02-27 07:09:34.681047 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_meta_v0.py
--rw-r--r--   0        0        0     2045 2023-02-27 07:09:34.669228 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_value_signature.py
--rw-r--r--   0        0        0     3105 2023-03-15 02:03:24.327398 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry.py
--rw-r--r--   0        0        0     4292 2023-03-15 02:03:24.327555 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_change.py
--rw-r--r--   0        0        0     1541 2023-02-27 06:10:44.192243 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_change_type.py
--rw-r--r--   0        0        0     2241 2023-02-27 07:07:22.857123 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_changes.py
--rw-r--r--   0        0        0     5915 2023-03-15 02:03:24.327807 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_data.py
--rw-r--r--   0        0        0     2162 2023-02-27 07:09:34.718360 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_ext.py
--rw-r--r--   0        0        0     2198 2023-02-27 07:09:34.725656 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_extension_v1.py
--rw-r--r--   0        0        0     1668 2023-02-27 07:09:34.720850 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
--rw-r--r--   0        0        0     1384 2023-03-15 02:03:24.327931 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_type.py
--rw-r--r--   0        0        0     7964 2023-02-27 07:09:34.821220 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header.py
--rw-r--r--   0        0        0     2173 2023-02-27 07:09:34.764174 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_ext.py
--rw-r--r--   0        0        0     2059 2023-02-27 07:09:34.797814 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_extension_v1.py
--rw-r--r--   0        0        0     1674 2023-02-27 07:09:34.763583 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
--rw-r--r--   0        0        0     1425 2023-03-15 02:03:24.328319 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_flags.py
--rw-r--r--   0        0        0     2422 2023-02-27 07:09:34.768126 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_history_entry.py
--rw-r--r--   0        0        0     1680 2023-02-27 07:09:34.780867 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py
--rw-r--r--   0        0        0     6398 2023-03-15 02:03:24.328563 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key.py
--rw-r--r--   0        0        0     1636 2023-02-27 07:09:34.795652 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_account.py
--rw-r--r--   0        0        0     1736 2023-02-27 07:09:34.810351 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_claimable_balance.py
--rw-r--r--   0        0        0     1944 2023-02-27 07:09:34.835875 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_data.py
--rw-r--r--   0        0        0     1740 2023-02-27 07:09:34.850815 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py
--rw-r--r--   0        0        0     1911 2023-02-27 07:09:34.870714 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_offer.py
--rw-r--r--   0        0        0     1959 2023-02-27 07:09:34.854856 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_trust_line.py
--rw-r--r--   0        0        0     2442 2023-02-27 07:09:34.857673 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_scp_messages.py
--rw-r--r--   0        0        0     5635 2023-03-15 02:03:24.328953 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_upgrade.py
--rw-r--r--   0        0        0     1501 2023-03-15 02:03:24.329295 stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_upgrade_type.py
--rw-r--r--   0        0        0     1798 2023-02-27 07:09:34.881512 stellar_sdk-8.2.0/stellar_sdk/xdr/liabilities.py
--rw-r--r--   0        0        0     2363 2023-03-15 02:03:24.329552 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
--rw-r--r--   0        0        0     3239 2023-03-15 02:03:24.329839 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py
--rw-r--r--   0        0        0     2052 2023-03-15 02:03:24.330012 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py
--rw-r--r--   0        0        0     2592 2023-02-27 06:10:44.198001 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
--rw-r--r--   0        0        0     2675 2023-03-15 02:03:24.330176 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry.py
--rw-r--r--   0        0        0     3023 2023-03-15 02:03:24.330353 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry_body.py
--rw-r--r--   0        0        0     3600 2023-03-15 02:03:24.330532 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
--rw-r--r--   0        0        0     2666 2023-03-15 02:03:24.330697 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_parameters.py
--rw-r--r--   0        0        0     1211 2023-02-27 06:10:44.198712 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_type.py
--rw-r--r--   0        0        0     2869 2023-03-15 02:03:24.330862 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
--rw-r--r--   0        0        0     2069 2023-03-15 02:03:24.331027 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
--rw-r--r--   0        0        0     2272 2023-03-15 02:03:24.331122 stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
--rw-r--r--   0        0        0     2979 2023-02-27 07:09:34.990343 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_op.py
--rw-r--r--   0        0        0     2450 2023-03-15 02:03:24.331281 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_result.py
--rw-r--r--   0        0        0     2928 2023-02-27 06:10:44.199553 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_result_code.py
--rw-r--r--   0        0        0     2153 2023-02-27 07:09:34.969421 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_op.py
--rw-r--r--   0        0        0     1865 2023-03-15 02:03:24.331544 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_result.py
--rw-r--r--   0        0        0     1863 2023-02-27 06:10:44.200106 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_result_code.py
--rw-r--r--   0        0        0     1323 2023-02-27 06:10:44.200197 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_effect.py
--rw-r--r--   0        0        0     2931 2023-03-15 02:03:24.331953 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_success_result.py
--rw-r--r--   0        0        0     2790 2023-03-15 02:03:24.332209 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_success_result_offer.py
--rw-r--r--   0        0        0     2899 2023-02-27 07:09:35.044051 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_op.py
--rw-r--r--   0        0        0     2467 2023-03-15 02:03:24.332476 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_result.py
--rw-r--r--   0        0        0     3030 2023-02-27 06:10:44.201057 stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_result_code.py
--rw-r--r--   0        0        0     4005 2023-03-15 02:03:24.332677 stellar_sdk-8.2.0/stellar_sdk/xdr/memo.py
--rw-r--r--   0        0        0     1293 2023-02-27 06:10:44.201300 stellar_sdk-8.2.0/stellar_sdk/xdr/memo_type.py
--rw-r--r--   0        0        0     2023 2023-03-15 02:03:24.332934 stellar_sdk-8.2.0/stellar_sdk/xdr/message_type.py
--rw-r--r--   0        0        0     3024 2023-03-15 02:03:24.333113 stellar_sdk-8.2.0/stellar_sdk/xdr/muxed_account.py
--rw-r--r--   0        0        0     1847 2023-02-27 09:45:12.987791 stellar_sdk-8.2.0/stellar_sdk/xdr/muxed_account_med25519.py
--rw-r--r--   0        0        0     1384 2023-02-27 06:10:44.201936 stellar_sdk-8.2.0/stellar_sdk/xdr/node_id.py
--rw-r--r--   0        0        0     3951 2023-02-27 07:09:35.097567 stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry.py
--rw-r--r--   0        0        0     1596 2023-02-27 07:09:35.057704 stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry_ext.py
--rw-r--r--   0        0        0     1256 2023-03-15 02:03:24.333370 stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry_flags.py
--rw-r--r--   0        0        0     4571 2023-03-15 02:03:24.333742 stellar_sdk-8.2.0/stellar_sdk/xdr/operation.py
--rw-r--r--   0        0        0    23123 2023-03-15 02:03:24.333953 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_body.py
--rw-r--r--   0        0        0     1632 2023-02-27 07:09:35.097581 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_meta.py
--rw-r--r--   0        0        0     4688 2023-03-15 02:03:24.334219 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result.py
--rw-r--r--   0        0        0     1842 2023-02-27 06:10:44.203541 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result_code.py
--rw-r--r--   0        0        0    27203 2023-03-15 02:03:24.334535 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result_tr.py
--rw-r--r--   0        0        0     2646 2023-03-15 02:03:24.334670 stellar_sdk-8.2.0/stellar_sdk/xdr/operation_type.py
--rw-r--r--   0        0        0     4041 2023-02-27 07:09:35.148450 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_op.py
--rw-r--r--   0        0        0     3795 2023-03-15 02:03:24.334849 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result.py
--rw-r--r--   0        0        0     3327 2023-02-27 06:10:44.204512 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
--rw-r--r--   0        0        0     2505 2023-02-27 07:09:35.159816 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
--rw-r--r--   0        0        0     4054 2023-02-27 07:09:35.167435 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_op.py
--rw-r--r--   0        0        0     3623 2023-03-15 02:03:24.335110 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result.py
--rw-r--r--   0        0        0     3217 2023-02-27 06:10:44.205168 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py
--rw-r--r--   0        0        0     2487 2023-02-27 07:09:35.189074 stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py
--rw-r--r--   0        0        0     2306 2023-02-27 07:09:35.203765 stellar_sdk-8.2.0/stellar_sdk/xdr/payment_op.py
--rw-r--r--   0        0        0     1810 2023-03-15 02:03:24.335275 stellar_sdk-8.2.0/stellar_sdk/xdr/payment_result.py
--rw-r--r--   0        0        0     2316 2023-02-27 06:10:44.205912 stellar_sdk-8.2.0/stellar_sdk/xdr/payment_result_code.py
--rw-r--r--   0        0        0     2323 2023-02-27 07:09:35.206616 stellar_sdk-8.2.0/stellar_sdk/xdr/peer_address.py
--rw-r--r--   0        0        0     2697 2023-03-15 02:03:24.335437 stellar_sdk-8.2.0/stellar_sdk/xdr/peer_address_ip.py
--rw-r--r--   0        0        0     2020 2023-02-27 07:07:22.860957 stellar_sdk-8.2.0/stellar_sdk/xdr/peer_stat_list.py
--rw-r--r--   0        0        0     7616 2023-02-27 07:09:35.317604 stellar_sdk-8.2.0/stellar_sdk/xdr/peer_stats.py
--rw-r--r--   0        0        0     1358 2023-02-27 06:10:44.206980 stellar_sdk-8.2.0/stellar_sdk/xdr/pool_id.py
--rw-r--r--   0        0        0     1257 2023-03-15 02:03:24.335655 stellar_sdk-8.2.0/stellar_sdk/xdr/precondition_type.py
--rw-r--r--   0        0        0     3135 2023-03-15 02:03:24.335894 stellar_sdk-8.2.0/stellar_sdk/xdr/preconditions.py
--rw-r--r--   0        0        0     5895 2023-03-15 02:03:24.336080 stellar_sdk-8.2.0/stellar_sdk/xdr/preconditions_v2.py
--rw-r--r--   0        0        0     1652 2023-02-27 07:09:35.332784 stellar_sdk-8.2.0/stellar_sdk/xdr/price.py
--rw-r--r--   0        0        0     2168 2023-03-15 02:03:24.336243 stellar_sdk-8.2.0/stellar_sdk/xdr/public_key.py
--rw-r--r--   0        0        0     1186 2023-02-27 06:10:44.208130 stellar_sdk-8.2.0/stellar_sdk/xdr/public_key_type.py
--rw-r--r--   0        0        0     3281 2023-03-15 02:03:24.336406 stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_op.py
--rw-r--r--   0        0        0     2058 2023-02-27 07:09:35.370178 stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
--rw-r--r--   0        0        0     1984 2023-03-15 02:03:24.336573 stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_result.py
--rw-r--r--   0        0        0     1847 2023-02-27 06:10:44.208840 stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py
--rw-r--r--   0        0        0     1312 2023-02-27 06:10:44.208976 stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_type.py
--rw-r--r--   0        0        0     1815 2023-02-27 07:09:35.666643 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_ballot.py
--rw-r--r--   0        0        0     1939 2023-02-27 07:09:35.643220 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_envelope.py
--rw-r--r--   0        0        0     2012 2023-02-27 07:09:35.696730 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_history_entry.py
--rw-r--r--   0        0        0     2709 2023-02-27 07:09:35.656405 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_history_entry_v0.py
--rw-r--r--   0        0        0     3171 2023-02-27 07:09:35.696650 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_nomination.py
--rw-r--r--   0        0        0     3250 2023-02-27 07:09:35.751972 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_quorum_set.py
--rw-r--r--   0        0        0     3468 2023-02-27 07:09:35.703928 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement.py
--rw-r--r--   0        0        0     2954 2023-02-27 07:09:35.718145 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_confirm.py
--rw-r--r--   0        0        0     2467 2023-02-27 07:09:35.753269 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_externalize.py
--rw-r--r--   0        0        0     5360 2023-03-15 02:03:24.336963 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_pledges.py
--rw-r--r--   0        0        0     3650 2023-02-27 07:09:35.761697 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_prepare.py
--rw-r--r--   0        0        0     1346 2023-02-27 06:10:44.211848 stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_type.py
--rw-r--r--   0        0        0     1594 2023-02-27 07:09:35.743453 stellar_sdk-8.2.0/stellar_sdk/xdr/send_more.py
--rw-r--r--   0        0        0     1499 2023-02-27 06:10:44.212058 stellar_sdk-8.2.0/stellar_sdk/xdr/sequence_number.py
--rw-r--r--   0        0        0     6199 2023-02-27 07:09:35.821732 stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_op.py
--rw-r--r--   0        0        0     1865 2023-03-15 02:03:24.337221 stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_result.py
--rw-r--r--   0        0        0     2584 2023-02-27 06:10:44.212488 stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_result_code.py
--rw-r--r--   0        0        0     2618 2023-02-27 07:09:35.795991 stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_op.py
--rw-r--r--   0        0        0     1992 2023-03-15 02:03:24.337602 stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_result.py
--rw-r--r--   0        0        0     1983 2023-02-27 06:10:44.213185 stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py
--rw-r--r--   0        0        0     1440 2023-02-27 06:10:44.213276 stellar_sdk-8.2.0/stellar_sdk/xdr/signature.py
--rw-r--r--   0        0        0     1513 2023-02-27 06:10:44.213379 stellar_sdk-8.2.0/stellar_sdk/xdr/signature_hint.py
--rw-r--r--   0        0        0     2192 2023-02-27 07:09:35.803084 stellar_sdk-8.2.0/stellar_sdk/xdr/signed_survey_request_message.py
--rw-r--r--   0        0        0     2228 2023-02-27 07:09:35.819578 stellar_sdk-8.2.0/stellar_sdk/xdr/signed_survey_response_message.py
--rw-r--r--   0        0        0     1793 2023-02-27 07:09:35.825049 stellar_sdk-8.2.0/stellar_sdk/xdr/signer.py
--rw-r--r--   0        0        0     4930 2023-03-15 02:03:24.337889 stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key.py
--rw-r--r--   0        0        0     2100 2023-03-15 02:03:24.338102 stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
--rw-r--r--   0        0        0     1504 2023-02-27 06:10:44.214632 stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key_type.py
--rw-r--r--   0        0        0     2256 2023-02-27 07:09:35.853507 stellar_sdk-8.2.0/stellar_sdk/xdr/simple_payment_result.py
--rw-r--r--   0        0        0     1868 2023-02-27 07:07:22.867582 stellar_sdk-8.2.0/stellar_sdk/xdr/sponsorship_descriptor.py
--rw-r--r--   0        0        0    13256 2023-03-15 02:03:24.338371 stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_message.py
--rw-r--r--   0        0        0     3780 2023-02-27 07:09:35.883226 stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value.py
--rw-r--r--   0        0        0     2671 2023-03-15 02:03:24.338661 stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value_ext.py
--rw-r--r--   0        0        0     1248 2023-02-27 06:10:44.216675 stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value_type.py
--rw-r--r--   0        0        0     1405 2023-02-27 06:10:44.216775 stellar_sdk-8.2.0/stellar_sdk/xdr/string32.py
--rw-r--r--   0        0        0     1405 2023-02-27 06:10:44.216875 stellar_sdk-8.2.0/stellar_sdk/xdr/string64.py
--rw-r--r--   0        0        0     1221 2023-02-27 06:10:44.216963 stellar_sdk-8.2.0/stellar_sdk/xdr/survey_message_command_type.py
--rw-r--r--   0        0        0     3354 2023-02-27 07:09:35.877193 stellar_sdk-8.2.0/stellar_sdk/xdr/survey_request_message.py
--rw-r--r--   0        0        0     2633 2023-03-15 02:03:24.338906 stellar_sdk-8.2.0/stellar_sdk/xdr/survey_response_body.py
--rw-r--r--   0        0        0     3346 2023-02-27 07:09:35.958688 stellar_sdk-8.2.0/stellar_sdk/xdr/survey_response_message.py
--rw-r--r--   0        0        0     1350 2023-02-27 06:10:44.217628 stellar_sdk-8.2.0/stellar_sdk/xdr/threshold_indexes.py
--rw-r--r--   0        0        0     1452 2023-02-27 06:10:44.217843 stellar_sdk-8.2.0/stellar_sdk/xdr/thresholds.py
--rw-r--r--   0        0        0     1885 2023-02-27 07:09:35.895489 stellar_sdk-8.2.0/stellar_sdk/xdr/time_bounds.py
--rw-r--r--   0        0        0     1419 2023-02-27 06:10:44.218083 stellar_sdk-8.2.0/stellar_sdk/xdr/time_point.py
--rw-r--r--   0        0        0     3111 2023-03-15 02:03:24.339015 stellar_sdk-8.2.0/stellar_sdk/xdr/topology_response_body.py
--rw-r--r--   0        0        0     4356 2023-02-27 07:09:35.956663 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction.py
--rw-r--r--   0        0        0     3675 2023-03-15 02:03:24.339208 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_envelope.py
--rw-r--r--   0        0        0     1602 2023-02-27 07:09:35.927110 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_ext.py
--rw-r--r--   0        0        0     2500 2023-03-15 02:03:24.339385 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_entry.py
--rw-r--r--   0        0        0     1674 2023-03-15 02:03:24.339545 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_entry_ext.py
--rw-r--r--   0        0        0     2681 2023-02-27 07:09:35.978745 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_result_entry.py
--rw-r--r--   0        0        0     1710 2023-02-27 07:09:35.979028 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py
--rw-r--r--   0        0        0     3762 2023-03-15 02:03:24.339725 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta.py
--rw-r--r--   0        0        0     2634 2023-02-27 07:09:36.037208 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta_v1.py
--rw-r--r--   0        0        0     3340 2023-02-27 07:09:36.035195 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta_v2.py
--rw-r--r--   0        0        0     2874 2023-03-15 02:03:24.339926 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result.py
--rw-r--r--   0        0        0     2894 2023-03-15 02:03:24.340178 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_code.py
--rw-r--r--   0        0        0     1638 2023-02-27 07:09:36.035528 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_ext.py
--rw-r--r--   0        0        0     2650 2023-02-27 07:09:36.078912 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_meta.py
--rw-r--r--   0        0        0     2122 2023-02-27 07:09:36.094441 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_pair.py
--rw-r--r--   0        0        0     4972 2023-03-15 02:03:24.340393 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_result.py
--rw-r--r--   0        0        0     2170 2023-02-27 07:09:36.084129 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_set.py
--rw-r--r--   0        0        0     2506 2023-02-27 07:09:36.135496 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_set.py
--rw-r--r--   0        0        0     2646 2023-02-27 07:09:36.121697 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_signature_payload.py
--rw-r--r--   0        0        0     3202 2023-03-15 02:03:24.340668 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
--rw-r--r--   0        0        0     4455 2023-02-27 09:45:12.988554 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0.py
--rw-r--r--   0        0        0     2607 2023-02-27 07:09:36.163640 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0_envelope.py
--rw-r--r--   0        0        0     1614 2023-02-27 07:09:36.159543 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0_ext.py
--rw-r--r--   0        0        0     2596 2023-02-27 07:09:36.225314 stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v1_envelope.py
--rw-r--r--   0        0        0     4167 2023-03-15 02:03:24.340937 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_asset.py
--rw-r--r--   0        0        0     3848 2023-02-27 07:09:36.198571 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry.py
--rw-r--r--   0        0        0     2472 2023-02-27 07:09:36.203763 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_ext.py
--rw-r--r--   0        0        0     2317 2023-02-27 07:09:36.193840 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py
--rw-r--r--   0        0        0     1686 2023-02-27 07:09:36.208507 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
--rw-r--r--   0        0        0     2194 2023-02-27 07:09:36.223550 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_v1.py
--rw-r--r--   0        0        0     2256 2023-02-27 07:09:36.227398 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py
--rw-r--r--   0        0        0     1710 2023-02-27 06:10:44.223999 stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_flags.py
--rw-r--r--   0        0        0     1404 2023-02-27 06:10:44.224094 stellar_sdk-8.2.0/stellar_sdk/xdr/uint256.py
--rw-r--r--   0        0        0     1394 2023-02-27 06:10:44.224187 stellar_sdk-8.2.0/stellar_sdk/xdr/uint32.py
--rw-r--r--   0        0        0     1390 2023-02-27 06:10:44.224277 stellar_sdk-8.2.0/stellar_sdk/xdr/uint64.py
--rw-r--r--   0        0        0     1978 2023-02-27 07:09:36.231344 stellar_sdk-8.2.0/stellar_sdk/xdr/upgrade_entry_meta.py
--rw-r--r--   0        0        0     1487 2023-02-27 06:10:44.224520 stellar_sdk-8.2.0/stellar_sdk/xdr/upgrade_type.py
--rw-r--r--   0        0        0     1386 2023-02-27 06:10:44.224619 stellar_sdk-8.2.0/stellar_sdk/xdr/value.py
--rw-r--r--   0        0        0     8112 1970-01-01 00:00:00.000000 stellar_sdk-8.2.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2021-10-20 03:21:42.904252 stellar_sdk-8.2.1/LICENSE
+-rw-r--r--   0        0        0     6068 2023-05-31 08:17:56.136490 stellar_sdk-8.2.1/README.rst
+-rw-r--r--   0        0        0     2877 2023-06-22 11:40:34.862113 stellar_sdk-8.2.1/pyproject.toml
+-rw-r--r--   0        0        0      962 2023-05-31 08:17:56.149111 stellar_sdk-8.2.1/stellar_sdk/__init__.py
+-rw-r--r--   0        0        0      853 2023-06-22 11:40:34.882041 stellar_sdk-8.2.1/stellar_sdk/__version__.py
+-rw-r--r--   0        0        0     4604 2023-06-22 10:47:37.978434 stellar_sdk-8.2.1/stellar_sdk/account.py
+-rw-r--r--   0        0        0     9246 2023-06-22 10:47:37.978745 stellar_sdk-8.2.1/stellar_sdk/asset.py
+-rw-r--r--   0        0        0    13673 2023-06-22 10:47:37.978992 stellar_sdk-8.2.1/stellar_sdk/base_server.py
+-rw-r--r--   0        0        0     5544 2023-06-22 10:47:37.979410 stellar_sdk-8.2.1/stellar_sdk/base_transaction_envelope.py
+-rw-r--r--   0        0        0        0 2021-11-23 14:13:01.306920 stellar_sdk-8.2.1/stellar_sdk/call_builder/__init__.py
+-rw-r--r--   0        0        0      824 2021-11-23 14:13:01.307012 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/__init__.py
+-rw-r--r--   0        0        0     3404 2023-06-22 10:47:37.979519 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_accounts_call_builder.py
+-rw-r--r--   0        0        0     1507 2023-06-22 10:47:37.979597 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_assets_call_builder.py
+-rw-r--r--   0        0        0     4794 2023-06-22 10:47:37.979689 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_call_builder.py
+-rw-r--r--   0        0        0     2777 2023-06-22 10:47:37.979781 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py
+-rw-r--r--   0        0        0      793 2023-06-22 10:47:37.979893 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_data_call_builder.py
+-rw-r--r--   0        0        0     3274 2023-06-22 10:47:37.979994 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_effects_call_builder.py
+-rw-r--r--   0        0        0      592 2023-06-22 10:47:37.980075 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py
+-rw-r--r--   0        0        0     1014 2023-06-22 10:47:37.980149 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_ledgers_call_builder.py
+-rw-r--r--   0        0        0     2146 2023-06-22 10:47:37.980443 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py
+-rw-r--r--   0        0        0     4237 2023-06-22 10:47:37.980680 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_offers_call_builder.py
+-rw-r--r--   0        0        0     4618 2023-06-22 10:47:37.980754 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_operations_call_builder.py
+-rw-r--r--   0        0        0     1143 2023-06-22 10:47:37.980971 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_orderbook_call_builder.py
+-rw-r--r--   0        0        0     2866 2023-06-22 10:47:37.981055 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_payments_call_builder.py
+-rw-r--r--   0        0        0      433 2023-06-22 10:47:37.981352 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_root_call_builder.py
+-rw-r--r--   0        0        0     2821 2023-06-22 10:47:37.981861 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2572 2023-06-22 10:47:37.982170 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     3235 2023-06-22 10:47:37.982296 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0     3273 2023-06-22 10:47:37.982424 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_trades_call_builder.py
+-rw-r--r--   0        0        0     3729 2023-06-22 10:47:37.982632 stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_transactions_call_builder.py
+-rw-r--r--   0        0        0      734 2021-11-23 14:13:01.308924 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/__init__.py
+-rw-r--r--   0        0        0      925 2023-06-22 10:47:37.982760 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py
+-rw-r--r--   0        0        0      887 2023-06-22 10:47:37.982856 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py
+-rw-r--r--   0        0        0     4165 2023-06-22 10:47:37.983168 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/base_call_builder.py
+-rw-r--r--   0        0        0      967 2023-06-22 10:47:37.983328 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py
+-rw-r--r--   0        0        0     1213 2023-06-22 10:47:37.983430 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/data_call_builder.py
+-rw-r--r--   0        0        0      895 2023-06-22 10:47:37.983523 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py
+-rw-r--r--   0        0        0      895 2023-06-22 10:47:37.983609 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py
+-rw-r--r--   0        0        0      895 2023-06-22 10:47:37.983706 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py
+-rw-r--r--   0        0        0      929 2023-06-22 10:47:37.983822 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py
+-rw-r--r--   0        0        0      887 2023-06-22 10:47:37.983916 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py
+-rw-r--r--   0        0        0      914 2023-06-22 10:47:37.984012 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py
+-rw-r--r--   0        0        0     1136 2023-06-22 10:47:37.984102 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py
+-rw-r--r--   0        0        0      914 2023-06-22 10:47:37.984192 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py
+-rw-r--r--   0        0        0      764 2023-06-22 10:47:37.984393 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/root_call_builder.py
+-rw-r--r--   0        0        0     2608 2023-06-22 10:47:37.984664 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2377 2023-06-22 10:47:37.984914 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     2182 2023-06-22 10:47:37.985067 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0      887 2023-06-22 10:47:37.985149 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py
+-rw-r--r--   0        0        0      935 2023-06-22 10:47:37.985242 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py
+-rw-r--r--   0        0        0      734 2021-11-23 14:13:01.310680 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/__init__.py
+-rw-r--r--   0        0        0      916 2023-06-22 10:47:37.985349 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py
+-rw-r--r--   0        0        0      878 2023-06-22 10:47:37.985440 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py
+-rw-r--r--   0        0        0     3967 2023-06-22 10:47:37.985577 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py
+-rw-r--r--   0        0        0      958 2023-06-22 10:47:37.985668 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py
+-rw-r--r--   0        0        0     1230 2023-06-22 10:47:37.985755 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py
+-rw-r--r--   0        0        0      886 2023-06-22 10:47:37.985844 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py
+-rw-r--r--   0        0        0      886 2023-06-22 10:47:37.985924 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py
+-rw-r--r--   0        0        0      886 2023-06-22 10:47:37.986012 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py
+-rw-r--r--   0        0        0      920 2023-06-22 10:47:37.986103 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py
+-rw-r--r--   0        0        0      878 2023-06-22 10:47:37.986198 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py
+-rw-r--r--   0        0        0      905 2023-06-22 10:47:37.986381 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py
+-rw-r--r--   0        0        0     1127 2023-06-22 10:47:37.986464 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py
+-rw-r--r--   0        0        0      905 2023-06-22 10:47:37.986547 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py
+-rw-r--r--   0        0        0      755 2023-06-22 10:47:37.986634 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py
+-rw-r--r--   0        0        0     2625 2023-06-22 10:47:37.986864 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py
+-rw-r--r--   0        0        0     2394 2023-06-22 10:47:37.987219 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py
+-rw-r--r--   0        0        0     2199 2023-06-22 10:47:37.987302 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py
+-rw-r--r--   0        0        0      878 2023-06-22 10:47:37.987389 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py
+-rw-r--r--   0        0        0      926 2023-06-22 10:47:37.987474 stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py
+-rw-r--r--   0        0        0        0 2021-10-20 03:21:42.917965 stellar_sdk-8.2.1/stellar_sdk/client/__init__.py
+-rw-r--r--   0        0        0     9190 2023-06-22 10:47:37.987847 stellar_sdk-8.2.1/stellar_sdk/client/aiohttp_client.py
+-rw-r--r--   0        0        0     1872 2023-06-22 10:47:37.988060 stellar_sdk-8.2.1/stellar_sdk/client/base_async_client.py
+-rw-r--r--   0        0        0     1754 2023-06-22 10:47:37.988519 stellar_sdk-8.2.1/stellar_sdk/client/base_sync_client.py
+-rw-r--r--   0        0        0      445 2021-10-20 03:21:42.918543 stellar_sdk-8.2.1/stellar_sdk/client/defines.py
+-rw-r--r--   0        0        0     8472 2023-06-22 10:47:37.988999 stellar_sdk-8.2.1/stellar_sdk/client/requests_client.py
+-rw-r--r--   0        0        0     1301 2023-06-22 10:47:37.989098 stellar_sdk-8.2.1/stellar_sdk/client/response.py
+-rw-r--r--   0        0        0     2684 2023-06-22 10:47:37.989237 stellar_sdk-8.2.1/stellar_sdk/client/simple_requests_client.py
+-rw-r--r--   0        0        0     1888 2023-06-22 10:47:37.989345 stellar_sdk-8.2.1/stellar_sdk/decorated_signature.py
+-rw-r--r--   0        0        0     4753 2023-06-22 10:47:37.989469 stellar_sdk-8.2.1/stellar_sdk/exceptions.py
+-rw-r--r--   0        0        0     5278 2023-06-22 10:47:37.989599 stellar_sdk-8.2.1/stellar_sdk/fee_bump_transaction.py
+-rw-r--r--   0        0        0     5614 2023-06-22 10:47:37.989869 stellar_sdk-8.2.1/stellar_sdk/fee_bump_transaction_envelope.py
+-rw-r--r--   0        0        0     2050 2023-06-22 10:47:37.989978 stellar_sdk-8.2.1/stellar_sdk/helpers.py
+-rw-r--r--   0        0        0    12132 2023-06-22 10:47:37.990262 stellar_sdk-8.2.1/stellar_sdk/keypair.py
+-rw-r--r--   0        0        0     2350 2023-06-22 10:47:37.990527 stellar_sdk-8.2.1/stellar_sdk/ledger_bounds.py
+-rw-r--r--   0        0        0     6049 2023-06-22 11:38:26.048845 stellar_sdk-8.2.1/stellar_sdk/liquidity_pool_asset.py
+-rw-r--r--   0        0        0     2247 2023-06-22 10:47:37.990751 stellar_sdk-8.2.1/stellar_sdk/liquidity_pool_id.py
+-rw-r--r--   0        0        0     9063 2023-06-22 10:47:37.991012 stellar_sdk-8.2.1/stellar_sdk/memo.py
+-rw-r--r--   0        0        0     6162 2023-06-22 10:47:37.991266 stellar_sdk-8.2.1/stellar_sdk/muxed_account.py
+-rw-r--r--   0        0        0     1794 2023-06-22 10:47:37.991362 stellar_sdk-8.2.1/stellar_sdk/network.py
+-rw-r--r--   0        0        0      845 2023-06-22 10:47:37.991480 stellar_sdk-8.2.1/stellar_sdk/operation/__init__.py
+-rw-r--r--   0        0        0     2141 2023-06-22 10:47:37.991597 stellar_sdk-8.2.1/stellar_sdk/operation/account_merge.py
+-rw-r--r--   0        0        0     6313 2023-06-22 10:47:37.991849 stellar_sdk-8.2.1/stellar_sdk/operation/allow_trust.py
+-rw-r--r--   0        0        0     2944 2023-06-22 10:47:37.991949 stellar_sdk-8.2.1/stellar_sdk/operation/begin_sponsoring_future_reserves.py
+-rw-r--r--   0        0        0     2217 2023-06-22 10:47:37.992160 stellar_sdk-8.2.1/stellar_sdk/operation/bump_sequence.py
+-rw-r--r--   0        0        0     3211 2023-06-22 10:47:37.992411 stellar_sdk-8.2.1/stellar_sdk/operation/change_trust.py
+-rw-r--r--   0        0        0     2583 2023-06-22 10:47:37.992520 stellar_sdk-8.2.1/stellar_sdk/operation/claim_claimable_balance.py
+-rw-r--r--   0        0        0     2733 2023-06-22 10:47:37.992629 stellar_sdk-8.2.1/stellar_sdk/operation/clawback.py
+-rw-r--r--   0        0        0     2564 2023-06-22 10:47:37.992720 stellar_sdk-8.2.1/stellar_sdk/operation/clawback_claimable_balance.py
+-rw-r--r--   0        0        0     3325 2023-06-22 10:47:37.992825 stellar_sdk-8.2.1/stellar_sdk/operation/create_account.py
+-rw-r--r--   0        0        0    16790 2023-06-22 10:47:37.993113 stellar_sdk-8.2.1/stellar_sdk/operation/create_claimable_balance.py
+-rw-r--r--   0        0        0     4411 2023-06-22 10:47:37.993241 stellar_sdk-8.2.1/stellar_sdk/operation/create_passive_sell_offer.py
+-rw-r--r--   0        0        0     1791 2023-06-22 10:47:37.993325 stellar_sdk-8.2.1/stellar_sdk/operation/end_sponsoring_future_reserves.py
+-rw-r--r--   0        0        0     1266 2023-06-22 10:47:37.993417 stellar_sdk-8.2.1/stellar_sdk/operation/inflation.py
+-rw-r--r--   0        0        0     4795 2023-06-22 10:47:37.993514 stellar_sdk-8.2.1/stellar_sdk/operation/liquidity_pool_deposit.py
+-rw-r--r--   0        0        0     4201 2023-06-22 10:47:37.993612 stellar_sdk-8.2.1/stellar_sdk/operation/liquidity_pool_withdraw.py
+-rw-r--r--   0        0        0     3935 2023-06-22 10:47:37.993703 stellar_sdk-8.2.1/stellar_sdk/operation/manage_buy_offer.py
+-rw-r--r--   0        0        0     3445 2023-06-22 10:47:37.993794 stellar_sdk-8.2.1/stellar_sdk/operation/manage_data.py
+-rw-r--r--   0        0        0     3946 2023-06-22 10:47:37.993893 stellar_sdk-8.2.1/stellar_sdk/operation/manage_sell_offer.py
+-rw-r--r--   0        0        0     4963 2023-06-22 10:47:37.994140 stellar_sdk-8.2.1/stellar_sdk/operation/operation.py
+-rw-r--r--   0        0        0     5055 2023-06-22 10:47:37.994372 stellar_sdk-8.2.1/stellar_sdk/operation/path_payment_strict_receive.py
+-rw-r--r--   0        0        0     4989 2023-06-22 10:47:37.994478 stellar_sdk-8.2.1/stellar_sdk/operation/path_payment_strict_send.py
+-rw-r--r--   0        0        0     2837 2023-06-22 10:47:37.994576 stellar_sdk-8.2.1/stellar_sdk/operation/payment.py
+-rw-r--r--   0        0        0    23802 2023-06-22 10:47:37.994856 stellar_sdk-8.2.1/stellar_sdk/operation/revoke_sponsorship.py
+-rw-r--r--   0        0        0    10531 2023-06-22 10:47:37.994981 stellar_sdk-8.2.1/stellar_sdk/operation/set_options.py
+-rw-r--r--   0        0        0     4687 2023-06-22 10:47:37.995073 stellar_sdk-8.2.1/stellar_sdk/operation/set_trust_line_flags.py
+-rw-r--r--   0        0        0     8384 2023-06-22 10:47:37.995429 stellar_sdk-8.2.1/stellar_sdk/preconditions.py
+-rw-r--r--   0        0        0     2924 2023-06-22 11:38:32.625912 stellar_sdk-8.2.1/stellar_sdk/price.py
+-rw-r--r--   0        0        0        0 2021-11-23 14:13:01.323130 stellar_sdk-8.2.1/stellar_sdk/py.typed
+-rw-r--r--   0        0        0        0 2021-10-20 03:21:42.923400 stellar_sdk-8.2.1/stellar_sdk/sep/__init__.py
+-rw-r--r--   0        0        0      817 2023-06-22 10:47:37.995617 stellar_sdk-8.2.1/stellar_sdk/sep/ed25519_public_key_signer.py
+-rw-r--r--   0        0        0     1550 2021-10-20 03:21:42.923854 stellar_sdk-8.2.1/stellar_sdk/sep/exceptions.py
+-rw-r--r--   0        0        0     9288 2023-06-22 10:47:37.995745 stellar_sdk-8.2.1/stellar_sdk/sep/federation.py
+-rw-r--r--   0        0        0     3209 2023-06-22 10:47:37.995971 stellar_sdk-8.2.1/stellar_sdk/sep/mnemonic.py
+-rw-r--r--   0        0        0     3143 2023-06-22 10:47:37.996061 stellar_sdk-8.2.1/stellar_sdk/sep/stellar_toml.py
+-rw-r--r--   0        0        0    19500 2023-06-22 10:47:37.996465 stellar_sdk-8.2.1/stellar_sdk/sep/stellar_uri.py
+-rw-r--r--   0        0        0    27755 2023-06-22 10:47:37.996852 stellar_sdk-8.2.1/stellar_sdk/sep/stellar_web_authentication.py
+-rw-r--r--   0        0        0     5025 2023-05-31 08:17:56.157136 stellar_sdk-8.2.1/stellar_sdk/sep/toid.py
+-rw-r--r--   0        0        0    71993 2023-06-22 10:47:37.997252 stellar_sdk-8.2.1/stellar_sdk/sep/txrep.py
+-rw-r--r--   0        0        0    15450 2023-06-22 10:47:37.997508 stellar_sdk-8.2.1/stellar_sdk/server.py
+-rw-r--r--   0        0        0    15574 2023-05-31 08:17:56.158318 stellar_sdk-8.2.1/stellar_sdk/server_async.py
+-rw-r--r--   0        0        0     4124 2023-06-22 10:47:37.997601 stellar_sdk-8.2.1/stellar_sdk/signer.py
+-rw-r--r--   0        0        0    11249 2023-06-22 10:47:37.998034 stellar_sdk-8.2.1/stellar_sdk/signer_key.py
+-rw-r--r--   0        0        0    12279 2023-06-22 10:47:37.998308 stellar_sdk-8.2.1/stellar_sdk/strkey.py
+-rw-r--r--   0        0        0     2568 2023-06-22 10:47:37.998622 stellar_sdk-8.2.1/stellar_sdk/time_bounds.py
+-rw-r--r--   0        0        0    10522 2023-06-22 11:38:26.049155 stellar_sdk-8.2.1/stellar_sdk/transaction.py
+-rw-r--r--   0        0        0    55433 2023-06-22 10:47:37.999332 stellar_sdk-8.2.1/stellar_sdk/transaction_builder.py
+-rw-r--r--   0        0        0     7188 2023-06-22 10:47:37.999642 stellar_sdk-8.2.1/stellar_sdk/transaction_envelope.py
+-rw-r--r--   0        0        0      682 2023-06-22 10:47:37.999909 stellar_sdk-8.2.1/stellar_sdk/type_checked.py
+-rw-r--r--   0        0        0     6028 2023-06-22 10:47:38.000142 stellar_sdk-8.2.1/stellar_sdk/utils.py
+-rw-r--r--   0        0        0    15456 2023-06-22 10:47:38.000715 stellar_sdk-8.2.1/stellar_sdk/xdr/__init__.py
+-rw-r--r--   0        0        0     5998 2023-06-22 10:47:38.001100 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry.py
+-rw-r--r--   0        0        0     2173 2023-06-22 10:47:38.001324 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_ext.py
+-rw-r--r--   0        0        0     2199 2023-06-22 10:47:38.001687 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v1.py
+-rw-r--r--   0        0        0     2239 2023-06-22 10:47:38.001836 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     3775 2023-06-22 10:47:38.001977 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v2.py
+-rw-r--r--   0        0        0     2239 2023-06-22 10:47:38.002214 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v2_ext.py
+-rw-r--r--   0        0        0     2600 2023-06-22 10:47:38.002441 stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v3.py
+-rw-r--r--   0        0        0     1975 2023-06-22 10:47:38.002711 stellar_sdk-8.2.1/stellar_sdk/xdr/account_flags.py
+-rw-r--r--   0        0        0     1435 2023-06-22 10:47:38.003044 stellar_sdk-8.2.1/stellar_sdk/xdr/account_id.py
+-rw-r--r--   0        0        0     2643 2023-06-22 10:47:38.003209 stellar_sdk-8.2.1/stellar_sdk/xdr/account_merge_result.py
+-rw-r--r--   0        0        0     2246 2023-06-22 10:47:38.003310 stellar_sdk-8.2.1/stellar_sdk/xdr/account_merge_result_code.py
+-rw-r--r--   0        0        0     2307 2023-06-22 10:47:38.003707 stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_op.py
+-rw-r--r--   0        0        0     1865 2023-06-22 10:47:38.004054 stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_result.py
+-rw-r--r--   0        0        0     2154 2023-06-22 10:47:38.004454 stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_result_code.py
+-rw-r--r--   0        0        0     1903 2023-06-22 10:47:38.004631 stellar_sdk-8.2.1/stellar_sdk/xdr/alpha_num12.py
+-rw-r--r--   0        0        0     1891 2023-06-22 10:47:38.004781 stellar_sdk-8.2.1/stellar_sdk/xdr/alpha_num4.py
+-rw-r--r--   0        0        0     3284 2023-06-22 10:47:38.004936 stellar_sdk-8.2.1/stellar_sdk/xdr/asset.py
+-rw-r--r--   0        0        0     3133 2023-06-22 10:47:38.005088 stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code.py
+-rw-r--r--   0        0        0     1482 2023-06-22 10:47:38.005213 stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code12.py
+-rw-r--r--   0        0        0     1462 2023-06-22 10:47:38.005307 stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code4.py
+-rw-r--r--   0        0        0     1368 2023-06-22 10:47:38.005433 stellar_sdk-8.2.1/stellar_sdk/xdr/asset_type.py
+-rw-r--r--   0        0        0     1586 2023-06-22 10:47:38.005584 stellar_sdk-8.2.1/stellar_sdk/xdr/auth.py
+-rw-r--r--   0        0        0     2203 2023-06-22 10:47:38.005839 stellar_sdk-8.2.1/stellar_sdk/xdr/auth_cert.py
+-rw-r--r--   0        0        0     2188 2023-06-22 10:47:38.005994 stellar_sdk-8.2.1/stellar_sdk/xdr/authenticated_message.py
+-rw-r--r--   0        0        0     2297 2023-06-22 10:47:38.006255 stellar_sdk-8.2.1/stellar_sdk/xdr/authenticated_message_v0.py
+-rw-r--r--   0        0        0     6074 2023-06-22 10:47:38.006348 stellar_sdk-8.2.1/stellar_sdk/xdr/base.py
+-rw-r--r--   0        0        0     1771 2023-06-22 10:47:38.006502 stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py
+-rw-r--r--   0        0        0     2290 2023-06-22 10:47:38.006660 stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py
+-rw-r--r--   0        0        0     1843 2023-06-22 10:47:38.006787 stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0        0        0     4114 2023-06-22 10:47:38.007055 stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_entry.py
+-rw-r--r--   0        0        0     1529 2023-06-22 10:47:38.007140 stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_entry_type.py
+-rw-r--r--   0        0        0     2165 2023-06-22 10:47:38.007303 stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_metadata.py
+-rw-r--r--   0        0        0     1620 2023-06-22 10:47:38.007497 stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_metadata_ext.py
+-rw-r--r--   0        0        0     1617 2023-06-22 10:47:38.007654 stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_op.py
+-rw-r--r--   0        0        0     1899 2023-06-22 10:47:38.007804 stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_result.py
+-rw-r--r--   0        0        0     1451 2023-06-22 10:47:38.007894 stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_result_code.py
+-rw-r--r--   0        0        0     4223 2023-06-22 10:47:38.008074 stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_asset.py
+-rw-r--r--   0        0        0     1907 2023-06-22 10:47:38.008246 stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_op.py
+-rw-r--r--   0        0        0     1882 2023-06-22 10:47:38.008398 stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_result.py
+-rw-r--r--   0        0        0     2395 2023-06-22 10:47:38.008483 stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_result_code.py
+-rw-r--r--   0        0        0     3812 2023-06-22 10:47:38.008707 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_atom.py
+-rw-r--r--   0        0        0     1327 2023-06-22 10:47:38.008811 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_atom_type.py
+-rw-r--r--   0        0        0     1737 2023-06-22 10:47:38.008966 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_op.py
+-rw-r--r--   0        0        0     2056 2023-06-22 10:47:38.009131 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_result.py
+-rw-r--r--   0        0        0     1795 2023-06-22 10:47:38.009379 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     3197 2023-06-22 10:47:38.009645 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_liquidity_atom.py
+-rw-r--r--   0        0        0     3449 2023-06-22 10:47:38.009915 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_offer_atom.py
+-rw-r--r--   0        0        0     3512 2023-06-22 10:47:38.010076 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_offer_atom_v0.py
+-rw-r--r--   0        0        0     7156 2023-06-22 10:47:38.010220 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_predicate.py
+-rw-r--r--   0        0        0     1604 2023-06-22 10:47:38.010401 stellar_sdk-8.2.1/stellar_sdk/xdr/claim_predicate_type.py
+-rw-r--r--   0        0        0     3858 2023-06-22 10:47:38.010555 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry.py
+-rw-r--r--   0        0        0     2273 2023-06-22 10:47:38.010700 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_ext.py
+-rw-r--r--   0        0        0     2176 2023-06-22 10:47:38.010877 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py
+-rw-r--r--   0        0        0     1728 2023-06-22 10:47:38.011068 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     1388 2023-06-22 10:47:38.011180 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_flags.py
+-rw-r--r--   0        0        0     2220 2023-06-22 10:47:38.011336 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_id.py
+-rw-r--r--   0        0        0     1235 2023-06-22 10:47:38.011425 stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_id_type.py
+-rw-r--r--   0        0        0     2258 2023-06-22 10:47:38.011572 stellar_sdk-8.2.1/stellar_sdk/xdr/claimant.py
+-rw-r--r--   0        0        0     1151 2023-06-22 10:47:38.011657 stellar_sdk-8.2.1/stellar_sdk/xdr/claimant_type.py
+-rw-r--r--   0        0        0     2075 2023-06-22 10:47:38.011804 stellar_sdk-8.2.1/stellar_sdk/xdr/claimant_v0.py
+-rw-r--r--   0        0        0     1758 2023-06-22 10:47:38.012131 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_op.py
+-rw-r--r--   0        0        0     2192 2023-06-22 10:47:38.012285 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_result.py
+-rw-r--r--   0        0        0     1783 2023-06-22 10:47:38.012373 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     2136 2023-06-22 10:47:38.012583 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_op.py
+-rw-r--r--   0        0        0     1827 2023-06-22 10:47:38.012737 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_result.py
+-rw-r--r--   0        0        0     1598 2023-06-22 10:47:38.012911 stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_result_code.py
+-rw-r--r--   0        0        0      847 2023-06-22 10:47:38.013130 stellar_sdk-8.2.1/stellar_sdk/xdr/constants.py
+-rw-r--r--   0        0        0     2123 2023-06-22 10:47:38.013368 stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_op.py
+-rw-r--r--   0        0        0     1916 2023-06-22 10:47:38.013501 stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_result.py
+-rw-r--r--   0        0        0     1857 2023-06-22 10:47:38.013587 stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_result_code.py
+-rw-r--r--   0        0        0     2745 2023-06-22 10:47:38.013724 stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_op.py
+-rw-r--r--   0        0        0     2670 2023-06-22 10:47:38.013867 stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_result.py
+-rw-r--r--   0        0        0     1804 2023-06-22 10:47:38.013937 stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_result_code.py
+-rw-r--r--   0        0        0     2543 2023-06-22 10:47:38.014071 stellar_sdk-8.2.1/stellar_sdk/xdr/create_passive_sell_offer_op.py
+-rw-r--r--   0        0        0     1578 2023-06-22 10:47:38.014288 stellar_sdk-8.2.1/stellar_sdk/xdr/crypto_key_type.py
+-rw-r--r--   0        0        0     1572 2023-06-22 10:47:38.014487 stellar_sdk-8.2.1/stellar_sdk/xdr/curve25519_public.py
+-rw-r--r--   0        0        0     1572 2023-06-22 10:47:38.014698 stellar_sdk-8.2.1/stellar_sdk/xdr/curve25519_secret.py
+-rw-r--r--   0        0        0     2750 2023-06-22 10:47:38.014850 stellar_sdk-8.2.1/stellar_sdk/xdr/data_entry.py
+-rw-r--r--   0        0        0     1590 2023-06-22 10:47:38.014993 stellar_sdk-8.2.1/stellar_sdk/xdr/data_entry_ext.py
+-rw-r--r--   0        0        0     1450 2023-06-22 10:47:38.015117 stellar_sdk-8.2.1/stellar_sdk/xdr/data_value.py
+-rw-r--r--   0        0        0     2004 2023-06-22 10:47:38.015401 stellar_sdk-8.2.1/stellar_sdk/xdr/decorated_signature.py
+-rw-r--r--   0        0        0     1830 2023-06-22 10:47:38.015534 stellar_sdk-8.2.1/stellar_sdk/xdr/dont_have.py
+-rw-r--r--   0        0        0     1392 2023-06-22 10:47:38.015839 stellar_sdk-8.2.1/stellar_sdk/xdr/duration.py
+-rw-r--r--   0        0        0     1527 2023-06-22 10:47:38.015918 stellar_sdk-8.2.1/stellar_sdk/xdr/encrypted_body.py
+-rw-r--r--   0        0        0     2256 2023-06-22 10:47:38.016052 stellar_sdk-8.2.1/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py
+-rw-r--r--   0        0        0     1589 2023-06-22 10:47:38.016127 stellar_sdk-8.2.1/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py
+-rw-r--r--   0        0        0     1642 2023-06-22 10:47:38.016361 stellar_sdk-8.2.1/stellar_sdk/xdr/envelope_type.py
+-rw-r--r--   0        0        0     1750 2023-06-22 10:47:38.016519 stellar_sdk-8.2.1/stellar_sdk/xdr/error.py
+-rw-r--r--   0        0        0     1401 2023-06-22 10:47:38.016615 stellar_sdk-8.2.1/stellar_sdk/xdr/error_code.py
+-rw-r--r--   0        0        0     1595 2023-06-22 10:47:38.016886 stellar_sdk-8.2.1/stellar_sdk/xdr/extension_point.py
+-rw-r--r--   0        0        0     2890 2023-06-22 10:47:38.017041 stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction.py
+-rw-r--r--   0        0        0     2668 2023-06-22 10:47:38.017223 stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_envelope.py
+-rw-r--r--   0        0        0     1644 2023-06-22 10:47:38.017364 stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_ext.py
+-rw-r--r--   0        0        0     2237 2023-06-22 10:47:38.017613 stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py
+-rw-r--r--   0        0        0     1353 2023-06-22 10:47:38.017722 stellar_sdk-8.2.1/stellar_sdk/xdr/hash.py
+-rw-r--r--   0        0        0     3538 2023-06-22 10:47:38.017943 stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage.py
+-rw-r--r--   0        0        0     2399 2023-06-22 10:47:38.018283 stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage_operation_id.py
+-rw-r--r--   0        0        0     3081 2023-06-22 10:47:38.018546 stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage_revoke_id.py
+-rw-r--r--   0        0        0     4324 2023-06-22 10:47:38.018787 stellar_sdk-8.2.1/stellar_sdk/xdr/hello.py
+-rw-r--r--   0        0        0     1551 2023-06-22 10:47:38.019019 stellar_sdk-8.2.1/stellar_sdk/xdr/hmac_sha256_key.py
+-rw-r--r--   0        0        0     1551 2023-06-22 10:47:38.019209 stellar_sdk-8.2.1/stellar_sdk/xdr/hmac_sha256_mac.py
+-rw-r--r--   0        0        0     1964 2023-06-22 10:47:38.019741 stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_payout.py
+-rw-r--r--   0        0        0     2804 2023-06-22 10:47:38.020070 stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_result.py
+-rw-r--r--   0        0        0     1386 2023-06-22 10:47:38.020154 stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_result_code.py
+-rw-r--r--   0        0        0     3356 2023-06-22 10:47:38.020297 stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result.py
+-rw-r--r--   0        0        0     1668 2023-06-22 10:47:38.020446 stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_ext.py
+-rw-r--r--   0        0        0     2231 2023-06-22 10:47:38.020596 stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_pair.py
+-rw-r--r--   0        0        0     6296 2023-06-22 10:47:38.020776 stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_result.py
+-rw-r--r--   0        0        0     1344 2023-06-22 10:47:38.020919 stellar_sdk-8.2.1/stellar_sdk/xdr/int32.py
+-rw-r--r--   0        0        0     1340 2023-06-22 10:47:38.021100 stellar_sdk-8.2.1/stellar_sdk/xdr/int64.py
+-rw-r--r--   0        0        0     1150 2023-06-22 10:47:38.021184 stellar_sdk-8.2.1/stellar_sdk/xdr/ip_addr_type.py
+-rw-r--r--   0        0        0     1948 2023-06-22 10:47:38.021329 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_bounds.py
+-rw-r--r--   0        0        0     2012 2023-06-22 10:47:38.021480 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_meta.py
+-rw-r--r--   0        0        0     5280 2023-06-22 10:47:38.021671 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_meta_v0.py
+-rw-r--r--   0        0        0     2045 2023-06-22 10:47:38.021821 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_value_signature.py
+-rw-r--r--   0        0        0     3105 2023-06-22 10:47:38.021974 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry.py
+-rw-r--r--   0        0        0     4292 2023-06-22 10:47:38.022121 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_change.py
+-rw-r--r--   0        0        0     1541 2023-06-22 10:47:38.022201 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_change_type.py
+-rw-r--r--   0        0        0     2241 2023-06-22 10:47:38.022345 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_changes.py
+-rw-r--r--   0        0        0     5915 2023-06-22 10:47:38.022632 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_data.py
+-rw-r--r--   0        0        0     2162 2023-06-22 10:47:38.022782 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_ext.py
+-rw-r--r--   0        0        0     2198 2023-06-22 10:47:38.022925 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_extension_v1.py
+-rw-r--r--   0        0        0     1668 2023-06-22 10:47:38.023063 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py
+-rw-r--r--   0        0        0     1384 2023-06-22 10:47:38.023148 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_type.py
+-rw-r--r--   0        0        0     7964 2023-06-22 10:47:38.023298 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header.py
+-rw-r--r--   0        0        0     2173 2023-06-22 10:47:38.023440 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_ext.py
+-rw-r--r--   0        0        0     2059 2023-06-22 10:47:38.023582 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_extension_v1.py
+-rw-r--r--   0        0        0     1674 2023-06-22 10:47:38.023729 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_extension_v1_ext.py
+-rw-r--r--   0        0        0     1425 2023-06-22 10:47:38.024600 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_flags.py
+-rw-r--r--   0        0        0     2422 2023-06-22 10:47:38.024870 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_history_entry.py
+-rw-r--r--   0        0        0     1680 2023-06-22 10:47:38.025238 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_history_entry_ext.py
+-rw-r--r--   0        0        0     6398 2023-06-22 10:47:38.025450 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key.py
+-rw-r--r--   0        0        0     1636 2023-06-22 10:47:38.025613 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_account.py
+-rw-r--r--   0        0        0     1736 2023-06-22 10:47:38.025998 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_claimable_balance.py
+-rw-r--r--   0        0        0     1944 2023-06-22 10:47:38.026182 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_data.py
+-rw-r--r--   0        0        0     1740 2023-06-22 10:47:38.026355 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_liquidity_pool.py
+-rw-r--r--   0        0        0     1911 2023-06-22 10:47:38.026569 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_offer.py
+-rw-r--r--   0        0        0     1959 2023-06-22 10:47:38.028265 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_trust_line.py
+-rw-r--r--   0        0        0     2442 2023-06-22 10:47:38.028460 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_scp_messages.py
+-rw-r--r--   0        0        0     5635 2023-06-22 10:47:38.028648 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_upgrade.py
+-rw-r--r--   0        0        0     1501 2023-06-22 10:47:38.029060 stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_upgrade_type.py
+-rw-r--r--   0        0        0     1798 2023-06-22 10:47:38.029243 stellar_sdk-8.2.1/stellar_sdk/xdr/liabilities.py
+-rw-r--r--   0        0        0     2363 2023-06-22 10:47:38.029421 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py
+-rw-r--r--   0        0        0     3239 2023-06-22 10:47:38.029601 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_op.py
+-rw-r--r--   0        0        0     2052 2023-06-22 10:47:38.029783 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_result.py
+-rw-r--r--   0        0        0     2592 2023-06-22 10:47:38.029885 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py
+-rw-r--r--   0        0        0     2675 2023-06-22 10:47:38.030053 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry.py
+-rw-r--r--   0        0        0     3023 2023-06-22 10:47:38.030383 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry_body.py
+-rw-r--r--   0        0        0     3600 2023-06-22 10:47:38.030573 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py
+-rw-r--r--   0        0        0     2666 2023-06-22 10:47:38.030736 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_parameters.py
+-rw-r--r--   0        0        0     1211 2023-06-22 10:47:38.030834 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_type.py
+-rw-r--r--   0        0        0     2869 2023-06-22 10:47:38.030997 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_op.py
+-rw-r--r--   0        0        0     2069 2023-06-22 10:47:38.031178 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_result.py
+-rw-r--r--   0        0        0     2272 2023-06-22 10:47:38.031283 stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py
+-rw-r--r--   0        0        0     2979 2023-06-22 10:47:38.031458 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_op.py
+-rw-r--r--   0        0        0     2450 2023-06-22 10:47:38.031628 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_result.py
+-rw-r--r--   0        0        0     2928 2023-06-22 10:47:38.031722 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_result_code.py
+-rw-r--r--   0        0        0     2153 2023-06-22 10:47:38.031959 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_op.py
+-rw-r--r--   0        0        0     1865 2023-06-22 10:47:38.032138 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_result.py
+-rw-r--r--   0        0        0     1863 2023-06-22 10:47:38.032237 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_result_code.py
+-rw-r--r--   0        0        0     1323 2023-06-22 10:47:38.032335 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_effect.py
+-rw-r--r--   0        0        0     2931 2023-06-22 10:47:38.032515 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_success_result.py
+-rw-r--r--   0        0        0     2790 2023-06-22 10:47:38.032681 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_success_result_offer.py
+-rw-r--r--   0        0        0     2899 2023-06-22 10:47:38.032860 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_op.py
+-rw-r--r--   0        0        0     2467 2023-06-22 10:47:38.033046 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_result.py
+-rw-r--r--   0        0        0     3030 2023-06-22 10:47:38.033216 stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_result_code.py
+-rw-r--r--   0        0        0     4005 2023-06-22 10:47:38.033356 stellar_sdk-8.2.1/stellar_sdk/xdr/memo.py
+-rw-r--r--   0        0        0     1293 2023-06-22 10:47:38.033428 stellar_sdk-8.2.1/stellar_sdk/xdr/memo_type.py
+-rw-r--r--   0        0        0     2023 2023-06-22 10:47:38.033670 stellar_sdk-8.2.1/stellar_sdk/xdr/message_type.py
+-rw-r--r--   0        0        0     3024 2023-06-22 10:47:38.033805 stellar_sdk-8.2.1/stellar_sdk/xdr/muxed_account.py
+-rw-r--r--   0        0        0     1847 2023-06-22 10:47:38.033947 stellar_sdk-8.2.1/stellar_sdk/xdr/muxed_account_med25519.py
+-rw-r--r--   0        0        0     1384 2023-06-22 10:47:38.034160 stellar_sdk-8.2.1/stellar_sdk/xdr/node_id.py
+-rw-r--r--   0        0        0     3951 2023-06-22 10:47:38.034414 stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry.py
+-rw-r--r--   0        0        0     1596 2023-06-22 10:47:38.034563 stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry_ext.py
+-rw-r--r--   0        0        0     1256 2023-06-22 10:47:38.034794 stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry_flags.py
+-rw-r--r--   0        0        0     4571 2023-06-22 10:47:38.034934 stellar_sdk-8.2.1/stellar_sdk/xdr/operation.py
+-rw-r--r--   0        0        0    23123 2023-06-22 10:47:38.035222 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_body.py
+-rw-r--r--   0        0        0     1632 2023-06-22 10:47:38.035364 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_meta.py
+-rw-r--r--   0        0        0     4688 2023-06-22 10:47:38.035513 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result.py
+-rw-r--r--   0        0        0     1842 2023-06-22 10:47:38.035584 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result_code.py
+-rw-r--r--   0        0        0    27203 2023-06-22 10:47:38.035858 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result_tr.py
+-rw-r--r--   0        0        0     2646 2023-06-22 10:47:38.035944 stellar_sdk-8.2.1/stellar_sdk/xdr/operation_type.py
+-rw-r--r--   0        0        0     4041 2023-06-22 10:47:38.036090 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_op.py
+-rw-r--r--   0        0        0     3795 2023-06-22 10:47:38.036237 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result.py
+-rw-r--r--   0        0        0     3327 2023-06-22 10:47:38.036505 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result_code.py
+-rw-r--r--   0        0        0     2505 2023-06-22 10:47:38.036661 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result_success.py
+-rw-r--r--   0        0        0     4054 2023-06-22 10:47:38.036864 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_op.py
+-rw-r--r--   0        0        0     3623 2023-06-22 10:47:38.037120 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result.py
+-rw-r--r--   0        0        0     3217 2023-06-22 10:47:38.037207 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result_code.py
+-rw-r--r--   0        0        0     2487 2023-06-22 10:47:38.037567 stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result_success.py
+-rw-r--r--   0        0        0     2306 2023-06-22 10:47:38.037709 stellar_sdk-8.2.1/stellar_sdk/xdr/payment_op.py
+-rw-r--r--   0        0        0     1810 2023-06-22 10:47:38.037872 stellar_sdk-8.2.1/stellar_sdk/xdr/payment_result.py
+-rw-r--r--   0        0        0     2316 2023-06-22 10:47:38.037966 stellar_sdk-8.2.1/stellar_sdk/xdr/payment_result_code.py
+-rw-r--r--   0        0        0     2323 2023-06-22 10:47:38.038133 stellar_sdk-8.2.1/stellar_sdk/xdr/peer_address.py
+-rw-r--r--   0        0        0     2697 2023-06-22 10:47:38.038294 stellar_sdk-8.2.1/stellar_sdk/xdr/peer_address_ip.py
+-rw-r--r--   0        0        0     2020 2023-06-22 10:47:38.038467 stellar_sdk-8.2.1/stellar_sdk/xdr/peer_stat_list.py
+-rw-r--r--   0        0        0     7616 2023-06-22 10:47:38.038632 stellar_sdk-8.2.1/stellar_sdk/xdr/peer_stats.py
+-rw-r--r--   0        0        0     1358 2023-06-22 10:47:38.038840 stellar_sdk-8.2.1/stellar_sdk/xdr/pool_id.py
+-rw-r--r--   0        0        0     1257 2023-06-22 10:47:38.039069 stellar_sdk-8.2.1/stellar_sdk/xdr/precondition_type.py
+-rw-r--r--   0        0        0     3135 2023-06-22 10:47:38.039210 stellar_sdk-8.2.1/stellar_sdk/xdr/preconditions.py
+-rw-r--r--   0        0        0     5895 2023-06-22 10:47:38.039361 stellar_sdk-8.2.1/stellar_sdk/xdr/preconditions_v2.py
+-rw-r--r--   0        0        0     1652 2023-06-22 10:47:38.039536 stellar_sdk-8.2.1/stellar_sdk/xdr/price.py
+-rw-r--r--   0        0        0     2168 2023-06-22 10:47:38.039681 stellar_sdk-8.2.1/stellar_sdk/xdr/public_key.py
+-rw-r--r--   0        0        0     1186 2023-06-22 10:47:38.039883 stellar_sdk-8.2.1/stellar_sdk/xdr/public_key_type.py
+-rw-r--r--   0        0        0     3281 2023-06-22 10:47:38.040025 stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_op.py
+-rw-r--r--   0        0        0     2058 2023-06-22 10:47:38.040177 stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_op_signer.py
+-rw-r--r--   0        0        0     1984 2023-06-22 10:47:38.040312 stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_result.py
+-rw-r--r--   0        0        0     1847 2023-06-22 10:47:38.040389 stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_result_code.py
+-rw-r--r--   0        0        0     1312 2023-06-22 10:47:38.040480 stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_type.py
+-rw-r--r--   0        0        0     1815 2023-06-22 10:47:38.040619 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_ballot.py
+-rw-r--r--   0        0        0     1939 2023-06-22 10:47:38.040863 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_envelope.py
+-rw-r--r--   0        0        0     2012 2023-06-22 10:47:38.040996 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_history_entry.py
+-rw-r--r--   0        0        0     2709 2023-06-22 10:47:38.041133 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_history_entry_v0.py
+-rw-r--r--   0        0        0     3171 2023-06-22 10:47:38.041271 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_nomination.py
+-rw-r--r--   0        0        0     3250 2023-06-22 10:47:38.041407 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_quorum_set.py
+-rw-r--r--   0        0        0     3468 2023-06-22 10:47:38.041560 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement.py
+-rw-r--r--   0        0        0     2954 2023-06-22 10:47:38.041707 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_confirm.py
+-rw-r--r--   0        0        0     2467 2023-06-22 10:47:38.041992 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_externalize.py
+-rw-r--r--   0        0        0     5360 2023-06-22 10:47:38.042251 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_pledges.py
+-rw-r--r--   0        0        0     3650 2023-06-22 10:47:38.042390 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_prepare.py
+-rw-r--r--   0        0        0     1346 2023-06-22 10:47:38.042463 stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_type.py
+-rw-r--r--   0        0        0     1594 2023-06-22 10:47:38.042589 stellar_sdk-8.2.1/stellar_sdk/xdr/send_more.py
+-rw-r--r--   0        0        0     1499 2023-06-22 10:47:38.042786 stellar_sdk-8.2.1/stellar_sdk/xdr/sequence_number.py
+-rw-r--r--   0        0        0     6199 2023-06-22 10:47:38.042928 stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_op.py
+-rw-r--r--   0        0        0     1865 2023-06-22 10:47:38.043062 stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_result.py
+-rw-r--r--   0        0        0     2584 2023-06-22 10:47:38.043143 stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_result_code.py
+-rw-r--r--   0        0        0     2618 2023-06-22 10:47:38.043278 stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_op.py
+-rw-r--r--   0        0        0     1992 2023-06-22 10:47:38.043596 stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_result.py
+-rw-r--r--   0        0        0     1983 2023-06-22 10:47:38.044400 stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_result_code.py
+-rw-r--r--   0        0        0     1440 2023-06-22 10:47:38.044599 stellar_sdk-8.2.1/stellar_sdk/xdr/signature.py
+-rw-r--r--   0        0        0     1513 2023-06-22 10:47:38.044678 stellar_sdk-8.2.1/stellar_sdk/xdr/signature_hint.py
+-rw-r--r--   0        0        0     2192 2023-06-22 10:47:38.044905 stellar_sdk-8.2.1/stellar_sdk/xdr/signed_survey_request_message.py
+-rw-r--r--   0        0        0     2228 2023-06-22 10:47:38.045037 stellar_sdk-8.2.1/stellar_sdk/xdr/signed_survey_response_message.py
+-rw-r--r--   0        0        0     1793 2023-06-22 10:47:38.045438 stellar_sdk-8.2.1/stellar_sdk/xdr/signer.py
+-rw-r--r--   0        0        0     4930 2023-06-22 10:47:38.045688 stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key.py
+-rw-r--r--   0        0        0     2100 2023-06-22 10:47:38.045878 stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py
+-rw-r--r--   0        0        0     1504 2023-06-22 10:47:38.046110 stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key_type.py
+-rw-r--r--   0        0        0     2256 2023-06-22 10:47:38.046277 stellar_sdk-8.2.1/stellar_sdk/xdr/simple_payment_result.py
+-rw-r--r--   0        0        0     1868 2023-06-22 10:47:38.046686 stellar_sdk-8.2.1/stellar_sdk/xdr/sponsorship_descriptor.py
+-rw-r--r--   0        0        0    13256 2023-06-22 10:47:38.046907 stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_message.py
+-rw-r--r--   0        0        0     3780 2023-06-22 10:47:38.047047 stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value.py
+-rw-r--r--   0        0        0     2671 2023-06-22 10:47:38.047185 stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value_ext.py
+-rw-r--r--   0        0        0     1248 2023-06-22 10:47:38.047263 stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value_type.py
+-rw-r--r--   0        0        0     1405 2023-06-22 10:47:38.047423 stellar_sdk-8.2.1/stellar_sdk/xdr/string32.py
+-rw-r--r--   0        0        0     1405 2023-06-22 10:47:38.047497 stellar_sdk-8.2.1/stellar_sdk/xdr/string64.py
+-rw-r--r--   0        0        0     1221 2023-06-22 10:47:38.047568 stellar_sdk-8.2.1/stellar_sdk/xdr/survey_message_command_type.py
+-rw-r--r--   0        0        0     3354 2023-06-22 10:47:38.047717 stellar_sdk-8.2.1/stellar_sdk/xdr/survey_request_message.py
+-rw-r--r--   0        0        0     2633 2023-06-22 10:47:38.047887 stellar_sdk-8.2.1/stellar_sdk/xdr/survey_response_body.py
+-rw-r--r--   0        0        0     3346 2023-06-22 10:47:38.048079 stellar_sdk-8.2.1/stellar_sdk/xdr/survey_response_message.py
+-rw-r--r--   0        0        0     1350 2023-06-22 10:47:38.048168 stellar_sdk-8.2.1/stellar_sdk/xdr/threshold_indexes.py
+-rw-r--r--   0        0        0     1452 2023-06-22 10:47:38.048385 stellar_sdk-8.2.1/stellar_sdk/xdr/thresholds.py
+-rw-r--r--   0        0        0     1885 2023-06-22 10:47:38.048539 stellar_sdk-8.2.1/stellar_sdk/xdr/time_bounds.py
+-rw-r--r--   0        0        0     1419 2023-06-22 10:47:38.048640 stellar_sdk-8.2.1/stellar_sdk/xdr/time_point.py
+-rw-r--r--   0        0        0     3111 2023-06-22 10:47:38.048883 stellar_sdk-8.2.1/stellar_sdk/xdr/topology_response_body.py
+-rw-r--r--   0        0        0     4356 2023-06-22 10:47:38.049070 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction.py
+-rw-r--r--   0        0        0     3675 2023-06-22 10:47:38.049244 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_envelope.py
+-rw-r--r--   0        0        0     1602 2023-06-22 10:47:38.049412 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_ext.py
+-rw-r--r--   0        0        0     2500 2023-06-22 10:47:38.049591 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_entry.py
+-rw-r--r--   0        0        0     1674 2023-06-22 10:47:38.049776 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_entry_ext.py
+-rw-r--r--   0        0        0     2681 2023-06-22 10:47:38.049956 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_result_entry.py
+-rw-r--r--   0        0        0     1710 2023-06-22 10:47:38.050244 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_result_entry_ext.py
+-rw-r--r--   0        0        0     3762 2023-06-22 10:47:38.050413 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta.py
+-rw-r--r--   0        0        0     2634 2023-06-22 10:47:38.050592 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta_v1.py
+-rw-r--r--   0        0        0     3340 2023-06-22 10:47:38.050780 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta_v2.py
+-rw-r--r--   0        0        0     2874 2023-06-22 10:47:38.051045 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result.py
+-rw-r--r--   0        0        0     2894 2023-06-22 10:47:38.051413 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_code.py
+-rw-r--r--   0        0        0     1638 2023-06-22 10:47:38.051581 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_ext.py
+-rw-r--r--   0        0        0     2650 2023-06-22 10:47:38.051745 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_meta.py
+-rw-r--r--   0        0        0     2122 2023-06-22 10:47:38.052015 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_pair.py
+-rw-r--r--   0        0        0     4972 2023-06-22 10:47:38.052203 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_result.py
+-rw-r--r--   0        0        0     2170 2023-06-22 10:47:38.052477 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_set.py
+-rw-r--r--   0        0        0     2506 2023-06-22 10:47:38.052634 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_set.py
+-rw-r--r--   0        0        0     2646 2023-06-22 10:47:38.052806 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_signature_payload.py
+-rw-r--r--   0        0        0     3202 2023-06-22 10:47:38.052998 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py
+-rw-r--r--   0        0        0     4455 2023-06-22 10:47:38.053287 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0.py
+-rw-r--r--   0        0        0     2607 2023-06-22 10:47:38.053453 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0_envelope.py
+-rw-r--r--   0        0        0     1614 2023-06-22 10:47:38.053611 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0_ext.py
+-rw-r--r--   0        0        0     2596 2023-06-22 10:47:38.053771 stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v1_envelope.py
+-rw-r--r--   0        0        0     4167 2023-06-22 10:47:38.053946 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_asset.py
+-rw-r--r--   0        0        0     3848 2023-06-22 10:47:38.054090 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry.py
+-rw-r--r--   0        0        0     2472 2023-06-22 10:47:38.054231 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_ext.py
+-rw-r--r--   0        0        0     2317 2023-06-22 10:47:38.054374 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_extension_v2.py
+-rw-r--r--   0        0        0     1686 2023-06-22 10:47:38.054507 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py
+-rw-r--r--   0        0        0     2194 2023-06-22 10:47:38.054640 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_v1.py
+-rw-r--r--   0        0        0     2256 2023-06-22 10:47:38.054775 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_v1_ext.py
+-rw-r--r--   0        0        0     1710 2023-06-22 10:47:38.054849 stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_flags.py
+-rw-r--r--   0        0        0     1404 2023-06-22 10:47:38.054936 stellar_sdk-8.2.1/stellar_sdk/xdr/uint256.py
+-rw-r--r--   0        0        0     1394 2023-06-22 10:47:38.055022 stellar_sdk-8.2.1/stellar_sdk/xdr/uint32.py
+-rw-r--r--   0        0        0     1390 2023-06-22 10:47:38.055097 stellar_sdk-8.2.1/stellar_sdk/xdr/uint64.py
+-rw-r--r--   0        0        0     1978 2023-06-22 10:47:38.055235 stellar_sdk-8.2.1/stellar_sdk/xdr/upgrade_entry_meta.py
+-rw-r--r--   0        0        0     1487 2023-06-22 10:47:38.055311 stellar_sdk-8.2.1/stellar_sdk/xdr/upgrade_type.py
+-rw-r--r--   0        0        0     1386 2023-06-22 10:47:38.055393 stellar_sdk-8.2.1/stellar_sdk/xdr/value.py
+-rw-r--r--   0        0        0     5257 2023-06-16 04:23:33.005976 stellar_sdk-8.2.1/stellar_sdk/xdr/xdrlib3.py
+-rw-r--r--   0        0        0     8112 1970-01-01 00:00:00.000000 stellar_sdk-8.2.1/PKG-INFO
```

### Comparing `stellar_sdk-8.2.0/LICENSE` & `stellar_sdk-8.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/README.rst` & `stellar_sdk-8.2.1/README.rst`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/pyproject.toml` & `stellar_sdk-8.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "stellar-sdk"
-version = "8.2.0"
+version = "8.2.1"
 description = "The Python Stellar SDK library provides APIs to build transactions and connect to Horizon."
 authors = [
     "overcat <4catcode@gmail.com>",
     "Eno <appweb.cn@gmail.com>"
 ]
 maintainers = ["overcat <4catcode@gmail.com>"]
 readme = "README.rst"
@@ -49,29 +49,29 @@
 requests = "^2.26.0"
 aiohttp = "^3.8.1"
 aiohttp-sse-client = "^0.2.1"
 stellar-base-sseclient = "^0.0.21"
 mnemonic = "^0.20"
 toml = "^0.10.2"
 typeguard = "^2.13.0"
-urllib3 = "^1.26.7"
+urllib3 = ">=1.26.7,<3.0.0"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.2.2"
-pytest-cov = "^4.0.0"
+pytest = "^7.3.2"
+pytest-cov = "^4.1.0"
 pytest-timeout = "^2.0.1"
-pytest-asyncio = "^0.20.1"
+pytest-asyncio = "^0.21.0"
 pytest-httpserver = "^1.0.6"
 # currently, mypy cannot run in pypy https://github.com/python/typed_ast/issues/111
 mypy = {version = "^1.0", markers = "platform_python_implementation == 'CPython'"}
 types-toml = {version = "^0.10.8", markers = "platform_python_implementation == 'CPython'"}
-types-requests = {version = "^2.28.11", markers = "platform_python_implementation == 'CPython'"}
-autoflake = "^2.0"
+types-requests = {version = "^2.31.0", markers = "platform_python_implementation == 'CPython'"}
+autoflake = "^2.1"
 isort = "^5.10.1"
-black = "^23.1.0"
+black = "^23.3.0"
 
 [tool.poetry.extras]
 docs = ["sphinx", "sphinx-rtd-theme", "sphinx-autodoc-typehints"]
 
 [tool.mypy]
 show_error_codes = true
 ignore_missing_imports = true
```

### Comparing `stellar_sdk-8.2.0/stellar_sdk/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/__version__.py` & `stellar_sdk-8.2.1/stellar_sdk/__version__.py`

 * *Files 11% similar despite different names*

```diff
@@ -7,11 +7,11 @@
  |_____/   |_|  |______|______|______/_/    \_\_|  \_\    |_____/|_____/|_|\_\
 """
 
 __title__ = "stellar-sdk"
 __description__ = "The Python Stellar SDK library provides APIs to build transactions and connect to Horizon."
 __url__ = "https://github.com/StellarCN/py-stellar-base"
 __issues__ = f"{__url__}/issues"
-__version__ = "8.2.0"
+__version__ = "8.2.1"
 __author__ = "Eno, overcat"
 __author_email__ = "appweb.cn@gmail.com, 4catcode@gmail.com"
 __license__ = "Apache License 2.0"
```

### Comparing `stellar_sdk-8.2.0/stellar_sdk/account.py` & `stellar_sdk-8.2.1/stellar_sdk/account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/asset.py` & `stellar_sdk-8.2.1/stellar_sdk/asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/base_server.py` & `stellar_sdk-8.2.1/stellar_sdk/base_server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/base_transaction_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/base_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_accounts_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_assets_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_data_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_effects_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_ledgers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_offers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_operations_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_orderbook_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_payments_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_trades_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/base/base_transactions_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/base/base_transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/base_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/data_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/root_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/root_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_async/transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/accounts_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/assets_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/base_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/claimable_balances_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/data_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/effects_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/fee_stats_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/ledgers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/liquidity_pools_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/offers_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/operations_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/orderbook_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/payments_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/root_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/strict_receive_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/strict_send_paths_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/trades_aggregation_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/trades_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/call_builder/call_builder_sync/transactions_call_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/aiohttp_client.py` & `stellar_sdk-8.2.1/stellar_sdk/client/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/base_async_client.py` & `stellar_sdk-8.2.1/stellar_sdk/client/base_async_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/base_sync_client.py` & `stellar_sdk-8.2.1/stellar_sdk/client/base_sync_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/requests_client.py` & `stellar_sdk-8.2.1/stellar_sdk/client/requests_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,16 +29,16 @@
 @type_checked
 class RequestsClient(BaseSyncClient):
     """The :class:`RequestsClient` object is a synchronous http client,
     which represents the interface for making requests to a server instance.
 
     :param pool_size: persistent connection to Horizon and connection pool
     :param num_retries: configurable request retry functionality
-    :param request_timeout: the timeout for all GET requests
-    :param post_timeout: the timeout for all POST requests
+    :param request_timeout: the timeout for all GET requests (for each retry)
+    :param post_timeout: the timeout for all POST requests (for each retry)
     :param backoff_factor: a backoff factor to apply between attempts after the second try
     :param session: the request session
     :param stream_session: the stream request session
     :param custom_headers: any additional HTTP headers to add in requests
     """
 
     def __init__(
```

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/response.py` & `stellar_sdk-8.2.1/stellar_sdk/client/response.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/client/simple_requests_client.py` & `stellar_sdk-8.2.1/stellar_sdk/client/simple_requests_client.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/decorated_signature.py` & `stellar_sdk-8.2.1/stellar_sdk/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/exceptions.py` & `stellar_sdk-8.2.1/stellar_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/fee_bump_transaction.py` & `stellar_sdk-8.2.1/stellar_sdk/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/fee_bump_transaction_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/helpers.py` & `stellar_sdk-8.2.1/stellar_sdk/helpers.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/keypair.py` & `stellar_sdk-8.2.1/stellar_sdk/keypair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/ledger_bounds.py` & `stellar_sdk-8.2.1/stellar_sdk/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/liquidity_pool_asset.py` & `stellar_sdk-8.2.1/stellar_sdk/liquidity_pool_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/liquidity_pool_id.py` & `stellar_sdk-8.2.1/stellar_sdk/liquidity_pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/memo.py` & `stellar_sdk-8.2.1/stellar_sdk/memo.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/muxed_account.py` & `stellar_sdk-8.2.1/stellar_sdk/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/network.py` & `stellar_sdk-8.2.1/stellar_sdk/network.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/account_merge.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/account_merge.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/allow_trust.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/allow_trust.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/begin_sponsoring_future_reserves.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/begin_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/bump_sequence.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/bump_sequence.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/change_trust.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/change_trust.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/claim_claimable_balance.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/claim_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/clawback.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/clawback.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/clawback_claimable_balance.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/clawback_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/create_account.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/create_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/create_claimable_balance.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/create_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/create_passive_sell_offer.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/create_passive_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/end_sponsoring_future_reserves.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/end_sponsoring_future_reserves.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/inflation.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/inflation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/liquidity_pool_deposit.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/liquidity_pool_deposit.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/liquidity_pool_withdraw.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/liquidity_pool_withdraw.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/manage_buy_offer.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/manage_buy_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/manage_data.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/manage_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/manage_sell_offer.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/manage_sell_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/operation.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/operation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/path_payment_strict_receive.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/path_payment_strict_receive.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/path_payment_strict_send.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/path_payment_strict_send.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/payment.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/payment.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/revoke_sponsorship.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/revoke_sponsorship.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/set_options.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/set_options.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/operation/set_trust_line_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/operation/set_trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/preconditions.py` & `stellar_sdk-8.2.1/stellar_sdk/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/price.py` & `stellar_sdk-8.2.1/stellar_sdk/price.py`

 * *Files 19% similar despite different names*

```diff
@@ -57,14 +57,39 @@
         :param xdr_object: The XDR Price object.
         :return: A new :class:`Price` object from the given XDR Price object.
         """
         n = xdr_object.n.int32
         d = xdr_object.d.int32
         return cls(n, d)
 
-    def __eq__(self, other: object) -> bool:
+    def __lt__(self, other):
         if not isinstance(other, self.__class__):
             return NotImplemented
-        return self.n == other.n and self.d == other.d
+        return (self.n * other.d) < (other.n * self.d)
+
+    def __le__(self, other):
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return (self.n * other.d) <= (other.n * self.d)
+
+    def __eq__(self, other):
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return (self.n * other.d) == (other.n * self.d)
+
+    def __ne__(self, other):
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return (self.n * other.d) != (other.n * self.d)
+
+    def __gt__(self, other):
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return (self.n * other.d) > (other.n * self.d)
+
+    def __ge__(self, other):
+        if not isinstance(other, self.__class__):
+            return NotImplemented
+        return (self.n * other.d) >= (other.n * self.d)
 
     def __str__(self):
         return f"<Price [n={self.n}, d={self.d}]>"
```

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/ed25519_public_key_signer.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/ed25519_public_key_signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/exceptions.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/exceptions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/federation.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/federation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/mnemonic.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/mnemonic.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/stellar_toml.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/stellar_toml.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/stellar_uri.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/stellar_uri.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/stellar_web_authentication.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/stellar_web_authentication.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/toid.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/toid.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/sep/txrep.py` & `stellar_sdk-8.2.1/stellar_sdk/sep/txrep.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/server.py` & `stellar_sdk-8.2.1/stellar_sdk/server.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/server_async.py` & `stellar_sdk-8.2.1/stellar_sdk/server_async.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/signer.py` & `stellar_sdk-8.2.1/stellar_sdk/signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/signer_key.py` & `stellar_sdk-8.2.1/stellar_sdk/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/strkey.py` & `stellar_sdk-8.2.1/stellar_sdk/strkey.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/time_bounds.py` & `stellar_sdk-8.2.1/stellar_sdk/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/transaction.py` & `stellar_sdk-8.2.1/stellar_sdk/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/transaction_builder.py` & `stellar_sdk-8.2.1/stellar_sdk/transaction_builder.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/transaction_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/type_checked.py` & `stellar_sdk-8.2.1/stellar_sdk/type_checked.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/utils.py` & `stellar_sdk-8.2.1/stellar_sdk/utils.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/__init__.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/__init__.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v1_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v2.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v2_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_entry_extension_v3.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_entry_extension_v3.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_merge_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_merge_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/account_merge_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/account_merge_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/allow_trust_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/allow_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/alpha_num12.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/alpha_num12.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/alpha_num4.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/alpha_num4.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/asset.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code12.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code12.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/asset_code4.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/asset_code4.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/asset_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/asset_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/auth.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/auth.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/auth_cert.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/auth_cert.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/authenticated_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/authenticated_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/authenticated_message_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/authenticated_message_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/base.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/base.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/begin_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_entry_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_metadata.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_metadata.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bucket_metadata_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bucket_metadata_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/bump_sequence_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/bump_sequence_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_asset.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/change_trust_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/change_trust_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_atom.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_atom_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_atom_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_claimable_balance_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_liquidity_atom.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_liquidity_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_offer_atom.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_offer_atom.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_offer_atom_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_offer_atom_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_predicate.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_predicate.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claim_predicate_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claim_predicate_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimable_balance_id_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimable_balance_id_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimant.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimant.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimant_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimant_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/claimant_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/claimant_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_claimable_balance_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/clawback_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/clawback_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/constants.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/constants.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_account_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_account_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_claimable_balance_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_claimable_balance_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/create_passive_sell_offer_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/create_passive_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/crypto_key_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/crypto_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/curve25519_public.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/curve25519_public.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/curve25519_secret.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/curve25519_secret.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/data_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/data_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/data_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/data_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/data_value.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/data_value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/decorated_signature.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/decorated_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/dont_have.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/dont_have.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/duration.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/duration.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/encrypted_body.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/encrypted_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/end_sponsoring_future_reserves_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/end_sponsoring_future_reserves_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/envelope_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/envelope_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/error.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/error.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/error_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/error_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/extension_point.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/extension_point.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/fee_bump_transaction_inner_tx.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hash.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hash.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage_operation_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage_operation_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hash_id_preimage_revoke_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hash_id_preimage_revoke_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hello.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hello.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hmac_sha256_key.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hmac_sha256_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/hmac_sha256_mac.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/hmac_sha256_mac.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_payout.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_payout.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inflation_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inflation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_pair.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/inner_transaction_result_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/inner_transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/int32.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/int32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/int64.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/int64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ip_addr_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ip_addr_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_bounds.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_meta.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_meta_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_meta_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_close_value_signature.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_close_value_signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_change.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_change.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_change_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_change_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_changes.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_changes.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_data.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_extension_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_entry_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_entry_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_extension_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_extension_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_extension_v1_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_extension_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_history_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_header_history_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_header_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_account.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_claimable_balance.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_claimable_balance.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_data.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_data.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_liquidity_pool.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_liquidity_pool.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_offer.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_key_trust_line.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_key_trust_line.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_scp_messages.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_scp_messages.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_upgrade.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_upgrade.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/ledger_upgrade_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/ledger_upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liabilities.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liabilities.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_constant_product_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_deposit_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry_body.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_entry_constant_product.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_parameters.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_parameters.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/liquidity_pool_withdraw_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_buy_offer_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_buy_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_data_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_data_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_effect.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_effect.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_success_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_success_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_offer_success_result_offer.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_offer_success_result_offer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/manage_sell_offer_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/manage_sell_offer_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/memo.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/memo.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/memo_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/memo_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/message_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/message_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/muxed_account.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/muxed_account.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/muxed_account_med25519.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/muxed_account_med25519.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/node_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/node_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/offer_entry_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/offer_entry_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_body.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_meta.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_result_tr.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_result_tr.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/operation_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/operation_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_receive_result_success.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_receive_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/path_payment_strict_send_result_success.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/path_payment_strict_send_result_success.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/payment_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/payment_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/payment_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/payment_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/payment_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/peer_address.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/peer_address.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/peer_address_ip.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/peer_address_ip.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/peer_stat_list.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/peer_stat_list.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/peer_stats.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/peer_stats.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/pool_id.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/pool_id.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/precondition_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/precondition_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/preconditions.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/preconditions.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/preconditions_v2.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/preconditions_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/price.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/price.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/public_key.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/public_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/public_key_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/public_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_op_signer.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_op_signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/revoke_sponsorship_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/revoke_sponsorship_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_ballot.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_ballot.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_history_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_history_entry_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_history_entry_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_nomination.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_nomination.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_quorum_set.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_quorum_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_confirm.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_confirm.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_externalize.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_externalize.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_pledges.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_pledges.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_prepare.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_prepare.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/scp_statement_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/scp_statement_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/send_more.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/send_more.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/sequence_number.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/sequence_number.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_options_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_options_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_op.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_op.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/set_trust_line_flags_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/set_trust_line_flags_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signature.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signature.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signature_hint.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signature_hint.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signed_survey_request_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signed_survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signed_survey_response_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signed_survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signer.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signer.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key_ed25519_signed_payload.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/signer_key_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/signer_key_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/simple_payment_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/simple_payment_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/sponsorship_descriptor.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/sponsorship_descriptor.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/stellar_value_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/stellar_value_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/string32.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/string32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/string64.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/string64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/survey_message_command_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/survey_message_command_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/survey_request_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/survey_request_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/survey_response_body.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/survey_response_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/survey_response_message.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/survey_response_message.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/threshold_indexes.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/threshold_indexes.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/thresholds.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/thresholds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/time_bounds.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/time_bounds.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/time_point.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/time_point.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/topology_response_body.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/topology_response_body.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_result_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_result_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_history_result_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_history_result_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_meta_v2.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_meta_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_code.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_code.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_meta.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_pair.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_pair.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_result.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_result.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_result_set.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_result_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_set.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_set.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_signature_payload.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_signature_payload.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_signature_payload_tagged_transaction.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v0_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v0_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/transaction_v1_envelope.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/transaction_v1_envelope.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_asset.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_asset.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_extension_v2.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_extension_v2.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_extension_v2_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_v1.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_v1.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_entry_v1_ext.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_entry_v1_ext.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/trust_line_flags.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/trust_line_flags.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/uint256.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/uint256.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/uint32.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/uint32.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/uint64.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/uint64.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/upgrade_entry_meta.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/upgrade_entry_meta.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/upgrade_type.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/upgrade_type.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/stellar_sdk/xdr/value.py` & `stellar_sdk-8.2.1/stellar_sdk/xdr/value.py`

 * *Files identical despite different names*

### Comparing `stellar_sdk-8.2.0/PKG-INFO` & `stellar_sdk-8.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stellar-sdk
-Version: 8.2.0
+Version: 8.2.1
 Summary: The Python Stellar SDK library provides APIs to build transactions and connect to Horizon.
 Home-page: https://github.com/StellarCN/py-stellar-base
 License: Apache-2.0
 Keywords: stellar-sdk,stellar,stellar.org,lumens,xlm,blockchain,distributed exchange,cryptocurrency,dex,horizon,sdex,trading
 Author: overcat
 Author-email: 4catcode@gmail.com
 Maintainer: overcat
@@ -32,15 +32,15 @@
 Requires-Dist: aiohttp (>=3.8.1,<4.0.0)
 Requires-Dist: aiohttp-sse-client (>=0.2.1,<0.3.0)
 Requires-Dist: mnemonic (>=0.20,<0.21)
 Requires-Dist: requests (>=2.26.0,<3.0.0)
 Requires-Dist: stellar-base-sseclient (>=0.0.21,<0.0.22)
 Requires-Dist: toml (>=0.10.2,<0.11.0)
 Requires-Dist: typeguard (>=2.13.0,<3.0.0)
-Requires-Dist: urllib3 (>=1.26.7,<2.0.0)
+Requires-Dist: urllib3 (>=1.26.7,<3.0.0)
 Project-URL: Bug Tracker, https://github.com/StellarCN/py-stellar-base/issues
 Project-URL: Documentation, https://stellar-sdk.readthedocs.io/
 Project-URL: Repository, https://github.com/StellarCN/py-stellar-base
 Description-Content-Type: text/x-rst
 
 Stellar Python SDK
 ==================
```

