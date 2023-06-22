# Comparing `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9-py3-none-any.whl.zip` & `tmp/odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,6 +1,6 @@
-Zip file size: 2138 bytes, number of entries: 4
--rw-r--r--  2.0 unx     5227 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      477 b- defN 23-Jun-15 02:37 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/RECORD
-4 files, 5797 bytes uncompressed, 1196 bytes compressed:  79.4%
+Zip file size: 2166 bytes, number of entries: 4
+-rw-r--r--  2.0 unx     5495 b- defN 23-Jun-22 02:36 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Jun-22 02:36 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-Jun-22 02:36 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      477 b- defN 23-Jun-22 02:36 odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/RECORD
+4 files, 6065 bytes uncompressed, 1224 bytes compressed:  79.8%
```

## zipnote {}

```diff
@@ -1,13 +1,13 @@
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/WHEEL
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/top_level.txt
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/RECORD
+Filename: odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230614.9.dist-info/METADATA` & `odoo14_addons_shopinvader_odoo_shopinvader-14.0.20230621.1.dist-info/METADATA`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: odoo14-addons-shopinvader-odoo-shopinvader
-Version: 14.0.20230614.9
+Version: 14.0.20230621.1
 Summary: Meta package for shopinvader-odoo-shopinvader Odoo addons
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python
 Classifier: Framework :: Odoo
 Classifier: Framework :: Odoo :: 14.0
@@ -38,14 +38,16 @@
 Requires-Dist: odoo14-addon-shopinvader-image
 Requires-Dist: odoo14-addon-shopinvader-import-image
 Requires-Dist: odoo14-addon-shopinvader-invoice
 Requires-Dist: odoo14-addon-shopinvader-lead
 Requires-Dist: odoo14-addon-shopinvader-locomotive
 Requires-Dist: odoo14-addon-shopinvader-locomotive-algolia
 Requires-Dist: odoo14-addon-shopinvader-locomotive-guest-mode
+Requires-Dist: odoo14-addon-shopinvader-locomotive-impersonate
+Requires-Dist: odoo14-addon-shopinvader-locomotive-product-seasonality
 Requires-Dist: odoo14-addon-shopinvader-locomotive-reset-password
 Requires-Dist: odoo14-addon-shopinvader-locomotive-sale-profile
 Requires-Dist: odoo14-addon-shopinvader-locomotive-wishlist
 Requires-Dist: odoo14-addon-shopinvader-mass-mailing-company-newsletter
 Requires-Dist: odoo14-addon-shopinvader-membership
 Requires-Dist: odoo14-addon-shopinvader-multi-cart
 Requires-Dist: odoo14-addon-shopinvader-multi-category
@@ -61,14 +63,16 @@
 Requires-Dist: odoo14-addon-shopinvader-product-brand-image
 Requires-Dist: odoo14-addon-shopinvader-product-brand-tag
 Requires-Dist: odoo14-addon-shopinvader-product-manufactured-for
 Requires-Dist: odoo14-addon-shopinvader-product-media
 Requires-Dist: odoo14-addon-shopinvader-product-new
 Requires-Dist: odoo14-addon-shopinvader-product-order
 Requires-Dist: odoo14-addon-shopinvader-product-price-tax
+Requires-Dist: odoo14-addon-shopinvader-product-seasonality
+Requires-Dist: odoo14-addon-shopinvader-product-seasonality-search-engine
 Requires-Dist: odoo14-addon-shopinvader-product-stock
 Requires-Dist: odoo14-addon-shopinvader-product-stock-assortment
 Requires-Dist: odoo14-addon-shopinvader-product-stock-forecast
 Requires-Dist: odoo14-addon-shopinvader-product-stock-forecast-expiry
 Requires-Dist: odoo14-addon-shopinvader-product-stock-state
 Requires-Dist: odoo14-addon-shopinvader-product-template-multi-link
 Requires-Dist: odoo14-addon-shopinvader-product-template-multi-link-date-span
```

