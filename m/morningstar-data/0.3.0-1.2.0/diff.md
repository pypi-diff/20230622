# Comparing `tmp/morningstar_data-0.3.0.tar.gz` & `tmp/morningstar_data-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "morningstar_data-0.3.0.tar", max compression
+gzip compressed data, was "morningstar_data-1.2.0.tar", max compression
```

## Comparing `morningstar_data-0.3.0.tar` & `morningstar_data-1.2.0.tar`

### file list

```diff
@@ -1,5 +1,70 @@
--rw-r--r--   0        0        0        0 2022-02-07 18:30:59.979546 morningstar_data-0.3.0/morningstar_data/__init__.py
--rw-r--r--   0        0        0       45 2022-02-07 18:30:59.979546 morningstar_data-0.3.0/morningstar_data/hello_world.py
--rw-r--r--   0        0        0      385 2022-02-07 18:31:41.540547 morningstar_data-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      516 2022-02-07 18:31:42.879158 morningstar_data-0.3.0/setup.py
--rw-r--r--   0        0        0      389 2022-02-07 18:31:42.879383 morningstar_data-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0      571 2023-06-22 18:47:41.613303 morningstar_data-1.2.0/LICENSE
+-rw-r--r--   0        0        0      214 2023-06-22 17:30:37.704074 morningstar_data-1.2.0/morningstar_data/__init__.py
+-rw-r--r--   0        0        0      615 2023-06-22 17:30:37.705075 morningstar_data-1.2.0/morningstar_data/_base.py
+-rw-r--r--   0        0        0     3155 2023-05-15 14:48:44.483407 morningstar_data-1.2.0/morningstar_data/_utils.py
+-rw-r--r--   0        0        0       85 2023-06-22 17:30:37.706072 morningstar_data-1.2.0/morningstar_data/_version.py
+-rw-r--r--   0        0        0       63 2023-03-17 18:42:29.108172 morningstar_data-1.2.0/morningstar_data/datalake/__init__.py
+-rw-r--r--   0        0        0       64 2023-03-17 18:42:29.109161 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/__init__.py
+-rw-r--r--   0        0        0      578 2023-03-17 18:42:29.110169 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/_file.py
+-rw-r--r--   0        0        0      791 2023-03-17 18:42:29.111162 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/_table.py
+-rw-r--r--   0        0        0     1030 2023-03-17 18:42:29.131158 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/csvfile.py
+-rw-r--r--   0        0        0     2220 2023-05-15 14:48:44.490241 morningstar_data-1.2.0/morningstar_data/datalake/_data_objects/temptable.py
+-rw-r--r--   0        0        0      559 2023-06-22 17:30:20.444782 morningstar_data-1.2.0/morningstar_data/datalake/_error_messages.py
+-rw-r--r--   0        0        0      966 2023-05-15 14:48:44.499809 morningstar_data-1.2.0/morningstar_data/datalake/_exceptions.py
+-rw-r--r--   0        0        0     5777 2023-06-22 17:30:20.445786 morningstar_data-1.2.0/morningstar_data/datalake/base.py
+-rw-r--r--   0        0        0      955 2023-03-24 17:52:36.333929 morningstar_data-1.2.0/morningstar_data/direct/__init__.py
+-rw-r--r--   0        0        0     2496 2023-05-15 14:48:44.510808 morningstar_data-1.2.0/morningstar_data/direct/_api.py
+-rw-r--r--   0        0        0      182 2023-05-15 14:48:44.515806 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/__init__.py
+-rw-r--r--   0        0        0     1881 2023-06-22 17:30:20.446780 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_delivery_backend.py
+-rw-r--r--   0        0        0     5291 2023-05-15 14:48:44.526813 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_holdings_backend.py
+-rw-r--r--   0        0        0     3445 2023-05-15 14:48:44.531804 morningstar_data-1.2.0/morningstar_data/direct/_backend_apis/_signed_url_backend.py
+-rw-r--r--   0        0        0     3848 2023-05-15 14:48:44.537806 morningstar_data-1.2.0/morningstar_data/direct/_base_api.py
+-rw-r--r--   0        0        0     5378 2023-06-22 19:25:30.774829 morningstar_data-1.2.0/morningstar_data/direct/_config.py
+-rw-r--r--   0        0        0     2109 2023-03-17 18:42:29.149897 morningstar_data-1.2.0/morningstar_data/direct/_config_key.py
+-rw-r--r--   0        0        0     7607 2023-06-22 17:30:37.706072 morningstar_data-1.2.0/morningstar_data/direct/_core_api.py
+-rw-r--r--   0        0        0      200 2023-03-17 18:42:29.152895 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/__init__.py
+-rw-r--r--   0        0        0     2366 2023-03-17 18:42:29.154899 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_custom_data_points_types.py
+-rw-r--r--   0        0        0    26357 2023-06-22 17:30:20.447779 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_data_points_object.py
+-rw-r--r--   0        0        0     7701 2023-03-17 18:42:29.157900 morningstar_data-1.2.0/morningstar_data/direct/_data_objects/_investments_object.py
+-rw-r--r--   0        0        0     2636 2023-06-22 17:30:20.447779 morningstar_data-1.2.0/morningstar_data/direct/_data_point.py
+-rw-r--r--   0        0        0     1078 2023-03-17 18:42:29.161693 morningstar_data-1.2.0/morningstar_data/direct/_data_type.py
+-rw-r--r--   0        0        0     1642 2023-06-22 17:30:37.707074 morningstar_data-1.2.0/morningstar_data/direct/_decorator.py
+-rw-r--r--   0        0        0    14023 2023-06-22 17:30:20.448778 morningstar_data-1.2.0/morningstar_data/direct/_error_messages.py
+-rw-r--r--   0        0        0     3583 2023-06-22 17:30:20.448778 morningstar_data-1.2.0/morningstar_data/direct/_exceptions.py
+-rw-r--r--   0        0        0        0 2023-03-17 18:42:29.173293 morningstar_data-1.2.0/morningstar_data/direct/_investment/__init__.py
+-rw-r--r--   0        0        0     4378 2023-05-15 14:48:44.577810 morningstar_data-1.2.0/morningstar_data/direct/_investment/_asset_flow_data.py
+-rw-r--r--   0        0        0     1581 2023-05-15 14:48:44.586805 morningstar_data-1.2.0/morningstar_data/direct/_investment/_common.py
+-rw-r--r--   0        0        0     6233 2023-05-15 14:48:44.592805 morningstar_data-1.2.0/morningstar_data/direct/_investment/_data.py
+-rw-r--r--   0        0        0     8550 2023-06-22 17:30:20.450784 morningstar_data-1.2.0/morningstar_data/direct/_investment/_normal_data.py
+-rw-r--r--   0        0        0     5154 2023-05-15 14:48:44.604807 morningstar_data-1.2.0/morningstar_data/direct/_investment/_peer_group_data.py
+-rw-r--r--   0        0        0      165 2023-03-17 18:42:29.183291 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/__init__.py
+-rw-r--r--   0        0        0     1312 2023-05-15 14:48:44.610805 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_common.py
+-rw-r--r--   0        0        0     8021 2023-05-15 14:48:44.615804 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_holdings_entity.py
+-rw-r--r--   0        0        0     8117 2023-05-15 14:48:44.621806 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_settings.py
+-rw-r--r--   0        0        0      980 2023-03-17 18:42:29.190337 morningstar_data-1.2.0/morningstar_data/direct/_portfolio/_portfolio_type.py
+-rw-r--r--   0        0        0    11166 2023-05-15 14:48:44.627805 morningstar_data-1.2.0/morningstar_data/direct/_portfolio_data_set.py
+-rw-r--r--   0        0        0     3470 2023-05-15 14:48:44.633807 morningstar_data-1.2.0/morningstar_data/direct/_utils.py
+-rw-r--r--   0        0        0    13355 2023-06-22 17:30:37.708073 morningstar_data-1.2.0/morningstar_data/direct/asset_flow.py
+-rw-r--r--   0        0        0    16635 2023-06-22 17:30:37.709081 morningstar_data-1.2.0/morningstar_data/direct/custom_database.py
+-rw-r--r--   0        0        0     1300 2023-03-17 18:42:29.200377 morningstar_data-1.2.0/morningstar_data/direct/data_type.py
+-rw-r--r--   0        0        0    43354 2023-06-22 17:30:37.710075 morningstar_data-1.2.0/morningstar_data/direct/holdings.py
+-rw-r--r--   0        0        0    13827 2023-06-22 17:30:37.711095 morningstar_data-1.2.0/morningstar_data/direct/investment.py
+-rw-r--r--   0        0        0    33055 2023-06-22 17:30:37.712053 morningstar_data-1.2.0/morningstar_data/direct/lookup.py
+-rw-r--r--   0        0        0     6130 2023-06-22 17:30:37.713064 morningstar_data-1.2.0/morningstar_data/direct/peer_group.py
+-rw-r--r--   0        0        0    19911 2023-06-22 17:30:37.714094 morningstar_data-1.2.0/morningstar_data/direct/performance_report.py
+-rw-r--r--   0        0        0    38033 2023-06-22 17:30:37.715091 morningstar_data-1.2.0/morningstar_data/direct/portfolio.py
+-rw-r--r--   0        0        0    12817 2023-06-22 17:30:37.716074 morningstar_data-1.2.0/morningstar_data/direct/returns.py
+-rw-r--r--   0        0        0      418 2023-03-17 18:42:29.214388 morningstar_data-1.2.0/morningstar_data/direct/user_items/__init__.py
+-rw-r--r--   0        0        0      762 2023-03-17 18:42:29.218384 morningstar_data-1.2.0/morningstar_data/direct/user_items/_utils.py
+-rw-r--r--   0        0        0     8114 2023-06-22 17:30:37.717076 morningstar_data-1.2.0/morningstar_data/direct/user_items/data_set.py
+-rw-r--r--   0        0        0    13305 2023-06-22 17:30:37.719075 morningstar_data-1.2.0/morningstar_data/direct/user_items/investment_lists.py
+-rw-r--r--   0        0        0    11412 2023-06-19 16:45:12.887904 morningstar_data-1.2.0/morningstar_data/direct/user_items/portfolio.py
+-rw-r--r--   0        0        0    10592 2023-06-22 17:30:37.720072 morningstar_data-1.2.0/morningstar_data/direct/user_items/search_criteria.py
+-rw-r--r--   0        0        0     4874 2023-06-22 17:30:37.720072 morningstar_data-1.2.0/morningstar_data/lookup.py
+-rw-r--r--   0        0        0      160 2023-03-24 17:52:36.359930 morningstar_data-1.2.0/morningstar_data/utils/__init__.py
+-rw-r--r--   0        0        0     6516 2023-03-24 17:52:36.360930 morningstar_data-1.2.0/morningstar_data/utils/_delivery_config.py
+-rw-r--r--   0        0        0     7973 2023-06-22 19:25:30.775831 morningstar_data-1.2.0/morningstar_data/utils/_helpers.py
+-rw-r--r--   0        0        0    10691 2023-06-22 17:30:37.722072 morningstar_data-1.2.0/morningstar_data/utils/delivery.py
+-rw-r--r--   0        0        0     2552 2023-06-22 18:47:41.615267 morningstar_data-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11502 2023-06-22 19:25:30.773829 morningstar_data-1.2.0/README.md
+-rw-r--r--   0        0        0    12382 1970-01-01 00:00:00.000000 morningstar_data-1.2.0/PKG-INFO
```

