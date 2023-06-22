# Comparing `tmp/stripe-5.5.0b4.tar.gz` & `tmp/stripe-5.5.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "stripe-5.5.0b4.tar", last modified: Fri Jun  2 18:36:55 2023, max compression
+gzip compressed data, was "stripe-5.5.0b5.tar", last modified: Thu Jun 22 20:53:39 2023, max compression
```

## Comparing `stripe-5.5.0b4.tar` & `stripe-5.5.0b5.tar`

### file list

```diff
@@ -1,333 +1,334 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.739111 stripe-5.5.0b4/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-02 18:36:33.000000 stripe-5.5.0b4/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-02 18:36:33.000000 stripe-5.5.0b4/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)    47974 2023-06-02 18:36:33.000000 stripe-5.5.0b4/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-02 18:36:33.000000 stripe-5.5.0b4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-02 18:36:33.000000 stripe-5.5.0b4/LONG_DESCRIPTION.rst
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-02 18:36:33.000000 stripe-5.5.0b4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 18:36:55.739111 stripe-5.5.0b4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8951 2023-06-02 18:36:33.000000 stripe-5.5.0b4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-02 18:36:33.000000 stripe-5.5.0b4/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.659109 stripe-5.5.0b4/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/charge.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/proxy.py
--rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-02 18:36:33.000000 stripe-5.5.0b4/examples/webhooks.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-02 18:36:33.000000 stripe-5.5.0b4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-02 18:36:55.739111 stripe-5.5.0b4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-02 18:36:33.000000 stripe-5.5.0b4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.663109 stripe-5.5.0b4/stripe/
--rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_requestor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.687110 stripe-5.5.0b4/stripe/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)     4750 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.687110 stripe-5.5.0b4/stripe/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/updateable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/abstract/verify_mixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/account_session.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/application_fee_refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/apps/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apps/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/apps/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/bank_account.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/billing_portal/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capability.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/capital/
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_offer.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/capital/financing_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/cash_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/charge.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.691110 stripe-5.5.0b4/stripe/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/checkout/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/credit_note_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/customer_cash_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/error_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/event.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/file_link.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/financial_connections/
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account.py
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account_owner.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/account_ownership.py
--rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/inferred_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/financial_connections/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/funding_instructions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/gift_cards/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/gift_cards/transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.695110 stripe-5.5.0b4/stripe/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/identity/verification_session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7996 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/invoice_line_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/card_design.py
--rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/issuing/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/login_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/order.py
--rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/person.py
--rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/price.py
--rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/product.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/quote_phase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/radar/value_list_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/recipient_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/refund.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reporting/report_type.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/review.py
--rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/shipping_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.699110 stripe-5.5.0b4/stripe/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/sigma/scheduled_query_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/source.py
--rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/subscription_schedule.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/tax/
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/registration.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/tax_rate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/location.py
--rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/terminal/reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.703110 stripe-5.5.0b4/stripe/api_resources/test_helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/test_helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/test_helpers/test_clock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/token.py
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.707110 stripe-5.5.0b4/stripe/api_resources/treasury/
--rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/credit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/debit_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/financial_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/inbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/outbound_payment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/outbound_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/received_credit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/received_debit.py
--rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/treasury/transaction_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_resources/webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/api_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.707110 stripe-5.5.0b4/stripe/data/
--rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/data/ca-certificates.crt
--rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/error.py
--rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     9432 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/object_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/request_metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/six.py
--rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/util.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-02 18:36:33.000000 stripe-5.5.0b4/stripe/webhook.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.667110 stripe-5.5.0b4/stripe.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11521 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-02 18:36:55.000000 stripe-5.5.0b4/stripe.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.711110 stripe-5.5.0b4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.727110 stripe-5.5.0b4/tests/api_resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_createable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_custom_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_deletable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_listable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_nested_resource_class_methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_searchable_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_singleton_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_test_helpers_api_resource.py
--rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/abstract/test_updateable_api_resource.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/billing_portal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/test_configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/billing_portal/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/checkout/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/checkout/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/checkout/test_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.731110 stripe-5.5.0b4/tests/api_resources/identity/
--rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/identity/test_verification_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/identity/test_verification_session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/issuing/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_authorization.py
--rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_cardholder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/issuing/test_transaction.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/radar/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_early_fraud_warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_value_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/radar/test_value_list_item.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/reporting/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/test_report_run.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/reporting/test_report_type.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.735111 stripe-5.5.0b4/tests/api_resources/sigma/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/sigma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/sigma/test_scheduled_query_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:55.739111 stripe-5.5.0b4/tests/api_resources/terminal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_connection_token.py
--rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_location.py
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/terminal/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_account_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_apple_pay_domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_application_fee.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_application_fee_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_balance.py
--rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_bank_account.py
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_capability.py
--rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_card.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_charge.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_country_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_coupon.py
--rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_credit_note.py
--rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_customer.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_customer_balance_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_dispute.py
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_ephemeral_key.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_exchange_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_file_upload.py
--rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice.py
--rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice_item.py
--rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_invoice_line_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_list_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_mandate.py
--rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payment_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payment_method.py
--rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_payout.py
--rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_person.py
--rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_plan.py
--rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_price.py
--rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_product.py
--rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_promotion_code.py
--rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_quote.py
--rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_refund.py
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_reversal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_review.py
--rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_search_result_object.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_setup_attempt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_setup_intent.py
--rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_source_transaction.py
--rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription.py
--rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_subscription_schedule.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_code.py
--rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_id.py
--rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_tax_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_topup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_transfer.py
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_usage_record.py
--rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_usage_record_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/api_resources/test_webhook_endpoint.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/request_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/stripe_mock.py
--rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_api_requestor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_error.py
--rw-r--r--   0 runner    (1001) docker     (123)   103511 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_generated_examples.py
--rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_multipart_data_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_oauth.py
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_oauth_error.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_preview.py
--rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_raw_request.py
--rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_stripe_object.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_stripe_response.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tests/test_webhook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-02 18:36:33.000000 stripe-5.5.0b4/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-22 20:53:19.000000 stripe-5.5.0b5/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)      361 2023-06-22 20:53:19.000000 stripe-5.5.0b5/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)    48386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-06-22 20:53:19.000000 stripe-5.5.0b5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-06-22 20:53:19.000000 stripe-5.5.0b5/LONG_DESCRIPTION.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-06-22 20:53:19.000000 stripe-5.5.0b5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-22 20:53:39.450146 stripe-5.5.0b5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9253 2023-06-22 20:53:19.000000 stripe-5.5.0b5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-22 20:53:19.000000 stripe-5.5.0b5/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.418146 stripe-5.5.0b5/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/proxy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      989 2023-06-22 20:53:19.000000 stripe-5.5.0b5/examples/webhooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-06-22 20:53:19.000000 stripe-5.5.0b5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-06-22 20:53:39.450146 stripe-5.5.0b5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2371 2023-06-22 20:53:19.000000 stripe-5.5.0b5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.422146 stripe-5.5.0b5/stripe/
+-rw-r--r--   0 runner    (1001) docker     (123)     1637 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15936 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_requestor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     4816 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)     1080 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5747 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4274 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2553 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1060 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/updateable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/abstract/verify_mixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5032 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/account_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1316 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/application_fee_refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/apps/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apps/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/apps/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3100 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/bank_account.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      579 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/billing_portal/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1391 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capability.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/capital/
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1402 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_offer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/capital/financing_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/cash_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2654 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/charge.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.430146 stripe-5.5.0b5/stripe/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)      203 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2998 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/checkout/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/credit_note_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7918 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1564 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_cash_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/customer_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2019 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/error_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2122 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/event.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2088 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      675 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/file_link.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/financial_connections/
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5215 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account_owner.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/account_ownership.py
+-rw-r--r--   0 runner    (1001) docker     (123)      499 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/inferred_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/financial_connections/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/funding_instructions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/gift_cards/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      980 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2748 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/gift_cards/transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1134 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/identity/verification_session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8011 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1686 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/invoice_line_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2640 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4918 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2937 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/card_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)      718 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1636 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/issuing/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      266 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4503 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/login_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3933 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/order.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6997 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2770 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1931 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1669 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/product.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12693 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1346 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/quote_phase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      696 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/radar/value_list_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/recipient_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2767 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/refund.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)      275 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reporting/report_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2556 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5029 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      735 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/shipping_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/sigma/scheduled_query_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3731 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      516 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4063 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3421 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/subscription_schedule.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.434146 stripe-5.5.0b5/stripe/api_resources/tax/
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      996 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/registration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2213 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1169 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)      825 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/tax_rate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      668 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9450 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/terminal/reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/test_helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/test_helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1879 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/test_helpers/test_clock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1262 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/api_resources/treasury/
+-rw-r--r--   0 runner    (1001) docker     (123)      880 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/credit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      604 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/debit_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/financial_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4940 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/inbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/outbound_payment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5478 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/outbound_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1172 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/received_credit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/received_debit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      409 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/treasury/transaction_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1350 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      258 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_resources/webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/api_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.438146 stripe-5.5.0b5/stripe/data/
+-rw-r--r--   0 runner    (1001) docker     (123)   215352 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/data/ca-certificates.crt
+-rw-r--r--   0 runner    (1001) docker     (123)     4284 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25754 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1022 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9510 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/object_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1878 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/request_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34581 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/six.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13407 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      963 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7811 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-06-22 20:53:19.000000 stripe-5.5.0b5/stripe/webhook.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.422146 stripe-5.5.0b5/stripe.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2466 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11562 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-22 20:53:39.000000 stripe-5.5.0b5/stripe.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.442146 stripe-5.5.0b5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.446146 stripe-5.5.0b5/tests/api_resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_createable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10208 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_custom_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_deletable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_listable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2798 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_nested_resource_class_methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3046 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_searchable_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_singleton_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2351 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_test_helpers_api_resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10616 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/abstract/test_updateable_api_resource.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/billing_portal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1810 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/test_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/billing_portal/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/checkout/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/checkout/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/checkout/test_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/identity/
+-rw-r--r--   0 runner    (1001) docker     (123)      864 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/identity/test_verification_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3701 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/identity/test_verification_session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/issuing/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_authorization.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1660 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_cardholder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1515 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/issuing/test_transaction.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/radar/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      778 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_early_fraud_warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_value_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/radar/test_value_list_item.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/reporting/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/test_report_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      760 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/reporting/test_report_type.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/sigma/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/sigma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/sigma/test_scheduled_query_run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:39.450146 stripe-5.5.0b5/tests/api_resources/terminal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_connection_token.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2549 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/terminal/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10097 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      517 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_account_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1538 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_apple_pay_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2028 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_application_fee.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_application_fee_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_balance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      745 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2273 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_bank_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_capability.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1877 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_card.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_charge.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_country_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_coupon.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2483 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_credit_note.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8370 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_customer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_customer_balance_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_dispute.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_ephemeral_key.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_exchange_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2730 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1503 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_file_upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5696 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2146 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)      376 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_invoice_line_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9820 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_list_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_mandate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3685 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payment_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payment_method.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2645 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_payout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1231 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_person.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2077 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_plan.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1604 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_price.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_product.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1594 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_promotion_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5849 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_quote.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1466 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_refund.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_reversal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1239 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_review.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6597 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_search_result_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_setup_attempt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2951 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_setup_intent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2699 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_source_transaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2659 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3357 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_subscription_schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)      669 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_code.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_id.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1548 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_tax_rate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2202 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_topup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3054 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_transfer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      875 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_usage_record.py
+-rw-r--r--   0 runner    (1001) docker     (123)      576 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_usage_record_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2317 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/api_resources/test_webhook_endpoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7389 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/request_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1976 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/stripe_mock.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25609 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_api_requestor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3142 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)   116386 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_generated_examples.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34161 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9928 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_multipart_data_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_oauth.py
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_oauth_error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_preview.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5161 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_raw_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11502 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_stripe_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_stripe_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4869 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tests/test_webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2211 2023-06-22 20:53:19.000000 stripe-5.5.0b5/tox.ini
```

### Comparing `stripe-5.5.0b4/CHANGELOG.md` & `stripe-5.5.0b5/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 # Changelog
 
+## 5.5.0b5 - 2023-06-22
+* [#982](https://github.com/stripe/stripe-python/pull/982) Update generated code for beta
+  * Add support for new resource `CustomerSession`
+  * Add support for `create` method on resource `CustomerSession`
+* [#979](https://github.com/stripe/stripe-python/pull/979) Update generated code for beta
+* [#976](https://github.com/stripe/stripe-python/pull/976) Update generated code for beta
+
 ## 5.5.0b4 - 2023-06-02
 * [#973](https://github.com/stripe/stripe-python/pull/973) Update generated code for beta
 * [#969](https://github.com/stripe/stripe-python/pull/969) Update generated code for beta
 * [#971](https://github.com/stripe/stripe-python/pull/971) Handle developer message in preview error responses
 
 ## 5.5.0b3 - 2023-05-19
 * [#966](https://github.com/stripe/stripe-python/pull/966) Update generated code for beta
```

### Comparing `stripe-5.5.0b4/LICENSE` & `stripe-5.5.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/LONG_DESCRIPTION.rst` & `stripe-5.5.0b5/LONG_DESCRIPTION.rst`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/PKG-INFO` & `stripe-5.5.0b5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b4
+Version: 5.5.0b5
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b4/README.md` & `stripe-5.5.0b5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -156,14 +156,27 @@
 
     ```python
     import logging
     logging.basicConfig()
     logging.getLogger('stripe').setLevel(logging.DEBUG)
     ```
 
+### Accessing response code and headers
+
+You can access the HTTP response code and headers using the `last_response` property of the returned resource. 
+
+```python
+customer = stripe.Customer.retrieve(
+    "cus_123456789"
+)
+
+print(customer.last_response.code)
+print(customer.last_response.headers)
+```
+
 ### Writing a Plugin
 
 If you're writing a plugin that uses the library, we'd appreciate it if you
 identified using `stripe.set_app_info()`:
 
 ```py
 stripe.set_app_info("MyAwesomePlugin", version="1.2.34", url="https://myawesomeplugin.info")
```

### Comparing `stripe-5.5.0b4/examples/oauth.py` & `stripe-5.5.0b5/examples/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/examples/proxy.py` & `stripe-5.5.0b5/examples/proxy.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/examples/webhooks.py` & `stripe-5.5.0b5/examples/webhooks.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/setup.py` & `stripe-5.5.0b5/setup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/__init__.py` & `stripe-5.5.0b5/stripe/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_requestor.py` & `stripe-5.5.0b5/stripe/api_requestor.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/__init__.py` & `stripe-5.5.0b5/stripe/api_resources/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,14 +44,15 @@
 from stripe.api_resources.customer import Customer
 from stripe.api_resources.customer_balance_transaction import (
     CustomerBalanceTransaction,
 )
 from stripe.api_resources.customer_cash_balance_transaction import (
     CustomerCashBalanceTransaction,
 )
+from stripe.api_resources.customer_session import CustomerSession
 from stripe.api_resources.dispute import Dispute
 from stripe.api_resources.ephemeral_key import EphemeralKey
 from stripe.api_resources.event import Event
 from stripe.api_resources.exchange_rate import ExchangeRate
 from stripe.api_resources.file import File
 from stripe.api_resources.file import FileUpload
 from stripe.api_resources.file_link import FileLink
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/__init__.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/createable_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/custom_method.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/deletable_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/listable_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/nested_resource_class_methods.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/searchable_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/singleton_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/test_helpers.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/test_helpers.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/abstract/updateable_api_resource.py` & `stripe-5.5.0b5/stripe/api_resources/abstract/updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/account.py` & `stripe-5.5.0b5/stripe/api_resources/account.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -10,23 +10,23 @@
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
 from stripe.api_resources.abstract import nested_resource_class_methods
 from stripe.six.moves.urllib.parse import quote_plus
 
 
 @nested_resource_class_methods(
-    "external_account",
-    operations=["create", "retrieve", "update", "delete", "list"],
-)
-@nested_resource_class_methods(
     "capability",
     operations=["retrieve", "update", "list"],
     resource_plural="capabilities",
 )
 @nested_resource_class_methods(
+    "external_account",
+    operations=["create", "retrieve", "update", "delete", "list"],
+)
+@nested_resource_class_methods(
     "login_link",
     operations=["create"],
 )
 @nested_resource_class_methods(
     "person",
     operations=["create", "retrieve", "update", "delete", "list"],
 )
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/account_link.py` & `stripe-5.5.0b5/stripe/api_resources/account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/account_session.py` & `stripe-5.5.0b5/stripe/api_resources/account_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/apple_pay_domain.py` & `stripe-5.5.0b5/stripe/api_resources/apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/application_fee.py` & `stripe-5.5.0b5/stripe/api_resources/application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/application_fee_refund.py` & `stripe-5.5.0b5/stripe/api_resources/application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/apps/secret.py` & `stripe-5.5.0b5/stripe/api_resources/apps/secret.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/balance.py` & `stripe-5.5.0b5/stripe/api_resources/balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/balance_transaction.py` & `stripe-5.5.0b5/stripe/api_resources/balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/bank_account.py` & `stripe-5.5.0b5/stripe/api_resources/bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/billing_portal/configuration.py` & `stripe-5.5.0b5/stripe/api_resources/billing_portal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/billing_portal/session.py` & `stripe-5.5.0b5/stripe/api_resources/billing_portal/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/capability.py` & `stripe-5.5.0b5/stripe/api_resources/capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/capital/financing_offer.py` & `stripe-5.5.0b5/stripe/api_resources/capital/financing_offer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/capital/financing_summary.py` & `stripe-5.5.0b5/stripe/api_resources/capital/financing_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/card.py` & `stripe-5.5.0b5/stripe/api_resources/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/cash_balance.py` & `stripe-5.5.0b5/stripe/api_resources/cash_balance.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/charge.py` & `stripe-5.5.0b5/stripe/api_resources/charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/checkout/session.py` & `stripe-5.5.0b5/stripe/api_resources/checkout/session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/country_spec.py` & `stripe-5.5.0b5/stripe/api_resources/country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/coupon.py` & `stripe-5.5.0b5/stripe/api_resources/coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/credit_note.py` & `stripe-5.5.0b5/stripe/api_resources/credit_note.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,21 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 
 from stripe import util
 from stripe.api_resources.abstract import CreateableAPIResource
 from stripe.api_resources.abstract import ListableAPIResource
 from stripe.api_resources.abstract import UpdateableAPIResource
+from stripe.api_resources.abstract import nested_resource_class_methods
 
 
+@nested_resource_class_methods(
+    "line",
+    operations=["list"],
+)
 class CreditNote(
     CreateableAPIResource,
     ListableAPIResource,
     UpdateableAPIResource,
 ):
     """
     Issue a credit note to adjust an invoice's amount after the invoice is finalized.
@@ -31,14 +36,27 @@
             api_key=api_key,
             stripe_version=stripe_version,
             stripe_account=stripe_account,
             params=params,
         )
 
     @classmethod
+    def preview_lines(
+        cls, api_key=None, stripe_version=None, stripe_account=None, **params
+    ):
+        return cls._static_request(
+            "get",
+            "/v1/credit_notes/preview/lines",
+            api_key=api_key,
+            stripe_version=stripe_version,
+            stripe_account=stripe_account,
+            params=params,
+        )
+
+    @classmethod
     def _cls_void_credit_note(
         cls,
         id,
         api_key=None,
         stripe_version=None,
         stripe_account=None,
         **params
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/customer.py` & `stripe-5.5.0b5/stripe/api_resources/customer.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 from stripe.api_resources.abstract import UpdateableAPIResource
 from stripe.api_resources.abstract import nested_resource_class_methods
 from stripe.api_resources.abstract import test_helpers
 
 
 @test_helpers
 @nested_resource_class_methods(
-    "source",
-    operations=["create", "retrieve", "update", "delete", "list"],
-)
-@nested_resource_class_methods(
     "balance_transaction",
     operations=["create", "retrieve", "update", "list"],
 )
 @nested_resource_class_methods(
     "cash_balance_transaction",
     operations=["retrieve", "list"],
 )
 @nested_resource_class_methods(
+    "source",
+    operations=["create", "retrieve", "update", "delete", "list"],
+)
+@nested_resource_class_methods(
     "tax_id",
     operations=["create", "retrieve", "delete", "list"],
 )
 class Customer(
     CreateableAPIResource,
     DeletableAPIResource,
     ListableAPIResource,
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/customer_balance_transaction.py` & `stripe-5.5.0b5/stripe/api_resources/customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/customer_cash_balance_transaction.py` & `stripe-5.5.0b5/stripe/api_resources/customer_cash_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/dispute.py` & `stripe-5.5.0b5/stripe/api_resources/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/ephemeral_key.py` & `stripe-5.5.0b5/stripe/api_resources/ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/error_object.py` & `stripe-5.5.0b5/stripe/api_resources/error_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/event.py` & `stripe-5.5.0b5/stripe/api_resources/event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/exchange_rate.py` & `stripe-5.5.0b5/stripe/api_resources/exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/file.py` & `stripe-5.5.0b5/stripe/api_resources/file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/file_link.py` & `stripe-5.5.0b5/stripe/api_resources/file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/financial_connections/__init__.py` & `stripe-5.5.0b5/stripe/api_resources/financial_connections/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/financial_connections/account.py` & `stripe-5.5.0b5/stripe/api_resources/financial_connections/account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/funding_instructions.py` & `stripe-5.5.0b5/stripe/api_resources/funding_instructions.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/gift_cards/card.py` & `stripe-5.5.0b5/stripe/api_resources/gift_cards/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/gift_cards/transaction.py` & `stripe-5.5.0b5/stripe/api_resources/gift_cards/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/identity/verification_report.py` & `stripe-5.5.0b5/stripe/api_resources/identity/verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/identity/verification_session.py` & `stripe-5.5.0b5/stripe/api_resources/identity/verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/invoice.py` & `stripe-5.5.0b5/stripe/api_resources/invoice.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 
     They contain [invoice items](https://stripe.com/docs/api#invoiceitems), and proration adjustments
     that may be caused by subscription upgrades/downgrades (if necessary).
 
     If your invoice is configured to be billed through automatic charges,
     Stripe automatically finalizes your invoice and attempts payment. Note
     that finalizing the invoice,
-    [when automatic](https://stripe.com/docs/billing/invoices/workflow/#auto_advance), does
+    [when automatic](https://stripe.com/docs/invoicing/integration/automatic-advancement-collection), does
     not happen immediately as the invoice is created. Stripe waits
     until one hour after the last webhook was successfully sent (or the last
     webhook timed out after failing). If you (and the platforms you may have
     connected to) have no webhooks configured, Stripe waits one hour after
     creation to finalize the invoice.
 
     If your invoice is configured to be billed by sending an email, then based on your
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/invoice_item.py` & `stripe-5.5.0b5/stripe/api_resources/invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/__init__.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/authorization.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/card.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/card_design.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/card_design.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/cardholder.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/dispute.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/issuing/transaction.py` & `stripe-5.5.0b5/stripe/api_resources/issuing/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/list_object.py` & `stripe-5.5.0b5/stripe/api_resources/list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/order.py` & `stripe-5.5.0b5/stripe/api_resources/order.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/payment_intent.py` & `stripe-5.5.0b5/stripe/api_resources/payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/payment_link.py` & `stripe-5.5.0b5/stripe/api_resources/payment_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/payment_method.py` & `stripe-5.5.0b5/stripe/api_resources/payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/payout.py` & `stripe-5.5.0b5/stripe/api_resources/payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/person.py` & `stripe-5.5.0b5/stripe/api_resources/person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/plan.py` & `stripe-5.5.0b5/stripe/api_resources/plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/price.py` & `stripe-5.5.0b5/stripe/api_resources/price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/product.py` & `stripe-5.5.0b5/stripe/api_resources/product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/promotion_code.py` & `stripe-5.5.0b5/stripe/api_resources/promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/quote.py` & `stripe-5.5.0b5/stripe/api_resources/quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/quote_phase.py` & `stripe-5.5.0b5/stripe/api_resources/quote_phase.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/radar/early_fraud_warning.py` & `stripe-5.5.0b5/stripe/api_resources/radar/early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/radar/value_list.py` & `stripe-5.5.0b5/stripe/api_resources/radar/value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/radar/value_list_item.py` & `stripe-5.5.0b5/stripe/api_resources/radar/value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/refund.py` & `stripe-5.5.0b5/stripe/api_resources/refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/reporting/report_run.py` & `stripe-5.5.0b5/stripe/api_resources/reporting/report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/reporting/report_type.py` & `stripe-5.5.0b5/stripe/api_resources/reporting/report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/reversal.py` & `stripe-5.5.0b5/stripe/api_resources/reversal.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,19 +14,19 @@
     connected account, either entirely or partially, and can also specify whether
     to refund any related application fees. Transfer reversals add to the
     platform's balance and subtract from the destination account's balance.
 
     Reversing a transfer that was made for a [destination
     charge](https://stripe.com/docs/connect/destination-charges) is allowed only up to the amount of
     the charge. It is possible to reverse a
-    [transfer_group](https://stripe.com/docs/connect/charges-transfers#transfer-options)
+    [transfer_group](https://stripe.com/docs/connect/separate-charges-and-transfers#transfer-options)
     transfer only if the destination account has enough balance to cover the
     reversal.
 
-    Related guide: [Reversing transfers](https://stripe.com/docs/connect/charges-transfers#reversing-transfers)
+    Related guide: [Reversing transfers](https://stripe.com/docs/connect/separate-charges-and-transfers#reversing-transfers)
     """
 
     OBJECT_NAME = "transfer_reversal"
 
     def instance_url(self):
         token = util.utf8(self.id)
         transfer = util.utf8(self.transfer)
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/review.py` & `stripe-5.5.0b5/stripe/api_resources/review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/search_result_object.py` & `stripe-5.5.0b5/stripe/api_resources/search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/setup_attempt.py` & `stripe-5.5.0b5/stripe/api_resources/setup_attempt.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/setup_intent.py` & `stripe-5.5.0b5/stripe/api_resources/setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/shipping_rate.py` & `stripe-5.5.0b5/stripe/api_resources/shipping_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/sigma/scheduled_query_run.py` & `stripe-5.5.0b5/stripe/api_resources/sigma/scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/source.py` & `stripe-5.5.0b5/stripe/api_resources/source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/source_transaction.py` & `stripe-5.5.0b5/stripe/api_resources/source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/subscription.py` & `stripe-5.5.0b5/stripe/api_resources/subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/subscription_item.py` & `stripe-5.5.0b5/stripe/api_resources/subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/subscription_schedule.py` & `stripe-5.5.0b5/stripe/api_resources/subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax/calculation.py` & `stripe-5.5.0b5/stripe/api_resources/tax/calculation.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax/registration.py` & `stripe-5.5.0b5/stripe/api_resources/tax/registration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax/settings.py` & `stripe-5.5.0b5/stripe/api_resources/tax/settings.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax/transaction.py` & `stripe-5.5.0b5/stripe/api_resources/tax/transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax_id.py` & `stripe-5.5.0b5/stripe/api_resources/tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/tax_rate.py` & `stripe-5.5.0b5/stripe/api_resources/tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/terminal/configuration.py` & `stripe-5.5.0b5/stripe/api_resources/terminal/configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/terminal/location.py` & `stripe-5.5.0b5/stripe/api_resources/terminal/location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/terminal/reader.py` & `stripe-5.5.0b5/stripe/api_resources/terminal/reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/test_helpers/test_clock.py` & `stripe-5.5.0b5/stripe/api_resources/test_helpers/test_clock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/token.py` & `stripe-5.5.0b5/stripe/api_resources/token.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/topup.py` & `stripe-5.5.0b5/stripe/api_resources/topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/transfer.py` & `stripe-5.5.0b5/stripe/api_resources/transfer.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,11 +23,11 @@
 
     Before April 6, 2017, transfers also represented movement of funds from a
     Stripe account to a card or bank account. This behavior has since been split
     out into a [Payout](https://stripe.com/docs/api#payout_object) object, with corresponding payout endpoints. For more
     information, read about the
     [transfer/payout split](https://stripe.com/docs/transfer-payout-split).
 
-    Related guide: [Creating separate charges and transfers](https://stripe.com/docs/connect/charges-transfers)
+    Related guide: [Creating separate charges and transfers](https://stripe.com/docs/connect/separate-charges-and-transfers)
     """
 
     OBJECT_NAME = "transfer"
```

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/__init__.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/__init__.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/credit_reversal.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/credit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/debit_reversal.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/debit_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/financial_account.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/financial_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/inbound_transfer.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/inbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/outbound_payment.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/outbound_payment.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/outbound_transfer.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/outbound_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/received_credit.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/received_credit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/received_debit.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/received_debit.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/treasury/transaction_entry.py` & `stripe-5.5.0b5/stripe/api_resources/treasury/transaction_entry.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/usage_record.py` & `stripe-5.5.0b5/stripe/api_resources/usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/api_resources/webhook_endpoint.py` & `stripe-5.5.0b5/stripe/api_resources/webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/data/ca-certificates.crt` & `stripe-5.5.0b5/stripe/data/ca-certificates.crt`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/error.py` & `stripe-5.5.0b5/stripe/error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/http_client.py` & `stripe-5.5.0b5/stripe/http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/multipart_data_generator.py` & `stripe-5.5.0b5/stripe/multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/oauth.py` & `stripe-5.5.0b5/stripe/oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/oauth_error.py` & `stripe-5.5.0b5/stripe/oauth_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/object_classes.py` & `stripe-5.5.0b5/stripe/object_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     api_resources.CountrySpec.OBJECT_NAME: api_resources.CountrySpec,
     api_resources.Coupon.OBJECT_NAME: api_resources.Coupon,
     api_resources.CreditNote.OBJECT_NAME: api_resources.CreditNote,
     api_resources.CreditNoteLineItem.OBJECT_NAME: api_resources.CreditNoteLineItem,
     api_resources.Customer.OBJECT_NAME: api_resources.Customer,
     api_resources.CustomerBalanceTransaction.OBJECT_NAME: api_resources.CustomerBalanceTransaction,
     api_resources.CustomerCashBalanceTransaction.OBJECT_NAME: api_resources.CustomerCashBalanceTransaction,
+    api_resources.CustomerSession.OBJECT_NAME: api_resources.CustomerSession,
     api_resources.Dispute.OBJECT_NAME: api_resources.Dispute,
     api_resources.EphemeralKey.OBJECT_NAME: api_resources.EphemeralKey,
     api_resources.Event.OBJECT_NAME: api_resources.Event,
     api_resources.ExchangeRate.OBJECT_NAME: api_resources.ExchangeRate,
     api_resources.File.OBJECT_NAME: api_resources.File,
     api_resources.File.OBJECT_NAME_ALT: api_resources.File,
     api_resources.FileLink.OBJECT_NAME: api_resources.FileLink,
```

### Comparing `stripe-5.5.0b4/stripe/preview.py` & `stripe-5.5.0b5/stripe/preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/raw_request.py` & `stripe-5.5.0b5/stripe/raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/six.py` & `stripe-5.5.0b5/stripe/six.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/stripe_object.py` & `stripe-5.5.0b5/stripe/stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/stripe_response.py` & `stripe-5.5.0b5/stripe/stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/util.py` & `stripe-5.5.0b5/stripe/util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe/webhook.py` & `stripe-5.5.0b5/stripe/webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/stripe.egg-info/PKG-INFO` & `stripe-5.5.0b5/stripe.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: stripe
-Version: 5.5.0b4
+Version: 5.5.0b5
 Summary: Python bindings for the Stripe API
 Home-page: https://github.com/stripe/stripe-python
 Author: Stripe
 Author-email: support@stripe.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/stripe/stripe-python/issues
 Project-URL: Changes, https://github.com/stripe/stripe-python/blob/master/CHANGELOG.md
```

### Comparing `stripe-5.5.0b4/stripe.egg-info/SOURCES.txt` & `stripe-5.5.0b5/stripe.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,15 @@
 stripe/api_resources/country_spec.py
 stripe/api_resources/coupon.py
 stripe/api_resources/credit_note.py
 stripe/api_resources/credit_note_line_item.py
 stripe/api_resources/customer.py
 stripe/api_resources/customer_balance_transaction.py
 stripe/api_resources/customer_cash_balance_transaction.py
+stripe/api_resources/customer_session.py
 stripe/api_resources/dispute.py
 stripe/api_resources/ephemeral_key.py
 stripe/api_resources/error_object.py
 stripe/api_resources/event.py
 stripe/api_resources/exchange_rate.py
 stripe/api_resources/file.py
 stripe/api_resources/file_link.py
```

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_createable_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_createable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_custom_method.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_custom_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_deletable_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_deletable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_listable_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_listable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_nested_resource_class_methods.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_nested_resource_class_methods.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_searchable_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_searchable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_singleton_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_singleton_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_test_helpers_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_test_helpers_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/abstract/test_updateable_api_resource.py` & `stripe-5.5.0b5/tests/api_resources/abstract/test_updateable_api_resource.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/billing_portal/test_configuration.py` & `stripe-5.5.0b5/tests/api_resources/billing_portal/test_configuration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/checkout/test_session.py` & `stripe-5.5.0b5/tests/api_resources/checkout/test_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/identity/test_verification_report.py` & `stripe-5.5.0b5/tests/api_resources/identity/test_verification_report.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/identity/test_verification_session.py` & `stripe-5.5.0b5/tests/api_resources/identity/test_verification_session.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/issuing/test_authorization.py` & `stripe-5.5.0b5/tests/api_resources/issuing/test_authorization.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/issuing/test_card.py` & `stripe-5.5.0b5/tests/api_resources/issuing/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/issuing/test_cardholder.py` & `stripe-5.5.0b5/tests/api_resources/issuing/test_cardholder.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/issuing/test_dispute.py` & `stripe-5.5.0b5/tests/api_resources/issuing/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/issuing/test_transaction.py` & `stripe-5.5.0b5/tests/api_resources/issuing/test_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/radar/test_early_fraud_warning.py` & `stripe-5.5.0b5/tests/api_resources/radar/test_early_fraud_warning.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/radar/test_value_list.py` & `stripe-5.5.0b5/tests/api_resources/radar/test_value_list.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/radar/test_value_list_item.py` & `stripe-5.5.0b5/tests/api_resources/radar/test_value_list_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/reporting/test_report_run.py` & `stripe-5.5.0b5/tests/api_resources/reporting/test_report_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/reporting/test_report_type.py` & `stripe-5.5.0b5/tests/api_resources/reporting/test_report_type.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/sigma/test_scheduled_query_run.py` & `stripe-5.5.0b5/tests/api_resources/sigma/test_scheduled_query_run.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/terminal/test_location.py` & `stripe-5.5.0b5/tests/api_resources/terminal/test_location.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/terminal/test_reader.py` & `stripe-5.5.0b5/tests/api_resources/terminal/test_reader.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_account.py` & `stripe-5.5.0b5/tests/api_resources/test_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_account_link.py` & `stripe-5.5.0b5/tests/api_resources/test_account_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_apple_pay_domain.py` & `stripe-5.5.0b5/tests/api_resources/test_apple_pay_domain.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_application_fee.py` & `stripe-5.5.0b5/tests/api_resources/test_application_fee.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_application_fee_refund.py` & `stripe-5.5.0b5/tests/api_resources/test_application_fee_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_balance_transaction.py` & `stripe-5.5.0b5/tests/api_resources/test_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_bank_account.py` & `stripe-5.5.0b5/tests/api_resources/test_bank_account.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_capability.py` & `stripe-5.5.0b5/tests/api_resources/test_capability.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_card.py` & `stripe-5.5.0b5/tests/api_resources/test_card.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_charge.py` & `stripe-5.5.0b5/tests/api_resources/test_charge.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_country_spec.py` & `stripe-5.5.0b5/tests/api_resources/test_country_spec.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_coupon.py` & `stripe-5.5.0b5/tests/api_resources/test_coupon.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_credit_note.py` & `stripe-5.5.0b5/tests/api_resources/test_credit_note.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_customer.py` & `stripe-5.5.0b5/tests/api_resources/test_customer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_customer_balance_transaction.py` & `stripe-5.5.0b5/tests/api_resources/test_customer_balance_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_dispute.py` & `stripe-5.5.0b5/tests/api_resources/test_dispute.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_ephemeral_key.py` & `stripe-5.5.0b5/tests/api_resources/test_ephemeral_key.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_event.py` & `stripe-5.5.0b5/tests/api_resources/test_event.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_exchange_rate.py` & `stripe-5.5.0b5/tests/api_resources/test_exchange_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_file.py` & `stripe-5.5.0b5/tests/api_resources/test_file.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_file_link.py` & `stripe-5.5.0b5/tests/api_resources/test_file_link.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_file_upload.py` & `stripe-5.5.0b5/tests/api_resources/test_file_upload.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_invoice.py` & `stripe-5.5.0b5/tests/api_resources/test_invoice.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_invoice_item.py` & `stripe-5.5.0b5/tests/api_resources/test_invoice_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_list_object.py` & `stripe-5.5.0b5/tests/api_resources/test_list_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_payment_intent.py` & `stripe-5.5.0b5/tests/api_resources/test_payment_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_payment_method.py` & `stripe-5.5.0b5/tests/api_resources/test_payment_method.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_payout.py` & `stripe-5.5.0b5/tests/api_resources/test_payout.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_person.py` & `stripe-5.5.0b5/tests/api_resources/test_person.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_plan.py` & `stripe-5.5.0b5/tests/api_resources/test_plan.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_price.py` & `stripe-5.5.0b5/tests/api_resources/test_price.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_product.py` & `stripe-5.5.0b5/tests/api_resources/test_product.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_promotion_code.py` & `stripe-5.5.0b5/tests/api_resources/test_promotion_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_quote.py` & `stripe-5.5.0b5/tests/api_resources/test_quote.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_refund.py` & `stripe-5.5.0b5/tests/api_resources/test_refund.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_reversal.py` & `stripe-5.5.0b5/tests/api_resources/test_reversal.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_review.py` & `stripe-5.5.0b5/tests/api_resources/test_review.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_search_result_object.py` & `stripe-5.5.0b5/tests/api_resources/test_search_result_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_setup_intent.py` & `stripe-5.5.0b5/tests/api_resources/test_setup_intent.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_source.py` & `stripe-5.5.0b5/tests/api_resources/test_source.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_source_transaction.py` & `stripe-5.5.0b5/tests/api_resources/test_source_transaction.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_subscription.py` & `stripe-5.5.0b5/tests/api_resources/test_subscription.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_subscription_item.py` & `stripe-5.5.0b5/tests/api_resources/test_subscription_item.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_subscription_schedule.py` & `stripe-5.5.0b5/tests/api_resources/test_subscription_schedule.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_tax_code.py` & `stripe-5.5.0b5/tests/api_resources/test_tax_code.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_tax_id.py` & `stripe-5.5.0b5/tests/api_resources/test_tax_id.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_tax_rate.py` & `stripe-5.5.0b5/tests/api_resources/test_tax_rate.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_topup.py` & `stripe-5.5.0b5/tests/api_resources/test_topup.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_transfer.py` & `stripe-5.5.0b5/tests/api_resources/test_transfer.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_usage_record.py` & `stripe-5.5.0b5/tests/api_resources/test_usage_record.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_usage_record_summary.py` & `stripe-5.5.0b5/tests/api_resources/test_usage_record_summary.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/api_resources/test_webhook_endpoint.py` & `stripe-5.5.0b5/tests/api_resources/test_webhook_endpoint.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/conftest.py` & `stripe-5.5.0b5/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/request_mock.py` & `stripe-5.5.0b5/tests/request_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/stripe_mock.py` & `stripe-5.5.0b5/tests/stripe_mock.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_api_requestor.py` & `stripe-5.5.0b5/tests/test_api_requestor.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_error.py` & `stripe-5.5.0b5/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_generated_examples.py` & `stripe-5.5.0b5/tests/test_generated_examples.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,23 @@
 # File generated from our OpenAPI spec
 from __future__ import absolute_import, division, print_function
 import stripe
 
 
 class TestGeneratedExamples(object):
+    def test_account_externalaccount_list(self, request_mock):
+        stripe.Account.list_external_accounts(
+            "acct_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts",
+        )
+
     def test_apps_secret_list(self, request_mock):
         stripe.apps.Secret.list(
             scope={"type": "account"},
             limit=2,
         )
         request_mock.assert_requested(
             "get",
@@ -120,14 +130,25 @@
             type="card",
         )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xyz/payment_methods",
         )
 
+    def test_customer_paymentsource_update(self, request_mock):
+        stripe.Customer.modify_source(
+            "cus_123",
+            "card_123",
+            account_holder_name="Kamil",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_123/sources/card_123",
+        )
+
     def test_financial_connections_account_list(self, request_mock):
         stripe.financial_connections.Account.list()
         request_mock.assert_requested(
             "get",
             "/v1/financial_connections/accounts",
         )
 
@@ -562,14 +583,21 @@
             reason="fraud",
         )
         request_mock.assert_requested(
             "post",
             "/v1/accounts/acct_xxxxxxxxxxxxx/reject",
         )
 
+    def test_account_capability_list(self, request_mock):
+        stripe.Account.list_capabilities("acct_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/capabilities",
+        )
+
     def test_account_capability_retrieve(self, request_mock):
         stripe.Account.retrieve_capability(
             "acct_xxxxxxxxxxxxx",
             "card_payments",
         )
         request_mock.assert_requested(
             "get",
@@ -583,14 +611,134 @@
             requested=True,
         )
         request_mock.assert_requested(
             "post",
             "/v1/accounts/acct_xxxxxxxxxxxxx/capabilities/card_payments",
         )
 
+    def test_account_externalaccount_create(self, request_mock):
+        stripe.Account.create_external_account(
+            "acct_xxxxxxxxxxxxx",
+            external_account="btok_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts",
+        )
+
+    def test_account_externalaccount_create2(self, request_mock):
+        stripe.Account.create_external_account(
+            "acct_xxxxxxxxxxxxx",
+            external_account="tok_xxxx_debit",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts",
+        )
+
+    def test_account_externalaccount_delete(self, request_mock):
+        stripe.Account.delete_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_account_externalaccount_delete2(self, request_mock):
+        stripe.Account.delete_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/card_xxxxxxxxxxxxx",
+        )
+
+    def test_account_externalaccount_retrieve(self, request_mock):
+        stripe.Account.retrieve_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_account_externalaccount_retrieve2(self, request_mock):
+        stripe.Account.retrieve_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/card_xxxxxxxxxxxxx",
+        )
+
+    def test_account_externalaccount_update(self, request_mock):
+        stripe.Account.modify_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_account_externalaccount_update2(self, request_mock):
+        stripe.Account.modify_external_account(
+            "acct_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/external_accounts/card_xxxxxxxxxxxxx",
+        )
+
+    def test_account_loginlink_create(self, request_mock):
+        stripe.Account.create_login_link("acct_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/login_links",
+        )
+
+    def test_account_person_list(self, request_mock):
+        stripe.Account.list_persons(
+            "acct_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/persons",
+        )
+
+    def test_account_person_create(self, request_mock):
+        stripe.Account.create_person(
+            "acct_xxxxxxxxxxxxx",
+            first_name="Jane",
+            last_name="Diaz",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/persons",
+        )
+
+    def test_account_person_delete(self, request_mock):
+        stripe.Account.delete_person(
+            "acct_xxxxxxxxxxxxx",
+            "person_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/accounts/acct_xxxxxxxxxxxxx/persons/person_xxxxxxxxxxxxx",
+        )
+
     def test_account_person_retrieve(self, request_mock):
         stripe.Account.retrieve_person(
             "acct_xxxxxxxxxxxxx",
             "person_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
@@ -618,14 +766,31 @@
     def test_applicationfee_retrieve(self, request_mock):
         stripe.ApplicationFee.retrieve("fee_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/application_fees/fee_xxxxxxxxxxxxx",
         )
 
+    def test_applicationfee_feerefund_list(self, request_mock):
+        stripe.ApplicationFee.list_refunds(
+            "fee_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/application_fees/fee_xxxxxxxxxxxxx/refunds",
+        )
+
+    def test_applicationfee_feerefund_create(self, request_mock):
+        stripe.ApplicationFee.create_refund("fee_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "post",
+            "/v1/application_fees/fee_xxxxxxxxxxxxx/refunds",
+        )
+
     def test_applicationfee_feerefund_retrieve(self, request_mock):
         stripe.ApplicationFee.retrieve_refund(
             "fee_xxxxxxxxxxxxx",
             "fr_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
@@ -900,14 +1065,24 @@
     def test_creditnote_void_credit_note(self, request_mock):
         stripe.CreditNote.void_credit_note("cn_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "post",
             "/v1/credit_notes/cn_xxxxxxxxxxxxx/void",
         )
 
+    def test_creditnote_creditnotelineitem_list(self, request_mock):
+        stripe.CreditNote.list_lines(
+            "cn_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/credit_notes/cn_xxxxxxxxxxxxx/lines",
+        )
+
     def test_creditnote_preview(self, request_mock):
         stripe.CreditNote.preview(
             invoice="in_xxxxxxxxxxxxx",
             lines=[
                 {
                     "type": "invoice_line_item",
                     "invoice_line_item": "il_xxxxxxxxxxxxx",
@@ -963,34 +1138,201 @@
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
             "post",
             "/v1/customers/cus_xxxxxxxxxxxxx",
         )
 
+    def test_customer_customerbalancetransaction_list(self, request_mock):
+        stripe.Customer.list_balance_transactions(
+            "cus_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/balance_transactions",
+        )
+
+    def test_customer_customerbalancetransaction_create(self, request_mock):
+        stripe.Customer.create_balance_transaction(
+            "cus_xxxxxxxxxxxxx",
+            amount=-500,
+            currency="usd",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/balance_transactions",
+        )
+
     def test_customer_customerbalancetransaction_retrieve(self, request_mock):
         stripe.Customer.retrieve_balance_transaction(
             "cus_xxxxxxxxxxxxx",
             "cbtxn_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xxxxxxxxxxxxx/balance_transactions/cbtxn_xxxxxxxxxxxxx",
         )
 
+    def test_customer_customerbalancetransaction_update(self, request_mock):
+        stripe.Customer.modify_balance_transaction(
+            "cus_xxxxxxxxxxxxx",
+            "cbtxn_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/balance_transactions/cbtxn_xxxxxxxxxxxxx",
+        )
+
     def test_customer_list_payment_methods2(self, request_mock):
         stripe.Customer.list_payment_methods(
             "cus_xxxxxxxxxxxxx",
             type="card",
         )
         request_mock.assert_requested(
             "get",
             "/v1/customers/cus_xxxxxxxxxxxxx/payment_methods",
         )
 
+    def test_customer_paymentsource_list(self, request_mock):
+        stripe.Customer.list_sources(
+            "cus_xxxxxxxxxxxxx",
+            object="bank_account",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources",
+        )
+
+    def test_customer_paymentsource_list2(self, request_mock):
+        stripe.Customer.list_sources(
+            "cus_xxxxxxxxxxxxx",
+            object="card",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources",
+        )
+
+    def test_customer_paymentsource_create(self, request_mock):
+        stripe.Customer.create_source(
+            "cus_xxxxxxxxxxxxx",
+            source="btok_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources",
+        )
+
+    def test_customer_paymentsource_create2(self, request_mock):
+        stripe.Customer.create_source(
+            "cus_xxxxxxxxxxxxx",
+            source="tok_xxxx",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources",
+        )
+
+    def test_customer_paymentsource_delete(self, request_mock):
+        stripe.Customer.delete_source(
+            "cus_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_paymentsource_delete2(self, request_mock):
+        stripe.Customer.delete_source(
+            "cus_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/card_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_paymentsource_retrieve(self, request_mock):
+        stripe.Customer.retrieve_source(
+            "cus_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_paymentsource_retrieve2(self, request_mock):
+        stripe.Customer.retrieve_source(
+            "cus_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/card_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_paymentsource_update2(self, request_mock):
+        stripe.Customer.modify_source(
+            "cus_xxxxxxxxxxxxx",
+            "ba_xxxxxxxxxxxxx",
+            metadata={"order_id": "6735"},
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/ba_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_paymentsource_update3(self, request_mock):
+        stripe.Customer.modify_source(
+            "cus_xxxxxxxxxxxxx",
+            "card_xxxxxxxxxxxxx",
+            name="Jenny Rosen",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/sources/card_xxxxxxxxxxxxx",
+        )
+
+    def test_customer_taxid_list(self, request_mock):
+        stripe.Customer.list_tax_ids(
+            "cus_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/customers/cus_xxxxxxxxxxxxx/tax_ids",
+        )
+
+    def test_customer_taxid_create(self, request_mock):
+        stripe.Customer.create_tax_id(
+            "cus_xxxxxxxxxxxxx",
+            type="eu_vat",
+            value="DE123456789",
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/customers/cus_xxxxxxxxxxxxx/tax_ids",
+        )
+
+    def test_customer_taxid_delete(self, request_mock):
+        stripe.Customer.delete_tax_id(
+            "cus_xxxxxxxxxxxxx",
+            "txi_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "delete",
+            "/v1/customers/cus_xxxxxxxxxxxxx/tax_ids/txi_xxxxxxxxxxxxx",
+        )
+
     def test_customer_taxid_retrieve(self, request_mock):
         stripe.Customer.retrieve_tax_id(
             "cus_xxxxxxxxxxxxx",
             "txi_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
@@ -2362,14 +2704,35 @@
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
             "post",
             "/v1/subscription_items/si_xxxxxxxxxxxxx",
         )
 
+    def test_subscriptionitem_usagerecordsummary_list(self, request_mock):
+        stripe.SubscriptionItem.list_usage_record_summaries(
+            "si_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/subscription_items/si_xxxxxxxxxxxxx/usage_record_summaries",
+        )
+
+    def test_subscriptionitem_usagerecord_create(self, request_mock):
+        stripe.SubscriptionItem.create_usage_record(
+            "si_xxxxxxxxxxxxx",
+            quantity=100,
+            timestamp=1571252444,
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/subscription_items/si_xxxxxxxxxxxxx/usage_records",
+        )
+
     def test_subscriptionschedule_list(self, request_mock):
         stripe.SubscriptionSchedule.list(limit=3)
         request_mock.assert_requested(
             "get",
             "/v1/subscription_schedules",
         )
 
@@ -2434,14 +2797,21 @@
             items=[{"price": "price_xxxxxxxxxxxxx"}],
         )
         request_mock.assert_requested(
             "post",
             "/v1/subscriptions",
         )
 
+    def test_subscription_cancel(self, request_mock):
+        stripe.Subscription.cancel("sub_xxxxxxxxxxxxx")
+        request_mock.assert_requested(
+            "delete",
+            "/v1/subscriptions/sub_xxxxxxxxxxxxx",
+        )
+
     def test_subscription_retrieve(self, request_mock):
         stripe.Subscription.retrieve("sub_xxxxxxxxxxxxx")
         request_mock.assert_requested(
             "get",
             "/v1/subscriptions/sub_xxxxxxxxxxxxx",
         )
 
@@ -2854,14 +3224,34 @@
             metadata={"order_id": "6735"},
         )
         request_mock.assert_requested(
             "post",
             "/v1/transfers/tr_xxxxxxxxxxxxx",
         )
 
+    def test_transfer_transferreversal_list(self, request_mock):
+        stripe.Transfer.list_reversals(
+            "tr_xxxxxxxxxxxxx",
+            limit=3,
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/transfers/tr_xxxxxxxxxxxxx/reversals",
+        )
+
+    def test_transfer_transferreversal_create(self, request_mock):
+        stripe.Transfer.create_reversal(
+            "tr_xxxxxxxxxxxxx",
+            amount=100,
+        )
+        request_mock.assert_requested(
+            "post",
+            "/v1/transfers/tr_xxxxxxxxxxxxx/reversals",
+        )
+
     def test_transfer_transferreversal_retrieve(self, request_mock):
         stripe.Transfer.retrieve_reversal(
             "tr_xxxxxxxxxxxxx",
             "trr_xxxxxxxxxxxxx",
         )
         request_mock.assert_requested(
             "get",
@@ -3251,7 +3641,17 @@
                 "address_source": "shipping",
             },
         )
         request_mock.assert_requested(
             "post",
             "/v1/tax/calculations",
         )
+
+    def test_creditnote_preview_lines(self, request_mock):
+        stripe.CreditNote.preview_lines(
+            limit=3,
+            invoice="in_xxxxxxxxxxxxx",
+        )
+        request_mock.assert_requested(
+            "get",
+            "/v1/credit_notes/preview/lines",
+        )
```

### Comparing `stripe-5.5.0b4/tests/test_http_client.py` & `stripe-5.5.0b5/tests/test_http_client.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_integration.py` & `stripe-5.5.0b5/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_multipart_data_generator.py` & `stripe-5.5.0b5/tests/test_multipart_data_generator.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_oauth.py` & `stripe-5.5.0b5/tests/test_oauth.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_preview.py` & `stripe-5.5.0b5/tests/test_preview.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_raw_request.py` & `stripe-5.5.0b5/tests/test_raw_request.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_stripe_object.py` & `stripe-5.5.0b5/tests/test_stripe_object.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_stripe_response.py` & `stripe-5.5.0b5/tests/test_stripe_response.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_util.py` & `stripe-5.5.0b5/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tests/test_webhook.py` & `stripe-5.5.0b5/tests/test_webhook.py`

 * *Files identical despite different names*

### Comparing `stripe-5.5.0b4/tox.ini` & `stripe-5.5.0b5/tox.ini`

 * *Files identical despite different names*

