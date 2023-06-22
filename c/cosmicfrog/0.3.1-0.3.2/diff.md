# Comparing `tmp/cosmicfrog-0.3.1.tar.gz` & `tmp/cosmicfrog-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmicfrog-0.3.1.tar", last modified: Wed Jun 21 12:39:26 2023, max compression
+gzip compressed data, was "cosmicfrog-0.3.2.tar", last modified: Thu Jun 22 18:05:28 2023, max compression
```

## Comparing `cosmicfrog-0.3.1.tar` & `cosmicfrog-0.3.2.tar`

### file list

```diff
@@ -1,235 +1,234 @@
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.148215 cosmicfrog-0.3.1/
--rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-06-21 12:39:26.148215 cosmicfrog-0.3.1/PKG-INFO
--rw-r--r--   0 gordon    (1000) gordon    (1000)      486 2023-06-13 10:31:10.000000 cosmicfrog-0.3.1/README.md
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.124215 cosmicfrog-0.3.1/cosmicfrog/
--rw-r--r--   0 gordon    (1000) gordon    (1000)       93 2023-06-13 18:36:15.000000 cosmicfrog-0.3.1/cosmicfrog/__init__.py
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.124215 cosmicfrog-0.3.1/cosmicfrog/anura/
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.148215 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8022 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2629 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Analytics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5905 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2198 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10838 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6637 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6430 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13497 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17710 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12342 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18271 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6525 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13321 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18203 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Customers.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12984 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31026 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Facilities.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    23117 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7737 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13103 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7405 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13438 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13943 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4504 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11840 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5179 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Groups.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2401 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Histograms.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9384 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InputFactors.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    37919 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    39657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6883 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Lookups.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3239 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Maps.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5949 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    19168 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9656 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9469 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3602 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5317 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4329 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2583 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Organizations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6687 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2796 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Periods.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    28592 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Processes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26042 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12346 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15370 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14833 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16683 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3296 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13977 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12389 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12870 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13999 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15546 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13797 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Products.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7335 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12348 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15376 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18561 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3189 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3278 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4718 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2879 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5353 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4340 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Scenarios.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10685 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Shipments.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5798 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_StepCosts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4536 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6481 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5864 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11580 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Suppliers.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3162 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TableFilters.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16686 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18492 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9955 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9181 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    22940 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    21819 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32814 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    30886 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9956 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4705 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5569 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4111 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4092 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    25027 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6574 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13974 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15701 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7661 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18790 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18860 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10171 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkResources.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11935 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10784 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3526 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20156 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7056 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16396 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16803 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    21094 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7914 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    34222 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    22234 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9424 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6017 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10219 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17471 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12634 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4522 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10498 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5722 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4787 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6799 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14082 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16823 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6246 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    28983 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14164 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4063 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12557 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5709 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4864 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9345 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6767 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12537 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9475 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     1961 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7043 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    15917 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    17090 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    34065 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    33862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18726 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    18541 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7903 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    39373 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    40023 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20366 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    20172 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2128 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2969 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2411 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    55257 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    55033 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    32484 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7506 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7319 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    63682 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    63410 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26655 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    26664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10273 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10109 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6316 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4594 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8524 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8551 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4040 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7997 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12980 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    13007 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5341 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5368 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    60336 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    60255 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31510 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    31476 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     2944 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5725 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    10657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16391 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11893 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    11920 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3619 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     3646 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     7968 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6540 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6364 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12327 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6846 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6885 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6204 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8923 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     8950 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     5664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     4045 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6275 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     6302 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)     9631 2023-05-26 16:01:42.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.148215 cosmicfrog-0.3.1/cosmicfrog/anura/table_masterlists/
--rw-r--r--   0 gordon    (1000) gordon    (1000)    57001 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    25920 2023-06-07 11:19:52.000000 cosmicfrog-0.3.1/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12634 2023-06-20 15:52:31.000000 cosmicfrog-0.3.1/cosmicfrog/frog_data copy.py
--rw-r--r--   0 gordon    (1000) gordon    (1000)    12277 2023-06-21 12:34:29.000000 cosmicfrog-0.3.1/cosmicfrog/frog_data.py
--rw-r--r--   0 gordon    (1000) gordon    (1000)      288 2023-04-14 21:19:53.000000 cosmicfrog-0.3.1/cosmicfrog/frog_excel.py
--rw-r--r--   0 gordon    (1000) gordon    (1000)     1534 2023-05-24 15:31:30.000000 cosmicfrog-0.3.1/cosmicfrog/frog_log.py
-drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-21 12:39:26.124215 cosmicfrog-0.3.1/cosmicfrog.egg-info/
--rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-06-21 12:39:26.000000 cosmicfrog-0.3.1/cosmicfrog.egg-info/PKG-INFO
--rw-r--r--   0 gordon    (1000) gordon    (1000)    16531 2023-06-21 12:39:26.000000 cosmicfrog-0.3.1/cosmicfrog.egg-info/SOURCES.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)        1 2023-06-21 12:39:26.000000 cosmicfrog-0.3.1/cosmicfrog.egg-info/dependency_links.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)      114 2023-06-21 12:39:26.000000 cosmicfrog-0.3.1/cosmicfrog.egg-info/requires.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)       11 2023-06-21 12:39:26.000000 cosmicfrog-0.3.1/cosmicfrog.egg-info/top_level.txt
--rw-r--r--   0 gordon    (1000) gordon    (1000)       38 2023-06-21 12:39:26.148215 cosmicfrog-0.3.1/setup.cfg
--rw-r--r--   0 gordon    (1000) gordon    (1000)      899 2023-06-21 12:39:12.000000 cosmicfrog-0.3.1/setup.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.150497 cosmicfrog-0.3.2/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-06-22 18:05:28.150497 cosmicfrog-0.3.2/PKG-INFO
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      486 2023-06-13 10:31:10.000000 cosmicfrog-0.3.2/README.md
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.126497 cosmicfrog-0.3.2/cosmicfrog/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       93 2023-06-13 18:36:15.000000 cosmicfrog-0.3.2/cosmicfrog/__init__.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.126497 cosmicfrog-0.3.2/cosmicfrog/anura/
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.150497 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8022 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2629 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Analytics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5905 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2198 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10838 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BusinessHours.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6637 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6430 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13497 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17710 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12342 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18271 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6525 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13321 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18203 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Customers.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12984 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31026 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Facilities.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    23117 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7737 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13103 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7405 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13438 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13943 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4504 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11840 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5179 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Groups.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2401 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Histograms.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9384 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InputFactors.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    37919 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    39657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6883 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Lookups.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3239 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Maps.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5949 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelInfo.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7320 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    19168 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelSettings.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9656 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9469 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3602 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5317 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4329 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2583 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Organizations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6687 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OutputFactors.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2796 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Periods.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    28592 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Processes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26042 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12346 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15370 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14833 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16683 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3296 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13977 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12389 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12870 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13999 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15546 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13797 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Products.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7335 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12348 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15376 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18561 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3189 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3278 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4718 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2879 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5353 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4340 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Scenarios.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10685 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Shipments.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5798 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_StepCosts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4536 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6481 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5864 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11580 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Suppliers.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3162 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TableFilters.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16686 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18492 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9955 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9181 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    22940 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationModes.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    21819 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32814 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    30886 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9956 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationRates.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4705 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5569 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4111 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4092 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3647 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    25027 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6574 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13974 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15701 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7661 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18790 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenters.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18860 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10171 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkResources.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11935 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10784 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3526 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20156 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7056 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16396 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16803 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    21094 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7914 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    34222 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    22234 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9424 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6017 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10219 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17471 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12634 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9490 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4522 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10498 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5722 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4787 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6799 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14082 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16823 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6246 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    28983 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14164 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4063 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12557 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5709 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4864 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9345 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6767 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12537 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9475 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     1961 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6460 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7043 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    15917 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    17090 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    34065 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    33862 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18726 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    18541 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7903 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7715 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    39373 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    40023 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20366 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    20172 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2128 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2969 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2411 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    55257 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    55033 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32669 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    32484 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7506 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7319 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    63682 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    63410 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26655 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    26664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    14419 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10273 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10109 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6316 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4594 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8524 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8551 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4040 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7970 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7997 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12980 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13007 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5341 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5368 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    60336 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    60255 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31510 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    31476 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     2944 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5725 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5764 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    10657 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16391 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11893 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    11920 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3619 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     3646 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     7968 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6540 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6364 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    12327 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6846 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6885 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6204 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6263 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8923 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     8950 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     5664 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     4045 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6275 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     6302 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9604 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     9631 2023-05-26 16:01:42.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.150497 cosmicfrog-0.3.2/cosmicfrog/anura/table_masterlists/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    57001 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    25920 2023-06-07 11:19:52.000000 cosmicfrog-0.3.2/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    13791 2023-06-22 18:02:57.000000 cosmicfrog-0.3.2/cosmicfrog/frog_data.py
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      288 2023-04-14 21:19:53.000000 cosmicfrog-0.3.2/cosmicfrog/frog_excel.py
+-rw-r--r--   0 gordon    (1000) gordon    (1000)     1502 2023-06-22 17:23:48.000000 cosmicfrog-0.3.2/cosmicfrog/frog_log.py
+drwxr-xr-x   0 gordon    (1000) gordon    (1000)        0 2023-06-22 18:05:28.126497 cosmicfrog-0.3.2/cosmicfrog.egg-info/
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      352 2023-06-22 18:05:28.000000 cosmicfrog-0.3.2/cosmicfrog.egg-info/PKG-INFO
+-rw-r--r--   0 gordon    (1000) gordon    (1000)    16502 2023-06-22 18:05:28.000000 cosmicfrog-0.3.2/cosmicfrog.egg-info/SOURCES.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)        1 2023-06-22 18:05:28.000000 cosmicfrog-0.3.2/cosmicfrog.egg-info/dependency_links.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      114 2023-06-22 18:05:28.000000 cosmicfrog-0.3.2/cosmicfrog.egg-info/requires.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       11 2023-06-22 18:05:28.000000 cosmicfrog-0.3.2/cosmicfrog.egg-info/top_level.txt
+-rw-r--r--   0 gordon    (1000) gordon    (1000)       38 2023-06-22 18:05:28.150497 cosmicfrog-0.3.2/setup.cfg
+-rw-r--r--   0 gordon    (1000) gordon    (1000)      899 2023-06-22 17:59:45.000000 cosmicfrog-0.3.2/setup.py
```

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_AdvancedQueueingDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Analytics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Analytics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BillsOfMaterials.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BusinessCalendars.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_BusinessHours.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_BusinessHours.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ChangeoverTimes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomSimulationScripts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerFulfillmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomerTransitConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Customers.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Customers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_CustomersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Facilities.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Facilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityDemand.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FacilityRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FlowConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_FlowCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GeographicRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GreenfieldServiceBands.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_GreenfieldSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Groups.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Groups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Histograms.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Histograms.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InputFactors.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_InventoryPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Lookups.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Lookups.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Maps.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Maps.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelInfo.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelInfo.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelRunOptions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ModelSettings.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ModelSettings.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_NetworkRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderFulfillmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderProfileProductAffinity.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderProfileProductSelection.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OrderedProductSubstitution.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Organizations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Organizations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_OutputFactors.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_OutputFactors.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Periods.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Periods.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Processes.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Processes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcessesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProcurementPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductUnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductionPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Products.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Products.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ProductsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrderProfiles.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentOrders.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ReplenishmentPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskBandDefinitions.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskRatingConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_RiskSummaryConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ScenarioItemAssignments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_ScenarioItems.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Scenarios.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Scenarios.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SequentialObjectives.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Shipments.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Shipments.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_StepCosts.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_StepCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierCapabilities.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierCapabilitiesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SupplierRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_Suppliers.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_Suppliers.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_SuppliersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TableFilters.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TableFilters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationAssets.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationAssetsMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationLaneModeQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationLaneQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationModes.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationModes.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationModesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_TransportationRates.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_TransportationRates.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UnitsOfMeasure.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedCosts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedForecasts.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedForecastsData.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UserDefinedVariables.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_UtilizationRiskConfigurations.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WarehousingPolicies.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WarehousingPoliciesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenterCountConstraints.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenterQueueDetails.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCenters.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCenters.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkCentersMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkResources.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkResources.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/anura_WorkResourcesMultiTimePeriod.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationBillsOfMaterialSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationConstraintSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeParentInformationReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationDemandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilityCostToServeSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldServiceBandSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationGreenfieldSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationInventorySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationProductionSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSequentialObjectiveSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationShipmentSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationSupplySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedCostSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUserDefinedVariableSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationUtilizationRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationWarehousingSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_OptimizationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationCustomerSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmInputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmOutputFactorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationEvolutionaryAlgorithmSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilityServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFacilitySummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFlowSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationFlowSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationGeographicRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationInventoryOnHandReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneModeQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationLaneSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkServiceSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationNetworkSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderFulfillmentQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationOrderReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProcessSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationProductionReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationRiskMetricsSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationShipmentReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierProductSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetrics.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierRiskMetricsReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationSupplierSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationValidationErrorReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueDepthReport.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterQueueSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummary.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_definitions/output_SimulationWorkCenterSummaryReplicationDetail.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_masterlists/anuraMasterTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json` & `cosmicfrog-0.3.2/cosmicfrog/anura/table_masterlists/anuraOutputTableList.json`

 * *Files identical despite different names*

### Comparing `cosmicfrog-0.3.1/cosmicfrog/frog_data copy.py` & `cosmicfrog-0.3.2/cosmicfrog/frog_data.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 import pandas as pd
 import numpy as np
 import json
 import os
 import sqlalchemy
-from sqlalchemy import text, MetaData, inspect
-from sqlalchemy.engine import Engine
+from sqlalchemy import text, inspect
+from contextlib import contextmanager
 from psycopg2 import sql
 import uuid
 from io import StringIO
 from typing import Type
 from collections.abc import Iterable
 import pkg_resources
 
 from .frog_log import get_logger
 
-# Questions: 
-# How to support feedback in CF UI?
-
 # TODO: 
-# Will need extending to support custom columns in Anura tables
+# How to support feedback in CF UI?
 # Will need extensions for custom tables in a model
 # Profile parallel write for xlsx
-# Test sql injection
 # Add batching to standard table writing
 
 # Define chunk size (number of rows to write per chunk)
-UPSERT_CHUNK_SIZE = 10000
+UPSERT_CHUNK_SIZE = 100000
 
 MASTER_LIST_PATH = 'anura/table_masterlists/anuraMasterTableList.json'
 TABLES_DIR = 'anura/table_definitions'
 
 class ValidationError(Exception):
     """Exception raised for validation errors.
 
@@ -85,94 +81,165 @@
             frog_model.anura_keys[table_name] = pk_columns
 
 
     def __init__(self, connection_string: str = None, engine: sqlalchemy.engine.Engine = None) -> None:
 
         self.engine = None
         self.connection = None
-        self.transaction = None
+        self.transactions = [] 
         self.log = get_logger()
 
         # One time read in of Anura data
         if not frog_model.anura_tables:
             self.log.info("Reading Anura schema")
             frog_model._read_anura()
 
         # Initialise connection
         if engine is not None:
             self.engine = engine
         elif connection_string is not None:
             self.engine = sqlalchemy.create_engine(connection_string, connect_args={'connect_timeout': 15}) 
 
-        if self.engine is not None:
-            self.connection = self.engine.connect()
-
+    
+    def __enter__(self):
+        self.start_transaction()
+        return self
+
+    def __exit__(self, exc_type, exc_val, exc_tb):
+        if exc_type is None:
+            # No exceptions occurred, so commit the transaction
+            self.commit_transaction()
+        else:
+            # An exception occurred, so roll back the transaction
+            self.rollback_transaction()
 
+    # Note: The following are for user managed transactions (do not use for library internal transactions)
     def start_transaction(self):
-        assert(self.connection is not None)
-        self.transaction = self.connection.begin()
-
+        if self.connection is None:
+            self.connection = self.engine.connect()
+        
+        if self.transactions:
+            self.transactions.append(self.connection.begin_nested())
+        else:
+            self.transactions.append(self.connection.begin())
 
     def commit_transaction(self):
-        self.transaction.commit()
-        self.transaction = None
+        if self.transactions:
+            transaction = self.transactions.pop()
+            transaction.commit()
+
+            if not self.transactions:
+                self.connection.close()
+                self.connection = None
 
 
     def rollback_transaction(self):
-        self.transaction.rollback()
-        self.transaction = None
+        if self.transactions:
+            transaction = self.transactions.pop()
+            transaction.rollback()
+
+            if not self.transactions:
+                self.connection.close()
+                self.connection = None
+
+    @contextmanager
+    def begin(self):
+
+        connection = None
+        try:
+            # Decide the context based on the transaction state
+            if self.transactions: # If user has opened a transaction, then nest one
+                connection = self.transactions[-1].connection
+                transaction = connection.begin_nested()
+            else: # else start a new one
+                connection = self.engine.connect()
+                transaction = connection.begin()
+            
+            yield connection  # yield the connection, not the transaction
 
+            transaction.commit()  # commit the transaction if everything goes well
 
+        except Exception:
+            transaction.rollback()
+            raise
+        finally:
+            # If the connection was created in this method, close it.
+            if not self.transactions:
+                connection.close()
+
+    # Dump data to a model table
     def write_table(self, table_name: str, data: pd.DataFrame | Iterable):
-        
+        """
+        This pushes data into a model table from a data frame or iterable object
+
+        Parameters:
+        table_name (str): The target table
+        data: The data to be written
+
+        Returns:
+        None
+        """
+
+        table_name = table_name.lower().strip()
+
         self.log.info("Writing table: " + table_name)
 
         if isinstance(data, pd.DataFrame) == False:
             data = pd.DataFrame(data)
 
+        data.columns = data.columns.str.lower().map(str.strip)
+
         # Initial implementation - pull everything into a df and dump with to_sql
-        data.to_sql(table_name, con=self.engine, if_exists="append", index=False)
+        with self.begin() as connection:
+            data.to_sql(table_name, con=connection, if_exists="append", index=False)
 
         # Note: tried a couple of ways to dump the generator rows directly, but didn't
         # give significant performance over dataframe (though may be better for memory)
         # Decided to leave as is for now 
 
-
+    # Read a model table to dataframe
     def read_table(self, table_name: str):
-        return pd.read_sql(table_name, self.engine)
+        
+        table_name = table_name.lower().strip()
+
+        with self.begin() as connection:
+            return pd.read_sql(table_name, con = connection)
 
-    def clear_table(self, table):
+    # Clear a model table
+    def clear_table(self, table_name : str):
 
-        assert(self.connection is not None)
+        table_name = table_name.lower().strip()
 
         # delete any existing data data from the table
-        self.connection.execute(text("delete from " + table))
+        self.exec_sql("delete from " + table_name)
 
         return True
 
-    def exec_sql(self, sql: str):
-
-        assert(self.connection is not None)
+    # Read from model using raw sql query
+    def read_sql(self, query: str):
 
-        self.connection.execute(text(sql))
+        with self.begin() as connection:
+            return pd.read_sql_query(query, connection)
 
-    def get_dataframe(self, sql: str):
+    # Execute raw sql on model
+    def exec_sql(self, query: str | sql.Composed):
 
-        return pd.read_sql_query(sql, self.engine)
+        with self.begin() as connection:
+            connection.execute(text(query))
 
-    # Upsert from a file
+    # Upsert from a csv file to a model table
     def upsert_csv(self, table_name: str, filename: str):
 
         for chunk in pd.read_csv(filename, chunksize=UPSERT_CHUNK_SIZE, dtype=str, skipinitialspace=True):
-            chunk.columns = chunk.columns.str.lower().map(str.strip)
+
             chunk.replace("", np.nan, inplace=True)
             self.upsert(table_name, chunk)
             break
 
-    # Upsert from an xls
+    # Upsert from an xls file to a model table
     def upsert_excel(self, filename: str):
 
         # TODO: If an issue could consider another way to load/stream from xlsx maybe?
 
         xls = pd.ExcelFile(filename)
 
         # For each sheet in the file
@@ -184,168 +251,147 @@
             df.columns = df.columns.str.lower().map(str.strip)
 
             for i in range(0, len(df), UPSERT_CHUNK_SIZE):
                 chunk = df[i:i+UPSERT_CHUNK_SIZE]
                 chunk.replace("", np.nan, inplace=True)
                 self.upsert(sheet_name, chunk)
 
-    # Upsert from a dataframe
-    def upsert(self, table_name: str, data: pd.DataFrame | Iterable):
 
-        print ("upsert called")
+    def __get_table_columns(self, table_name: str):
+        
+        # Create an Inspector object
+        inspector = inspect(self.engine)
+
+        # Get the column names for a specific table
+        column_names = inspector.get_columns(table_name)
+        
+        column_names = [column['name'] for column in column_names]
+
+        return [name.lower().strip() for name in column_names]
 
-        # TODO: Not sure what validation to do here
-        # TODO: Anura only, or custom tables?  (can pass in keys for those)
-        # TODO: Custom columns and how to handle
-        # TODO: up front validation, what are the rules?
+
+    # Upsert from a dataframe
+    def upsert(self, table_name: str, data: pd.DataFrame):
 
         table_name = table_name.strip().lower()
 
+        data.columns = data.columns.str.lower().map(str.strip)
+
         if table_name not in frog_model.anura_tables:
             #Skip it
             self.log.warning(f"""Worksheet name not recognised as Anura table (skipping): {table_name}""")
             return
 
         self.log.info(f"""Importing worksheet to table: {table_name}""")   
+        self.log.info(f"""Inserting {len(data)} rows""")
 
-        #TODO: Will need more code for handling custom columns here, behavior should be:
+        # Behavior rules:
         # Key columns - get used to match (Note: possible future requirement, some custom columns may also be key columns)
         # Other Anura columns - get updated
         # Other Custom columns - get updated
         # Other columns (neither Anura or Custom) - get ignored
 
-        # Skipping unrecognised rows (note: does not support custom columns yet)
+        all_column_names = self.__get_table_columns(table_name)
+        if "id" in all_column_names:
+            all_column_names.remove("id")
+
+        # TODO: Seperate out:
+        # 1) Anura key cols
+        # 2) Custom key cols
+        # 3) Update cols
+        # Cleanup below (by using table and filtering input can avoid using input cols, so make safe easier)
+
+        anura_key_columns = frog_model.anura_keys[table_name]
+        custom_key_columns = [] # This is for later
+        combined_key_columns = anura_key_columns + custom_key_columns
+        update_columns = [col for col in all_column_names if col not in combined_key_columns]
+
+
+        # Skipping unrecognised rows (Do not trust column names from user data)
+        cols_to_drop = [col for col in data.columns if col not in all_column_names]
 
-        self.log.info(f"""Found {len(frog_model.anura_cols[table_name])} columns""")
 
-        cols_to_drop = [col for col in data.columns if col not in frog_model.anura_cols[table_name]]
         for col in cols_to_drop:
             self.log.info(f"""Skipping unknown column: {col}""")
-        data.drop(cols_to_drop, axis=1, inplace=True)
+        data = data.drop(cols_to_drop, axis=1)
          
-        key_columns = frog_model.anura_keys[table_name]
-        non_key_columns = [col for col in data.columns if col not in key_columns]
-        all_columns = key_columns + non_key_columns
-
-        assert(self.connection is not None)
 
-        temp_table_name = "temp_table_" + str(uuid.uuid4()).replace('-', '')
-
-        with self.engine.begin() as connection:
-        
-            self.log.info(f"""Moving data to temporary table: {temp_table_name}""")   
+        # Want to either make a transaction, or a nested transaction depending on the presence or absense
+        # of a user transaction (if one exists then nest another, else create a root)
+        with self.begin() as connection:
 
             # Create temporary table
+            temp_table_name = "temp_table_" + str(uuid.uuid4()).replace('-', '')
+            self.log.info(f"""Moving data to temporary table: {temp_table_name}""") 
+
             # Note: this will also clone custom columns
-            create_temp_table_sql = text(f"""
+            create_temp_table_sql = f"""
                 CREATE TEMPORARY TABLE {temp_table_name} AS
                 SELECT *
                 FROM {table_name}
                 WITH NO DATA;
-                """)
+                """
             
-            connection.execute(create_temp_table_sql)   
+            connection.execute(text(create_temp_table_sql))
 
             # Copy data from df to temporary table
             copy_sql = sql.SQL("COPY {table} ({fields}) FROM STDIN WITH (FORMAT CSV, HEADER TRUE)").format(
                 table=sql.Identifier(temp_table_name),
                 fields=sql.SQL(', ').join(map(sql.Identifier, data.columns))
             )
-
+       
             cursor = connection.connection.cursor()
             cursor.copy_expert(copy_sql, StringIO(data.to_csv(index=False)))
             del data
             self.log.info(f"""Temporary table populated.""")   
 
-
-            # Get all columns from the target table directly (allowing for custom columns)
-            metadata = MetaData()
-
-            # Create an Inspector object
-            inspector = inspect(self.engine)
-
-            # Get the column names for a specific table
-            column_names = inspector.get_columns(table_name)
-            target_table_column_names = [column['name'] for column in column_names]
-
-            # Print the column names
-            print("Target columns: {0}".format(target_table_column_names))
-
-            target_table_column_names.remove("id")
-
             # Now upsert from temporary table to final table
 
             # Note: Looked at ON CONFLICT for upsert here, but seems not possible without defining constraints on target table
             # so doing insert and update separately
 
-            # Note: For SQL injection, columns here are from Anura, also target table name. Temp table name is above.
-            # non_key_columns are vulnerable (from import) so protected
-
-            # Do not trust column names from user:
-            safe_all_columns_list = sql.SQL(", ").join([sql.Identifier(col_name) for col_name in all_columns])
-            safe_update_column_clause = sql.SQL(", ").join([sql.SQL('{0} = {1}.{0}').format(sql.Identifier(col_name), sql.Identifier(temp_table_name)) for col_name in non_key_columns])
-
-            if key_columns:
-
-                placeholder = "{0}"
+            all_columns_list = ", ".join([f'"{col_name}"' for col_name in all_column_names])
 
-                ############## UPDATE
+            if combined_key_columns:
 
-                update_key_condition = " AND ".join([f"{table_name}.{key_col} = {temp_table_name}.{key_col}" for key_col in key_columns])
+                update_column_list = ", ".join([f'"{col_name}" = "{temp_table_name}"."{col_name}"' for col_name in update_columns])
+                key_condition = " AND ".join([f'"{table_name}"."{key_col}" IS NOT DISTINCT FROM "{temp_table_name}"."{key_col}"' for key_col in combined_key_columns])
 
-                update_query = sql.SQL(f"""
+                update_query = f"""
                     UPDATE {table_name}
-                    SET {placeholder}
+                    SET {update_column_list}
                     FROM {temp_table_name}
-                    WHERE {update_key_condition}
-                """).format(safe_update_column_clause)
+                    WHERE {key_condition}
+                """
 
-                self.log.info(f"""Running (upsert) update query.""")  
+                self.log.info(f"""Running (upsert) update query.""")    
                 cursor.execute(update_query)
                 updated_rows = cursor.rowcount
 
-
-                ############## INSERT
-
-                # insert_query = sql.SQL(f"""
-                #     INSERT INTO {table_name} ({placeholder})
-                #     SELECT {placeholder} FROM {temp_table_name}
-                #     WHERE NOT EXISTS (
-                #         SELECT 1 FROM {table_name}
-                #         WHERE {key_condition}
-                #     )
-                # """).format(safe_all_columns_list)
-
-                select_columns = ', '.join([f'{col}' for col in target_table_column_names])
-                temp_select_columns = ', '.join([f'temp.{col}' for col in target_table_column_names])
-                key_condition = " AND ".join([f"main.{key_col} = temp.{key_col}" for key_col in key_columns])
-                null_condition = " AND ".join([f"main.{key_col} IS NULL" for key_col in key_columns])
-
-                insert_query = sql.SQL(f"""
-                    INSERT INTO {table_name} ({select_columns})
-                    SELECT {temp_select_columns} FROM {temp_table_name} AS temp
-                    LEFT JOIN {table_name} AS main ON {key_condition}
-                    WHERE {null_condition}
-                """).format(safe_all_columns_list)
-
-
+                insert_query = f"""
+                    INSERT INTO {table_name} ({all_columns_list})
+                    SELECT {all_columns_list} FROM {temp_table_name}
+                    WHERE NOT EXISTS (
+                        SELECT 1 FROM {table_name}
+                        WHERE {key_condition}
+                    )
+                """
 
                 self.log.info(f"""Running (upsert) insert query.""")  
                 cursor.execute(insert_query)
                 inserted_rows = cursor.rowcount 
 
             else:
-                self.log.info(f"""Running insert query.""")  
-                insert_query = sql.SQL(f"""
-                    INSERT INTO {table_name} ({placeholder})
-                    SELECT {placeholder} FROM {temp_table_name}
-                """).format(safe_all_columns_list)
+                insert_query = f"""
+                    INSERT INTO {table_name} ({all_columns_list})
+                    SELECT {all_columns_list}
+                    FROM {temp_table_name}
+                """
                 
                 updated_rows = 0
+                self.log.info(f"""Running insert query.""")
                 cursor.execute(insert_query)
                 inserted_rows = cursor.rowcount 
-                
-                connection.execute(insert_query)
 
         #TODO: Could return this?
         self.log.info("Updated rows  = {}".format(updated_rows))
         self.log.info("Inserted rows = {}".format(inserted_rows))
```

### Comparing `cosmicfrog-0.3.1/cosmicfrog/frog_log.py` & `cosmicfrog-0.3.2/cosmicfrog/frog_log.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,37 +10,36 @@
 def get_logger(console_only=False):
 
     global app_logger
 
     current_pid = str(os.getpid())
 
     if current_pid in app_logger:
-        print("returning existing logger " + current_pid)
+        #print("returning existing logger " + current_pid)
         return app_logger[current_pid]
     else:
         log_level = os.getenv("FROG_LOG_LEVEL") or logging.DEBUG
         log_level = int(log_level)
-        print(log_level)
+        #print(log_level)
 
         logger = logging.getLogger(current_pid)
         app_logger[current_pid] = logger
 
         # Add log to Insights
         if not console_only:
-            print("Logging to Azure Insights")
+            #print("Logging to Azure Insights")
             if os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING") is not None:
                 logger.addHandler(AzureLogHandler(connection_string=os.getenv("APPLICATIONINSIGHTS_CONNECTION_STRING")))
             else:
                 print("APPLICATIONINSIGHTS_CONNECTION_STRING is not configured")
 
         # Add log to console
-        print("Logging to console")
         stdhandler = logging.StreamHandler(sys.stdout)
         stdhandler.setLevel(log_level)
         formatter = logging.Formatter('%(asctime)s - %(name)s - %(levelname)s - %(message)s')
         stdhandler.setFormatter(formatter)
         logger.addHandler(stdhandler)
 
         logger.setLevel(log_level)
-        print("created logger for pid " + current_pid)
+        #print("created logger for pid " + current_pid)
 
     return logger
```

### Comparing `cosmicfrog-0.3.1/cosmicfrog.egg-info/SOURCES.txt` & `cosmicfrog-0.3.2/cosmicfrog.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 README.md
 setup.py
 cosmicfrog/__init__.py
-cosmicfrog/frog_data copy.py
 cosmicfrog/frog_data.py
 cosmicfrog/frog_excel.py
 cosmicfrog/frog_log.py
 cosmicfrog.egg-info/PKG-INFO
 cosmicfrog.egg-info/SOURCES.txt
 cosmicfrog.egg-info/dependency_links.txt
 cosmicfrog.egg-info/requires.txt
```

### Comparing `cosmicfrog-0.3.1/setup.py` & `cosmicfrog-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 setup(
     name="cosmicfrog",
     
     include_package_data=True,
 
-    version="0.3.1",
+    version="0.3.2",
     description='Helpful utilities for working with Cosmic Frog models',
     url='https://cosmicfrog.com',
     author='Optilogic',
     packages=['cosmicfrog'],
     package_data={
         'cosmicfrog': ['anura/table_definitions/*.json',
                         'anura/table_masterlists/*.json'
                        ],
     },
     license='MIT',
     install_requires=[
         'numpy>=1.21.0',
-        'pandas>=1.3.0',
+        'pandas>=2.0.0',
         'psycopg2-binary>=2.9.6',
         'sqlalchemy',
         'opencensus-ext-azure>=1.1.7',
         'openpyxl',
         'optilogic>=2.5',
     ],
     classifiers=[
```

