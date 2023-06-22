# Comparing `tmp/gs-netsuite-api-1.1.0.tar.gz` & `tmp/gs-netsuite-api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gs-netsuite-api-1.1.0.tar", last modified: Thu Jun 22 14:50:07 2023, max compression
+gzip compressed data, was "gs-netsuite-api-1.1.1.tar", last modified: Thu Jun 22 18:17:44 2023, max compression
```

## Comparing `gs-netsuite-api-1.1.0.tar` & `gs-netsuite-api-1.1.1.tar`

### file list

```diff
@@ -1,115 +1,115 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.246274 gs-netsuite-api-1.1.0/
--rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.gitlab-ci.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.206274 gs-netsuite-api-1.1.0/.idea/
--rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.idea/.gitignore
--rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.idea/GitlabLint.xml
--rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.idea/misc.xml
--rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.idea/modules.xml
--rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.idea/vcs.xml
--rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.local-antora-playbook.yml
--rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.pre-commit-config.yaml
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/.ruff
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-22 14:50:07.242274 gs-netsuite-api-1.1.0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/README.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.210274 gs-netsuite-api-1.1.0/docs/
--rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/antora.yml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.194274 gs-netsuite-api-1.1.0/docs/modules/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.210274 gs-netsuite-api-1.1.0/docs/modules/ROOT/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.194274 gs-netsuite-api-1.1.0/docs/modules/ROOT/examples/
--rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/modules/ROOT/nav.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.210274 gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/
--rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/api.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2996 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/convertion.adoc
--rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/index.adoc
--rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/types.adoc
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.214274 gs-netsuite-api-1.1.0/example/
--rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/example/sample_item_fulfillment_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/example/sample_item_receipt_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/example/sample_product_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/example/sample_purchase_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/example/sample_sale_api.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/mkdocs.yml
--rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.0/netsuite-api.iml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/wsdl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.214274 gs-netsuite-api-1.1.0/output/wsdl/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/wsdl/v2022_2_0/netsuite.wsdl
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.202274 gs-netsuite-api-1.1.0/output/xsd/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/activities/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.218274 gs-netsuite-api-1.1.0/output/xsd/activities/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/activities/v2022_2_0/scheduling.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/documents/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.218274 gs-netsuite-api-1.1.0/output/xsd/documents/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/documents/v2022_2_0/fileCabinet.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/general/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.218274 gs-netsuite-api-1.1.0/output/xsd/general/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/general/v2022_2_0/communication.xsd
--rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/general/v2022_2_0/communicationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/lists/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.226274 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/accounting.xsd
--rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/accountingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/marketing.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/marketingTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/relationships.xsd
--rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supplyChain.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/support.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supportTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/website.xsd
--rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/websiteTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/platform/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.230274 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/common.xsd
--rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/commonTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/core.xsd
--rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/coreTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/faultTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/faults.xsd
--rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/messages.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.198274 gs-netsuite-api-1.1.0/output/xsd/setup/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.230274 gs-netsuite-api-1.1.0/output/xsd/setup/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/setup/v2022_2_0/customization.xsd
--rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/setup/v2022_2_0/customizationTypes.xsd
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.202274 gs-netsuite-api-1.1.0/output/xsd/transactions/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.238274 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/
--rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/bank.xsd
--rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/bankTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/customerTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/customers.xsd
--rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/employees.xsd
--rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/financial.xsd
--rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/financialTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/general.xsd
--rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/inventory.xsd
--rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/purchases.xsd
--rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/saleTypes.xsd
--rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/sales.xsd
--rw-rw-rw-   0 root         (0) root         (0)      627 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 14:50:07.246274 gs-netsuite-api-1.1.0/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.202274 gs-netsuite-api-1.1.0/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.242274 gs-netsuite-api-1.1.0/src/gs_netsuite_api/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/__init__.py
--rw-r--r--   0 root         (0) root         (0)      160 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/_version.py
--rw-rw-rw-   0 root         (0) root         (0)    26267 2023-06-22 14:47:38.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/api.py
--rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/api.py.adoc
--rw-rw-rw-   0 root         (0) root         (0)     4159 2023-06-22 14:47:38.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/data_types.py
--rw-rw-rw-   0 root         (0) root         (0)     4296 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api/ns_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 14:50:07.242274 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)      186 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3235 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       52 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 14:50:07.000000 gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)     3862 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.0/wsdldownloader.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.955770 gs-netsuite-api-1.1.1/
+-rw-rw-rw-   0 root         (0) root         (0)     1910 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      382 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.gitlab-ci.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.935770 gs-netsuite-api-1.1.1/.idea/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.idea/.gitignore
+-rw-rw-rw-   0 root         (0) root         (0)      391 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.idea/GitlabLint.xml
+-rw-rw-rw-   0 root         (0) root         (0)      284 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.idea/misc.xml
+-rw-rw-rw-   0 root         (0) root         (0)      265 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.idea/modules.xml
+-rw-rw-rw-   0 root         (0) root         (0)      168 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.idea/vcs.xml
+-rw-rw-rw-   0 root         (0) root         (0)      366 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.local-antora-playbook.yml
+-rw-rw-rw-   0 root         (0) root         (0)      905 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.pre-commit-config.yaml
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/.ruff
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-22 18:17:44.955770 gs-netsuite-api-1.1.1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/README.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.935770 gs-netsuite-api-1.1.1/docs/
+-rw-rw-rw-   0 root         (0) root         (0)      141 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/antora.yml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/docs/modules/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.935770 gs-netsuite-api-1.1.1/docs/modules/ROOT/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/docs/modules/ROOT/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       90 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/modules/ROOT/nav.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.935770 gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/
+-rw-rw-rw-   0 root         (0) root         (0)     3361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/api.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2996 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/convertion.adoc
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/index.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     2206 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/types.adoc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.939770 gs-netsuite-api-1.1.1/example/
+-rw-rw-rw-   0 root         (0) root         (0)     1319 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/example/sample_item_fulfillment_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1311 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/example/sample_item_receipt_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1300 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/example/sample_product_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1820 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/example/sample_purchase_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/example/sample_sale_api.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/mkdocs.yml
+-rw-rw-rw-   0 root         (0) root         (0)      495 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.1/netsuite-api.iml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/wsdl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.939770 gs-netsuite-api-1.1.1/output/wsdl/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   133803 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/wsdl/v2022_2_0/netsuite.wsdl
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.931770 gs-netsuite-api-1.1.1/output/xsd/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/xsd/activities/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.939770 gs-netsuite-api-1.1.1/output/xsd/activities/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    38231 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/activities/v2022_2_0/scheduling.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7111 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/activities/v2022_2_0/schedulingTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/xsd/documents/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.939770 gs-netsuite-api-1.1.1/output/xsd/documents/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)     8963 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/documents/v2022_2_0/fileCabinet.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4282 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/xsd/general/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.939770 gs-netsuite-api-1.1.1/output/xsd/general/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    14530 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/general/v2022_2_0/communication.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      915 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/general/v2022_2_0/communicationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/xsd/lists/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.943770 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   424972 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/accounting.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    40848 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/accountingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    11949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    31010 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    27949 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/marketing.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5751 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/marketingTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     7100 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/relationshipTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   102099 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/relationships.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    16989 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supplyChain.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1222 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    29653 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/support.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2906 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supportTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     6213 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/website.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      350 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/websiteTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.927770 gs-netsuite-api-1.1.1/output/xsd/platform/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.947770 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   744517 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/common.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    59244 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/commonTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    47859 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/core.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    37883 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/coreTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    72361 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/faultTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3764 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/faults.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    28339 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/messages.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.931770 gs-netsuite-api-1.1.1/output/xsd/setup/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.947770 gs-netsuite-api-1.1.1/output/xsd/setup/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)   102180 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/setup/v2022_2_0/customization.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     4880 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/setup/v2022_2_0/customizationTypes.xsd
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.931770 gs-netsuite-api-1.1.1/output/xsd/transactions/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.951770 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/
+-rw-rw-rw-   0 root         (0) root         (0)    13345 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/bank.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      354 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/bankTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/customerTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    75538 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/customers.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    10022 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/demandPlanning.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2094 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      615 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/employeeTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    43650 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/employees.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     5844 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/financial.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      561 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/financialTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    23444 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/general.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    49374 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/inventory.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     2071 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)     1983 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    64002 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/purchases.xsd
+-rw-rw-rw-   0 root         (0) root         (0)    32740 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/saleTypes.xsd
+-rw-rw-rw-   0 root         (0) root         (0)   141383 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/sales.xsd
+-rw-rw-rw-   0 root         (0) root         (0)      627 2023-06-22 14:42:03.000000 gs-netsuite-api-1.1.1/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-06-22 18:17:44.955770 gs-netsuite-api-1.1.1/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.931770 gs-netsuite-api-1.1.1/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.951770 gs-netsuite-api-1.1.1/src/gs_netsuite_api/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      160 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/_version.py
+-rw-rw-rw-   0 root         (0) root         (0)    27039 2023-06-22 17:03:09.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/api.py
+-rw-rw-rw-   0 root         (0) root         (0)       60 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/api.py.adoc
+-rw-rw-rw-   0 root         (0) root         (0)     4252 2023-06-22 17:03:09.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/data_types.py
+-rw-rw-rw-   0 root         (0) root         (0)     4296 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api/ns_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-06-22 18:17:44.955770 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      186 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       52 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2023-06-22 18:17:44.000000 gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)     3862 2023-06-22 14:37:57.000000 gs-netsuite-api-1.1.1/wsdldownloader.py
```

### Comparing `gs-netsuite-api-1.1.0/.gitignore` & `gs-netsuite-api-1.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/.pre-commit-config.yaml` & `gs-netsuite-api-1.1.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/README.adoc` & `gs-netsuite-api-1.1.1/README.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/api.adoc` & `gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/api.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/convertion.adoc` & `gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/convertion.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/index.adoc` & `gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/index.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/docs/modules/ROOT/pages/types.adoc` & `gs-netsuite-api-1.1.1/docs/modules/ROOT/pages/types.adoc`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/example/sample_item_fulfillment_api.py` & `gs-netsuite-api-1.1.1/example/sample_item_fulfillment_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/example/sample_item_receipt_api.py` & `gs-netsuite-api-1.1.1/example/sample_item_receipt_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/example/sample_product_api.py` & `gs-netsuite-api-1.1.1/example/sample_product_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/example/sample_purchase_api.py` & `gs-netsuite-api-1.1.1/example/sample_purchase_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/example/sample_sale_api.py` & `gs-netsuite-api-1.1.1/example/sample_sale_api.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/mkdocs.yml` & `gs-netsuite-api-1.1.1/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/wsdl/v2022_2_0/netsuite.wsdl` & `gs-netsuite-api-1.1.1/output/wsdl/v2022_2_0/netsuite.wsdl`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/activities/v2022_2_0/scheduling.xsd` & `gs-netsuite-api-1.1.1/output/xsd/activities/v2022_2_0/scheduling.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/activities/v2022_2_0/schedulingTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/activities/v2022_2_0/schedulingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/documents/v2022_2_0/fileCabinet.xsd` & `gs-netsuite-api-1.1.1/output/xsd/documents/v2022_2_0/fileCabinet.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/documents/v2022_2_0/fileCabinetTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/general/v2022_2_0/communication.xsd` & `gs-netsuite-api-1.1.1/output/xsd/general/v2022_2_0/communication.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/general/v2022_2_0/communicationTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/general/v2022_2_0/communicationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/accounting.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/accounting.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/accountingTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/accountingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/marketing.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/marketing.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/marketingTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/marketingTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/relationshipTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/relationshipTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/relationships.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/relationships.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supplyChain.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supplyChain.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supplyChainTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/support.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/support.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/supportTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/supportTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/lists/v2022_2_0/website.xsd` & `gs-netsuite-api-1.1.1/output/xsd/lists/v2022_2_0/website.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/common.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/common.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/commonTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/commonTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/core.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/core.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/coreTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/coreTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/faultTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/faultTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/faults.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/faults.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/platform/v2022_2_0/messages.xsd` & `gs-netsuite-api-1.1.1/output/xsd/platform/v2022_2_0/messages.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/setup/v2022_2_0/customization.xsd` & `gs-netsuite-api-1.1.1/output/xsd/setup/v2022_2_0/customization.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/setup/v2022_2_0/customizationTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/setup/v2022_2_0/customizationTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/bank.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/bank.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/customerTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/customerTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/customers.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/customers.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/demandPlanning.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/demandPlanning.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/demandPlanningTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/employeeTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/employeeTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/employees.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/employees.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/financial.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/financial.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/financialTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/financialTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/general.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/general.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/inventory.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/inventory.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/inventoryTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/purchaseTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/purchases.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/purchases.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/saleTypes.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/saleTypes.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/output/xsd/transactions/v2022_2_0/sales.xsd` & `gs-netsuite-api-1.1.1/output/xsd/transactions/v2022_2_0/sales.xsd`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/pyproject.toml` & `gs-netsuite-api-1.1.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/src/gs_netsuite_api/api.py` & `gs-netsuite-api-1.1.1/src/gs_netsuite_api/api.py`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .ns_utils import search_with_pref, assertSuccess, SearchParams, extract_custom_field, NetSuiteCredential
 from .data_types import RecordRef
 from .data_types import ProductData, ProductAvailability
 from .data_types import PurchaseOrderData, PurchaseOrderLineData
 from .data_types import SaleOrderData, SaleOrderLineData
 from .data_types import ItemPicking, ItemMove
 from .data_types import InventoryAdjustment, InventoryAdjustmentLine
+from .data_types import RelationShip
 
 _logger = logging.getLogger(__name__)
 RT = TypeVar("RT", bound=RecordRef)
 R = TypeVar("R", bound=Any)
 
 
 class GsNetSuiteApi(abc.ABC, Generic[RT]):
@@ -136,15 +137,15 @@
 class BaseGsNetSuiteApi(GsNetSuiteApi[RT], abc.ABC):
     """
     Base d'implementation de l'API Netsuite.
     Permet d'avoir à surcgharcgher les informations particulieres des objets, mais pas chaque fonction d'appel.
     """
 
     _netsuite_ressource_name: str = None
-    """Champ a définir depuis la liste "RecordType" dans coreTpes.xsd de la wsdl"""
+    """Champ a définir depuis la liste "RecordType" dans coreTypes.xsd de la wsdl"""
 
     netsuite_api: NetSuiteSoapApi
     """Le client pour se connecter à l'API NetSuite"""
 
     def __init__(self, credential: "NetSuiteCredential", search_params: SearchParams = None):
         assert self._netsuite_ressource_name
         self._credential = credential
@@ -623,7 +624,31 @@
                 current_value=sub_el.currentValue,
                 adjust_qty_by=sub_el.adjustQtyBy,
                 new_quantity=sub_el.newQuantity,
                 inventory_detail=sub_el.inventoryDetail,
             )
             data.lines.append(line)
         return data
+
+
+class RelationShipAPI(BaseGsNetSuiteApi[RelationShip]):
+    _netsuite_ressource_name = "vendor"
+
+    def _get_criteria_created_since(self, created_since: datetime.datetime) -> Any:
+        raise NotImplementedError()
+
+    def search_record_type(self, **construc_kwargs) -> Any:
+        raise NotImplementedError()
+
+    def _column_search_selector(self) -> Any:
+        raise NotImplementedError()
+
+    def _default_criteria(self) -> Any:
+        raise NotImplementedError()
+
+    def _convert_to_data(self, record) -> RT:
+        return RelationShip(
+            internalId=record.internalId,
+            name=record.entityId,
+            company_name=record.companyName,
+            email=record.email or record.altEmail,
+        )
```

### Comparing `gs-netsuite-api-1.1.0/src/gs_netsuite_api/data_types.py` & `gs-netsuite-api-1.1.1/src/gs_netsuite_api/data_types.py`

 * *Files 5% similar despite different names*

```diff
@@ -23,14 +23,20 @@
 
     @staticmethod
     def from_rec_named(record) -> "RecordRef":
         return RecordRef(internalId=record.internalId, name=record.name)
 
 
 @dataclasses.dataclass
+class RelationShip(RecordRef):
+    company_name: str
+    email: str
+
+
+@dataclasses.dataclass
 class ProductData(RecordRef):
     """
     Classe contenant les champs "Catalogue" du fichier excel
     """
 
     ean13: str
     hs_code: str
```

### Comparing `gs-netsuite-api-1.1.0/src/gs_netsuite_api/ns_utils.py` & `gs-netsuite-api-1.1.1/src/gs_netsuite_api/ns_utils.py`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/src/gs_netsuite_api.egg-info/SOURCES.txt` & `gs-netsuite-api-1.1.1/src/gs_netsuite_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `gs-netsuite-api-1.1.0/wsdldownloader.py` & `gs-netsuite-api-1.1.1/wsdldownloader.py`

 * *Files identical despite different names*

