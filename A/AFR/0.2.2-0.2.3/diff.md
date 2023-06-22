# Comparing `tmp/AFR-0.2.2.tar.gz` & `tmp/AFR-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/AFR-0.2.2.tar", last modified: Sat Mar 25 14:18:19 2023, max compression
+gzip compressed data, was "dist/AFR-0.2.3.tar", last modified: Thu Jun 22 05:28:57 2023, max compression
```

## Comparing `AFR-0.2.2.tar` & `AFR-0.2.3.tar`

### file list

```diff
@@ -1,40 +1,16 @@
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.750142 AFR-0.2.2/
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.741842 AFR-0.2.2/AFR/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      815 2023-03-25 14:17:44.000000 AFR-0.2.2/AFR/__init__.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      956 2023-03-23 18:06:27.000000 AFR-0.2.2/AFR/adjr2_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      997 2023-03-23 17:39:30.000000 AFR-0.2.2/AFR/aic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1011 2023-03-23 17:39:47.000000 AFR-0.2.2/AFR/bic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2112 2023-03-23 17:57:07.000000 AFR-0.2.2/AFR/check_betas.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2302 2023-03-22 14:08:47.000000 AFR-0.2.2/AFR/checkdata.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     2165 2023-03-23 10:29:48.000000 AFR-0.2.2/AFR/corsel.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      768 2023-03-23 16:57:47.000000 AFR-0.2.2/AFR/dec_plot.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      298 2023-03-25 14:06:07.000000 AFR-0.2.2/AFR/finratKZ.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      275 2023-03-25 14:06:07.000000 AFR-0.2.2/AFR/macroKZ.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1225 2023-03-23 14:36:17.000000 AFR-0.2.2/AFR/opt_size.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1331 2023-03-20 10:35:47.000000 AFR-0.2.2/AFR/pt_multi.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1171 2023-03-20 10:23:59.000000 AFR-0.2.2/AFR/pt_one.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1275 2023-03-23 16:54:05.000000 AFR-0.2.2/AFR/reg_test.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     3852 2023-03-20 06:19:52.000000 AFR-0.2.2/AFR/regsel_f.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1039 2023-03-23 17:41:23.000000 AFR-0.2.2/AFR/sbic_score.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      962 2023-03-06 09:18:06.000000 AFR-0.2.2/AFR/vif_reg.py
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13441 2023-03-25 12:01:16.000000 AFR-0.2.2/AFR manual.md
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.743624 AFR-0.2.2/AFR.egg-info/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13849 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      669 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/SOURCES.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/dependency_links.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/requires.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)        4 2023-03-25 14:18:19.000000 AFR-0.2.2/AFR.egg-info/top_level.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.2/LICENSE.rtf
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      111 2023-03-25 13:53:52.000000 AFR-0.2.2/MANIFEST.in
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13849 2023-03-25 14:18:19.749833 AFR-0.2.2/PKG-INFO
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.2/example_process.ipynb
-drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-03-25 14:18:19.748867 AFR-0.2.2/load/
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    62368 2023-02-28 05:06:29.000000 AFR-0.2.2/load/finratKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    10137 2023-02-28 06:28:15.000000 AFR-0.2.2/load/finratKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1843 2023-03-15 10:12:56.000000 AFR-0.2.2/load/finratKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    18665 2023-03-01 15:07:14.000000 AFR-0.2.2/load/macroKZ.csv
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)    13295 2023-02-27 21:25:57.000000 AFR-0.2.2/load/macroKZ_dataset.html
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)     4178 2023-02-27 21:25:57.000000 AFR-0.2.2/load/macroKZ_dataset.rst
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      133 2023-03-25 05:55:12.000000 AFR-0.2.2/requirements.txt
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-03-25 14:18:19.750238 AFR-0.2.2/setup.cfg
--rw-r--r--   0 aluamakhmetova   (501) staff       (20)      981 2023-03-25 14:17:23.000000 AFR-0.2.2/setup.py
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-22 05:28:57.981857 AFR-0.2.3/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-22 05:28:57.969461 AFR-0.2.3/AFR/
+drwxr-xr-x   0 aluamakhmetova   (501) staff       (20)        0 2023-06-22 05:28:57.980683 AFR-0.2.3/AFR/AFR.egg-info/
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-22 05:28:57.000000 AFR-0.2.3/AFR/AFR.egg-info/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      239 2023-06-22 05:28:57.000000 AFR-0.2.3/AFR/AFR.egg-info/SOURCES.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-22 05:28:57.000000 AFR-0.2.3/AFR/AFR.egg-info/dependency_links.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       87 2023-06-22 05:28:57.000000 AFR-0.2.3/AFR/AFR.egg-info/requires.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)        1 2023-06-22 05:28:57.000000 AFR-0.2.3/AFR/AFR.egg-info/top_level.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14541 2023-06-19 13:01:26.000000 AFR-0.2.3/AFR manual.md
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)     1878 2023-03-25 06:06:59.000000 AFR-0.2.3/LICENSE.rtf
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      126 2023-06-12 09:46:50.000000 AFR-0.2.3/MANIFEST.in
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)    14949 2023-06-22 05:28:57.981348 AFR-0.2.3/PKG-INFO
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)   105732 2023-03-25 08:12:22.000000 AFR-0.2.3/example_process.ipynb
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      159 2023-06-16 09:24:14.000000 AFR-0.2.3/requirements.txt
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)       38 2023-06-22 05:28:57.982004 AFR-0.2.3/setup.cfg
+-rw-r--r--   0 aluamakhmetova   (501) staff       (20)      959 2023-06-12 11:04:17.000000 AFR-0.2.3/setup.py
```

### Comparing `AFR-0.2.2/AFR manual.md` & `AFR-0.2.3/AFR/AFR.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: AFR
+Version: 0.2.3
+Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
+Home-page: https://github.com/AFRKZ/AFR
+Author: Timur Abilkassymov, Alua Makhmetova
+Author-email: alua.makhmetova@gmail.com
+License: 3-clause BSD
+Description-Content-Type: text/markdown
+License-File: LICENSE.rtf
+
 # Package ‘AFR’
 
 
 Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data.
 
 It was designed by the team of the Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market (ARDFM).
 
@@ -31,15 +42,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -72,98 +83,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -318,14 +329,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/AFR.egg-info/PKG-INFO` & `AFR-0.2.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AFR
-Version: 0.2.2
+Version: 0.2.3
 Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
 Home-page: https://github.com/AFRKZ/AFR
 Author: Timur Abilkassymov, Alua Makhmetova
 Author-email: alua.makhmetova@gmail.com
 License: 3-clause BSD
 Description-Content-Type: text/markdown
 License-File: LICENSE.rtf
@@ -42,15 +42,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -83,98 +83,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -329,14 +329,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/LICENSE.rtf` & `AFR-0.2.3/LICENSE.rtf`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/PKG-INFO` & `AFR-0.2.3/AFR manual.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: AFR
-Version: 0.2.2
-Summary: Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data
-Home-page: https://github.com/AFRKZ/AFR
-Author: Timur Abilkassymov, Alua Makhmetova
-Author-email: alua.makhmetova@gmail.com
-License: 3-clause BSD
-Description-Content-Type: text/markdown
-License-File: LICENSE.rtf
-
 # Package ‘AFR’
 
 
 Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data.
 
 It was designed by the team of the Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market (ARDFM).
 
@@ -42,15 +31,15 @@
 ## Datasets
 
   
 AFR has built-in datasets named _macroKZ_ and _finratKZ_ that were gathered by the ARDFM team. More details below.
   
 ## finratKZ dataset
 
-Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated financial ratios.
+Dataset *finratKZ* was gathered during the supervisory procedure of the banking sector of Kazakhstan. ARDFM team analyzed financial statements of the corporate borrowers and calculated 29 financial ratios.
 
 The data was collected during regular supervisory asset quality review(AQR) procedure. During the AQR corporate borrowers were classified as default and standard (IFRS stage 1).
 
 **Dataset contains following data** :
 
 - **Default** - Dummy variable where 0 - standard(IFRS stage 1) borrower, 1 - default borrower
 - **Rev_gr** - Revenue growth rate
@@ -83,98 +72,98 @@
 - **FA** - Fixed assets turnover
 - **WC** - Working capital turnover
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    finrat = pd.read_csv('./finratKZ.csv')
+    import AFR
+    finrat = load_finratKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.
   
   
 ## macroKZ dataset
 
 The dataset was gathered by the ARDFM based on Kazakhstan' official and public data from the [Bureau of National Statistics](https://stat.gov.kz/).
 
-The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 50 quarters of 2010-2022 period.
+The dataset contains 50 historic macroeconomic and 10 hypothetical financial data over 52 quarters of 2010-2022 period.
 
 The *macroKZ* dataset will be updated periodically as the official statistical information is released.
 
 **Dataset contains following data** :
 
-- **real_gdp** Real GDP
-- **GDD_Agr_R** Real gross value added Agriculture
-- **GDD_Min_R** Real gross value added Mining
-- **GDD_Man_R** Real gross value added Manufacture
-- **GDD_Elc_R** Real gross value added Electricity
-- **GDD_Con_R** Real gross value added Construction
-- **GDD_Trd_R** Real gross value added Trade
-- **GDD_Trn_R** Real gross value added Transportation
-- **GDD_Inf_R** Real gross value added Information
-- **GDD_Est_R** Real gross value added for Real estate
-- **GDD_R** Real gross value added
-- **GDP_DEF** GDP deflator
-- **Rincpop_q** Real population average monthly income
-- **Rexppop_q** Real population average monthly expenses
-- **Rwage_q** Real population average monthly wage
-- **imp** Import
-- **exp** Export
-- **cpi** Inflation
-- **realest_resed_prim** Real price for estate in primary market
-- **realest_resed_sec** Real price for estate in secondary market
-- **realest_comm** Real price for commercial estate
-- **index_stock_weighted** Change in stock value for traded companies
-- **ntrade_Agr** Change in stock value for non-traded companies Agriculture
-- **ntrade_Min** Change in stock value for non-traded companies Mining
-- **ntrade_Man** Change in stock value for non-traded companies Manufacture
-- **ntrade_Elc** Change in stock value for non-traded companies Electricity
-- **ntrade_Con** Change in stock value for non-traded companies Construction
-- **ntrade_Trd** Change in stock value for non-traded companies Trade
-- **ntrade_Trn** Change in stock value for non-traded companies Transportation
-- **ntrade_Inf** Change in stock value for non-traded companies Information
-- **fed_fund_rate** Federal Funds Rate
-- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m
-- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year
-- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years
-- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years
-- **tonia_rate** TONIA
-- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year
-- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year
-- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year
-- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year
-- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year
-- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year
-- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
-- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year
+- **real_gdp** Real GDP, in 2005 base-year prices (bln KZT)
+- **GDD_Agr_R** Real gross value added Agriculture, in 2005 base-year prices (bln KZT)
+- **GDD_Min_R** Real gross value added Mining, in 2005 base-year prices (bln KZT)
+- **GDD_Man_R** Real gross value added Manufacture, in 2005 base-year prices (bln KZT)
+- **GDD_Elc_R** Real gross value added Electricity, in 2005 base-year prices (bln KZT)
+- **GDD_Con_R** Real gross value added Construction, in 2005 base-year prices (bln KZT)
+- **GDD_Trd_R** Real gross value added Trade, in 2005 base-year prices (bln KZT)
+- **GDD_Trn_R** Real gross value added Transportation, in 2005 base-year prices (bln KZT)
+- **GDD_Inf_R** Real gross value added Information, in 2005 base-year prices (bln KZT)
+- **GDD_Est_R** Real gross value added for Real estate, in 2005 base-year prices (bln KZT)
+- **GDD_R** Real gross value added, in 2005 base-year prices (bln KZT)
+- **GDP_DEF** GDP deflator, relative to 2005 base-year prices (bln KZT)
+- **Rincpop_q** Real population average monthly income, in 2005 base-year prices (ths KZT)
+- **Rexppop_q** Real population average monthly expenses, in 2005 base-year prices (ths KZT)
+- **Rwage_q** Real population average monthly wage, in 2005 base-year prices (ths KZT)
+- **imp** Import (mln KZT)
+- **exp** Export (mln kZT)
+- **cpi** Inflation, relative to 2005 base-year prices
+- **realest_resed_prim** Real price for estate in primary market (Q\Q)
+- **realest_resed_sec** Real price for estate in secondary market (Q\Q)
+- **realest_comm** Real price for commercial estate (Q\Q)
+- **index_stock_weighted** Change in stock value for traded companies (Q\Q)
+- **ntrade_Agr** Change in stock value for non-traded companies Agriculture (Q\Q)
+- **ntrade_Min** Change in stock value for non-traded companies Mining (Q\Q)
+- **ntrade_Man** Change in stock value for non-traded companies Manufacture (Q\Q)
+- **ntrade_Elc** Change in stock value for non-traded companies Electricity (Q\Q)
+- **ntrade_Con** Change in stock value for non-traded companies Construction (Q\Q)
+- **ntrade_Trd** Change in stock value for non-traded companies Trade (Q\Q)
+- **ntrade_Trn** Change in stock value for non-traded companies Transportation (Q\Q)
+- **ntrade_Inf** Change in stock value for non-traded companies Information (Q\Q)
+- **fed_fund_rate** Federal Funds Rate (%)
+- **govsec_rate_kzt_3m** Return on government securities in KZT, 3 m (%)
+- **govsec_rate_kzt_1y** Return on government securities in KZT, 1 year (%)
+- **govsec_rate_kzt_7y** Return on government securities in KZT, 7 years (%)
+- **govsec_rate_kzt_10y** Return on government securities in KZT, 10 years (%)
+- **tonia_rate** TONIA (%)
+- **rate_kzt_mort_0y_1y** Weighted average mortgage lending rate for new loans, less than a year (%)
+- **rate_kzt_mort_1y_iy** Weighted average mortgage lending rate for new loans, more than a year (%)
+- **rate_kzt_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, less than a year (%)
+- **rate_usd_corp_0y_1y** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, less than a year (%)
+- **rate_kzt_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in KZT, more than a year (%)
+- **rate_usd_corp_1y_iy** Weighted average mortgage lending rate for new loans to non-financial organizations in CKB, more than a year (%)
+- **rate_kzt_indv_0y_1y** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
+- **rate_kzt_indv_1y_iy** Weighted average mortgage lending rate for consumer loans in KZT, less than a year (%)
 - **usdkzt** USD KZT exchange rate
 - **eurkzt** EUR KZT exchange rate
 - **rurkzt** RUB KZT exchange rate
-- **poil** Price for Brent
-- **realest_resed_prim_rus** Real price for estate in primary market in Russia
-- **realest_resed_sec_rus** Real price for estate in secondary market in Russia
-- **cred_portfolio** credit portfolio
+- **poil** Price for Brent ($/barrel)
+- **realest_resed_prim_rus** Real price for estate in primary market in Russia (Q\Q)
+- **realest_resed_sec_rus** Real price for estate in secondary market in Russia (Q\Q)
+- **cred_portfolio** credit portfolio (mln KZT)
 - **coef_k1** k1 prudential coefficient
 - **coef_k3** k3 prudential coefficient
 - **provisions** provisions
 - **percent_margin** percent margin
-- **com_inc** commissionary income
-- **com_exp** commissionary expenses
-- **oper_inc** operational income
-- **oth_inc** other income
+- **com_inc** commissionary income (ths KZT)
+- **com_exp** commissionary expenses (ths KZT)
+- **oper_inc** operational income (ths KZT)
+- **oth_inc** other income (ths KZT)
 - **DR** default rate
 
 **Example** :
 
 .. code-block:: python
 
-    import pandas as pd
-    macro = pd.read_csv('./macroKZ.csv')
+    import AFR
+    macroKZ = load_macroKZ()
 
 **Reference** :
 The Agency of the Republic of Kazakhstan for Regulation and Development of Financial Market.   
   
 
 
 ## Functions
@@ -329,14 +318,42 @@
 
 model = ols('real_gdp ~ poil + cpi + usdkzt + imp', data = macro).fit()
 
 dec_plot(model, macro)
 
 
 
+* **load_finratKZ**
+
+Loads finratKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : finratKZ dataset.
+
+_Example_:
+
+df = load_finratKZ()
+
+
+
+* **load_macroKZ**
+
+Loads macroKZ dataset. More details in the description of the dataset.
+
+_Result_:
+
+dataset : macroKZ dataset.
+
+_Example_:
+
+df = load_macroKZ()
+
+
+
 * **opt_size**
 
 Calculation of the number of observations necessary to generate the regression for a given number of regressors.
 
 _Arguments_:
 
 model: OLS linear regression model.
```

### Comparing `AFR-0.2.2/example_process.ipynb` & `AFR-0.2.3/example_process.ipynb`

 * *Files identical despite different names*

### Comparing `AFR-0.2.2/setup.py` & `AFR-0.2.3/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,28 @@
-from setuptools import setup
+from setuptools import setup, find_packages
 
 with open('AFR manual.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='AFR',
-    version='0.2.2',
+    version='0.2.3',
     description='Statistical toolkit aimed to help statisticians, data analysts, data scientists, bankers and other professionals to analyze financial data',
     author='Timur Abilkassymov, Alua Makhmetova',
     author_email='alua.makhmetova@gmail.com',
     url='https://github.com/AFRKZ/AFR',
     license="3-clause BSD",
-    packages=['AFR'],
-    package_dir={'': '.'},
+    packages=find_packages(where="AFR"),
     install_requires=[
         'setuptools', 'pandas', 'sklearn',
         'scikit-learn', 'numpy', 'statsmodels', 'matplotlib',
         'matplotlib', 'mlxtend'
     ],
-    package_data={'AFR': ['load/macroKZ.csv', 'load/finratKZ.csv']},
-    include_package_data=True,
+    package_dir={"": "AFR"},
+    package_data={'AFR.load': ['*.csv']},
     long_description=long_description,
     long_description_content_type='text/markdown',
     options={
         'bdist_wheel': {
             'universal': True,
         }
     }
```

